# Comparing `tmp/nonebot_plugin_animeres-1.0.0.tar.gz` & `tmp/nonebot_plugin_animeres-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animeres-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_animeres-1.0.1.tar", max compression
```

## Comparing `nonebot_plugin_animeres-1.0.0.tar` & `nonebot_plugin_animeres-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.0/LICENSE
--rw-r--r--   0        0        0     2947 2023-05-30 11:50:40.494073 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/__init__.py
--rw-r--r--   0        0        0      447 2023-05-30 11:50:00.391161 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/config.py
--rw-r--r--   0        0        0     2172 2023-05-30 07:25:43.874767 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/internal.py
--rw-r--r--   0        0        0     1820 2023-05-30 12:08:11.397488 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/resources/__init__.py
--rw-r--r--   0        0        0     1557 2023-05-30 11:50:29.754653 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/resources/myheartsite.py
--rw-r--r--   0        0        0     1036 2023-05-30 12:07:42.320956 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/schemas.py
--rw-r--r--   0        0        0     1558 2023-05-30 08:09:48.266513 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/utils.py
--rw-r--r--   0        0        0      919 2023-05-31 02:00:42.970686 nonebot_plugin_animeres-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1553 2023-05-27 11:30:14.109179 nonebot_plugin_animeres-1.0.0/README.md
--rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3155 2023-06-01 02:27:06.839785 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/__init__.py
+-rw-r--r--   0        0        0      447 2023-05-30 11:50:00.391161 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/config.py
+-rw-r--r--   0        0        0     2761 2023-06-01 02:07:17.139133 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/internal.py
+-rw-r--r--   0        0        0     1979 2023-06-01 01:55:55.418675 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/__init__.py
+-rw-r--r--   0        0        0     1235 2023-06-01 02:27:45.060418 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/dongmanhuayuan.py
+-rw-r--r--   0        0        0     1557 2023-05-30 11:50:29.754653 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/myheartsite.py
+-rw-r--r--   0        0        0     1036 2023-05-30 12:07:42.320956 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/schemas.py
+-rw-r--r--   0        0        0     1558 2023-05-30 08:09:48.266513 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/utils.py
+-rw-r--r--   0        0        0      946 2023-06-01 02:33:34.562119 nonebot_plugin_animeres-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1648 2023-06-01 02:29:30.768042 nonebot_plugin_animeres-1.0.1/README.md
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_animeres-1.0.0/LICENSE` & `nonebot_plugin_animeres-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/__init__.py` & `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 @anime_res_cmd.got("param", prompt="动漫名字叫什么呀！")
 async def _(matcher: Matcher, state: T_State, param: str = ArgPlainText()):
     if param:
         anime_search = await search(param)
         if anime_search:
             state["anime_search"] = anime_search
             tags = await anime_search.get_tags()
-            await matcher.send("选择哪种呢？\n" + "\n".join(repr(tag) for tag in tags))
+            if anime_search.oneskip():
+                msg: Message = state["param"].copy()
+                msg.clear()
+                matcher.set_arg("index", msg + tags[0].name)
+            else:
+                await matcher.send("选择哪种呢？\n" + "\n".join(repr(tag) for tag in tags))
         else:
             await matcher.finish("没有找到相关资源！看看是不是哪里写错了？")
     else:
         await matcher.finish()
 
 
 @anime_res_cmd.got("index")
```

### Comparing `nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/internal.py` & `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/internal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional
+from fake_useragent import UserAgent
 
 from httpx import AsyncClient
 from .config import plugin_config
 from .schemas import AnimeRes, Tag
 
 
 class BaseAnimeSearch(ABC):
@@ -12,19 +13,32 @@
     name: str = ""
     base_url: Optional[str] = None
     _client: Optional[AsyncClient] = None
 
     def __init__(self) -> None:
         self.tags: List[Tag] = []
         self.anime_res: Dict[str, List[AnimeRes]] = {}
+        self.headers = {
+            "User-Agent": UserAgent().chrome,
+        }
+
+    def set_header(self, key: str, value: str):
+        """修改请求头
+
+        Args:
+            key (str): key
+            value (str): value
+        """
+        self.headers[key] = value
 
     @property
     def client(self) -> AsyncClient:
         if self._client is None:
             self._client = AsyncClient(
+                headers=self.headers,
                 base_url=self.base_url or "",
                 proxies=plugin_config.animeres_proxy,
                 trust_env=True,
                 timeout=600,
             )
         return self._client
 
@@ -57,15 +71,22 @@
 
         Args:
             keyword (str): 关键字
 
         Returns:
             List[Tag]: 类型
         """
-        return [Tag(id=i, name=tag) for i, tag in enumerate(self.anime_res.keys(), 1)]
+        self.tags = [
+            Tag(id=i, name=tag) for i, tag in enumerate(self.anime_res.keys(), 1)
+        ]
+        return self.tags
+
+    def oneskip(self) -> bool:
+        """如果只有一种类型的资源，跳过选项"""
+        return plugin_config.animeres_oneskip and len(self.tags) == 1
 
     def add_resource(self, anime_res: AnimeRes):
         """添加资源"""
         self.anime_res.setdefault(anime_res.tag, []).append(anime_res)
 
     async def get_tag(self, index: str):
         tags = await self.get_tags()
```

### Comparing `nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/resources/__init__.py` & `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Dict, Optional, Type
 from nonebot.log import logger
 
 from httpx import ConnectError
 from .myheartsite import AnimeSearch as MyHeartSiteSearch
+from .dongmanhuayuan import AnimeSearch as DongManHuaYuanSearch
 from ..internal import BaseAnimeSearch
 from ..config import plugin_config
 
 site: Dict[str, Type[BaseAnimeSearch]] = {
     MyHeartSiteSearch.name: MyHeartSiteSearch,
+    DongManHuaYuanSearch.name: DongManHuaYuanSearch,
 }
 
 
 async def search(keyword: str) -> Optional[BaseAnimeSearch]:
     """对站点资源进行搜索
 
     Args:
@@ -25,14 +27,15 @@
         if animeres := await search("海贼王"):
             tags = await animeres.get_tags()
             print(tags)
             anime_list = await animeres.get_resources(tags[0])
             print(anime_list)
         ```
     """
+    print(plugin_config.animeres_site)
     if plugin_config.animeres_site is not None:
         if anime_search := site.get(plugin_config.animeres_site):
             try:
                 search_ = anime_search()
                 if await search_.search(keyword):
                     return search_
             except ConnectError:
```

### Comparing `nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/resources/myheartsite.py` & `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/myheartsite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/schemas.py` & `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/schemas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/utils.py` & `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.0/pyproject.toml` & `nonebot_plugin_animeres-1.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "nonebot-plugin-animeres"
-version = "1.0.0"
+version = "1.0.1"
 description = "动漫资源获取插件"
 authors = ["MelodyKnit <2711402357@qq.com>"]
 readme = "README.md"
 license = "GPL-2.0"
 packages = [{include = "nonebot_plugin_animeres"}]
 keywords = ["nonebot", "nonebot2", "animeres", "anime"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = { version = "^2.0.0rc1", extras = ["fastapi"] }
 httpx = "^0.24.1"
 lxml = "^4.9.2"
 nonebot-adapter-onebot = { version = "^2.2.3", optional = true }
+fake-useragent = "^1.1.3"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 extend-exclude = '''
 '''
```

### Comparing `nonebot_plugin_animeres-1.0.0/PKG-INFO` & `nonebot_plugin_animeres-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-animeres
-Version: 1.0.0
+Version: 1.0.1
 Summary: 动漫资源获取插件
 License: GPL-2.0
 Keywords: nonebot,nonebot2,animeres,anime
 Author: MelodyKnit
 Author-email: 2711402357@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 动漫资源获取插件
@@ -37,32 +38,35 @@
   - `资源`、`动漫资源`
 - 参数
   - `资源名称`
 
 ## 配置参数
 
 ```env
-CARTOON_PROXY=                        # 设置代理端口
-CARTOON_FORWARD=false                 # 合并转发的形式发送消息
-CARTOON_LENGTH=3                      # 每次发送的数量，用-1表示全部取出
-CARTOON_FORMANT="{title}\n{magnet}"   # 发送的消息格式化
-CARTOON_ONESKIP=true                  # 当只有一个选项时跳过
+ANIMERES_PROXY=""                      # 设置代理端口
+ANIMERES_SITE=""                       # 选择资源站点
+ANIMERES_FORWARD=false                 # 合并转发的形式发送消息
+ANIMERES_LENGTH=3                      # 每次发送的数量，用-1表示全部取出
+ANIMERES_FORMANT="{title}\n{magnet}"   # 发送的消息格式化
+ANIMERES_ONESKIP=true                  # 当只有一个选项时跳过
+ANIEMRES_PRIORITY=100
+
 ```
 
-### CARTOON_PROXY
+### ANIMERES_PROXY
 
-通过`CARTOON_PROXY`参数可以设置代理来加速资源的获取或者获取不到的情况
+通过`ANIMERES_PROXY`参数可以设置代理来加速资源的获取或者获取不到的情况
 
-### CARTOON_FORWARD
+### ANIMERES_FORWARD
 
 用来发送合并消息
 
 ![合并消息转发](image/forward.png)
 
-### CARTOON_FORMANT
+### ANIMERES_FORMANT
 
 格式化字符串
 
 | 标签 | 说明 |
 |---|---|
 | title | 资源名称 |
 | tag | 资源标签类型 |
```

