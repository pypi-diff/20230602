# Comparing `tmp/nonebot_plugin_al-0.0.1.tar.gz` & `tmp/nonebot_plugin_al-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_al-0.0.1.tar` & `nonebot_plugin_al-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1091 2023-05-30 02:26:50.534952 nonebot_plugin_al-0.0.1/LICENSE
--rw-r--r--   0        0        0     1418 2023-05-30 05:21:21.482509 nonebot_plugin_al-0.0.1/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0     2361 2023-05-30 05:06:38.896053 nonebot_plugin_al-0.0.1/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0      956 2023-05-30 07:23:07.310958 nonebot_plugin_al-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1883 2023-05-30 05:28:17.299310 nonebot_plugin_al-0.0.1/README.md
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-30 02:26:50.534952 nonebot_plugin_al-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1546 2023-06-02 07:19:07.918501 nonebot_plugin_al-0.0.2/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0     2361 2023-05-30 05:06:38.896053 nonebot_plugin_al-0.0.2/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0      964 2023-06-02 07:19:44.389387 nonebot_plugin_al-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1570 2023-06-02 06:46:21.539695 nonebot_plugin_al-0.0.2/README.md
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.0.1/LICENSE` & `nonebot_plugin_al-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.0.1/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.0.2/nonebot_plugin_al/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from .bili import jinghao,get_data
 
 __version__ = "0.0.1"
 __plugin_meta__ = PluginMetadata(
     name="碧蓝航线攻略",
     description='碧蓝航线井号榜等等攻略',
     usage='碧蓝航线攻略',
+    type="application",
+    homepage="https://github.com/Agnes4m/nonebot_plugin_AL",
+    supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 al_command = on_command('al',aliases={'碧蓝'},priority=30,block=True)
```

### Comparing `nonebot_plugin_al-0.0.1/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.0.2/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.0.1/pyproject.toml` & `nonebot_plugin_al-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.0.1"
+version = "0.0.2"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
-keywords = ["game", "nonebot2", "plugin"]
+keywords = ["game", "nonebot2", "plugin","bilibili"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = "^2.0.0rc3"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.2.1"
 aiohttp = ">=3.8.3"
 bs4 = "^0.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_al-0.0.1/README.md` & `nonebot_plugin_al-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_AL/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_AL 0.0.1
 
 _✨Nonebot & 碧蓝航线攻略✨_
-<div align = "center">
-        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
-</div><br>
+
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_AL" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_AL" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
@@ -33,11 +29,12 @@
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
 ## 指令
 
 - 碧蓝帮助 | 碧蓝指令
+- 显示的指令为【碧蓝】+xxx
 
 ## 介绍
 
 爬取b站井号榜攻略等，在群聊展示攻略
```

#### html2text {}

```diff
@@ -1,9 +1,6 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-        # nonebot_plugin_AL 0.0.1 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_
-                ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
-
-[GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
-                                   [NoneBot]
-## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ ## ä»ç»
-ç¬åbç«äºå·æ¦æ»ç¥ç­ï¼å¨ç¾¤èå±ç¤ºæ»ç¥
+# nonebot_plugin_AL 0.0.1 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
+   [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python] [NoneBot]
+## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ - æ¾ç¤ºçæä»¤ä¸ºãç¢§èã+xxx ##
+ä»ç» ç¬åbç«äºå·æ¦æ»ç¥ç­ï¼å¨ç¾¤èå±ç¤ºæ»ç¥
```

### Comparing `nonebot_plugin_al-0.0.1/PKG-INFO` & `nonebot_plugin_al-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.0.1
+Version: 0.0.2
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: GPLv3
-Keywords: game,nonebot2,plugin
+Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -18,34 +18,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
-Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_AL/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_AL 0.0.1
 
 _✨Nonebot & 碧蓝航线攻略✨_
-<div align = "center">
-        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
-</div><br>
+
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_AL" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_AL" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
@@ -61,11 +57,12 @@
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
 ## 指令
 
 - 碧蓝帮助 | 碧蓝指令
+- 显示的指令为【碧蓝】+xxx
 
 ## 介绍
 
 爬取b站井号榜攻略等，在群聊展示攻略
```

#### html2text {}

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.0.1 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.0.2 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
-License: GPLv3 Keywords: game,nonebot2,plugin Author: Agnes_Digital Author-
-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License ::
-OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3) Requires-Dist: bs4
+License: GPLv3 Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
+Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3) Requires-Dist: bs4
 (>=0.0.1,<0.0.2) Requires-Dist: nonebot-adapter-onebot (>=2.2.1) Requires-Dist:
-nonebot2 (>=2.0.0rc3,<3.0.0) Project-URL: Repository, https://github.com/
-Agnes4m/nonebot_plugin_AL Description-Content-Type: text/markdown
+nonebot2 (>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
+nonebot_plugin_AL Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-        # nonebot_plugin_AL 0.0.1 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_
-                ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
-
-[GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
-                                   [NoneBot]
-## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ ## ä»ç»
-ç¬åbç«äºå·æ¦æ»ç¥ç­ï¼å¨ç¾¤èå±ç¤ºæ»ç¥
+# nonebot_plugin_AL 0.0.1 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
+   [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python] [NoneBot]
+## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ - æ¾ç¤ºçæä»¤ä¸ºãç¢§èã+xxx ##
+ä»ç» ç¬åbç«äºå·æ¦æ»ç¥ç­ï¼å¨ç¾¤èå±ç¤ºæ»ç¥
```

