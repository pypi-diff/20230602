# Comparing `tmp/gpt4-openai-api-0.3.0.tar.gz` & `tmp/gpt4-openai-api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gpt4-openai-api-0.3.0.tar", last modified: Sat May 20 10:57:13 2023, max compression
+gzip compressed data, was "dist\gpt4-openai-api-0.4.0.tar", last modified: Fri Jun  2 17:58:02 2023, max compression
```

## Comparing `gpt4-openai-api-0.3.0.tar` & `gpt4-openai-api-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.876604 gpt4-openai-api-0.3.0/
--rw-rw-rw-   0        0        0     5826 2023-05-20 10:57:13.875604 gpt4-openai-api-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.825606 gpt4-openai-api-0.3.0/gpt4_openai/
--rw-rw-rw-   0        0        0     2607 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/gpt4_openai/__init__.py
--rw-rw-rw-   0        0        0    24200 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/gpt4_openai/driver.py
-drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.865604 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/
--rw-rw-rw-   0        0        0     5826 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 10:57:13.877604 gpt4-openai-api-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.872604 gpt4-openai-api-0.3.0/test/
--rw-rw-rw-   0        0        0      460 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/test/test-browsing.py
--rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/test/test.py
--rw-rw-rw-   0        0        0      997 2023-05-07 23:29:24.000000 gpt4-openai-api-0.3.0/test/test_langchain.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.082621 gpt4-openai-api-0.4.0/
+-rw-rw-rw-   0        0        0     5005 2023-06-02 17:58:02.080621 gpt4-openai-api-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.022624 gpt4-openai-api-0.4.0/gpt4_openai/
+-rw-rw-rw-   0        0        0     1366 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/gpt4_openai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.059627 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/
+-rw-rw-rw-   0        0        0     5005 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:58:02.082621 gpt4-openai-api-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-02 17:57:20.000000 gpt4-openai-api-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.077626 gpt4-openai-api-0.4.0/test/
+-rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.4.0/test/test.py
+-rw-rw-rw-   0        0        0      637 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/test/test_browsing.py
+-rw-rw-rw-   0        0        0      987 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/test/test_langchain.py
+-rw-rw-rw-   0        0        0      931 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/test/test_plugins.py
```

### Comparing `gpt4-openai-api-0.3.0/PKG-INFO` & `gpt4-openai-api-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,129 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.3.0
-Summary: Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser
+Version: 0.4.0
+Summary: Python package for unofficial GPT-4 API access via chat.openai.com
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
-License: UNKNOWN
-Description: # GPT4 OpenAI unofficial API
-        
-        ## Unofficial GPT-4 API access via chat.openai.com using Selenium
-        
-        Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. It uses [selenium webdriver](https://www.selenium.dev/) to emulate user interaction on [chat.openai.com](chat.openai.com). If the account has `ChatGPT Plus`, the driver **will use GPT-4**, otherwise it will use the default GPT-3.5.
-        
-        It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
-        
-        **Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
-        
-        The core logic was taken from the [IntelligenzaArtificiale/Free-Auto-GPT](https://github.com/IntelligenzaArtificiale/Free-Auto-GPT).
-        
-        ## Demo
-        
-        ![Demo GIF](https://user-images.githubusercontent.com/18037362/236707120-e93d40bc-b73b-4f72-bc7d-d0449a082946.gif)
-        
-        ## Demo script
-        
-        ```python
-        from gpt4_openai import GPT4OpenAI
-        
-        # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4')
-        # GPT3.5 will answer 8, while GPT4 should be smart enough to answer 10
-        response = llm('If there are 10 books in a room and I read 2, how many books are still in the room?')
-        print(response)
-        ```
-        
-        As seen on the demo gif (above), GPT-4 answers correctly.
-        
-        ## Browsing support
-        
-        ```python
-        from gpt4_openai import GPT4OpenAI
-        
-        # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4-browsing')
-        # ChatGPT will first browse the web for the name/age of her boyfriend, then return the answer
-        response = llm('What is the age difference between Dua Lipa and her boyfriend?')
-        print(response)
-        ```
-        
-        ## Langchain support
-        
-        `GPT4OpenAI` actually extends `LLM` class from `langchain.llms.base`. So you can easily use this library inside langchain ecosystem. Example:
-        
-        ```python
-        from gpt4_openai import GPT4OpenAI
-        from langchain import LLMChain
-        from langchain.prompts.chat import (ChatPromptTemplate, SystemMessagePromptTemplate, AIMessagePromptTemplate, HumanMessagePromptTemplate)
-        
-        template="You are a helpful assistant that translates english to pirate."
-        system_message_prompt = SystemMessagePromptTemplate.from_template(template)
-        example_human = HumanMessagePromptTemplate.from_template("Hi")
-        example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
-        human_message_prompt = HumanMessagePromptTemplate.from_template("{text}")
-        
-        chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
-        
-        # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token)
-        
-        chain = LLMChain(llm=llm, prompt=chat_prompt)
-        print(chain.run("My name is John and I like to eat pizza."))
-        ```
-        
-        Output will be:
-        ```
-        AI: Ahoy, me name be John an' I be likin' ta feast on some pizza, arr!
-        ```
-        
-        ## How to get the session token
-        
-        1. Go to https://chat.openai.com and open the developer tools by `F12`.
-        2. Find the `__Secure-next-auth.session-token` cookie in `Application` > `Storage` > `Cookies` > `https://chat.openai.com`.
-        3. Copy the value in the `Cookie Value` field.
-        
-        ![image](https://user-images.githubusercontent.com/19218518/206170122-61fbe94f-4b0c-4782-a344-e26ac0d4e2a7.png)
-        
-        ## OpenAI's GPT4 vs other providers
-        
-        Initially, I tried [poe.com ](https://poe.com/) (private API implemented at [gpt4free](https://github.com/gptforfree/gpt4free/tree/main/quora)), but noticed that input context window is smaller than one of OpenAI ChatGPT. And the same goes for Bing's GPT4.
-        
-        ## Installation
-        
-        To install this Python package, run the following command:
-        
-        ```bash
-        pip install gpt4-openai-api
-        ```
-        
-        ## Dependencies
-        
-        These dependencies get downloaded directly:
-        
-        - `undetected-chromedriver` (selenium browser)
-        - `markdownify`
-        - `langchain`
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# GPT4 OpenAI unofficial API
+
+## Unofficial GPT-4 API access via chat.openai.com using Selenium
+
+Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. If the account has `ChatGPT Plus`, you can use **GPT-4**.
+
+It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
+
+**Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
+
+The core logic was taken from the [acheong08/ChatGPT](https://github.com/acheong08/ChatGPT).
+
+## Demo
+
+![Demo GIF](https://user-images.githubusercontent.com/18037362/236707120-e93d40bc-b73b-4f72-bc7d-d0449a082946.gif)
+
+## Demo script
+
+```python
+from gpt4_openai import GPT4OpenAI
+
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=my_token, model='gpt-4')
+# GPT3.5 will answer 8, while GPT4 should be smart enough to answer 10
+response = llm('If there are 10 books in a room and I read 2, how many books are still in the room?')
+print(response)
+```
+
+As seen on the demo gif (above), GPT-4 answers correctly.
+
+## Browsing support
+
+```python
+from gpt4_openai import GPT4OpenAI
+
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=my_token, model='gpt-4-browsing')
+# ChatGPT will first browse the web for the name/age of her boyfriend, then return the answer
+response = llm('What is the age difference between Dua Lipa and her boyfriend?')
+print(response)
+```
+
+## Plugin support
+
+List of plugin IDs can be [found here](https://github.com/acheong08/ChatGPT/blob/main/docs/plugins.json).
+
+```python
+llm = GPT4OpenAI(token=my_token, model='gpt-4',
+                 plugin_ids=['plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51'] # Wolfram Alpha
+                 )
+
+# ChatGPT will use Wolfram Alpha plugin to calculate the equation
+response = llm('Calculate the square root of 12345 to 10 decimal places')
+print(response)
+```
+
+## Langchain support
+
+`GPT4OpenAI` actually extends `LLM` class from `langchain.llms.base`. So you can easily use this library inside langchain ecosystem. Example:
+
+```python
+from gpt4_openai import GPT4OpenAI
+from langchain import LLMChain
+from langchain.prompts.chat import (ChatPromptTemplate, SystemMessagePromptTemplate, AIMessagePromptTemplate, HumanMessagePromptTemplate)
+
+template="You are a helpful assistant that translates english to pirate."
+system_message_prompt = SystemMessagePromptTemplate.from_template(template)
+example_human = HumanMessagePromptTemplate.from_template("Hi")
+example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
+human_message_prompt = HumanMessagePromptTemplate.from_template("{text}")
+
+chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
+
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=my_token)
+
+chain = LLMChain(llm=llm, prompt=chat_prompt)
+print(chain.run("My name is John and I like to eat pizza."))
+```
+
+Output will be:
+```
+AI: Ahoy, me name be John an' I be likin' ta feast on some pizza, arr!
+```
+
+## How to get the access token
+
+1. Go to https://chat.openai.com/api/auth/session
+2. In the JSON, copy the whole `accessToken` field.
+
+![image](https://github.com/Erol444/gpt4-openai-api/assets/18037362/c0bdfd9c-8ad1-48ca-8344-621a4513e04b)
+
+## OpenAI's GPT4 vs other providers
+
+Initially, I tried [poe.com ](https://poe.com/) (private API implemented at [gpt4free](https://github.com/gptforfree/gpt4free/tree/main/quora)), but noticed that input context window is smaller than one of OpenAI ChatGPT. And the same goes for Bing's GPT4.
+
+## Installation
+
+To install this Python package, run the following command:
+
+```bash
+pip install gpt4-openai-api
+```
+
+## Dependencies
+
+These dependencies get downloaded directly:
+
+- `revChatGPT` ([acheong08/ChatGPT](https://github.com/acheong08/ChatGPT))
+- `langchain`
```

### Comparing `gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/PKG-INFO` & `gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,129 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.3.0
-Summary: Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser
+Version: 0.4.0
+Summary: Python package for unofficial GPT-4 API access via chat.openai.com
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
-License: UNKNOWN
-Description: # GPT4 OpenAI unofficial API
-        
-        ## Unofficial GPT-4 API access via chat.openai.com using Selenium
-        
-        Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. It uses [selenium webdriver](https://www.selenium.dev/) to emulate user interaction on [chat.openai.com](chat.openai.com). If the account has `ChatGPT Plus`, the driver **will use GPT-4**, otherwise it will use the default GPT-3.5.
-        
-        It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
-        
-        **Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
-        
-        The core logic was taken from the [IntelligenzaArtificiale/Free-Auto-GPT](https://github.com/IntelligenzaArtificiale/Free-Auto-GPT).
-        
-        ## Demo
-        
-        ![Demo GIF](https://user-images.githubusercontent.com/18037362/236707120-e93d40bc-b73b-4f72-bc7d-d0449a082946.gif)
-        
-        ## Demo script
-        
-        ```python
-        from gpt4_openai import GPT4OpenAI
-        
-        # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4')
-        # GPT3.5 will answer 8, while GPT4 should be smart enough to answer 10
-        response = llm('If there are 10 books in a room and I read 2, how many books are still in the room?')
-        print(response)
-        ```
-        
-        As seen on the demo gif (above), GPT-4 answers correctly.
-        
-        ## Browsing support
-        
-        ```python
-        from gpt4_openai import GPT4OpenAI
-        
-        # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4-browsing')
-        # ChatGPT will first browse the web for the name/age of her boyfriend, then return the answer
-        response = llm('What is the age difference between Dua Lipa and her boyfriend?')
-        print(response)
-        ```
-        
-        ## Langchain support
-        
-        `GPT4OpenAI` actually extends `LLM` class from `langchain.llms.base`. So you can easily use this library inside langchain ecosystem. Example:
-        
-        ```python
-        from gpt4_openai import GPT4OpenAI
-        from langchain import LLMChain
-        from langchain.prompts.chat import (ChatPromptTemplate, SystemMessagePromptTemplate, AIMessagePromptTemplate, HumanMessagePromptTemplate)
-        
-        template="You are a helpful assistant that translates english to pirate."
-        system_message_prompt = SystemMessagePromptTemplate.from_template(template)
-        example_human = HumanMessagePromptTemplate.from_template("Hi")
-        example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
-        human_message_prompt = HumanMessagePromptTemplate.from_template("{text}")
-        
-        chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
-        
-        # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token)
-        
-        chain = LLMChain(llm=llm, prompt=chat_prompt)
-        print(chain.run("My name is John and I like to eat pizza."))
-        ```
-        
-        Output will be:
-        ```
-        AI: Ahoy, me name be John an' I be likin' ta feast on some pizza, arr!
-        ```
-        
-        ## How to get the session token
-        
-        1. Go to https://chat.openai.com and open the developer tools by `F12`.
-        2. Find the `__Secure-next-auth.session-token` cookie in `Application` > `Storage` > `Cookies` > `https://chat.openai.com`.
-        3. Copy the value in the `Cookie Value` field.
-        
-        ![image](https://user-images.githubusercontent.com/19218518/206170122-61fbe94f-4b0c-4782-a344-e26ac0d4e2a7.png)
-        
-        ## OpenAI's GPT4 vs other providers
-        
-        Initially, I tried [poe.com ](https://poe.com/) (private API implemented at [gpt4free](https://github.com/gptforfree/gpt4free/tree/main/quora)), but noticed that input context window is smaller than one of OpenAI ChatGPT. And the same goes for Bing's GPT4.
-        
-        ## Installation
-        
-        To install this Python package, run the following command:
-        
-        ```bash
-        pip install gpt4-openai-api
-        ```
-        
-        ## Dependencies
-        
-        These dependencies get downloaded directly:
-        
-        - `undetected-chromedriver` (selenium browser)
-        - `markdownify`
-        - `langchain`
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# GPT4 OpenAI unofficial API
+
+## Unofficial GPT-4 API access via chat.openai.com using Selenium
+
+Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. If the account has `ChatGPT Plus`, you can use **GPT-4**.
+
+It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
+
+**Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
+
+The core logic was taken from the [acheong08/ChatGPT](https://github.com/acheong08/ChatGPT).
+
+## Demo
+
+![Demo GIF](https://user-images.githubusercontent.com/18037362/236707120-e93d40bc-b73b-4f72-bc7d-d0449a082946.gif)
+
+## Demo script
+
+```python
+from gpt4_openai import GPT4OpenAI
+
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=my_token, model='gpt-4')
+# GPT3.5 will answer 8, while GPT4 should be smart enough to answer 10
+response = llm('If there are 10 books in a room and I read 2, how many books are still in the room?')
+print(response)
+```
+
+As seen on the demo gif (above), GPT-4 answers correctly.
+
+## Browsing support
+
+```python
+from gpt4_openai import GPT4OpenAI
+
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=my_token, model='gpt-4-browsing')
+# ChatGPT will first browse the web for the name/age of her boyfriend, then return the answer
+response = llm('What is the age difference between Dua Lipa and her boyfriend?')
+print(response)
+```
+
+## Plugin support
+
+List of plugin IDs can be [found here](https://github.com/acheong08/ChatGPT/blob/main/docs/plugins.json).
+
+```python
+llm = GPT4OpenAI(token=my_token, model='gpt-4',
+                 plugin_ids=['plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51'] # Wolfram Alpha
+                 )
+
+# ChatGPT will use Wolfram Alpha plugin to calculate the equation
+response = llm('Calculate the square root of 12345 to 10 decimal places')
+print(response)
+```
+
+## Langchain support
+
+`GPT4OpenAI` actually extends `LLM` class from `langchain.llms.base`. So you can easily use this library inside langchain ecosystem. Example:
+
+```python
+from gpt4_openai import GPT4OpenAI
+from langchain import LLMChain
+from langchain.prompts.chat import (ChatPromptTemplate, SystemMessagePromptTemplate, AIMessagePromptTemplate, HumanMessagePromptTemplate)
+
+template="You are a helpful assistant that translates english to pirate."
+system_message_prompt = SystemMessagePromptTemplate.from_template(template)
+example_human = HumanMessagePromptTemplate.from_template("Hi")
+example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
+human_message_prompt = HumanMessagePromptTemplate.from_template("{text}")
+
+chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
+
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=my_token)
+
+chain = LLMChain(llm=llm, prompt=chat_prompt)
+print(chain.run("My name is John and I like to eat pizza."))
+```
+
+Output will be:
+```
+AI: Ahoy, me name be John an' I be likin' ta feast on some pizza, arr!
+```
+
+## How to get the access token
+
+1. Go to https://chat.openai.com/api/auth/session
+2. In the JSON, copy the whole `accessToken` field.
+
+![image](https://github.com/Erol444/gpt4-openai-api/assets/18037362/c0bdfd9c-8ad1-48ca-8344-621a4513e04b)
+
+## OpenAI's GPT4 vs other providers
+
+Initially, I tried [poe.com ](https://poe.com/) (private API implemented at [gpt4free](https://github.com/gptforfree/gpt4free/tree/main/quora)), but noticed that input context window is smaller than one of OpenAI ChatGPT. And the same goes for Bing's GPT4.
+
+## Installation
+
+To install this Python package, run the following command:
+
+```bash
+pip install gpt4-openai-api
+```
+
+## Dependencies
+
+These dependencies get downloaded directly:
+
+- `revChatGPT` ([acheong08/ChatGPT](https://github.com/acheong08/ChatGPT))
+- `langchain`
```

### Comparing `gpt4-openai-api-0.3.0/setup.py` & `gpt4-openai-api-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 root = Path(__file__).parent.resolve()
 readme_file = root / 'readme.md'
 long_description = readme_file.read_text(encoding='utf-8')
 
 setup(
     name="gpt4-openai-api",
-    version="0.3.0",
-    description="Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser",
+    version="0.4.0",
+    description="Python package for unofficial GPT-4 API access via chat.openai.com",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Erol444",
     author_email="erol123444@gmail.com",
     url="https://github.com/Erol444/gpt4-openai-api",
     packages=["gpt4_openai"],
     install_requires=[
-        "undetected-chromedriver>=3.4.6",
-        "markdownify>=0.11.6",
+        "revChatGPT==6.0.1",
         "langchain",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gpt4-openai-api-0.3.0/test/test_langchain.py` & `gpt4-openai-api-0.4.0/test/test_langchain.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 system_message_prompt = SystemMessagePromptTemplate.from_template(template)
 example_human = HumanMessagePromptTemplate.from_template("Hi")
 example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
 human_message_prompt = HumanMessagePromptTemplate.from_template("{text}")
 
 chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
 
-# Token is the __Secure-next-auth.session-token from chat.openai.com
-llm = GPT4OpenAI(token=os.environ["OPENAI_SESSION_TOKEN"])
+# accessToken from https://chat.openai.com/api/auth/session
+llm = GPT4OpenAI(token=os.environ["OPENAI_ACCESS_TOKEN"])
 chain = LLMChain(llm=llm, prompt=chat_prompt)
 print(chain.run("My name is John and I like to eat pizza."))
```

