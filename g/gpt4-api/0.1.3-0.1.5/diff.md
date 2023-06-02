# Comparing `tmp/gpt4-api-0.1.3.tar.gz` & `tmp/gpt4-api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.1.3.tar", last modified: Fri Jun  2 03:30:34 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.1.5.tar", last modified: Fri Jun  2 05:45:24 2023, max compression
```

## Comparing `gpt4-api-0.1.3.tar` & `gpt4-api-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.3/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    16527 2023-06-02 03:26:55.000000 gpt4-api-0.1.3/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-02 03:30:34.000000 gpt4-api-0.1.3/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.3/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.5/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    16517 2023-06-02 05:45:06.000000 gpt4-api-0.1.5/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.5/setup.py
```

### Comparing `gpt4-api-0.1.3/api/gpt.py` & `gpt4-api-0.1.5/api/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.completion_tokens = completion_tokens
         self.prompt_tokens = prompt_tokens
         self.total_tokens = total_tokens
         self.case_name = case_name
 
 
 class GPTTaskManager:
-    def __init__(self, num_thread, keys, stream=False, max_retries=3, key_limit=4096, model='gpt-4', temperature=0, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None, call_black=None):
+    def __init__(self, num_thread, keys, stream=False, max_retries=3, key_limit=4096, model='gpt-4', temperature=0, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None, call_back=None):
         self.num_threads = num_thread
         self.stream = stream
         self.max_retries = max_retries
         self.task_queue = JoinableQueue()
         self.key_lock = threading.Lock()
         self.usable_openai_keys = self.process_token(keys=keys) or []
         self.key_limit = key_limit
@@ -44,15 +44,15 @@
         self.frequency_penalty = frequency_penalty
         # 要生成的文本的数量。默认为1，表示生成一段文本
         self.n = n
         # 是否将生成的文本作为流返回，而不是一次性返回所有文本。默认为False，表示一次性返回所有文本
         # 系统默认内容
         self.system_content = system_content
         self.total_tokens = 0
-        self.call_black = call_black
+        self.call_back = call_back
 
     def __worker(self, run_func):
         logging.disable(logging.NOTSET)
         while True:
             try:
                 task = self.task_queue.get(timeout=1)
                 content = task.get("ask")
@@ -170,16 +170,16 @@
                 logging.info("total tokens: %s" % total_tokens)
                 for openaiKey in self.usable_openai_keys:
                     if openaiKey.get("api_key", None) == open_ai_key:
                         openaiKey["token_limit"] += total_tokens
                 logging.info("active threads: %s" % self.get_active_thread_count())
                 if self.task_is_empty():
                     logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
-                if call_back_func and self.call_black:
-                    call_back_func = self.call_black.get(call_back_func, None)
+                if call_back_func and self.call_back:
+                    call_back_func = self.call_back.get(call_back_func, None)
                     if call_back_func:
                         call_back_func(call_black_parameter(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name))
             except openai.error.RateLimitError as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
                 self.__release_token(open_ai_key)
                 self.__retry_on_error(task, ask_content, messages, retries=retries)
             except openai.error.Timeout as e:
@@ -195,18 +195,18 @@
             self.task_queue.put(task)
 
     def task_run_tasks(self, tasks):
         self.__run_tasks(tasks=tasks, run_func=self.__process_task)
 
 
 class GPTAsyncTaskManager(GPTTaskManager):
-    def __init__(self, num_thread, keys, stream, max_retries, key_limit, model, temperature, top_p, presence_penalty, frequency_penalty, n, system_content, call_black=None):
+    def __init__(self, num_thread, keys, stream, max_retries, key_limit, model, temperature, top_p, presence_penalty, frequency_penalty, n, system_content, call_back=None):
         self.loop = asyncio.get_event_loop()
         self.task_queue = asyncio.Queue(maxsize=0)
-        super(GPTAsyncTaskManager, self).__init__(num_thread, keys, stream=stream, max_retries=max_retries, key_limit=key_limit, model=model, temperature=temperature, top_p=top_p, presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, n=n, system_content=system_content, call_black=call_black)
+        super(GPTAsyncTaskManager, self).__init__(num_thread, keys, stream=stream, max_retries=max_retries, key_limit=key_limit, model=model, temperature=temperature, top_p=top_p, presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, n=n, system_content=system_content, call_back=call_back)
 
     async def __worker(self, run_func):
         logging.disable(logging.NOTSET)
         while True:
             try:
                 task = await self.task_queue.get()
                 if task is None:
@@ -310,17 +310,17 @@
             #     logging.error(f"Retrying: {case_name}/{retries}, OpenAI API returned an API Error: {e}")
             #     self.retry_on_error(task, ask_content, messages, retries=retries)
         else:
             await self.task_queue.put(task)
 
 
 class GPT4(GPTAsyncTaskManager):
-    def __init__(self, keys=None, model='gpt-4', temperature=0, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, stream=False, system_content=None, num_threads=50, key_limit=4096, max_retries=3, call_black=None):
-        super(GPT4, self).__init__(num_thread=num_threads, keys=keys, stream=stream, max_retries=max_retries, key_limit=key_limit, model=model, temperature=temperature, top_p=top_p, presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, n=n, system_content=system_content, call_black=call_black)
+    def __init__(self, keys=None, model='gpt-4', temperature=0, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, stream=False, system_content=None, num_threads=50, key_limit=4096, max_retries=3, call_back=None):
+        super(GPT4, self).__init__(num_thread=num_threads, keys=keys, stream=stream, max_retries=max_retries, key_limit=key_limit, model=model, temperature=temperature, top_p=top_p, presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, n=n, system_content=system_content, call_back=call_back)
 
     def run_tasks(self, tasks):
         if not self.stream:
             logging.info("Mode: Multi threaded synchronous request gpt")
             self.task_run_tasks(tasks=tasks)
         else:
             logging.info("Mode: Multi threaded asynchronous request gpt")
-            self.loop.run_until_complete(self.async_task_run_tasks(tasks=tasks))
+            self.loop.run_until_complete(self.async_task_run_tasks(tasks=tasks))
```

### Comparing `gpt4-api-0.1.3/setup.py` & `gpt4-api-0.1.5/setup.py`

 * *Files identical despite different names*

