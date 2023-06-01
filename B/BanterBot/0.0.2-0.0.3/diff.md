# Comparing `tmp/BanterBot-0.0.2.tar.gz` & `tmp/BanterBot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanterBot-0.0.2.tar", last modified: Thu Jun  1 22:31:53 2023, max compression
+gzip compressed data, was "BanterBot-0.0.3.tar", last modified: Thu Jun  1 22:53:33 2023, max compression
```

## Comparing `BanterBot-0.0.2.tar` & `BanterBot-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.214872 BanterBot-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.122371 BanterBot-0.0.2/BanterBot.egg-info/
--rw-rw-rw-   0        0        0     5206 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5206 2023-06-01 22:31:53.215371 BanterBot-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4101 2023-06-01 22:09:18.000000 BanterBot-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.123372 BanterBot-0.0.2/banterbot/
--rw-rw-rw-   0        0        0      645 2023-05-30 22:17:56.000000 BanterBot-0.0.2/banterbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.135871 BanterBot-0.0.2/banterbot/core/
--rw-rw-rw-   0        0        0      251 2023-05-30 22:17:56.000000 BanterBot-0.0.2/banterbot/core/__init__.py
--rw-rw-rw-   0        0        0     7373 2023-05-31 21:07:43.000000 BanterBot-0.0.2/banterbot/core/openai_manager.py
--rw-rw-rw-   0        0        0     6355 2023-06-01 22:30:44.000000 BanterBot-0.0.2/banterbot/core/speech_to_text.py
--rw-rw-rw-   0        0        0    12535 2023-06-01 22:30:45.000000 BanterBot-0.0.2/banterbot/core/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.148371 BanterBot-0.0.2/banterbot/data/
--rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/data/__init__.py
--rw-rw-rw-   0        0        0     7198 2023-05-31 21:31:32.000000 BanterBot-0.0.2/banterbot/data/azure_neural_voices.py
--rw-rw-rw-   0        0        0      455 2023-05-30 21:54:12.000000 BanterBot-0.0.2/banterbot/data/config.py
--rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.2/banterbot/data/enums.py
--rw-rw-rw-   0        0        0     2981 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/data/openai_models.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.164872 BanterBot-0.0.2/banterbot/gui/
--rw-rw-rw-   0        0        0      185 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/gui/__init__.py
--rw-rw-rw-   0        0        0     8550 2023-06-01 21:50:45.000000 BanterBot-0.0.2/banterbot/gui/banter_bot_interface.py
--rw-rw-rw-   0        0        0     7048 2023-06-01 22:30:45.000000 BanterBot-0.0.2/banterbot/gui/banter_bot_tk.py
--rw-rw-rw-   0        0        0     1626 2023-05-29 13:12:28.000000 BanterBot-0.0.2/banterbot/gui/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.188372 BanterBot-0.0.2/banterbot/utils/
--rw-rw-rw-   0        0        0       67 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/utils/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-05-31 21:31:32.000000 BanterBot-0.0.2/banterbot/utils/message.py
--rw-rw-rw-   0        0        0     5725 2023-05-31 21:25:27.000000 BanterBot-0.0.2/banterbot/utils/nlp.py
--rw-rw-rw-   0        0        0     7633 2023-05-31 22:27:47.000000 BanterBot-0.0.2/banterbot/utils/speech_to_text_output.py
--rw-rw-rw-   0        0        0     3887 2023-05-30 21:54:12.000000 BanterBot-0.0.2/banterbot/utils/text_to_speech_output.py
--rw-rw-rw-   0        0        0     2895 2023-05-28 15:33:48.000000 BanterBot-0.0.2/banterbot/utils/thread_queue.py
--rw-rw-rw-   0        0        0     3097 2023-05-31 22:01:51.000000 BanterBot-0.0.2/banterbot/utils/word.py
--rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-06-01 22:31:53.217873 BanterBot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2189 2023-06-01 22:30:45.000000 BanterBot-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.190872 BanterBot-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.195371 BanterBot-0.0.2/tests/core/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/core/__init__.py
--rw-rw-rw-   0        0        0     8818 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/core/test_openai_manager.py
--rw-rw-rw-   0        0        0     2661 2023-06-01 22:30:45.000000 BanterBot-0.0.2/tests/core/test_text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.212372 BanterBot-0.0.2/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_message.py
--rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_nlp.py
--rw-rw-rw-   0        0        0     3087 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_text_to_speech_output.py
--rw-rw-rw-   0        0        0     1239 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_text_to_speech_word.py
--rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_thread_queue.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.681945 BanterBot-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.597945 BanterBot-0.0.3/BanterBot.egg-info/
+-rw-rw-rw-   0        0        0     5220 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5220 2023-06-01 22:53:33.682445 BanterBot-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4115 2023-06-01 22:52:41.000000 BanterBot-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.598945 BanterBot-0.0.3/banterbot/
+-rw-rw-rw-   0        0        0      645 2023-05-30 22:17:56.000000 BanterBot-0.0.3/banterbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.610444 BanterBot-0.0.3/banterbot/core/
+-rw-rw-rw-   0        0        0      251 2023-05-30 22:17:56.000000 BanterBot-0.0.3/banterbot/core/__init__.py
+-rw-rw-rw-   0        0        0     7373 2023-05-31 21:07:43.000000 BanterBot-0.0.3/banterbot/core/openai_manager.py
+-rw-rw-rw-   0        0        0     6355 2023-06-01 22:30:44.000000 BanterBot-0.0.3/banterbot/core/speech_to_text.py
+-rw-rw-rw-   0        0        0    12535 2023-06-01 22:30:45.000000 BanterBot-0.0.3/banterbot/core/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.621445 BanterBot-0.0.3/banterbot/data/
+-rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/data/__init__.py
+-rw-rw-rw-   0        0        0     7198 2023-05-31 21:31:32.000000 BanterBot-0.0.3/banterbot/data/azure_neural_voices.py
+-rw-rw-rw-   0        0        0      455 2023-05-30 21:54:12.000000 BanterBot-0.0.3/banterbot/data/config.py
+-rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.3/banterbot/data/enums.py
+-rw-rw-rw-   0        0        0     2981 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/data/openai_models.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.635945 BanterBot-0.0.3/banterbot/gui/
+-rw-rw-rw-   0        0        0      185 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/gui/__init__.py
+-rw-rw-rw-   0        0        0     8550 2023-06-01 21:50:45.000000 BanterBot-0.0.3/banterbot/gui/banter_bot_interface.py
+-rw-rw-rw-   0        0        0     7048 2023-06-01 22:30:45.000000 BanterBot-0.0.3/banterbot/gui/banter_bot_tk.py
+-rw-rw-rw-   0        0        0     1911 2023-06-01 22:49:44.000000 BanterBot-0.0.3/banterbot/gui/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.657945 BanterBot-0.0.3/banterbot/utils/
+-rw-rw-rw-   0        0        0       67 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/utils/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-05-31 21:31:32.000000 BanterBot-0.0.3/banterbot/utils/message.py
+-rw-rw-rw-   0        0        0     5725 2023-05-31 21:25:27.000000 BanterBot-0.0.3/banterbot/utils/nlp.py
+-rw-rw-rw-   0        0        0     7633 2023-05-31 22:27:47.000000 BanterBot-0.0.3/banterbot/utils/speech_to_text_output.py
+-rw-rw-rw-   0        0        0     3887 2023-05-30 21:54:12.000000 BanterBot-0.0.3/banterbot/utils/text_to_speech_output.py
+-rw-rw-rw-   0        0        0     2895 2023-05-28 15:33:48.000000 BanterBot-0.0.3/banterbot/utils/thread_queue.py
+-rw-rw-rw-   0        0        0     3097 2023-05-31 22:01:51.000000 BanterBot-0.0.3/banterbot/utils/word.py
+-rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-06-01 22:53:33.683945 BanterBot-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2214 2023-06-01 22:49:28.000000 BanterBot-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.659945 BanterBot-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.663945 BanterBot-0.0.3/tests/core/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     8818 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/core/test_openai_manager.py
+-rw-rw-rw-   0        0        0     2661 2023-06-01 22:30:45.000000 BanterBot-0.0.3/tests/core/test_text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.679945 BanterBot-0.0.3/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_message.py
+-rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_nlp.py
+-rw-rw-rw-   0        0        0     3087 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_text_to_speech_output.py
+-rw-rw-rw-   0        0        0     1239 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_text_to_speech_word.py
+-rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_thread_queue.py
```

### Comparing `BanterBot-0.0.2/BanterBot.egg-info/PKG-INFO` & `BanterBot-0.0.3/BanterBot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.2
-Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and tkinter frontend.
+Version: 0.0.3
+Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.2-alpha/BanterBot-0.0.2.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.3-alpha/BanterBot-0.0.3.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -59,15 +59,15 @@
 
 ### BanterBotTK
 
 A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
 
 ## Installation
 
-### Pip
+### Pip (Recommended)
 
 BanterBot is installable using the Python Package Index (PyPi):
 
 ```bash
 python -m pip install banterbot
 ```
```

### Comparing `BanterBot-0.0.2/BanterBot.egg-info/SOURCES.txt` & `BanterBot-0.0.3/BanterBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/PKG-INFO` & `BanterBot-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.2
-Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and tkinter frontend.
+Version: 0.0.3
+Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.2-alpha/BanterBot-0.0.2.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.3-alpha/BanterBot-0.0.3.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -59,15 +59,15 @@
 
 ### BanterBotTK
 
 A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
 
 ## Installation
 
-### Pip
+### Pip (Recommended)
 
 BanterBot is installable using the Python Package Index (PyPi):
 
 ```bash
 python -m pip install banterbot
 ```
```

### Comparing `BanterBot-0.0.2/README.md` & `BanterBot-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 ### BanterBotTK
 
 A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
 
 ## Installation
 
-### Pip
+### Pip (Recommended)
 
 BanterBot is installable using the Python Package Index (PyPi):
 
 ```bash
 python -m pip install banterbot
 ```
```

### Comparing `BanterBot-0.0.2/banterbot/__init__.py` & `BanterBot-0.0.3/banterbot/__init__.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/core/openai_manager.py` & `BanterBot-0.0.3/banterbot/core/openai_manager.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/core/speech_to_text.py` & `BanterBot-0.0.3/banterbot/core/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/core/text_to_speech.py` & `BanterBot-0.0.3/banterbot/core/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/data/azure_neural_voices.py` & `BanterBot-0.0.3/banterbot/data/azure_neural_voices.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/data/enums.py` & `BanterBot-0.0.3/banterbot/data/enums.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/data/openai_models.py` & `BanterBot-0.0.3/banterbot/data/openai_models.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/gui/banter_bot_interface.py` & `BanterBot-0.0.3/banterbot/gui/banter_bot_interface.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/gui/banter_bot_tk.py` & `BanterBot-0.0.3/banterbot/gui/banter_bot_tk.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/gui/cli.py` & `BanterBot-0.0.3/banterbot/gui/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,35 +8,40 @@
     """
     The main function to run the BanterBot Command Line Interface.
 
     This function parses command line arguments, sets up the necessary configurations, and initializes the BanterBotTK
     graphical user interface for user interaction.
     """
     parser = argparse.ArgumentParser(
-        prog="BanterBot Command Line Interface",
+        prog="BanterBot GUI",
         description=(
-            "This program defines an interface for a text-based conversational agent based on the Persona class. The "
-            "program uses the termighty library to create a graphical user interface for user interaction and handles "
-            "input and output processing, as well as text-to-speech synthesis."
+            "This program initializes a GUI that allows users to interact with a chatbot by entering a name and a "
+            "message, and it displays the conversation history in a scrollable text area. Users can send messages by "
+            "pressing the `Send` button or the `Enter` key. The chatbot's responses are generated using the specified "
+            "OpenAI model and can be played back using the specified Azure Neural Voice. Additionally, users can "
+            "toggle speech-to-text input by pressing the `Listen` button."
         ),
         epilog=(
             "Requires three environment variables for full functionality. "
-            "1) OPENAI_API_KEY: A valid OpenAI API key, "
-            "2) AZURE_SPEECH_KEY: A valid Azure Cognitive Services Speech API key for TTS functionality, and "
+            "1) OPENAI_API_KEY: A valid OpenAI API key,\n"
+            "2) AZURE_SPEECH_KEY: A valid Azure Cognitive Services Speech API key for text-to-speech and "
+            "speech-to-text functionality,\n"
             "3) AZURE_SPEECH_REGION: The region associated with your Azure Cognitive Services Speech API key."
         ),
     )
 
     parser.add_argument(
         "-g",
         "--gpt4",
         action="store_true",
         dest="gpt4",
         help="Enable GPT-4; only works if you have GPT-4 API access.",
     )
 
+    args=parser.parse_args()
+
     kwargs = {
         "model": get_model_by_name("gpt-4") if args.gpt4 else get_model_by_name("gpt-3.5-turbo"),
     }
 
     gui = BanterBotTK(**kwargs)
     gui.run()
```

### Comparing `BanterBot-0.0.2/banterbot/utils/message.py` & `BanterBot-0.0.3/banterbot/utils/message.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/utils/nlp.py` & `BanterBot-0.0.3/banterbot/utils/nlp.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/utils/speech_to_text_output.py` & `BanterBot-0.0.3/banterbot/utils/speech_to_text_output.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/utils/text_to_speech_output.py` & `BanterBot-0.0.3/banterbot/utils/text_to_speech_output.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/utils/thread_queue.py` & `BanterBot-0.0.3/banterbot/utils/thread_queue.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/banterbot/utils/word.py` & `BanterBot-0.0.3/banterbot/utils/word.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/setup.py` & `BanterBot-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 dependencies = ["openai", "tiktoken", "requests", "azure-cognitiveservices-speech", "spacy"]
 
 url = "https://github.com/GabrielSCabrera/BanterBot"
 
 description = (
     "BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech "
-    "interactions. Features real-time monitoring and tkinter frontend."
+    "interactions. Features real-time monitoring and Tkinter frontend."
 )
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 # For running tests: python -m unittest discover -s tests
 # For building: python setup.py sdist bdist_wheel
@@ -20,27 +20,27 @@
 
 
 def run_tests():
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover("tests", pattern="test_*.py")
     return test_suite
 
-
+version = "0.0.3"
 setup(
     name="BanterBot",
     packages=find_packages(),
     test_suite="setup.run_tests",
-    version="0.0.2",
+    version=version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Gabriel S. Cabrera",
     author_email="gabriel.sigurd.cabrera@gmail.com",
     url=url,
-    download_url=url + f"/releases/download/v0.0.2-alpha/BanterBot-0.0.2.tar.gz",
+    download_url=url + f"/releases/download/v{version}-alpha/BanterBot-{version}.tar.gz",
     keywords=[
         "tkinter",
         "tk",
         "gpt",
         "gui",
         "windows",
         "linux",
```

### Comparing `BanterBot-0.0.2/tests/core/test_openai_manager.py` & `BanterBot-0.0.3/tests/core/test_openai_manager.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/tests/core/test_text_to_speech.py` & `BanterBot-0.0.3/tests/core/test_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/tests/utils/test_message.py` & `BanterBot-0.0.3/tests/utils/test_message.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/tests/utils/test_nlp.py` & `BanterBot-0.0.3/tests/utils/test_nlp.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/tests/utils/test_text_to_speech_output.py` & `BanterBot-0.0.3/tests/utils/test_text_to_speech_output.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/tests/utils/test_text_to_speech_word.py` & `BanterBot-0.0.3/tests/utils/test_text_to_speech_word.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.2/tests/utils/test_thread_queue.py` & `BanterBot-0.0.3/tests/utils/test_thread_queue.py`

 * *Files identical despite different names*

