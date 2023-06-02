# Comparing `tmp/edubot-0.6.8.tar.gz` & `tmp/edubot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.6.8.tar", max compression
+gzip compressed data, was "edubot-0.7.0.tar", max compression
```

## Comparing `edubot-0.6.8.tar` & `edubot-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.6.8/LICENSE
--rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.6.8/README.md
--rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.6.8/edubot/__init__.py
--rw-r--r--   0        0        0    19428 2023-05-29 09:39:28.101401 edubot-0.6.8/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.6.8/edubot/sql.py
--rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.6.8/edubot/types.py
--rw-r--r--   0        0        0      632 2023-05-29 09:44:42.044374 edubot-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-24 18:21:26.784597 edubot-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1400 2023-03-29 15:28:01.248879 edubot-0.7.0/README.md
+-rw-r--r--   0        0        0      894 2023-05-19 11:19:02.481354 edubot-0.7.0/edubot/__init__.py
+-rw-r--r--   0        0        0    22396 2023-06-02 18:11:58.660024 edubot-0.7.0/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2023-02-23 10:32:46.665675 edubot-0.7.0/edubot/sql.py
+-rw-r--r--   0        0        0      636 2023-06-02 16:51:19.347235 edubot-0.7.0/edubot/types.py
+-rw-r--r--   0        0        0      624 2023-06-02 18:11:37.951095 edubot-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.7.0/PKG-INFO
```

### Comparing `edubot-0.6.8/LICENSE` & `edubot-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.6.8/README.md` & `edubot-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.6.8/edubot/__init__.py` & `edubot-0.7.0/edubot/__init__.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.8/edubot/bot.py` & `edubot-0.7.0/edubot/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 from stability_sdk.client import StabilityInference, process_artifacts_from_answers
 from stability_sdk.utils import generation
 
 from edubot import DREAMSTUDIO_KEY, OPENAI_KEY, REPLICATE_KEY
 from edubot.sql import Bot, Completion, Message, Session, Thread
 from edubot.types import CompletionInfo, ImageInfo, MessageInfo
 
+# The limit for GPT-4 is 8192 tokens.
+MAX_GPT_TOKENS = 8192
 # The maximum number of GPT tokens that chat context can be.
-# The limit for GPT-4 is 8192.
-# We limit to 7200 to allow extra room for the response and the personality.
-MAX_GPT_TOKENS = 7200
+MAX_PROMPT_TOKENS = MAX_GPT_TOKENS - 1192
+# The maximum number of GPT tokens that can be used for completion.
+MAX_COMPLETION_TOKENS = MAX_GPT_TOKENS - MAX_PROMPT_TOKENS
 
 # The maximum allowed size of images in megabytes
 MAX_IMAGE_SIZE_MB = 50
 
 # Prompt for GPT to summarise web pages
 WEB_SUMMARY_PROMPT = (
     "Your input is scraped text from a website. Your job is to summarise the text and post it to a chatroom.\n"
@@ -34,15 +36,19 @@
     "If the page doesn't contain long-form text return the phrase 'NO CONTENT' and nothing else.\n"
     "If the page mentions any variation of 'requiring javascript', or 'enable javascript' you should also return 'NO CONTENT' and nothing else.\n"
     "If the page DOES contain long-form text return a brief 2 sentence summary of the text content. "
     "This summary will then be sent to users.\n"
 )
 
 # Settings for GPT completion generation
-GPT_SETTINGS = {"model": "gpt-4", "temperature": 0.3, "max_tokens": 700}
+GPT_SETTINGS = {
+    "model": "gpt-4",
+    "temperature": 0.3,
+    "max_tokens": MAX_COMPLETION_TOKENS,
+}
 
 logger = logging.getLogger(__name__)
 
 REPLICATE_CLIENT = replicate.Client(api_token=REPLICATE_KEY)
 
 
 # TODO: use tiktoken for this, the function is currently inaccurate
@@ -145,14 +151,31 @@
             ).fetchone()
 
             if thread:
                 return thread[0]
             else:
                 return None
 
+    def __get_completion_from_message(self, msg_info: MessageInfo) -> Completion | None:
+        """
+        Gets the bots response to a specific message.
+        """
+        with Session() as session:
+            msg = self.__get_message(msg_info)
+            completion = session.execute(
+                select(Completion)
+                .where(Completion.bot == self.__bot_pk)
+                .where(Completion.reply_to == msg.id)
+            ).fetchone()
+
+            if completion:
+                return completion[0]
+            else:
+                return None
+
     def __add_completion(self, completion: str, reply_to: MessageInfo) -> None:
         """
         Add a completion to the database.
 
         :param completion: The text the bot generated.
         :param reply_to: The message the bot was replying to.
         """
@@ -190,15 +213,15 @@
                 role = "user"
 
             content = f"{msg['username']}: {msg['message']}"
             gpt_context.append({"role": role, "content": content})
 
             token_count += estimate_tokens(content)
 
-        while token_count > MAX_GPT_TOKENS:
+        while token_count > MAX_PROMPT_TOKENS:
             token_count -= estimate_tokens(gpt_context.pop(0)["content"])
 
         system_messages = [
             {"role": "system", "content": "You are a chatbot named " + self.username},
             {"role": "system", "content": f"Your personality is: {personality}"},
             {
                 "role": "system",
@@ -217,62 +240,71 @@
                 "role": "system",
                 "content": f"You use the language model {GPT_SETTINGS['model']}",
             },
         ]
 
         return system_messages + gpt_context
 
-    def save_image_to_context(self, image: ImageInfo, thread_name: str) -> str | None:
+    @staticmethod
+    def __describe_image(image: Image.Image) -> str:
         """
-        Saves an AI generated description of an image to the database. This allows GPT to understand what images are
-         and how to describe them. The maximum image size in MB can be read from the MAX_IMAGE_SIZE_MB constant.
-
-        :param image: An ImageInfo object.
-        :param thread_name: A unique identifier for the thread the image was posted in.
-        :returns: The description of the image or None if an error occurred.
+        Gets an AI generated description of an image.
         """
         if not REPLICATE_KEY:
             raise RuntimeError(
                 "Replicate key is not defined, make sure to supply it in the config."
             )
 
         image_bytes = io.BytesIO()
-        image["image"].save(image_bytes, format="PNG")
+        image.save(image_bytes, format="PNG")
 
         if image_bytes.tell() / 1048576 > MAX_IMAGE_SIZE_MB:
-            logger.info(f"Skipped image in {thread_name} because it was too large.")
-            return
+            logger.info(f"Skipped image because it was too large.")
+            return None
 
         output: str = REPLICATE_CLIENT.run(
             "j-min/clip-caption-reward:de37751f75135f7ebbe62548e27d6740d5155dfefdf6447db35c9865253d7e06",
             input={"image": image_bytes},
         )
 
         if not output:
             logger.error("Replicate returned an empty response.")
-            return
+            return None
+
+        return output
+
+    def save_image_to_context(self, image: ImageInfo, thread_name: str) -> str | None:
+        """
+        Saves an AI generated description of a user-sent image to the database. This allows GPT to understand what images are
+         and how to describe them. The maximum image size in MB can be read from the MAX_IMAGE_SIZE_MB constant.
+
+        :param image: An ImageInfo object.
+        :param thread_name: A unique identifier for the thread the image was posted in.
+        :returns: The description of the image or None if an error occurred.
+        """
+        image_description = self.__describe_image(image["image"])
 
         with Session() as session:
             thread = self.__get_thread(thread_name)
             if not thread:
                 thread = Thread(thread_name=thread_name, platform=self.platform)
                 session.add(thread)
                 session.commit()
 
             message = Message(
                 thread=thread.id,
                 username=image["username"],
-                message=f"*An image of {output}",
+                message=f"*An image of {image_description}",
                 time=image["time"],
             )
-
             session.add(message)
+
             session.commit()
 
-        return output
+        return image_description
 
     # TODO: return None on error instead of empty string.
     def gpt_answer(
         self,
         new_context: list[MessageInfo],
         thread_name: str,
         personality_override: str = None,
@@ -314,30 +346,30 @@
                     "message": existing_msg.message,
                     "time": existing_msg.time,
                 }
                 if row_as_msg_info not in new_context:
                     existing_context.append(row_as_msg_info)
 
             # The existing context in this timeframe + the new messages
-            complete_context: list[MessageInfo] = []
+            new_and_existing_context: list[MessageInfo] = []
 
             for index, msg in enumerate(new_context):
                 # Figure out where to insert the extra context chronologically
                 for extra_msg in existing_context:
                     check = extra_msg["time"] < msg["time"]
                     if index > 0:
                         check = (
                             check and extra_msg["time"] > new_context[index - 1]["time"]
                         )
 
                     if check:
-                        complete_context.append(extra_msg)
+                        new_and_existing_context.append(extra_msg)
                         existing_context.remove(extra_msg)
 
-                complete_context.append(msg)
+                new_and_existing_context.append(msg)
 
                 # If the message is already in the database
                 if self.__get_message(msg) is not None:
                     continue
 
                 # If the message was written by a bot
                 if self.__get_bot(msg["username"]) is not None:
@@ -346,14 +378,32 @@
                 row: dict = msg
                 row["thread"] = thread.id
 
                 session.add(Message(**row))
 
             session.commit()
 
+        # Ensure that all bot completions are included in context, notably image completions.
+        complete_context: list[MessageInfo] = []
+        for message in new_and_existing_context:
+            if self.__get_bot(message["username"]) is not None:
+                continue
+            complete_context.append(message)
+
+            if completion := self.__get_completion_from_message(message):
+                complete_context.append(
+                    {
+                        "username": completion.bot,
+                        "message": completion.message,
+                        "time": message[
+                            "time"
+                        ],  # Estimate this, it doesn't matter for gpt_context
+                    }
+                )
+
         gpt_context = self.__format_context(
             complete_context, personality_override=personality_override
         )
 
         try:
             response = openai.ChatCompletion.create(
                 messages=gpt_context,
@@ -361,19 +411,19 @@
             )
         except OpenAIError as e:
             logger.error(f"OpenAI request failed: {e}")
             return ""
 
         completion: str = response["choices"][0]["message"]["content"]
 
-        # Strip username from completion
-        completion = completion.replace(f"{self.username}: ", "").lstrip()
+        # Strip username from completion, sometimes GPT messes this up.
+        completion = completion.replace(f"{self.username}:", "").lstrip()
 
         # Add a new completion to the database using the completion text and the message being replied to
-        self.__add_completion(completion, new_context[-1])
+        self.__add_completion(completion, complete_context[-1])
 
         # Return the completion result back to the integration
         return completion
 
     def change_completion_score(
         self, offset: int, completion: CompletionInfo, thread_name: str
     ) -> None:
@@ -422,20 +472,24 @@
             completion.score += offset
 
             session.add(completion)
             session.commit()
 
             logger.info(f"Completion {completion.id} incremented by {offset}.")
 
-    def generate_image(self, prompt: str) -> Image.Image | None:
+    def generate_image(
+        self, prompt: str, reply_to_msg: MessageInfo, thread_name: str
+    ) -> Image.Image | None:
         """
         Generate an image using Stability AI's DreamStudio.
 
         :param prompt: A description of the image that should be generated.
-        :return: A PIL.Image instance.
+        :param reply_to_msg: The message the bot is replying to.
+        :param thread_name: A unique identifier for the thread the message resides in.
+        :return: A PIL.Image.Image instance.
         """
         if not DREAMSTUDIO_KEY:
             raise RuntimeError(
                 "DreamStudio key is not defined, make sure to supply it in the config."
             )
 
         # Lazy load client
@@ -447,25 +501,56 @@
 
         # Get Answer objects from stability
         answers = self.stability_client.generate(prompt)
 
         # Convert answer objects into artifacts we can use
         artifacts = process_artifacts_from_answers("", "", answers, write=False)
 
+        image: Image.Image | None = None
         try:
             for _, artifact in artifacts:
                 # Check that the artifact is an Image, not sure why this is necessary.
                 # See: https://github.com/Stability-AI/stability-sdk/blob/d8f140f8828022d0ad5635acbd0fecd6f6fc317a/src/stability_sdk/utils.py#L80
                 if artifact.type == generation.ARTIFACT_IMAGE:
-                    img = PIL.Image.open(io.BytesIO(artifact.binary))
-                    return img
+                    image = PIL.Image.open(io.BytesIO(artifact.binary))
+                    break
         # Exception only happens when prompt is inappropriate.
         except Exception:
             return None
 
+        if image is None:
+            return None
+
+        with Session() as session:
+            thread = self.__get_thread(thread_name)
+
+            if not thread:
+                thread = Thread(thread_name=thread_name, platform=self.platform)
+
+                session.add(thread)
+                session.commit()
+
+            message = Message(
+                username=reply_to_msg["username"],
+                message=reply_to_msg["message"],
+                time=reply_to_msg["time"],
+                thread=thread.id,
+            )
+            session.add(message)
+            session.commit()
+
+        image_description = self.__describe_image(image)
+        completion = (
+            f"*An image you generated based on the prompt: '{prompt}'.\n"
+            f"*Your interpretation of the image is: '{image_description}'."
+        )
+        self.__add_completion(completion, reply_to_msg)
+
+        return image
+
     def summarise_url(self, url: str, msg: MessageInfo, thread_name: str) -> str | None:
         """
         Use GPT to summarise the text content of a URL.
 
         Returns None if the webpage cannot be fetched or doesn't contain long-form text to summarise.
 
         :param url: A valid url.
@@ -482,15 +567,15 @@
         text = trafilatura.extract(resp)
 
         # If error converting to plaintext
         if text is None:
             return None
 
         # Ensure text doesn't exceed GPT limits
-        while estimate_tokens(text) > MAX_GPT_TOKENS:
+        while estimate_tokens(text) > MAX_PROMPT_TOKENS:
             text = text[:-100]
 
         gpt_context = [
             {"role": "system", "content": WEB_SUMMARY_PROMPT},
             {"role": "user", "content": text},
         ]
         try:
```

### Comparing `edubot-0.6.8/edubot/sql.py` & `edubot-0.7.0/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.8/edubot/types.py` & `edubot-0.7.0/edubot/types.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.8/pyproject.toml` & `edubot-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "edubot"
-version = "0.6.8"
+version = "0.7.0"
 description = ""
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sqlalchemy = {version = ">=1.4.45,<1.5.0", extras = ["mypy"]}
-openai = "^0.27.2"
-stability-sdk = "^0.4.0"
-pillow = "^9.4.0"
-beautifulsoup4 = "^4.11.2"
-trafilatura = "^1.4.1"
+sqlalchemy = {version = "^2.0.14", extras = ["mypy"]}
+openai = "^0.27.6"
+stability-sdk = "^0.8.1"
+pillow = "^9.5.0"
+beautifulsoup4 = "^4.12.2"
+trafilatura = "^1.6.0"
 replicate = "^0.8.1"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^3.2.0"
-mypy = "^1.1.1"
+pre-commit = "^3.3.2"
+mypy = "^1.3.0"
 
 [tool.mypy]
 plugins = "sqlalchemy.ext.mypy.plugin"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edubot-0.6.8/PKG-INFO` & `edubot-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.6.8
+Version: 0.7.0
 Summary: 
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: openai (>=0.27.2,<0.28.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: replicate (>=0.8.1,<0.9.0)
-Requires-Dist: sqlalchemy[mypy] (>=1.4.45,<1.5.0)
-Requires-Dist: stability-sdk (>=0.4.0,<0.5.0)
-Requires-Dist: trafilatura (>=1.4.1,<2.0.0)
+Requires-Dist: sqlalchemy[mypy] (>=2.0.14,<3.0.0)
+Requires-Dist: stability-sdk (>=0.8.1,<0.9.0)
+Requires-Dist: trafilatura (>=1.6.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edubot
 
 A self-improving AI-based chatbot library that is completely platform-agnostic.
 
 Edubot intuitively jumps into conversations to give advice, make jokes, and add to the discussion. Its personality can be completely customised to suit the tone of different rooms.
```

