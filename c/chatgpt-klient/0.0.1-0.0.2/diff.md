# Comparing `tmp/chatgpt-klient-0.0.1.tar.gz` & `tmp/chatgpt-klient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.0.1.tar", last modified: Fri Jun  2 09:54:27 2023, max compression
+gzip compressed data, was "chatgpt-klient-0.0.2.tar", last modified: Fri Jun  2 10:22:06 2023, max compression
```

## Comparing `chatgpt-klient-0.0.1.tar` & `chatgpt-klient-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 09:54:27.773649 chatgpt-klient-0.0.1/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-02 09:54:27.773649 chatgpt-klient-0.0.1/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.1/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-06-02 09:53:29.000000 chatgpt-klient-0.0.1/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-06-02 09:54:27.773649 chatgpt-klient-0.0.1/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 09:54:27.765649 chatgpt-klient-0.0.1/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 09:54:27.769649 chatgpt-klient-0.0.1/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5335 2023-06-02 06:39:23.000000 chatgpt-klient-0.0.1/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.1/src/chatgpt_klient/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 09:54:27.773649 chatgpt-klient-0.0.1/src/chatgpt_klient.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-02 09:54:27.000000 chatgpt-klient-0.0.1/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      293 2023-06-02 09:54:27.000000 chatgpt-klient-0.0.1/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-06-02 09:54:27.000000 chatgpt-klient-0.0.1/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-06-02 09:54:27.000000 chatgpt-klient-0.0.1/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-06-02 09:54:27.000000 chatgpt-klient-0.0.1/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.494628 chatgpt-klient-0.0.2/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-02 10:22:06.490628 chatgpt-klient-0.0.2/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.2/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-06-02 10:20:12.000000 chatgpt-klient-0.0.2/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-06-02 10:22:06.494628 chatgpt-klient-0.0.2/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.486628 chatgpt-klient-0.0.2/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.490628 chatgpt-klient-0.0.2/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-06-02 10:20:30.000000 chatgpt-klient-0.0.2/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5338 2023-06-02 10:11:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.2/src/chatgpt_klient/consts.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.490628 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/top_level.txt
```

### Comparing `chatgpt-klient-0.0.1/src/chatgpt_klient/__init__.py` & `chatgpt-klient-0.0.2/src/chatgpt_klient/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-__version__ = "0.0.3"
-
 import openai
 import tiktoken
+import time
 from logutils import get_logger
-from consts import MAX_TOKENS, SUPPORTED_ENGINES, ENGINES0, ENGINES1
+from chatgpt_klient.consts import MAX_TOKENS, SUPPORTED_ENGINES, ENGINES0, ENGINES1
 from rich.console import Console
 
 logger = get_logger(__name__)
 console = Console()
 
 
 class ChatGPTPrompt:
@@ -119,15 +118,14 @@
             try:
                 r = self.send_prompt(text=input_text, max_tokens=max_tokens)
             except openai.error.RateLimitError:
                 logger.warning("You are sending requests too fast. Delaying 20s...")
                 time.sleep(20)
                 r = self.send_prompt(text=input_text, max_tokens=max_tokens)
 
-
             console.print(f"[bold green]ChatGPT>[/] [green]{r}[/]")
             self.msg_history["messages"].append(
                 {
                     "role": "assistant",
                     "content": r,
                 }
             )
```

### Comparing `chatgpt-klient-0.0.1/src/chatgpt_klient/consts.py` & `chatgpt-klient-0.0.2/src/chatgpt_klient/consts.py`

 * *Files identical despite different names*

