# Comparing `tmp/openai_forward-0.2.2.tar.gz` & `tmp/openai_forward-0.2.3.tar.gz`

## Comparing `openai_forward-0.2.2.tar` & `openai_forward-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/__init__.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/__main__.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/app.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/base.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/config.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/openai.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.2/LICENSE
--rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 openai_forward-0.2.2/README.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 openai_forward-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 openai_forward-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/__main__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/app.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/base.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/config.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/openai.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.3/LICENSE
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 openai_forward-0.2.3/README.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 openai_forward-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 openai_forward-0.2.3/PKG-INFO
```

### Comparing `openai_forward-0.2.2/openai_forward/__main__.py` & `openai_forward-0.2.3/openai_forward/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
             workers=workers,
             app_dir="..",
             ssl_keyfile=ssl_keyfile,
             ssl_certfile=ssl_certfile,
         )
 
     @staticmethod
-    def convert(
-        log_path: str = "./Log/chat.log", target_path: str = "./Log/chat.jsonl"
-    ):
+    def convert(log_path: str = "./Log/chat.log", target_path: str = "./Log/chat.json"):
         """Convert log file  to jsonl file"""
         from openai_forward.tool import convert_chatlog_to_jsonl
 
         print(f"Convert {log_path} to {target_path}")
         convert_chatlog_to_jsonl(log_path, target_path)
```

### Comparing `openai_forward-0.2.2/openai_forward/base.py` & `openai_forward-0.2.3/openai_forward/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     IP_BLACKLIST = env2list("IP_BLACKLIST", sep=" ")
 
     if ROUTE_PREFIX:
         if ROUTE_PREFIX.endswith("/"):
             ROUTE_PREFIX = ROUTE_PREFIX[:-1]
         if not ROUTE_PREFIX.startswith("/"):
             ROUTE_PREFIX = "/" + ROUTE_PREFIX
-    timeout = 60
+    timeout = 600
 
     print_startup_info(
         BASE_URL, ROUTE_PREFIX, _openai_api_key_list, _no_auth_mode, _LOG_CHAT
     )
     if _LOG_CHAT:
         setting_log(save_file=False)
         chatsaver = ChatSaver()
```

### Comparing `openai_forward-0.2.2/openai_forward/config.py` & `openai_forward-0.2.3/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/openai_forward/openai.py` & `openai_forward-0.2.3/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/openai_forward/tool.py` & `openai_forward-0.2.3/openai_forward/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast
 import os
 from typing import Dict, List, Union
 
 import orjson
+from rich import print
 from sparrow import relp
 
 
 def yaml_dump(data, filepath, rel_path=False, mode="w"):
     abs_path = relp(filepath, parents=1) if rel_path else filepath
     from yaml import dump
 
@@ -56,42 +57,49 @@
 
 
 def env2list(env_name: str, sep=" "):
     return str2list(os.environ.get(env_name, "").strip(), sep=sep)
 
 
 def get_matches(messages: List[Dict], assistant: List[Dict]):
+    msg_len, ass_len = len(messages), len(assistant)
+    if msg_len != ass_len:
+        print(f"message({msg_len}) 与 assistant({ass_len}) 长度不匹配")
     matches = []
     assis_idx_to_remove, msg_idx_to_remove = [], []
+
+    def cvt(msg: dict, ass: dict):
+        return {
+            "forwarded-for": msg["forwarded-for"],
+            "model": msg["model"],
+            "messages": msg["messages"],
+            "assistant": ass["assistant"],
+        }
+
     for idx_msg in range(len(messages)):
         win = min(5, len(messages) - 1)
         range_list = [idx_msg + (i + 1) // 2 * (-1) ** (i + 1) for i in range(win)]
         # range_list = [idx_msg + 0, idx_msg + 1, idx_msg - 1, idx_msg + 2, idx_msg - 2, ...]
         for idx_ass in range_list:
             if idx_ass >= len(assistant):
                 break
             if messages[idx_msg]["uid"] == assistant[idx_ass]["uid"]:
-                matches.append(
-                    [
-                        {"messages": messages[idx_msg]["messages"]},
-                        {"assistant": assistant[idx_ass]["assistant"]},
-                    ]
-                )
+                matches.append(cvt(messages[idx_msg], assistant[idx_ass]))
                 assis_idx_to_remove.append(idx_ass)
                 msg_idx_to_remove.append(idx_msg)
                 break
     assis_remain = [i for j, i in enumerate(assistant) if j not in assis_idx_to_remove]
     msg_remain = [i for j, i in enumerate(messages) if j not in msg_idx_to_remove]
     remains = [
-        [{"messages": x["messages"]}, {"assistant": y["assistant"]}]
-        for x in msg_remain
-        for y in assis_remain
-        if x["uid"] == y["uid"]
+        cvt(x, y) for x in msg_remain for y in assis_remain if x["uid"] == y["uid"]
     ]
     matches.extend(remains)
+    ref_len = max(msg_len, ass_len)
+    if len(matches) != ref_len:
+        print(f"存在{ref_len-len(matches)}条未匹配数据")
     return matches
 
 
 def parse_chat_log(filepath: str):
     with open(filepath, "r", encoding="utf-8") as f:
         messages, assistant = [], []
         for line in f.readlines():
@@ -100,15 +108,9 @@
                 messages.append(content)
             else:
                 assistant.append(content)
         return get_matches(messages, assistant)
 
 
 def convert_chatlog_to_jsonl(log_path: str, target_path: str):
-    try:
-        import orjsonl
-    except ImportError:
-        raise ImportError(
-            "import orjsonl error, please `pip install openai_forward[tool]` first"
-        )
     content_list = parse_chat_log(log_path)
-    orjsonl.save(target_path, content_list)
+    json_dump(content_list, target_path, indent_2=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai_forward-0.2.2/openai_forward/content/chat.py` & `openai_forward-0.2.3/openai_forward/content/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,23 +49,23 @@
 
 class ChatSaver:
     def __init__(self):
         self.logger = logger.bind(chat=True)
 
     @staticmethod
     async def parse_payload_to_content(request: Request, route_path: str):
-        uid = uuid.uuid4().__str__()
-        payload = await request.json()
         if route_path == "/v1/chat/completions":
+            uid = uuid.uuid4().__str__()
+            payload = await request.json()
             msgs = payload["messages"]
             model = payload["model"]
             content = {
                 "messages": [{msg["role"]: msg["content"]} for msg in msgs],
                 "model": model,
-                "host": request.headers.get("x-real-ip") or "",
+                "forwarded-for": request.headers.get("x-forwarded-for") or "",
                 "uid": uid,
             }
         else:
             content = {}
         return content
 
     @staticmethod
```

### Comparing `openai_forward-0.2.2/openai_forward/routers/openai_v1.py` & `openai_forward-0.2.3/openai_forward/routers/openai_v1.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/openai_forward/routers/schemas.py` & `openai_forward-0.2.3/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/.gitignore` & `openai_forward-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/LICENSE` & `openai_forward-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/README.md` & `openai_forward-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 [聊天日志](#聊天日志)
 
 [![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tejCum?referralCode=U0-kXv)  
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/beidongjiedeguang/openai-forward)
 
 </div>
 
-本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai
-api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务
+本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问OpenAI API的(云)服务器上，
+通过该服务转发OpenAI的请求。即搭建反向代理服务; 允许输入多个OpenAI API-KEY 组成轮询池; 可自定义二次分发api key.
 
 ---
 
 由本项目搭建的长期代理地址：
-> https://api.openai-forward.com
+> https://api.openai-forward.com  
 
 ## 功能
 
 **基础功能**
 
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
@@ -68,37 +68,38 @@
 - [x] cloudflare 部署
 - [x] ~~Vercel一键部署(不建议)~~
 - [x] Railway 一键部署
 - [x] Render 一键部署
 
 **高级功能**
 
-- [x] 实时记录聊天记录(包括流式响应的聊天内容)
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 转发api key (见[高级配置](#高级配置))
+- [x] 实时记录聊天记录(包括流式响应的聊天内容)
 
 ## 部署指南
 
-提供以下几种部署方式
+[部署文档](deploy.md)
 
+提供以下几种部署方式  
 **有海外vps方案**
 
-1. [pip 安装部署](deploy.md#pip-推荐) (推荐)
-2. [Docker部署](deploy.md#docker-推荐) (推荐)
+1. [pip 安装部署](deploy.md#pip部署) (推荐)
+2. [Docker部署](deploy.md#docker部署) (推荐)
    > https://api.openai-forward.com
 
 **无vps免费部署方案**
 
 1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
    > ~~https://vercel.openai-forward.com~~
 2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
    > https://cloudflare.openai-forward.com
 3. [Railway部署](deploy.md#Railway-一键部署)
    > https://railway.openai-forward.com
-4. [Render一键部署](deploy.md#render-一键部署) (推荐)
+4. [Render一键部署](deploy.md#render-一键部署) (较推荐)
    > https://render.openai-forward.com
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
@@ -170,43 +171,49 @@
 ```
 
 </details>
 
 ## 配置选项
 
 配置的设置方式支持两种  
-一种为在shell中运行`openai-forward run --port=8000`的命令行方式指定;  
+一种为在命令行中执行`openai-forward run`的运行参数(如`--port=8000`)中指定;  
 另一种为读取环境变量的方式指定。
 
+### 命令行参数
+可通过 `openai-forward run --help` 查看
+
 <details markdown="1">
-<summary>Click for more details</summary>  
+  <summary>Click for more details</summary>
 
 **`openai-forward run`参数配置项**
 
 | 配置项 | 说明                |          默认值           |
 |-----------------|-------------------|:----------------------:|
 | --port | 服务端口号             |          8000          |
 | --workers | 工作进程数             |           1            |
 | --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
 | --api_key | 同 OPENAI_API_KEY  |         `None`         |
 | --forward_key | 同 FORWARD_KEY     |         `None`         |
 | --route_prefix | 同 ROUTE_PREFIX    |          `None`          |
 | --log_chat | 同 LOG_CHAT        |        `False`         |
 
-也可通过 `openai-forward run --help` 查看
 
-**环境变量配置项**  
+</details>
+
+### 环境变量配置项
 支持从运行目录下的`.env`文件中读取
 
+<details markdown="1">
+  <summary>Click for more details</summary>
+
 | 环境变量            | 说明                                                                                                                                |           默认值            |
 |-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
 | OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
-| OPENAI_BASE_URL | 转发base url                                                                                                                        | `https://api.openai.com` |
 | ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
 | LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
 </details>
 
 ## 高级配置
 
@@ -265,55 +272,51 @@
 <details markdown="1">
   <summary>Click for more details</summary>
 
 保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
-{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
 {'assistant': 'Hello! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
-{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
+{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
 {'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
-...
 ```
 
-转换为`jsonl`格式：
+转换为`json`格式：
 
 ```bash
 openai-forward convert
 ```
 
-即可转换为以下格式：
+得到`chat.json`：
 
-```json lines
+```json
 [
     {
+        "forwarded-for": "",
+        "model": "gpt-3.5-turbo",
         "messages": [
             {
-                "user": "hi!"
+                "user": "hi"
             }
-        ]
+        ],
+        "assistant": "Hello there! How can I assist you today?"
     },
     {
-        "assistant": "Hello! How can I assist you today?"
-    }
-]
-[
-    {
+        "forwarded-for": "",
+        "model": "gpt-3.5-turbo",
         "messages": [
             {
                 "user": "Hello!"
             }
-        ]
-    },
-    {
+        ],
         "assistant": "Hi there! How can I assist you today?"
     }
 ]
-...
 ```
 
 </details>
 
 ## Backer and Sponsor
 
 <a href="https://www.jetbrains.com/?from=beidongjiedeguang/openai-forward" target="_blank">
```

#### html2text {}

```diff
@@ -8,34 +8,36 @@
                 image_size] [tests] [pypi_downloads] [codecov]
    [åè½](#åè½) | [é¨ç½²æå](#é¨ç½²æå) | [åºç¨](#åºç¨) |
   [éç½®éé¡¹](#éç½®éé¡¹) | [èå¤©æ¥å¿](#èå¤©æ¥å¿) [![Deploy on
     Railway](https://railway.app/button.svg)](https://railway.app/template/
   tejCum?referralCode=U0-kXv) [![Deploy to Render](https://render.com/images/
      deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
                  github.com/beidongjiedeguang/openai-forward)
-æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®openai
-apiçæå¡å¨ä¸ï¼éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡
---- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.com
-## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ - [x]
-æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² -
-[x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
+æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®OpenAI
+APIç(äº)æå¡å¨ä¸ï¼
+éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡;
+åè®¸è¾å¥å¤ä¸ªOpenAI API-KEY ç»æè½®è¯¢æ± ; å¯èªå®ä¹äºæ¬¡ååapi
+key. --- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-
+forward.com ## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ -
+[x] æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½²
+- [x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
 (ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
-**é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
-(åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
-ç»æè½®è¯¢æ±  - [x] èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®]
-(#é«çº§éç½®)) ## é¨ç½²æå æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼
-**ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²](deploy.md#pip-æ¨è) (æ¨è) 2.
-[Dockeré¨ç½²](deploy.md#docker-æ¨è) (æ¨è) > https://api.openai-
-forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²]
-(deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-
-forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) >
-https://cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
+**é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key ç»æè½®è¯¢æ±  - [x]
+èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®](#é«çº§éç½®)) - [x]
+å®æ¶è®°å½èå¤©è®°å½(åæ¬æµå¼ååºçèå¤©åå®¹) ## é¨ç½²æå
+[é¨ç½²ææ¡£](deploy.md) æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡**
+1. [pip å®è£é¨ç½²](deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²]
+(deploy.md#dockeré¨ç½²) (æ¨è) > https://api.openai-forward.com
+**æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-
+ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-forward.com~~ 2.
+[cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://
+cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
 ä¸é®é¨ç½²) > https://railway.openai-forward.com 4. [Renderä¸é®é¨ç½²]
-(deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://render.openai-forward.com ##
-åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
+(deploy.md#render-ä¸é®é¨ç½²) (è¾æ¨è) > https://render.openai-forward.com
+## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
 åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
 Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
 ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
 e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
 chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
@@ -47,41 +49,40 @@
 v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
 Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role":
 "user", "content": "Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl
 --location 'https://api.openai-forward.com/v1/images/generations' \ --header
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
 --data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ```  ##
 éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
-ä¸ç§ä¸ºå¨shellä¸­è¿è¡`openai-forward run --
-port=8000`çå½ä»¤è¡æ¹å¼æå®;
-å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã  Click for more details
-**`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |---
---------------|-------------------|:----------------------:| | --port |
-æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --base_url | å
-OPENAI_BASE_URL | https://api.openai.com | | --api_key | å OPENAI_API_KEY |
-`None` | | --forward_key | å FORWARD_KEY | `None` | | --route_prefix | å
-ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT | `False` | ä¹å¯éè¿
-`openai-forward run --help` æ¥ç **ç¯å¢åééç½®é¡¹**
-æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
-é»è®¤å¼ | |-----------------|------------------------------------------------
+ä¸ç§ä¸ºå¨å½ä»¤è¡ä¸­æ§è¡`openai-forward run`çè¿è¡åæ°(å¦`--
+port=8000`)ä¸­æå®; å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã ###
+å½ä»¤è¡åæ° å¯éè¿ `openai-forward run --help` æ¥ç  Click for more
+details **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
+é»è®¤å¼ | |-----------------|-------------------|:----------------------:| |
+--port | æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --
+base_url | å OPENAI_BASE_URL | https://api.openai.com | | --api_key | å
+OPENAI_API_KEY | `None` | | --forward_key | å FORWARD_KEY | `None` | | --
+route_prefix | å ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT |
+`False` |  ### ç¯å¢åééç½®é¡¹
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å  Click for more details |
+ç¯å¢åé | è¯´æ | é»è®¤å¼ | |-----------------|------------------------
 -------------------------------------------------------------------------------
-----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
-å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
-keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
-FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
-keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
+----------------------------|:------------------------:| | OPENAI_BASE_URL |
+é»è®¤ openaiå®æ¹ api å°å | https://api.openai.com | | OPENAI_API_KEY |
+é»è®¤openai api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼
+ä»¥ç©ºæ ¼åå² | æ  | | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai
+api keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
 å¦æè®¾ç½®äºOPENAI_API_KEYï¼èæ²¡æè®¾ç½®FORWARD_KEY,
 åå®¢æ·ç«¯è°ç¨æ¶æ éæä¾å¯é¥,
-æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | OPENAI_BASE_URL |
-è½¬åbase url | `https://api.openai.com` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ 
-| | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ## é«çº§éç½®
-**è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½® OPENAI_API_KEY å
-FORWARD_KEY, ä¾å¦  Click for more details ```bash OPENAI_API_KEY=sk-*******
-FORWARD_KEY=fk-****** # è¿éfk-tokenç±æä»¬èªå·±å®ä¹ ```
-è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
+æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | ROUTE_PREFIX |
+è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ##
+é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½®
+OPENAI_API_KEY å FORWARD_KEY, ä¾å¦  Click for more details ```bash
+OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
+tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
 ******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
 èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã å¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-******`
 **ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
 H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
@@ -90,19 +91,20 @@
 /api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
 "fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
 e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
 e CODE="" \ yidadaa/chatgpt-next-web ```  ## èå¤©æ¥å¿
 é»è®¤ä¸è®°å½èå¤©æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
 Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
 chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
-'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
 e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
 '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
-'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
 e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
-'f844d156-e747-4887-aef8-e40d977b5ee7'} ... ``` è½¬æ¢ä¸º`jsonl`æ ¼å¼ï¼
-```bash openai-forward convert ``` å³å¯è½¬æ¢ä¸ºä»¥ä¸æ ¼å¼ï¼ ```json lines
-[ { "messages": [ { "user": "hi!" } ] }, { "assistant": "Hello! How can I
-assist you today?" } ] [ { "messages": [ { "user": "Hello!" } ] },
-{ "assistant": "Hi there! How can I assist you today?" } ] ... ```  ## Backer
-and Sponsor [.github/images/jetbrains.svg] ## License OpenAI-Forward is
-licensed under the [MIT](https://opensource.org/license/mit/) license.
+'f844d156-e747-4887-aef8-e40d977b5ee7'} ``` è½¬æ¢ä¸º`json`æ ¼å¼ï¼ ```bash
+openai-forward convert ``` å¾å°`chat.json`ï¼ ```json [ { "forwarded-for":
+"", "model": "gpt-3.5-turbo", "messages": [ { "user": "hi" } ], "assistant":
+"Hello there! How can I assist you today?" }, { "forwarded-for": "", "model":
+"gpt-3.5-turbo", "messages": [ { "user": "Hello!" } ], "assistant": "Hi there!
+How can I assist you today?" } ] ```  ## Backer and Sponsor [.github/images/
+jetbrains.svg] ## License OpenAI-Forward is licensed under the [MIT](https://
+opensource.org/license/mit/) license.
```

### Comparing `openai_forward-0.2.2/pyproject.toml` & `openai_forward-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.2/PKG-INFO` & `openai_forward-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.2.2
+Version: 0.2.3
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
@@ -80,21 +80,21 @@
 [聊天日志](#聊天日志)
 
 [![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tejCum?referralCode=U0-kXv)  
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/beidongjiedeguang/openai-forward)
 
 </div>
 
-本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai
-api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务
+本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问OpenAI API的(云)服务器上，
+通过该服务转发OpenAI的请求。即搭建反向代理服务; 允许输入多个OpenAI API-KEY 组成轮询池; 可自定义二次分发api key.
 
 ---
 
 由本项目搭建的长期代理地址：
-> https://api.openai-forward.com
+> https://api.openai-forward.com  
 
 ## 功能
 
 **基础功能**
 
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
@@ -104,37 +104,38 @@
 - [x] cloudflare 部署
 - [x] ~~Vercel一键部署(不建议)~~
 - [x] Railway 一键部署
 - [x] Render 一键部署
 
 **高级功能**
 
-- [x] 实时记录聊天记录(包括流式响应的聊天内容)
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 转发api key (见[高级配置](#高级配置))
+- [x] 实时记录聊天记录(包括流式响应的聊天内容)
 
 ## 部署指南
 
-提供以下几种部署方式
+[部署文档](deploy.md)
 
+提供以下几种部署方式  
 **有海外vps方案**
 
-1. [pip 安装部署](deploy.md#pip-推荐) (推荐)
-2. [Docker部署](deploy.md#docker-推荐) (推荐)
+1. [pip 安装部署](deploy.md#pip部署) (推荐)
+2. [Docker部署](deploy.md#docker部署) (推荐)
    > https://api.openai-forward.com
 
 **无vps免费部署方案**
 
 1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
    > ~~https://vercel.openai-forward.com~~
 2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
    > https://cloudflare.openai-forward.com
 3. [Railway部署](deploy.md#Railway-一键部署)
    > https://railway.openai-forward.com
-4. [Render一键部署](deploy.md#render-一键部署) (推荐)
+4. [Render一键部署](deploy.md#render-一键部署) (较推荐)
    > https://render.openai-forward.com
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
@@ -206,43 +207,49 @@
 ```
 
 </details>
 
 ## 配置选项
 
 配置的设置方式支持两种  
-一种为在shell中运行`openai-forward run --port=8000`的命令行方式指定;  
+一种为在命令行中执行`openai-forward run`的运行参数(如`--port=8000`)中指定;  
 另一种为读取环境变量的方式指定。
 
+### 命令行参数
+可通过 `openai-forward run --help` 查看
+
 <details markdown="1">
-<summary>Click for more details</summary>  
+  <summary>Click for more details</summary>
 
 **`openai-forward run`参数配置项**
 
 | 配置项 | 说明                |          默认值           |
 |-----------------|-------------------|:----------------------:|
 | --port | 服务端口号             |          8000          |
 | --workers | 工作进程数             |           1            |
 | --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
 | --api_key | 同 OPENAI_API_KEY  |         `None`         |
 | --forward_key | 同 FORWARD_KEY     |         `None`         |
 | --route_prefix | 同 ROUTE_PREFIX    |          `None`          |
 | --log_chat | 同 LOG_CHAT        |        `False`         |
 
-也可通过 `openai-forward run --help` 查看
 
-**环境变量配置项**  
+</details>
+
+### 环境变量配置项
 支持从运行目录下的`.env`文件中读取
 
+<details markdown="1">
+  <summary>Click for more details</summary>
+
 | 环境变量            | 说明                                                                                                                                |           默认值            |
 |-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
 | OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
-| OPENAI_BASE_URL | 转发base url                                                                                                                        | `https://api.openai.com` |
 | ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
 | LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
 </details>
 
 ## 高级配置
 
@@ -301,55 +308,51 @@
 <details markdown="1">
   <summary>Click for more details</summary>
 
 保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
-{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
 {'assistant': 'Hello! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
-{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
+{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
 {'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
-...
 ```
 
-转换为`jsonl`格式：
+转换为`json`格式：
 
 ```bash
 openai-forward convert
 ```
 
-即可转换为以下格式：
+得到`chat.json`：
 
-```json lines
+```json
 [
     {
+        "forwarded-for": "",
+        "model": "gpt-3.5-turbo",
         "messages": [
             {
-                "user": "hi!"
+                "user": "hi"
             }
-        ]
+        ],
+        "assistant": "Hello there! How can I assist you today?"
     },
     {
-        "assistant": "Hello! How can I assist you today?"
-    }
-]
-[
-    {
+        "forwarded-for": "",
+        "model": "gpt-3.5-turbo",
         "messages": [
             {
                 "user": "Hello!"
             }
-        ]
-    },
-    {
+        ],
         "assistant": "Hi there! How can I assist you today?"
     }
 ]
-...
 ```
 
 </details>
 
 ## Backer and Sponsor
 
 <a href="https://www.jetbrains.com/?from=beidongjiedeguang/openai-forward" target="_blank">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.2.2 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.2.3 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· stream forwarding Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
@@ -27,34 +27,36 @@
                 image_size] [tests] [pypi_downloads] [codecov]
    [åè½](#åè½) | [é¨ç½²æå](#é¨ç½²æå) | [åºç¨](#åºç¨) |
   [éç½®éé¡¹](#éç½®éé¡¹) | [èå¤©æ¥å¿](#èå¤©æ¥å¿) [![Deploy on
     Railway](https://railway.app/button.svg)](https://railway.app/template/
   tejCum?referralCode=U0-kXv) [![Deploy to Render](https://render.com/images/
      deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
                  github.com/beidongjiedeguang/openai-forward)
-æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®openai
-apiçæå¡å¨ä¸ï¼éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡
---- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.com
-## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ - [x]
-æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² -
-[x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
+æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®OpenAI
+APIç(äº)æå¡å¨ä¸ï¼
+éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡;
+åè®¸è¾å¥å¤ä¸ªOpenAI API-KEY ç»æè½®è¯¢æ± ; å¯èªå®ä¹äºæ¬¡ååapi
+key. --- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-
+forward.com ## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ -
+[x] æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½²
+- [x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
 (ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
-**é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
-(åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
-ç»æè½®è¯¢æ±  - [x] èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®]
-(#é«çº§éç½®)) ## é¨ç½²æå æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼
-**ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²](deploy.md#pip-æ¨è) (æ¨è) 2.
-[Dockeré¨ç½²](deploy.md#docker-æ¨è) (æ¨è) > https://api.openai-
-forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²]
-(deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-
-forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) >
-https://cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
+**é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key ç»æè½®è¯¢æ±  - [x]
+èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®](#é«çº§éç½®)) - [x]
+å®æ¶è®°å½èå¤©è®°å½(åæ¬æµå¼ååºçèå¤©åå®¹) ## é¨ç½²æå
+[é¨ç½²ææ¡£](deploy.md) æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡**
+1. [pip å®è£é¨ç½²](deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²]
+(deploy.md#dockeré¨ç½²) (æ¨è) > https://api.openai-forward.com
+**æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-
+ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-forward.com~~ 2.
+[cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://
+cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
 ä¸é®é¨ç½²) > https://railway.openai-forward.com 4. [Renderä¸é®é¨ç½²]
-(deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://render.openai-forward.com ##
-åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
+(deploy.md#render-ä¸é®é¨ç½²) (è¾æ¨è) > https://render.openai-forward.com
+## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
 åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
 Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
 ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
 e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
 chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
@@ -66,41 +68,40 @@
 v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
 Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role":
 "user", "content": "Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl
 --location 'https://api.openai-forward.com/v1/images/generations' \ --header
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
 --data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ```  ##
 éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
-ä¸ç§ä¸ºå¨shellä¸­è¿è¡`openai-forward run --
-port=8000`çå½ä»¤è¡æ¹å¼æå®;
-å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã  Click for more details
-**`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |---
---------------|-------------------|:----------------------:| | --port |
-æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --base_url | å
-OPENAI_BASE_URL | https://api.openai.com | | --api_key | å OPENAI_API_KEY |
-`None` | | --forward_key | å FORWARD_KEY | `None` | | --route_prefix | å
-ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT | `False` | ä¹å¯éè¿
-`openai-forward run --help` æ¥ç **ç¯å¢åééç½®é¡¹**
-æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
-é»è®¤å¼ | |-----------------|------------------------------------------------
+ä¸ç§ä¸ºå¨å½ä»¤è¡ä¸­æ§è¡`openai-forward run`çè¿è¡åæ°(å¦`--
+port=8000`)ä¸­æå®; å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã ###
+å½ä»¤è¡åæ° å¯éè¿ `openai-forward run --help` æ¥ç  Click for more
+details **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
+é»è®¤å¼ | |-----------------|-------------------|:----------------------:| |
+--port | æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --
+base_url | å OPENAI_BASE_URL | https://api.openai.com | | --api_key | å
+OPENAI_API_KEY | `None` | | --forward_key | å FORWARD_KEY | `None` | | --
+route_prefix | å ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT |
+`False` |  ### ç¯å¢åééç½®é¡¹
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å  Click for more details |
+ç¯å¢åé | è¯´æ | é»è®¤å¼ | |-----------------|------------------------
 -------------------------------------------------------------------------------
-----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
-å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
-keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
-FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
-keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
+----------------------------|:------------------------:| | OPENAI_BASE_URL |
+é»è®¤ openaiå®æ¹ api å°å | https://api.openai.com | | OPENAI_API_KEY |
+é»è®¤openai api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼
+ä»¥ç©ºæ ¼åå² | æ  | | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai
+api keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
 å¦æè®¾ç½®äºOPENAI_API_KEYï¼èæ²¡æè®¾ç½®FORWARD_KEY,
 åå®¢æ·ç«¯è°ç¨æ¶æ éæä¾å¯é¥,
-æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | OPENAI_BASE_URL |
-è½¬åbase url | `https://api.openai.com` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ 
-| | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ## é«çº§éç½®
-**è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½® OPENAI_API_KEY å
-FORWARD_KEY, ä¾å¦  Click for more details ```bash OPENAI_API_KEY=sk-*******
-FORWARD_KEY=fk-****** # è¿éfk-tokenç±æä»¬èªå·±å®ä¹ ```
-è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
+æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | ROUTE_PREFIX |
+è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ##
+é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½®
+OPENAI_API_KEY å FORWARD_KEY, ä¾å¦  Click for more details ```bash
+OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
+tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
 ******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
 èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã å¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-******`
 **ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
 H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
@@ -109,19 +110,20 @@
 /api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
 "fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
 e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
 e CODE="" \ yidadaa/chatgpt-next-web ```  ## èå¤©æ¥å¿
 é»è®¤ä¸è®°å½èå¤©æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
 Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
 chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
-'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
 e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
 '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
-'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
 e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
-'f844d156-e747-4887-aef8-e40d977b5ee7'} ... ``` è½¬æ¢ä¸º`jsonl`æ ¼å¼ï¼
-```bash openai-forward convert ``` å³å¯è½¬æ¢ä¸ºä»¥ä¸æ ¼å¼ï¼ ```json lines
-[ { "messages": [ { "user": "hi!" } ] }, { "assistant": "Hello! How can I
-assist you today?" } ] [ { "messages": [ { "user": "Hello!" } ] },
-{ "assistant": "Hi there! How can I assist you today?" } ] ... ```  ## Backer
-and Sponsor [.github/images/jetbrains.svg] ## License OpenAI-Forward is
-licensed under the [MIT](https://opensource.org/license/mit/) license.
+'f844d156-e747-4887-aef8-e40d977b5ee7'} ``` è½¬æ¢ä¸º`json`æ ¼å¼ï¼ ```bash
+openai-forward convert ``` å¾å°`chat.json`ï¼ ```json [ { "forwarded-for":
+"", "model": "gpt-3.5-turbo", "messages": [ { "user": "hi" } ], "assistant":
+"Hello there! How can I assist you today?" }, { "forwarded-for": "", "model":
+"gpt-3.5-turbo", "messages": [ { "user": "Hello!" } ], "assistant": "Hi there!
+How can I assist you today?" } ] ```  ## Backer and Sponsor [.github/images/
+jetbrains.svg] ## License OpenAI-Forward is licensed under the [MIT](https://
+opensource.org/license/mit/) license.
```

