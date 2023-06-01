# Comparing `tmp/BanterBot-0.0.1.tar.gz` & `tmp/BanterBot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanterBot-0.0.1.tar", last modified: Sun May 28 17:48:18 2023, max compression
+gzip compressed data, was "BanterBot-0.0.2.tar", last modified: Thu Jun  1 22:31:53 2023, max compression
```

## Comparing `BanterBot-0.0.1.tar` & `BanterBot-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.235823 BanterBot-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.144822 BanterBot-0.0.1/BanterBot.egg-info/
--rw-rw-rw-   0        0        0     3996 2023-05-28 17:48:18.000000 BanterBot-0.0.1/BanterBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1086 2023-05-28 17:48:18.000000 BanterBot-0.0.1/BanterBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 17:48:18.000000 BanterBot-0.0.1/BanterBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-28 17:48:18.000000 BanterBot-0.0.1/BanterBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-05-28 17:48:18.000000 BanterBot-0.0.1/BanterBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 17:48:18.000000 BanterBot-0.0.1/BanterBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3996 2023-05-28 17:48:18.235823 BanterBot-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3439 2023-05-28 16:17:48.000000 BanterBot-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.145823 BanterBot-0.0.1/banterbot/
--rw-rw-rw-   0        0        0      233 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.153823 BanterBot-0.0.1/banterbot/core/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/core/__init__.py
--rw-rw-rw-   0        0        0     7327 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/core/openai_manager.py
--rw-rw-rw-   0        0        0    12540 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/core/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.161823 BanterBot-0.0.1/banterbot/data/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/data/__init__.py
--rw-rw-rw-   0        0        0     6935 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/data/azure_neural_voices.py
--rw-rw-rw-   0        0        0      800 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/data/config.py
--rw-rw-rw-   0        0        0     2336 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/data/openai_models.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.176323 BanterBot-0.0.1/banterbot/gui/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/gui/__init__.py
--rw-rw-rw-   0        0        0     5962 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/gui/banter_bot_interface.py
--rw-rw-rw-   0        0        0     6227 2023-05-28 16:00:59.000000 BanterBot-0.0.1/banterbot/gui/banter_bot_tk.py
--rw-rw-rw-   0        0        0     1648 2023-05-28 16:00:59.000000 BanterBot-0.0.1/banterbot/gui/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.194323 BanterBot-0.0.1/banterbot/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/utils/__init__.py
--rw-rw-rw-   0        0        0     3310 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/utils/message.py
--rw-rw-rw-   0        0        0     4149 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/utils/nlp.py
--rw-rw-rw-   0        0        0     4471 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/utils/text_to_speech_output.py
--rw-rw-rw-   0        0        0     2708 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/utils/text_to_speech_word.py
--rw-rw-rw-   0        0        0     2895 2023-05-28 15:33:48.000000 BanterBot-0.0.1/banterbot/utils/thread_queue.py
--rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-05-28 17:48:18.240324 BanterBot-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1426 2023-05-28 16:20:27.000000 BanterBot-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.196323 BanterBot-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.217323 BanterBot-0.0.1/tests/core/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/core/__init__.py
--rw-rw-rw-   0        0        0     8818 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/core/test_openai_manager.py
--rw-rw-rw-   0        0        0     2661 2023-05-28 16:00:59.000000 BanterBot-0.0.1/tests/core/test_text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:48:18.233324 BanterBot-0.0.1/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/utils/test_message.py
--rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/utils/test_nlp.py
--rw-rw-rw-   0        0        0     3087 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/utils/test_text_to_speech_output.py
--rw-rw-rw-   0        0        0     1239 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/utils/test_text_to_speech_word.py
--rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.1/tests/utils/test_thread_queue.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.214872 BanterBot-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.122371 BanterBot-0.0.2/BanterBot.egg-info/
+-rw-rw-rw-   0        0        0     5206 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 22:31:53.000000 BanterBot-0.0.2/BanterBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5206 2023-06-01 22:31:53.215371 BanterBot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4101 2023-06-01 22:09:18.000000 BanterBot-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.123372 BanterBot-0.0.2/banterbot/
+-rw-rw-rw-   0        0        0      645 2023-05-30 22:17:56.000000 BanterBot-0.0.2/banterbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.135871 BanterBot-0.0.2/banterbot/core/
+-rw-rw-rw-   0        0        0      251 2023-05-30 22:17:56.000000 BanterBot-0.0.2/banterbot/core/__init__.py
+-rw-rw-rw-   0        0        0     7373 2023-05-31 21:07:43.000000 BanterBot-0.0.2/banterbot/core/openai_manager.py
+-rw-rw-rw-   0        0        0     6355 2023-06-01 22:30:44.000000 BanterBot-0.0.2/banterbot/core/speech_to_text.py
+-rw-rw-rw-   0        0        0    12535 2023-06-01 22:30:45.000000 BanterBot-0.0.2/banterbot/core/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.148371 BanterBot-0.0.2/banterbot/data/
+-rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/data/__init__.py
+-rw-rw-rw-   0        0        0     7198 2023-05-31 21:31:32.000000 BanterBot-0.0.2/banterbot/data/azure_neural_voices.py
+-rw-rw-rw-   0        0        0      455 2023-05-30 21:54:12.000000 BanterBot-0.0.2/banterbot/data/config.py
+-rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.2/banterbot/data/enums.py
+-rw-rw-rw-   0        0        0     2981 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/data/openai_models.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.164872 BanterBot-0.0.2/banterbot/gui/
+-rw-rw-rw-   0        0        0      185 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/gui/__init__.py
+-rw-rw-rw-   0        0        0     8550 2023-06-01 21:50:45.000000 BanterBot-0.0.2/banterbot/gui/banter_bot_interface.py
+-rw-rw-rw-   0        0        0     7048 2023-06-01 22:30:45.000000 BanterBot-0.0.2/banterbot/gui/banter_bot_tk.py
+-rw-rw-rw-   0        0        0     1626 2023-05-29 13:12:28.000000 BanterBot-0.0.2/banterbot/gui/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.188372 BanterBot-0.0.2/banterbot/utils/
+-rw-rw-rw-   0        0        0       67 2023-05-29 12:59:46.000000 BanterBot-0.0.2/banterbot/utils/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-05-31 21:31:32.000000 BanterBot-0.0.2/banterbot/utils/message.py
+-rw-rw-rw-   0        0        0     5725 2023-05-31 21:25:27.000000 BanterBot-0.0.2/banterbot/utils/nlp.py
+-rw-rw-rw-   0        0        0     7633 2023-05-31 22:27:47.000000 BanterBot-0.0.2/banterbot/utils/speech_to_text_output.py
+-rw-rw-rw-   0        0        0     3887 2023-05-30 21:54:12.000000 BanterBot-0.0.2/banterbot/utils/text_to_speech_output.py
+-rw-rw-rw-   0        0        0     2895 2023-05-28 15:33:48.000000 BanterBot-0.0.2/banterbot/utils/thread_queue.py
+-rw-rw-rw-   0        0        0     3097 2023-05-31 22:01:51.000000 BanterBot-0.0.2/banterbot/utils/word.py
+-rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-06-01 22:31:53.217873 BanterBot-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2189 2023-06-01 22:30:45.000000 BanterBot-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.190872 BanterBot-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.195371 BanterBot-0.0.2/tests/core/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     8818 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/core/test_openai_manager.py
+-rw-rw-rw-   0        0        0     2661 2023-06-01 22:30:45.000000 BanterBot-0.0.2/tests/core/test_text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:31:53.212372 BanterBot-0.0.2/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_message.py
+-rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_nlp.py
+-rw-rw-rw-   0        0        0     3087 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_text_to_speech_output.py
+-rw-rw-rw-   0        0        0     1239 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_text_to_speech_word.py
+-rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.2/tests/utils/test_thread_queue.py
```

### Comparing `BanterBot-0.0.1/BanterBot.egg-info/PKG-INFO` & `BanterBot-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1
-Name: BanterBot
-Version: 0.0.1
-Summary: ChatGPT-Powered Text-To-Speech Interaction
-Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBotarchive/v0.0.1.tar.gz
-Author: Gabriel S. Cabrera
-Author-email: gabriel.sigurd.cabrera@gmail.com
-Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,tts,chatbot
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # BanterBot
 
-BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses and Azure Neural Voices for text-to-speech synthesis. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
+BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses, Azure Neural Voices for text-to-speech synthesis, and Azure speech-to-text recognition. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
 
 ## Features
 
 * Employs OpenAI models for generating context-sensitive responses
 * Utilizes Azure Neural Voices for high-quality text-to-speech synthesis
 * Supports a variety of output formats, voices, and speaking styles
 * Enables real-time monitoring of the chatbot's responses
+* Features asynchronous speech-to-text microphone input
 * Provides an abstract base class for crafting frontends for the BanterBot application
 * Includes a tkinter-based frontend implementation
 
 ## Requirements
 
 Three environment variables are required for full functionality:
 
 * `OPENAI_API_KEY`: A valid OpenAI API key
-* `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for TTS functionality
+* `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for text-to-speech and speech-to-text functionality
 * `AZURE_SPEECH_REGION`: The region associated with your Azure Cognitive Services Speech API key
 
 ## Components
 
 ### OpenAIManager
 
 A class responsible for managing interactions with the OpenAI ChatCompletion API. It offers functionality to generate responses from the API based on input messages. It supports generating responses in their entirety or as a stream of response blocks.
 
 ### TextToSpeech
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
+### SpeechToText
+A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
+
 ### BanterBotInterface
 
-An abstract base class for designing frontends for the BanterBot application. It provides a high-level interface for managing conversations with the bot, including sending messages, receiving responses, and updating the conversation area.
+An abstract base class for designing frontends for the BanterBot application. It provides a high-level interface for managing conversations with the bot, including sending messages, receiving responses, and updating the conversation area. Accepts both keyboard inputs and microphone voice inputs.
 
 ### BanterBotTK
 
-A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses and Azure Neural Voices for text-to-speech. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
+A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
 
 ## Installation
 
+### Pip
+
+BanterBot is installable using the Python Package Index (PyPi):
+
+```bash
+python -m pip install banterbot
+```
+
+### Manual
+
 To install BanterBot, simply clone the repository and install the required dependencies:
 
 ```bash
 git clone https://github.com/gabrielscabrera/banterbot.git
 cd banterbot
 python -m pip install .
 ```
 
 ## Usage
 
+### Launch with Command Line
+
+Start BanterBot by running the `banterbot` command in your terminal. Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+
 ### Launch with a Python script
 
-To use BanterBot, just import the necessary components and create an instance of the BanterBotTK class:
+To use BanterBot in a script, create an instance of the `BanterBotTK` class and call the `run` method:
 
 ```python
-from banterbot import BanterBotTK
-from banterbot.data.azure_neural_voices import get_voice_by_name
-from banterbot.data.openai_models import openai_models
+from banterbot import BanterBotTK, get_voice_by_name, get_model_by_name
 
-model = openai_models["gpt-3.5-turbo"]
+model = get_model_by_name("gpt-3.5-turbo")
 voice = get_voice_by_name("Aria")
 style = "chat"
 
-app = BanterBotTK(model=model, voice=voice, style=style)
-app.run()
+# The three arguments `model`, `voice`, and `style` are optional.
+BBTK = BanterBotTK(model=model, voice=voice, style=style)
+BBTK.run()
 ```
 
-### Launch with Command Line
-
-Start the BanterBot Command Line Interface (CLI) by executing the `banterbot` command. Use the `-g` or `--gpt4` flags to enable GPT-4; this only works if you have GPT-4 API access.
-
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
 
 For a complete set of documentation, please refer to the [BanterBot Documentation](https://gabrielscabrera.github.io/BanterBot/).
```

### Comparing `BanterBot-0.0.1/BanterBot.egg-info/SOURCES.txt` & `BanterBot-0.0.2/BanterBot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 BanterBot.egg-info/dependency_links.txt
 BanterBot.egg-info/entry_points.txt
 BanterBot.egg-info/requires.txt
 BanterBot.egg-info/top_level.txt
 banterbot/__init__.py
 banterbot/core/__init__.py
 banterbot/core/openai_manager.py
+banterbot/core/speech_to_text.py
 banterbot/core/text_to_speech.py
 banterbot/data/__init__.py
 banterbot/data/azure_neural_voices.py
 banterbot/data/config.py
+banterbot/data/enums.py
 banterbot/data/openai_models.py
 banterbot/gui/__init__.py
 banterbot/gui/banter_bot_interface.py
 banterbot/gui/banter_bot_tk.py
 banterbot/gui/cli.py
 banterbot/utils/__init__.py
 banterbot/utils/message.py
 banterbot/utils/nlp.py
+banterbot/utils/speech_to_text_output.py
 banterbot/utils/text_to_speech_output.py
-banterbot/utils/text_to_speech_word.py
 banterbot/utils/thread_queue.py
+banterbot/utils/word.py
 tests/__init__.py
 tests/core/__init__.py
 tests/core/test_openai_manager.py
 tests/core/test_text_to_speech.py
 tests/utils/__init__.py
 tests/utils/test_message.py
 tests/utils/test_nlp.py
```

### Comparing `BanterBot-0.0.1/PKG-INFO` & `BanterBot-0.0.2/BanterBot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,112 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.1
-Summary: ChatGPT-Powered Text-To-Speech Interaction
+Version: 0.0.2
+Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBotarchive/v0.0.1.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.2-alpha/BanterBot-0.0.2.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
-Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,tts,chatbot
+Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # BanterBot
 
-BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses and Azure Neural Voices for text-to-speech synthesis. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
+BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses, Azure Neural Voices for text-to-speech synthesis, and Azure speech-to-text recognition. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
 
 ## Features
 
 * Employs OpenAI models for generating context-sensitive responses
 * Utilizes Azure Neural Voices for high-quality text-to-speech synthesis
 * Supports a variety of output formats, voices, and speaking styles
 * Enables real-time monitoring of the chatbot's responses
+* Features asynchronous speech-to-text microphone input
 * Provides an abstract base class for crafting frontends for the BanterBot application
 * Includes a tkinter-based frontend implementation
 
 ## Requirements
 
 Three environment variables are required for full functionality:
 
 * `OPENAI_API_KEY`: A valid OpenAI API key
-* `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for TTS functionality
+* `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for text-to-speech and speech-to-text functionality
 * `AZURE_SPEECH_REGION`: The region associated with your Azure Cognitive Services Speech API key
 
 ## Components
 
 ### OpenAIManager
 
 A class responsible for managing interactions with the OpenAI ChatCompletion API. It offers functionality to generate responses from the API based on input messages. It supports generating responses in their entirety or as a stream of response blocks.
 
 ### TextToSpeech
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
+### SpeechToText
+A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
+
 ### BanterBotInterface
 
-An abstract base class for designing frontends for the BanterBot application. It provides a high-level interface for managing conversations with the bot, including sending messages, receiving responses, and updating the conversation area.
+An abstract base class for designing frontends for the BanterBot application. It provides a high-level interface for managing conversations with the bot, including sending messages, receiving responses, and updating the conversation area. Accepts both keyboard inputs and microphone voice inputs.
 
 ### BanterBotTK
 
-A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses and Azure Neural Voices for text-to-speech. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
+A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
 
 ## Installation
 
+### Pip
+
+BanterBot is installable using the Python Package Index (PyPi):
+
+```bash
+python -m pip install banterbot
+```
+
+### Manual
+
 To install BanterBot, simply clone the repository and install the required dependencies:
 
 ```bash
 git clone https://github.com/gabrielscabrera/banterbot.git
 cd banterbot
 python -m pip install .
 ```
 
 ## Usage
 
+### Launch with Command Line
+
+Start BanterBot by running the `banterbot` command in your terminal. Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+
 ### Launch with a Python script
 
-To use BanterBot, just import the necessary components and create an instance of the BanterBotTK class:
+To use BanterBot in a script, create an instance of the `BanterBotTK` class and call the `run` method:
 
 ```python
-from banterbot import BanterBotTK
-from banterbot.data.azure_neural_voices import get_voice_by_name
-from banterbot.data.openai_models import openai_models
+from banterbot import BanterBotTK, get_voice_by_name, get_model_by_name
 
-model = openai_models["gpt-3.5-turbo"]
+model = get_model_by_name("gpt-3.5-turbo")
 voice = get_voice_by_name("Aria")
 style = "chat"
 
-app = BanterBotTK(model=model, voice=voice, style=style)
-app.run()
+# The three arguments `model`, `voice`, and `style` are optional.
+BBTK = BanterBotTK(model=model, voice=voice, style=style)
+BBTK.run()
 ```
 
-### Launch with Command Line
-
-Start the BanterBot Command Line Interface (CLI) by executing the `banterbot` command. Use the `-g` or `--gpt4` flags to enable GPT-4; this only works if you have GPT-4 API access.
-
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
 
 For a complete set of documentation, please refer to the [BanterBot Documentation](https://gabrielscabrera.github.io/BanterBot/).
```

### Comparing `BanterBot-0.0.1/banterbot/core/openai_manager.py` & `BanterBot-0.0.2/banterbot/core/openai_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import time
 from typing import Generator, Iterator, List, Union
 
 import openai
 
-from banterbot.data.config import OPENAI_API_KEY, RETRY_LIMIT
+from banterbot.data.config import RETRY_LIMIT
+from banterbot.data.enums import EnvVar
 from banterbot.data.openai_models import OpenAIModel
 from banterbot.utils.message import Message
 from banterbot.utils.nlp import NLP
 
 # Set the OpenAI API key
-openai.api_key = os.environ.get(OPENAI_API_KEY)
+openai.api_key = os.environ.get(EnvVar.OPENAI_API_KEY.value)
 
 
 class OpenAIManager:
     """
     A class that handles the interaction with the OpenAI ChatCompletion API. It provides functionality to generate
     responses from the API based on the input messages. It supports generating responses as a whole or as a stream of
     response blocks.
@@ -123,15 +124,15 @@
                 time.sleep(0.25)
 
         if not success:
             raise openai.error.APIError
 
         return response if stream else response.choices[0].message.content.strip()
 
-    def interrupt(self):
+    def interrupt(self) -> None:
         """
         Sets the interruption flag to True, which will stop the streaming response. This can be used to manually
         interrupt the streaming response if needed, for example, if the user sends a new message before the current
         response is completed.
         """
         self._interrupt = True
 
@@ -143,16 +144,16 @@
             messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
             **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
             and frequency_penalty.
 
         Returns:
-            List[str]: A list of sentences forming the response from the OpenAI API. This can be used to display the
-            generated response to the user or for further processing.
+            List[str]: A list of sentences forming the response from the OpenAI API. This can be used to display
+            the generated response to the user or for further processing.
         """
         response = self._request(messages=messages, stream=False, **kwargs)
         return NLP.segment_sentences(response)
 
     def prompt_stream(self, messages: List[Message], **kwargs) -> Generator[List[str], None, None]:
         """
         Sends messages to the OpenAI API and retrieves the response as a stream of blocks of sentences.
```

### Comparing `BanterBot-0.0.1/banterbot/core/text_to_speech.py` & `BanterBot-0.0.2/banterbot/core/text_to_speech.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import datetime
 import os
 import threading
 import time
-from typing import Dict, Generator, List, Optional
+from typing import Generator, List, Optional, TypedDict
 
 import azure.cognitiveservices.speech as speechsdk
 from azure.cognitiveservices.speech import SpeechSynthesisOutputFormat
 
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
-from banterbot.data.config import AZURE_SPEECH_KEY, AZURE_SPEECH_REGION
+from banterbot.data.enums import EnvVar, SpeechProcessingType, WordCategory
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
-from banterbot.utils.text_to_speech_word import TextToSpeechWord
+from banterbot.utils.word import Word
+
+
+class TimedEvent(TypedDict):
+    """
+    A specifically typed dictionary which is appended to the list of events in a TextToSpeech instance during speech
+    synthesis in a callback, containing the exact time at which the words in the event should be synthesized.
+    """
+
+    event: speechsdk.SessionEventArgs
+    time: int
 
 
 class TextToSpeech:
     """
     A class to handle text-to-speech synthesis utilizing Azure's Cognitive Services.
 
-    This class provides an interface to convert text into speech using Azure's Cognitive Services.
-    It supports various output formats, voices, and speaking styles. The synthesized speech can be
-    interrupted, and the progress can be monitored in real-time.
+    This class provides an interface to convert text into speech using Azure's Cognitive Services. It supports various
+    output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be
+    monitored in real-time.
     """
 
     # Create a lock that prevents race conditions when speaking
     _speech_lock = threading.Lock()
 
     def __init__(
         self,
@@ -35,52 +45,54 @@
         Args:
             output_format (SpeechSynthesisOutputFormat, optional): The desired output format for the synthesized speech.
                 Default is Audio16Khz32KBitRateMonoMp3.
         """
 
         # Initialize the speech configuration with the Azure subscription and region
         self._speech_config = speechsdk.SpeechConfig(
-            subscription=os.environ.get(AZURE_SPEECH_KEY),
-            region=os.environ.get(AZURE_SPEECH_REGION),
+            subscription=os.environ.get(EnvVar.AZURE_SPEECH_KEY.value),
+            region=os.environ.get(EnvVar.AZURE_SPEECH_REGION.value),
         )
 
         # Initialize the output and total length variables
         self._outputs: List[TextToSpeechOutput] = []
 
         # Initialize the speech synthesizer with the speech configuration
         self._synthesizer = speechsdk.SpeechSynthesizer(speech_config=self._speech_config)
 
         # Set the speech synthesis output format to the specified output format
         self._speech_config.set_speech_synthesis_output_format(output_format)
 
         # Connect the speech synthesizer events to their corresponding callbacks
         self._synthesizer_events_connect()
 
-        # Preconnecting the speech synthesizer for reduced latency
+        # Creating a new instance of Connection class
         self._connection = speechsdk.Connection.from_speech_synthesizer(self._synthesizer)
+
+        # Preconnecting the speech synthesizer for reduced latency
         self._connection.open(True)
 
-        # Reset the state variables of the TTS synthesizer
+        # Reset the state variables of the text-to-speech synthesizer
         self._reset()
 
     @property
     def output(self) -> List[TextToSpeechOutput]:
         """
         Getter for the output property, which is a list of TextToSpeechOutput objects.
 
         Returns:
             List[TextToSpeechOutput]: The list of synthesized outputs.
         """
         return self._outputs
 
     def interrupt(self) -> None:
         """
-        Interrupts an ongoing TTS process, if any.
+        Interrupts an ongoing text-to-speech process, if any.
 
-        This method sets the interrupt flag, which will cause the ongoing TTS process to stop.
+        This method sets the interrupt flag, which will cause the ongoing text-to-speech process to stop.
         """
         self._interrupt = True
 
     def _callback_completed(self, event: speechsdk.SessionEventArgs) -> None:
         """
         Callback function for synthesis completed event.
         Sets the synthesis completed flag to True.
@@ -88,46 +100,37 @@
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the synthesis completed.
         """
         self._synthesis_completed = True
 
     def _callback_started(self, event: speechsdk.SessionEventArgs) -> None:
         """
-        Callback function for synthesis started event.
-        Signals that the synthesis process has started.
+        Callback function for synthesis started event. Signals that the synthesis process has started.
 
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the synthesis started.
         """
         self._start_synthesis.set()
 
     def _callback_word_boundary(self, event: speechsdk.SessionEventArgs) -> None:
         """
         Callback function for word boundary event.
         Appends the boundary information to the boundaries list.
 
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the word boundary.
         """
-        # Check if the boundary is not a sentence boundary
+        # Check if the type is not a sentence boundary
         if event.boundary_type != speechsdk.SpeechSynthesisBoundaryType.Sentence:
 
-            # Calculate the offset and duration of the boundary in nanoseconds
-            offset_ns = 100 * event.audio_offset
-            duration = 1e9 * event.duration.total_seconds()
-
-            # Add the boundary information to the list of boundaries
-            self._boundaries.append(
+            # Add the event and timing information to the list of events
+            self._events.append(
                 {
-                    "offset_ns": offset_ns,
-                    "text": event.text,
-                    "word_length": event.word_length,
-                    "duration": duration,
-                    "boundary_type": event.boundary_type,
-                    "t_word": offset_ns + duration / event.word_length,
+                    "event": event,
+                    "time": 5e8 + 100 * event.audio_offset + 1e9 * event.duration.total_seconds() / event.word_length,
                 }
             )
 
     def _create_ssml(self, text: str, voice: str, style: Optional[str] = None) -> str:
         """
         Creates an SSML string from the given text, voice, and style.
 
@@ -157,150 +160,150 @@
 
         # Close the voice and speak tags and return the SSML string
         ssml += "</voice></speak>"
         return ssml
 
     def _reset(self) -> None:
         """
-        Resets the state variables of the TTS synthesizer.
-
-        This method resets the state variables, such as the list of boundaries, synthesis completed flag,
-        synthesis started flag, and interrupt flag.
+        Resets the state variables of the text-to-speech synthesizer, such as the list of events, synthesis timer,
+        synthesis started flag, synthesis completed flag, and interrupt flag.
         """
         # Reset the list of boundaries that have been processed
-        self._boundaries: List[Dict[str, str]] = []
+        self._events: List[TimedEvent] = []
 
-        # Reset the synthesis completed, synthesis started, and interrupt flags
+        # Reset the synthesis threading.Event, set the start timer to None, and reset the interrupt & completed flags
         self._interrupt = False
+        self._start_timer = None
         self._synthesis_completed = False
         self._start_synthesis = threading.Event()
 
     def _synthesizer_events_connect(self) -> None:
         """
-        Connects the TTS synthesizer events to their corresponding callbacks.
+        Connects the text-to-speech synthesizer events to their corresponding callbacks.
 
-        This method connects the synthesis_started, synthesis_word_boundary, synthesis_canceled,
-        and synthesis_completed events to their respective callback functions.
+        This method connects the synthesis_started, synthesis_word_boundary, synthesis_canceled, and synthesis_completed
+        events to their respective callback functions.
         """
         # Connect the synthesis_started event to the _callback_started method
         self._synthesizer.synthesis_started.connect(self._callback_started)
 
         # Connect the synthesis_word_boundary event to the _callback_word_boundary method
         self._synthesizer.synthesis_word_boundary.connect(self._callback_word_boundary)
 
         # Connect the synthesis_canceled and synthesis_completed events to the _callback_completed method
         self._synthesizer.synthesis_canceled.connect(self._callback_completed)
         self._synthesizer.synthesis_completed.connect(self._callback_completed)
 
-    def _process_boundary(
-        self, boundary: dict, word_index: int, timestamp: datetime.datetime, output: TextToSpeechOutput
-    ) -> TextToSpeechWord:
+    def _process_boundary(self, word_index: int) -> Word:
         """
-        Processes a synthesis boundary and updates the output and total length.
+        Processes a synthesis boundary event and returns an instance of class Word.
 
         Args:
-            boundary (dict): The synthesis boundary to be processed.
-            word_index (int): The index of the current word.
-            timestamp (datetime.datetime): The timestamp of the current boundary.
-            output (TextToSpeechOutput): The output object to which the processed word will be added.
+            word_index (int): The index of the word relative to the full text.
 
         Returns:
-            TextToSpeechWord: The processed word with contextual information.
+            Word: The processed word with contextual information.
         """
-        text = boundary["text"]
-        if word_index > 0 and boundary["boundary_type"] == speechsdk.SpeechSynthesisBoundaryType.Word:
-            text = f" {text}"
-        word = TextToSpeechWord(
-            word=text, timestamp=timestamp, word_index=word_index, category=boundary["boundary_type"]
+        event = self._events[word_index]["event"]
+        whitespace = ""
+        if event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Word:
+            category = WordCategory.WORD
+            if word_index > 0:
+                whitespace = " "
+        elif event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Punctuation:
+            category = WordCategory.PUNCTUATION
+
+        word = Word(
+            word=whitespace + event.text,
+            offset=datetime.timedelta(microseconds=event.audio_offset / 10),
+            duration=event.duration,
+            category=category,
+            source=SpeechProcessingType.TTS,
         )
         return word
 
-    def _process_callbacks(self, output: TextToSpeechOutput) -> Generator[TextToSpeechWord, None, bool]:
+    def _process_callbacks(self, output: TextToSpeechOutput) -> Generator[Word, None, bool]:
         """
         Monitors the synthesis progress and updates the output accordingly.
 
-        This method continuously checks the synthesis progress and processes the boundaries.
-        It updates the output object with the processed words and yields them one by one.
+        This method continuously checks the synthesis progress and processes the boundaries. It updates the output
+        object with the processed words and yields them one by one.
 
         Args:
             output (TextToSpeechOutput): The output object to which the processed words will be added.
 
         Yields:
-            TextToSpeechWord: A word with contextual information.
+            Word: A word with contextual information.
 
         Returns:
             bool: True if the process completed successfully, False otherwise.
         """
         # Initialize variables
         word_index = 0
-        self._interrupt = False
-        self._outputs.append(output)
-        status = False
+        success = False
 
         # Wait until the synthesis has started before proceeding
         self._start_synthesis.wait()
-
-        # Record the start time
-        start_time = time.perf_counter_ns()
+        self._start_timer = time.perf_counter_ns()
 
         # Continuously monitor the synthesis progress
-        while not self._interrupt and (not self._synthesis_completed or word_index < len(self._boundaries)):
+        while not self._interrupt and (not self._synthesis_completed or word_index < len(self._events)):
 
-            current_time = time.perf_counter_ns()
-            elapsed_time = current_time - start_time
+            dt = time.perf_counter_ns() - self._start_timer
 
-            while (
-                not self._interrupt
-                and word_index < len(self._boundaries)
-                and elapsed_time >= self._boundaries[word_index]["t_word"]
-            ):
-                word = self._process_boundary(self._boundaries[word_index], word_index, current_time, output)
+            while not self._interrupt and word_index < len(self._events) and dt >= self._events[word_index]["time"]:
+                word = self._process_boundary(word_index=word_index)
                 output.append(word)
                 word_index += 1
                 yield word
 
             # Wait for a short amount of time before checking the synthesis progress again
             time.sleep(0.005)
 
         if not self._interrupt:
-            status = True
+            success = True
 
         # Stop the synthesizer
         self._synthesizer.stop_speaking()
-        return status
+        return success
 
-    def _speak(self, ssml: str):
+    def _speak(self, ssml: str) -> None:
         self._synthesizer.speak_ssml(ssml)
 
-    def speak(self, input_string: str, voice: AzureNeuralVoice, style: str) -> Generator[TextToSpeechWord, None, bool]:
+    def speak(self, input_string: str, voice: AzureNeuralVoice, style: str) -> Generator[Word, None, bool]:
         """
         Speaks the given text using the specified voice and style.
 
-        This method converts the input text into speech using the specified voice and style.
-        It yields the synthesized words one by one, along with their contextual information.
+        This method converts the input text into speech using the specified voice and style. It yields the synthesized
+        words one by one, along with their contextual information.
 
         Args:
             input_string (str): The input string that is to be converted into speech.
             voice (AzureNeuralVoice): The voice to be used.
             style (str): The speaking style to be applied.
 
         Yields:
-            TextToSpeechWord: A word with contextual information.
+            Word: A word with contextual information.
         """
         # Create SSML markup for the given input_string, voice, and style
         ssml = self._create_ssml(input_string, voice, style)
 
-        # Prepare an instance of TextToSpeechOutput while will yield values iteratively
-        output = TextToSpeechOutput(input_string=input_string, voice=voice, style=style)
+        # Create a new thread to handle the speech synthesis
+        speech_thread = threading.Thread(target=self._speak, args=(ssml,), daemon=True)
 
         with self.__class__._speech_lock:
 
             # Reset all state attributes
             self._reset()
 
-            # Create a new thread to handle the speech synthesis, and start it
-            speech_thread = threading.Thread(target=self._speak, args=(ssml,), daemon=True)
+            # Prepare an instance of TextToSpeechOutput while will receive values iteratively
+            output = TextToSpeechOutput(
+                input_string=input_string, timestamp=datetime.datetime.now(), voice=voice, style=style
+            )
+            self._outputs.append(output)
+
+            # Starting the speech synthesizer
             speech_thread.start()
 
-            # Continuously monitor the synthesis progress in the main thread
+            # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
             for word in self._process_callbacks(output):
                 yield word
```

### Comparing `BanterBot-0.0.1/banterbot/data/azure_neural_voices.py` & `BanterBot-0.0.2/banterbot/data/azure_neural_voices.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 """
 This program defines a dataclass and utility functions to represent and manage Azure Neural Voice profiles for speech
 synthesis. The main components of the program are:
 
     1.  AzureNeuralVoice dataclass: Represents an Azure Neural Voice profile with attributes such as name, voice
         identifier, gender, pitch, and available styles (tones/emotions).
 
-    2.  neural_voices: A dictionary containing instances of AzureNeuralVoice for each available voice profile.
+    2.  _neural_voices: A dictionary containing instances of AzureNeuralVoice for each available voice profile.
 
     3.  Utility functions:>
             a.  get_voice_by_name(name: str) -> AzureNeuralVoice: Retrieves an AzureNeuralVoice instance by its name.
 
-            b.  get_voices_by_gender(gender: Literal[MALE, FEMALE]) -> List[AzureNeuralVoice]: Retrieves a list of
+            b.  get_voices_by_gender(gender: AzureNeuralVoiceGender) -> List[AzureNeuralVoice]: Retrieves a list of
             AzureNeuralVoice instances with the specified gender.
 
 The purpose of this program is to provide an organized and easily accessible representation of Azure Neural Voice
 profiles for speech synthesis. Users can utilize the provided data and utility functions to easily retrieve voice
 profiles based on their requirements (e.g., gender, pitch, or available styles).
 """
 
 from dataclasses import dataclass
-from typing import List, Literal
+from typing import List
 
-from banterbot.data.config import FEMALE, MALE
+from banterbot.data.enums import AzureNeuralVoiceGender
 
 
 @dataclass
 class AzureNeuralVoice:
     """
     A dataclass representing an Azure Neural Voice profile for speech synthesis.
 
     Attributes:
         name (str): The name of the voice profile.
         voice (str): The voice identifier used by Azure Text-to-Speech API.
-        gender (Literal[MALE, FEMALE]): The gender of the voice (either MALE or FEMALE).
+        gender (AzureNeuralVoiceGender): The gender of the voice (either MALE or FEMALE).
         pitch (int): The relative (by gender) pitch level of the voice, where a lower value indicates a lower pitch.
         styles (List[str]): The available styles (i.e., tones/emotions) for the voice.
     """
 
     name: str
     voice: str
-    gender: Literal[MALE, FEMALE]
+    gender: AzureNeuralVoiceGender
     pitch: int
     styles: List[str]
 
 
 # Dictionary containing voice profile data
 _neural_voice_data = {
     "Aria": {
-        "gender": FEMALE,
+        "gender": AzureNeuralVoiceGender.FEMALE,
         "pitch": 3,
         "voice": "en-US-AriaNeural",
         "styles": [
             "angry",
             "chat",
             "cheerful",
             "customerservice",
@@ -66,15 +66,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Davis": {
-        "gender": MALE,
+        "gender": AzureNeuralVoiceGender.MALE,
         "pitch": 0,
         "voice": "en-US-DavisNeural",
         "styles": [
             "angry",
             "chat",
             "cheerful",
             "excited",
@@ -84,15 +84,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Guy": {
-        "gender": MALE,
+        "gender": AzureNeuralVoiceGender.MALE,
         "pitch": 3,
         "voice": "en-US-GuyNeural",
         "styles": [
             "angry",
             "cheerful",
             "excited",
             "friendly",
@@ -102,15 +102,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Jane": {
-        "gender": FEMALE,
+        "gender": AzureNeuralVoiceGender.FEMALE,
         "pitch": 4,
         "voice": "en-US-JaneNeural",
         "styles": [
             "angry",
             "cheerful",
             "excited",
             "friendly",
@@ -119,15 +119,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Jason": {
-        "gender": MALE,
+        "gender": AzureNeuralVoiceGender.MALE,
         "pitch": 2,
         "voice": "en-US-JasonNeural",
         "styles": [
             "angry",
             "cheerful",
             "excited",
             "friendly",
@@ -136,15 +136,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Jenny": {
-        "gender": FEMALE,
+        "gender": AzureNeuralVoiceGender.FEMALE,
         "pitch": 0,
         "voice": "en-US-JennyNeural",
         "styles": [
             "angry",
             "assistant",
             "chat",
             "cheerful",
@@ -157,15 +157,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Nancy": {
-        "gender": FEMALE,
+        "gender": AzureNeuralVoiceGender.FEMALE,
         "pitch": 2,
         "voice": "en-US-NancyNeural",
         "styles": [
             "angry",
             "cheerful",
             "excited",
             "friendly",
@@ -174,15 +174,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Sara": {
-        "gender": FEMALE,
+        "gender": AzureNeuralVoiceGender.FEMALE,
         "pitch": 1,
         "voice": "en-US-SaraNeural",
         "styles": [
             "angry",
             "cheerful",
             "excited",
             "friendly",
@@ -191,15 +191,15 @@
             "shouting",
             "terrified",
             "unfriendly",
             "whispering",
         ],
     },
     "Tony": {
-        "gender": MALE,
+        "gender": AzureNeuralVoiceGender.MALE,
         "pitch": 1,
         "voice": "en-US-TonyNeural",
         "styles": [
             "angry",
             "cheerful",
             "excited",
             "friendly",
@@ -210,37 +210,37 @@
             "unfriendly",
             "whispering",
         ],
     },
 }
 
 # Create instances of AzureNeuralVoice for each voice in the dictionary
-neural_voices = {name: AzureNeuralVoice(name=name, **voice) for name, voice in _neural_voice_data.items()}
+_neural_voices = {name: AzureNeuralVoice(name=name, **voice) for name, voice in _neural_voice_data.items()}
 
 
 def get_voice_by_name(name: str) -> AzureNeuralVoice:
     """
     Retrieve an AzureNeuralVoice instance by its name.
 
     Args:
         name (str): The name of the voice profile.
 
     Returns:
         AzureNeuralVoice: The corresponding AzureNeuralVoice instance.
 
     Raises:
-        KeyError: If the specified name is not found in the neural_voices dictionary.
+        KeyError: If the specified name is not found in the _neural_voices dictionary.
     """
-    return neural_voices[name]
+    return _neural_voices[name]
 
 
-def get_voices_by_gender(gender: Literal[MALE, FEMALE]) -> List[AzureNeuralVoice]:
+def get_voices_by_gender(gender: AzureNeuralVoiceGender) -> List[AzureNeuralVoice]:
     """
     Retrieve a list of AzureNeuralVoice instances with the specified gender.
 
     Args:
-        gender (Literal[MALE, FEMALE]): The gender of the voices to retrieve (either MALE or FEMALE).
+        gender (AzureNeuralVoiceGender): The gender of the voices to retrieve (either AzureNeuralVoiceGender.MALE or AzureNeuralVoiceGender.FEMALE).
 
     Returns:
         List[AzureNeuralVoice]: A list of AzureNeuralVoice instances with the specified gender.
     """
-    return [voice for voice in neural_voices.values() if voice.gender == gender]
+    return [voice for voice in _neural_voices.values() if voice.gender == gender]
```

### Comparing `BanterBot-0.0.1/banterbot/data/openai_models.py` & `BanterBot-0.0.2/banterbot/data/openai_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 This module provides an overview of the GPT models offered by OpenAI as of May 2023 for the ChatCompletion API. Each
 model entry is represented by an instance of the OpenAIModel class, which provides information about the model's name,
 maximum tokens, version, rank, and tokenizer.
 
+    1.  OpenAIModel dataclass: Represents an OpenAI ChatCompletion model with attributes such as name, max_tokens
+        version, rank, and a tokenizer.
+
+    2.  _openai_models: A dictionary containing instances of OpenAIModel for each available model.
+
+    3.  get_model_by_name(name: str) -> OpenAIModel: Retrieves an OpenAIModel instance by its name.
+
 The purpose of this module is to make it easy for users to access information about the available GPT models and their
 properties. This can be useful when selecting a model for a specific task or when working with the ChatCompletion API.
-
-Attributes:
-    openai_models (Dict[str, OpenAIModel]): A dictionary containing instances of OpenAIModel for each available model.
 """
-
 from dataclasses import dataclass
 from typing import Dict
 
 import tiktoken
 from tiktoken.core import Encoding
 
 
@@ -42,15 +45,15 @@
         The tokenizer attribute is an instance of the tiktoken package's Encoding object, which is used to tokenize text
         for the specific GPT model.
         """
         self.tokenizer: Encoding = tiktoken.encoding_for_model(self.name)
 
 
 # Define the available OpenAI models
-openai_models_dict = {
+_openai_models_dict = {
     "gpt-3.5-turbo": {
         "max_tokens": 4095,
         "version": 3,
         "rank": 2,
     },
     "gpt-4": {
         "max_tokens": 8191,
@@ -61,10 +64,26 @@
         "max_tokens": 32767,
         "version": 4,
         "rank": 1,
     },
 }
 
 # Create instances of OpenAIModel for each model in the dictionary
-openai_models: Dict[str, OpenAIModel] = {
-    name: OpenAIModel(name=name, **model) for name, model in openai_models_dict.items()
+_openai_models: Dict[str, OpenAIModel] = {
+    name: OpenAIModel(name=name, **model) for name, model in _openai_models_dict.items()
 }
+
+
+def get_model_by_name(name: str) -> OpenAIModel:
+    """
+    Retrieve an OpenAIModel instance by its name.
+
+    Args:
+        name (str): The name of the OpenAI ChatCompletion model.
+
+    Returns:
+        OpenAIModel: The corresponding OpenAIModel instance.
+
+    Raises:
+        KeyError: If the specified name is not found in the _openai_models dictionary.
+    """
+    return _openai_models[name]
```

### Comparing `BanterBot-0.0.1/banterbot/gui/banter_bot_interface.py` & `BanterBot-0.0.2/banterbot/gui/banter_bot_tk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,162 @@
-import datetime
-import threading
-from abc import ABC, abstractmethod
-from typing import List, Optional
-
-from banterbot.core.openai_manager import OpenAIManager
-from banterbot.core.text_to_speech import TextToSpeech
-from banterbot.data.azure_neural_voices import AzureNeuralVoice
-from banterbot.data.config import chat_logs
-from banterbot.data.openai_models import OpenAIModel
-from banterbot.utils.message import Message
-from banterbot.utils.thread_queue import ThreadQueue
+import tkinter as tk
+from tkinter import ttk
 
+from banterbot.data.azure_neural_voices import AzureNeuralVoice, get_voice_by_name
+from banterbot.data.openai_models import OpenAIModel, get_model_by_name
+from banterbot.gui.banter_bot_interface import BanterBotInterface
 
-class BanterBotInterface(ABC):
+
+class BanterBotTK(tk.Tk, BanterBotInterface):
     """
-    BanterBotInterface is an abstract base class for creating frontends for the BanterBot application. It provides a
-    high-level interface for managing conversation with the bot, including sending messages, receiving responses, and
-    updating the conversation area.
+    BanterBotTK is a graphical user interface (GUI) for a chatbot application that uses OpenAI models for generating
+    responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text recognition. The class inherits from
+    both tkinter.Tk and BanterBotInterface, providing a seamless integration of the chatbot functionality with a
+    user-friendly interface.
+
+    The GUI allows users to interact with the chatbot by entering their name and message, and it displays the
+    conversation history in a scrollable text area. Users can send messages by pressing the "Send" button or the "Enter"
+    key. The chatbot's responses are generated using the specified OpenAI model and can be played back using the
+    specified Azure Neural Voice. Additionally, users can toggle speech-to-text input by pressing the "Listen" button.
     """
 
-    def __init__(self, model: OpenAIModel, voice: AzureNeuralVoice, style: str) -> None:
+    def __init__(
+        self,
+        model: OpenAIModel = get_model_by_name("gpt-3.5-turbo"),
+        voice: AzureNeuralVoice = get_voice_by_name("Aria"),
+        style: str = "chat",
+    ) -> None:
         """
-        Initialize the BanterBotInterface with the given model, voice, and style.
+        Initialize the BanterBotTK class, which inherits from both tkinter.Tk and BanterBotInterface.
 
         Args:
-            model (OpenAIModel): The OpenAI model to use for generating responses.
-            voice (AzureNeuralVoice): The voice to use for text-to-speech synthesis.
-            style (str): The speaking style to use for text-to-speech synthesis.
-        """
-        self._openai_manager = OpenAIManager(model=model)
-        self._text_to_speech = TextToSpeech()
-        self._messages: List[Message] = []
-        self._output_lock = threading.Lock()
-        self._log_lock = threading.Lock()
-        self._log_path = chat_logs / f"chat_{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}.txt"
-        self._response_thread = None
-        self._thread_queue = ThreadQueue()
-        self._voice = voice
-        self._style = style
-        self._init_gui()
+            model (OpenAIModel, optional): The OpenAI model to be used for generating responses.
+            voice (AzureNeuralVoice, optional): The Azure Neural Voice to be used for text-to-speech.
+            style (str, optional): The style of the conversation (e.g., "cheerful", "sad", "chat").
+        """
+        tk.Tk.__init__(self)
+        BanterBotInterface.__init__(self, model=model, voice=voice, style=style)
+        self._listening = False
 
-    @abstractmethod
     def _init_gui(self) -> None:
         """
-        Initialize the graphical user interface for the frontend.
-        This method should be implemented by subclasses to create the specific GUI components.
+        Initialize the graphical user interface for the BanterBot application.
+        This method sets up the main window, conversation area, input fields, and buttons.
         """
+        self.title("BanterBot")
+        self.configure(bg="black")
+        self.geometry("1024x768")
+        self._font = ("Cascadia Code", 16)
+
+        self.style = ttk.Style()
+        self.style.theme_use("clam")
+        self.style.configure(".", font=self._font, bg="black", fg="white")
+        self.style.configure("Vertical.TScrollbar", background="black", bordercolor="black", arrowcolor="black")
+
+        self.history_frame = ttk.Frame(self)
+        self.conversation_area = tk.Text(
+            self.history_frame, wrap=tk.WORD, state=tk.DISABLED, bg="black", fg="white", font=self._font
+        )
+        self.conversation_area.grid(row=0, column=0, ipadx=5, padx=5, pady=5, sticky="nsew")
+        self.history_frame.rowconfigure(0, weight=1)
+        self.history_frame.columnconfigure(0, weight=1)
+
+        self.scrollbar = ttk.Scrollbar(self.history_frame, command=self.conversation_area.yview)
+        self.scrollbar.grid(row=0, column=1, sticky="ns")
+        self.conversation_area["yscrollcommand"] = self.scrollbar.set
+
+        self.history_frame.grid(row=0, column=0, padx=10, pady=10, sticky="nsew")
+        self.rowconfigure(0, weight=1)
+        self.columnconfigure(0, weight=1)
 
-    @abstractmethod
-    def update_conversation_area(self, word: str) -> None:
-        """
-        Update the conversation area with the given word, and add the word to the chat log.
-        This method should be implemented by subclasses to handle updating the specific GUI components.
+        self.entry_frame = ttk.Frame(self)
+        self.entry_frame.grid(row=1, column=0, padx=10, pady=10, sticky="nsew")
 
-        Args:
-            word (str): The word to add to the conversation area.
-        """
-        self._append_to_chat_log(word)
+        self.name_entry = tk.Entry(
+            self.entry_frame, bg="black", fg="white", insertbackground="white", font=self._font, width=12
+        )
+        self.name_entry.grid(row=0, column=0, padx=(5, 0), pady=5, sticky="nsew")
+        self.name_entry.insert(0, "User")
+        self.name_entry.bind("<FocusIn>", self.select_all_on_focus)
+        self._name_entry_focused = False
 
-    def send_message(self, user_message: str, name: Optional[str] = None) -> None:
-        """
-        Send a message from the user to the conversation.
+        self.message_entry = tk.Entry(
+            self.entry_frame, bg="black", fg="white", insertbackground="white", font=self._font
+        )
+        self.message_entry.grid(row=0, column=1, padx=(5, 5), pady=5, sticky="nsew")
+        self.message_entry.focus_set()
+        self.entry_frame.columnconfigure(1, weight=1)
 
-        Args:
-            user_message (str): The message content from the user.
-            name (Optional[str]): The name of the user sending the message. Defaults to None.
-        """
-        message = Message(role="user", name=name, content=user_message)
-        text = f"{message.name.title() if message.name is not None else 'User'}: {user_message}\n\n"
-        self._messages.append(message)
-        self.update_conversation_area(word=text)
+        self.send_btn = ttk.Button(self.entry_frame, text="Send", command=self.prompt, width=7)
+        self.send_btn.grid(row=0, column=2, padx=(0, 5), pady=5, sticky="nsew")
 
-    def prompt(self, user_message: str, name: Optional[str] = None) -> None:
+        self.listen_btn = ttk.Button(self.entry_frame, text="Listen", command=self.toggle_listen, width=7)
+        self.listen_btn.grid(row=0, column=3, padx=(0, 5), pady=5, sticky="nsew")
+
+        self.message_entry.bind("<Return>", lambda event: self.prompt())
+
+    def update_conversation_area(self, word: str) -> None:
         """
-        Prompt the bot with the given user message.
+        Update the conversation area with the given word.
 
         Args:
-            user_message (str): The message content from the user.
-            name (Optional[str]): The name of the user sending the message. Defaults to None.
+            word (str): The word to be added to the conversation area.
         """
-        if self._thread_queue.is_alive():
-            self._openai_manager.interrupt()
-            self._text_to_speech.interrupt()
-
-        self._message_thread = threading.Thread(
-            target=self.send_message,
-            args=(
-                user_message,
-                name,
-            ),
-            daemon=True,
-        )
-        self._thread_queue.add_task(self._message_thread, unskippable=True)
+        super().update_conversation_area(word)
+        self.conversation_area["state"] = tk.NORMAL
+        self.conversation_area.insert(tk.END, word)
+        self.conversation_area.update_idletasks()
+        self.conversation_area["state"] = tk.DISABLED
+        self.conversation_area.see(tk.END)
 
-        self._response_thread = threading.Thread(target=self.get_response, daemon=True)
-        self._thread_queue.add_task(self._response_thread)
-
-    def _append_to_chat_log(self, word: str) -> None:
+    def select_all_on_focus(self, event) -> None:
         """
-        Updates the chat log with the latest output.
+        Select all text in the widget when it receives focus.
 
         Args:
-            word (str): The word to be added to the conversation area.
+            event: The event object containing information about the focus event.
         """
-        with self._log_lock:
-            with open(self._log_path, "a+") as fs:
-                fs.write(word)
+        widget = event.widget
+        if widget == self.name_entry:
+            self._name_entry_focused = True
+            widget.selection_range(0, tk.END)
+            widget.icursor(tk.END)
+        else:
+            self._name_entry_focused = False
 
-    def get_response(self) -> None:
+    def reset_on_send(self) -> None:
         """
-        Get a response from the bot and update the conversation area with the response. This method handles generating
-        the bot's response using the OpenAIManager and updating the conversation area with the response text using
-        text-to-speech synthesis.
+        Reset the focus state of the name entry field after sending a message.
         """
-        prefixed = False
-        content = []
-        for block in self._openai_manager.prompt_stream(messages=self._messages):
-            if not prefixed:
-                self.update_conversation_area("Assistant: ")
-                prefixed = True
-
-            sentences = " ".join(block)
-            for word in self._text_to_speech.speak(sentences, voice=self._voice, style=self._style):
-                self.update_conversation_area(word.word)
-                content.append(word.word)
+        self._name_entry_focused = False
 
-            self.update_conversation_area(" ")
-            content.append(" ")
+    def toggle_listen(self) -> None:
+        """
+        Toggle the speech-to-text functionality.
+        """
+        if self.listening:
+            self.listen_btn["text"] = "Listen"
+        else:
+            self.listen_btn["text"] = "Stop"
 
-        content = "".join(content)
-        self._messages.append(Message(role="assistant", content=content.strip()))
-        self.end_response()
+        user_name = self.name_entry.get().split(" ")[0].strip()
+        super().toggle_listen(user_name)
 
-    def end_response(self) -> None:
+    def prompt(self) -> None:
         """
-        End the bot's response and update the conversation area accordingly. This method should be called after the
-        bot's response has been fully generated and added to the conversation area.
+        Prompt the user for input and process the message.
+        This method retrieves the user's name and message, and then calls the superclass's prompt method.
         """
-        self.update_conversation_area("\n\n")
+        user_name = self.name_entry.get().split(" ")[0].strip()
+        user_message = self.message_entry.get()
+        if not user_message:
+            return
+        else:
+            super().prompt(user_message, user_name)
+            self.message_entry.delete(0, tk.END)
 
-    @abstractmethod
     def run(self) -> None:
         """
-        Run the frontend application.
-        This method should be implemented by subclasses to handle the main event loop of the specific GUI framework.
+        Run the BanterBot application.
+        This method starts the main event loop of the tkinter application.
         """
+        self.mainloop()
```

### Comparing `BanterBot-0.0.1/banterbot/gui/cli.py` & `BanterBot-0.0.2/banterbot/gui/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 
-from banterbot.data.openai_models import openai_models
+from banterbot.data.openai_models import get_model_by_name
 from banterbot.gui.banter_bot_tk import BanterBotTK
 
 
 def run() -> None:
     """
     The main function to run the BanterBot Command Line Interface.
 
@@ -30,15 +30,13 @@
         "-g",
         "--gpt4",
         action="store_true",
         dest="gpt4",
         help="Enable GPT-4; only works if you have GPT-4 API access.",
     )
 
-    args = parser.parse_args()
-
     kwargs = {
-        "model": openai_models["gpt-4"] if args.gpt4 else openai_models["gpt-3.5-turbo"],
+        "model": get_model_by_name("gpt-4") if args.gpt4 else get_model_by_name("gpt-3.5-turbo"),
     }
 
     gui = BanterBotTK(**kwargs)
     gui.run()
```

### Comparing `BanterBot-0.0.1/banterbot/utils/message.py` & `BanterBot-0.0.2/banterbot/utils/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from dataclasses import dataclass
-from typing import Dict, Literal, Optional
+from typing import Dict, Optional
 
-from banterbot.data.config import ASSISTANT, SYSTEM, USER
+from banterbot.data.enums import ChatCompletionRoles
 from banterbot.data.openai_models import OpenAIModel
 
 
 @dataclass
 class Message:
     """
     Represents a message that can be sent to the OpenAI ChatCompletion API.
 
     The purpose of this class is to create a structured representation of a message that can be easily converted into a
     format compatible with the OpenAI API. This class is designed to be used in conjunction with the OpenAI
     ChatCompletion API to generate context-aware responses from an AI model.
 
     Attributes:
-        role (Literal[ASSISTANT, SYSTEM, USER]): The role of the message sender.
+        role (ChatCompletionRoles): The role of the message sender.
             - ASSISTANT: Represents a message sent by the AI assistant.
             - SYSTEM: Represents a message sent by the system, usually containing instructions or context.
             - USER: Represents a message sent by the user interacting with the AI assistant.
 
         content (str): The content of the message.
 
         name (Optional[str]): The name of the message sender. This is an optional field and can be used to provide a
         more personalized experience by addressing the sender by their name.
     """
 
-    role: Literal[ASSISTANT, SYSTEM, USER]
+    role: ChatCompletionRoles
     content: str
     name: Optional[str] = None
 
     def count_tokens(self, model: OpenAIModel) -> int:
         """
         Counts the number of tokens in the current message.
```

### Comparing `BanterBot-0.0.1/banterbot/utils/nlp.py` & `BanterBot-0.0.2/banterbot/utils/nlp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 
 import spacy
 
-from banterbot.data.config import EN_CORE_WEB_MD, EN_CORE_WEB_SM
+from banterbot.data.enums import SpaCyLangModel
 
 
 class NLP:
     """
     A comprehensive toolkit that provides a set of Natural Language Processing utilities. It leverages the capabilities
     of the SpaCy package. The toolkit is designed to automatically download the necessary models if they are not
     available.
@@ -20,22 +20,32 @@
     def _init_models(cls) -> None:
         """
         Initializes and configures the required SpaCy models for sentence segmentation and keyword extraction.
         This method is called upon import to ensure that the necessary models are available and configured.
         """
         cls._models = {}
 
-        # Define a set of pipeline components to disable for the sentence segmenter.
-        segmenter_disable = ["tok2vec", "tagger", "parser", "attribute_ruler", "lemmatizer", "ner"]
-        segmenter = cls._load_model(name=EN_CORE_WEB_SM, disable=segmenter_disable)
-        # Enable the sentence segmentation pipeline component for the segmenter model.
-        segmenter.enable_pipe("senter")
-
-        cls._models["segmenter"] = segmenter
-        cls._models[EN_CORE_WEB_MD] = cls._load_model(name=EN_CORE_WEB_MD)
+        # Define a set of pipeline components to disable for the sentence senter.
+        senter_disable = ["tok2vec", "tagger", "parser", "attribute_ruler", "lemmatizer", "ner"]
+        senter = cls._load_model(name=SpaCyLangModel.EN_CORE_WEB_SM.value, disable=senter_disable)
+        # Enable the sentence segmentation pipeline component for the senter model.
+        senter.enable_pipe("senter")
+
+        rules = {}
+        splitter = cls._load_model(name=SpaCyLangModel.EN_CORE_WEB_MD.value)
+        # Customize the tokenization rules for the word splitter in order to prevent splitting of contractions.
+        ignore = ("'", "’", "‘")
+        for key, value in splitter.tokenizer.rules.items():
+            if all(i not in key for i in ignore):
+                rules[key] = value
+        splitter.tokenizer.rules = rules
+
+        cls._models["senter"] = senter
+        cls._models["splitter"] = splitter
+        cls._models[SpaCyLangModel.EN_CORE_WEB_MD.value] = cls._load_model(name=SpaCyLangModel.EN_CORE_WEB_MD.value)
 
     @classmethod
     def _load_model(cls, *, name: str, **kwargs) -> spacy.language.Language:
         """
         Loads a SpaCy model by its name. If the model is not available, it is downloaded automatically.
 
         Args:
@@ -74,36 +84,60 @@
 
         Returns:
             spacy.language.Language: The requested SpaCy model.
         """
         return cls._models[name]
 
     @classmethod
-    def segment_sentences(cls, string: str) -> Tuple[str, ...]:
+    def segment_sentences(cls, string: str, whitespace: bool = True) -> Tuple[str, ...]:
         """
-        Splits a text string into individual sentences using a specialized SpaCy model. The model is a lightweight version
-        of `en_core_web_sm` designed specifically for sentence segmentation.
+        Splits a text string into individual sentences using a specialized SpaCy model. The model is a lightweight
+        version of `en_core_web_sm` designed specifically for sentence segmentation.
 
         Args:
             string (str): The input text string.
+            whitespace (str): If True, keep whitespace at the beginning/end of sentences; if False, strip it.
 
         Returns:
             Tuple[str, ...]: A tuple of individual sentences as strings.
         """
-        return tuple(sentence.text_with_ws for sentence in cls._models["segmenter"](string).sents)
+        return tuple(
+            sentence.text_with_ws if whitespace else sentence.text for sentence in cls._models["senter"](string).sents
+        )
+
+    @classmethod
+    def segment_words(cls, string: str, whitespace: bool = True) -> Tuple[str, ...]:
+        """
+        Splits a text string into individual words using a specialized SpaCy model. The model is customized version of
+        `en_core_web_md` in which words are not split on apostrophes, in order to preserve contractions.
+
+        Args:
+            string (str): The input text string.
+            whitespace (str): If True, include whitespace characters between words; if False, omit it.
+
+        Returns:
+            Tuple[str, ...]: A tuple of individual words as strings.
+        """
+        words = []
+        for word in cls._models["splitter"](string):
+            words.append(word.text)
+            if whitespace and word.whitespace_:
+                words.append(word.whitespace_)
+
+        return tuple(words)
 
     @classmethod
     def extract_keywords(cls, string: str) -> Tuple[str, ...]:
         """
         Extracts keywords from a text string using the `en_core_web_md` SpaCy model.
 
         Args:
             string (str): The input text string.
 
         Returns:
             Tuple[str, ...]: A tuple of extracted keywords as strings.
         """
-        return tuple([str(entity) for entity in cls._models[EN_CORE_WEB_MD](string).ents])
+        return tuple([str(entity) for entity in cls._models[SpaCyLangModel.EN_CORE_WEB_MD.value](string).ents])
 
 
 # Upon import, NLP initializes and downloads (if necessary) all models.
 NLP._init_models()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `BanterBot-0.0.1/banterbot/utils/text_to_speech_output.py` & `BanterBot-0.0.2/banterbot/utils/text_to_speech_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,94 @@
+import datetime
 from typing import Iterator, List
 
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
-from banterbot.utils.text_to_speech_word import TextToSpeechWord
+from banterbot.utils.word import Word
 
 
 class TextToSpeechOutput:
     """
     The TextToSpeechOutput class encapsulates the output of a text-to-speech conversion, providing a convenient
     interface for working with and manipulating the converted data. This class is designed to store the input text, the
-    voice and style used for conversion, and the list of TextToSpeechWord objects representing the individual words in
-    the output.
+    timestamp, the voice and style used for conversion, and the list of Word objects representing the individual words
+    in the output.
 
     The primary use case for this class is to store the output of a text-to-speech conversion and provide an easy way to
-    access and manipulate the words in the output. This can be useful for applications that require further processing
-    or analysis of the converted text, such as natural language processing or speech synthesis.
+    access the words in the output. This can be useful for applications that require further processing or analysis of
+    the converted text, such as natural language processing or speech synthesis.
     """
 
-    def __init__(self, input_string: str, voice: AzureNeuralVoice, style: str) -> None:
+    def __init__(self, input_string: str, timestamp: datetime.datetime, voice: AzureNeuralVoice, style: str) -> None:
         """
         Initializes a new TextToSpeechOutput instance, setting up the input string and preparing the words list for the
         converted words.
 
         Args:
             input_string (str): The input string that is to be converted into speech.
 
+            timestamp (datetime.datetime): The time at which the speech began.
+
             voice (AzureNeuralVoice): The voice to be used for the text-to-speech conversion. This should be an instance
             of the AzureNeuralVoice class, which represents a specific voice available in the Azure Cognitive Services
             Text-to-Speech API.
 
             style (str): The speaking style to be applied to the text-to-speech conversion. This should be a string
             representing one of the available speaking styles in the Azure Cognitive Services Text-to-Speech API, such
             as "cheerful", "sad", or "angry".
         """
         self.input_string = input_string
+        self.timestamp = timestamp
         self.voice = voice
         self.style = style
 
-        self.words: List[TextToSpeechWord] = []
+        self.words: List[Word] = []
 
-    def __getitem__(self, idx: int) -> TextToSpeechWord:
+    def __getitem__(self, idx: int) -> Word:
         """
         Allows for indexing into the TextToSpeechOutput object to retrieve words at specific positions.
 
         Args:
             idx (int): The index of the word to retrieve.
 
         Returns:
-            TextToSpeechWord: The word at the specified index.
+            Word: The word at the specified index.
         """
         return self.words[idx]
 
-    def __iter__(self) -> Iterator[TextToSpeechWord]:
+    def __iter__(self) -> Iterator[Word]:
         """
-        Provides an iterator to iterate over the TextToSpeechWord objects in the output.
+        Provides an iterator to iterate over the Word objects in the output.
 
         Yields:
-            TextToSpeechWord: The next TextToSpeechWord object in the output.
+            Word: The next Word object in the output.
         """
         for word in self.words:
             yield word
 
     def __len__(self) -> int:
         """
         Allows for the use of len() on a TextToSpeechOutput instance, returning the number of words in the output.
 
         Returns:
             int: The number of words in the output.
         """
         return len(self.words)
 
-    def __setitem__(self, idx: int, value: TextToSpeechWord) -> None:
-        """
-        Allows for setting the value of a word at a specific index in the output.
-
-        Args:
-            idx (int): The index of the word to be replaced.
-
-            value (TextToSpeechWord): The new word to be placed at the specified index. This should be an instance of
-            the TextToSpeechWord class, which represents a single word in the text-to-speech output along with its
-            associated metadata.
-        """
-        self.words[idx] = value
-
     def __str__(self) -> str:
         """
         Converts the TextToSpeechOutput instance into a string, concatenating all the words in the output.
 
         Returns:
             str: The string representation of the text-to-speech output. This will be a concatenation of all the words
             in the output, in the order they appear in the words list.
         """
         return "".join(word.word for word in self.words)
 
-    def append(self, entry: TextToSpeechWord) -> None:
+    def append(self, entry: Word) -> None:
         """
-        Appends a TextToSpeechWord object to the words list in the output.
+        Appends a Word object to the words list in the output.
 
         Args:
-            entry (TextToSpeechWord): The word to be appended to the output. This should be an instance of the
-            TextToSpeechWord class, which represents a single word in the text-to-speech output along with its
-            associated metadata.
+            entry (Word): The word to be appended to the output. This should be an instance of the Word class, which
+            represents a single word in the text-to-speech output along with its associated metadata.
         """
         self.words.append(entry)
```

### Comparing `BanterBot-0.0.1/banterbot/utils/text_to_speech_word.py` & `BanterBot-0.0.2/banterbot/utils/word.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import datetime
 from dataclasses import dataclass
+from typing import Optional
 
 import azure.cognitiveservices.speech as speechsdk
 
+from banterbot.data.enums import SpeechProcessingType, WordCategory
+
 
 @dataclass(frozen=True)
-class TextToSpeechWord:
+class Word:
     """
-    This class encapsulates a word in the output of a text-to-speech conversion. It includes the word itself, the timestamp when the word was spoken, its index in the text, and its category (e.g., word, punctuation), using Azure's Speech Synthesis Boundary Type.
-
-    The purpose of this class is to provide a structured representation of a word in the output of a text-to-speech
-    conversion, allowing for easy access to its properties and enabling further processing or analysis of the spoken
-    text.
+    This class encapsulates a word in the output of a text-to-speech synthesis or input from a speech-to-text
+    recognition. It includes the word itself and the timestamp when the word was spoken. Optionally, its category (e.g.,
+    word, punctuation using Azure's Speech Synthesis Boundary Type), and its confidence score can be included too.
 
     Attributes:
-        word (str): The word that has been converted to speech.
-        timestamp (datetime.datetime): The datetime when the word was spoken.
-        word_index (int): The position of the word in the original text.
-        category (speechsdk.SpeechSynthesisBoundaryType): The category of the word (e.g., word, punctuation).
+        word (str): The word that has been synthesized/recognized.
+        offset (datetime.timedelta): Time elapsed between initialization and synthesis/recognition.
+        duration (datetime.timedelta): Amount of time required for the word to be fully spoken.
+        category (WordCategory): The category of the text contents.
+        confidence (Optional[int]): The confidence score (for speech-to-text) for the given word.
+        source: SpeechProcessingType: Whether the word's source is text-to-speech (TTS) or speech-to-text (STT).
     """
 
     word: str
-    timestamp: datetime.datetime
-    word_index: int
-    category: speechsdk.SpeechSynthesisBoundaryType
+    offset: datetime.timedelta
+    duration: datetime.timedelta
+    category: WordCategory
+    source: SpeechProcessingType
+    confidence: Optional[float] = None
 
     def __len__(self) -> int:
         """
         Computes and returns the length of the word.
 
         This method is useful for determining the length of the word without having to access the `word` attribute
-        directly. It can be used, for example, in filtering or sorting operations on a list of `TextToSpeechWord`
+        directly. It can be used, for example, in filtering or sorting operations on a list of `Word`
         instances.
 
         Returns:
             int: The length of the word.
         """
         return len(self.word)
 
@@ -42,23 +47,30 @@
         """
         Provides a string representation of the instance, including the word and its timestamp.
 
         This method is useful for displaying a human-readable representation of the instance, which can be helpful for
         debugging or logging purposes.
 
         Returns:
-            str: A string containing the word and its timestamp in ISO 8601 format.
+            str: A string containing the word, the time elapsed since the beginning of speech synthesis, and its source.
         """
-        description = f"<TextToSpeechWord '{self.word}' at {self.timestamp}>"
+        description = (
+            f"<"
+            "word: '{self.word}' "
+            f"| offset: {self.offset.seconds}s "
+            f"| duration: {self.duration.seconds}s "
+            f"| source: {self.source}"
+            ">"
+        )
         return description
 
     def __repr__(self) -> str:
         """
         Returns the word itself as its string representation. This simplifies the display of the object in certain
-        contexts, such as when printing a list of `TextToSpeechWord` instances.
+        contexts, such as when printing a list of `Word` instances.
 
         This method is called by built-in Python functions like `repr()` and is used, for example, when displaying the
         object in an interactive Python session or when printing a list containing the object.
 
         Returns:
             str: The word itself.
         """
```

### Comparing `BanterBot-0.0.1/banterbot/utils/thread_queue.py` & `BanterBot-0.0.2/banterbot/utils/thread_queue.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/core/test_openai_manager.py` & `BanterBot-0.0.2/tests/core/test_openai_manager.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/core/test_text_to_speech.py` & `BanterBot-0.0.2/tests/core/test_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/utils/test_message.py` & `BanterBot-0.0.2/tests/utils/test_message.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/utils/test_nlp.py` & `BanterBot-0.0.2/tests/utils/test_nlp.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/utils/test_text_to_speech_output.py` & `BanterBot-0.0.2/tests/utils/test_text_to_speech_output.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/utils/test_text_to_speech_word.py` & `BanterBot-0.0.2/tests/utils/test_text_to_speech_word.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.1/tests/utils/test_thread_queue.py` & `BanterBot-0.0.2/tests/utils/test_thread_queue.py`

 * *Files identical despite different names*

