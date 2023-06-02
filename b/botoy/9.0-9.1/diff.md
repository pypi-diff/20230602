# Comparing `tmp/botoy-9.0.tar.gz` & `tmp/botoy-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/botoy-9.0.tar", last modified: Sun May 14 14:20:14 2023, max compression
+gzip compressed data, was "dist/botoy-9.1.tar", last modified: Fri Jun  2 01:05:39 2023, max compression
```

## Comparing `botoy-9.0.tar` & `botoy-9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 14:19:59.000000 botoy-9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-14 14:20:14.000000 botoy-9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-14 14:19:59.000000 botoy-9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-14 14:19:59.000000 botoy-9.0/botoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 14:19:59.000000 botoy-9.0/botoy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-14 14:19:59.000000 botoy-9.0/botoy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46439 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/_internal/config/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/contrib.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/mahiro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/_internal/models/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/models/friend_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/models/group_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    29298 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 14:19:59.000000 botoy-9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:20:14.000000 botoy-9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-14 14:19:59.000000 botoy-9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 01:05:28.000000 botoy-9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-02 01:05:39.000000 botoy-9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-02 01:05:28.000000 botoy-9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 01:05:28.000000 botoy-9.1/botoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 01:05:28.000000 botoy-9.1/botoy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-02 01:05:28.000000 botoy-9.1/botoy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44649 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/_internal/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/mahiro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/_internal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/models/friend_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/models/group_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 01:05:28.000000 botoy-9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:05:39.000000 botoy-9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-02 01:05:28.000000 botoy-9.1/setup.py
```

### Comparing `botoy-9.0/PKG-INFO` & `botoy-9.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: botoy
-Version: 9.0
+Version: 9.1
 Summary: OPQBot/IOTQQ/IOTBot的Python开发助手
 Home-page: https://github.com/xiyaowong/botoy
 Author: wongxy
 Author-email: xiyao.wong@foxmail.com
 License: MIT
 Description: # botoy
         
         [![QQ Group](https://img.shields.io/badge/QQ%E7%BE%A4-856337734-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=K8iQy7i7)
         
         [![pypi](https://img.shields.io/pypi/v/botoy?style=flat-square 'pypi')](https://pypi.org/project/botoy/)
         [![python](https://img.shields.io/badge/python-3.8+-blue 'python')](https://pypi.org/project/botoy/)
+        [![Lines of code](https://img.shields.io/tokei/lines/github/opq-osc/botoy?label=lines&style=flat-square)](https://github.com/opq-osc/botoy)
+        [![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy)
         [![LICENSE](https://img.shields.io/github/license/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy/blob/main/LICENSE)
         
         对机器人框架[OPQ](https://github.com/OPQBOT/OPQ/)接口的 Python 封装,
         因为功能模块耦合度低, 所以你可以完全使用该框架开发，也可以选取需要的内容到自己的项目中
         
         ---
         
@@ -81,9 +83,9 @@
         
         ## V0.0.1
         
         初次发布
         
 Keywords: iotbot,iotqq,OPQ,OPQBot,botoy
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `botoy-9.0/README.md` & `botoy-9.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # botoy
 
 [![QQ Group](https://img.shields.io/badge/QQ%E7%BE%A4-856337734-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=K8iQy7i7)
 
 [![pypi](https://img.shields.io/pypi/v/botoy?style=flat-square 'pypi')](https://pypi.org/project/botoy/)
 [![python](https://img.shields.io/badge/python-3.8+-blue 'python')](https://pypi.org/project/botoy/)
+[![Lines of code](https://img.shields.io/tokei/lines/github/opq-osc/botoy?label=lines&style=flat-square)](https://github.com/opq-osc/botoy)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy)
 [![LICENSE](https://img.shields.io/github/license/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy/blob/main/LICENSE)
 
 对机器人框架[OPQ](https://github.com/OPQBOT/OPQ/)接口的 Python 封装,
 因为功能模块耦合度低, 所以你可以完全使用该框架开发，也可以选取需要的内容到自己的项目中
 
 ---
```

### Comparing `botoy-9.0/botoy/__init__.py` & `botoy-9.1/botoy/__init__.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/__version__.py` & `botoy-9.1/botoy/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=C0415,C0413
 # type: ignore
-__version__ = "9.0"
+__version__ = "9.1"
 
 
 def check_version(daemon=True):
     def _check_version():
         from distutils.version import LooseVersion as V
         from xml.etree import ElementTree
```

### Comparing `botoy-9.0/botoy/_internal/action.py` & `botoy-9.1/botoy/_internal/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,33 @@
-# FIXME: 先凑合用
 import asyncio
 import re
 from typing import List, Optional, TypeVar, Union
 from urllib.parse import urlparse
 
 import httpx
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
-# from . import macro, utils
 from .config import jconfig
 from .context import GroupMsg
 from .log import logger
 
-# from botoy.parser import event as eventParser
-
-
-# from .model import EventMsg, FriendMsg, GroupMsg
-
 
 class BaseResponse(BaseModel):
     Ret: int = 0
     ErrMsg: str = ""
 
 
 class Response(BaseModel):
     CgiBaseResponse: BaseResponse
     ResponseData: dict
 
 
-# TODO: 发送接收数据结构化，但是用pydantic好麻烦哦... 后面再弄合适的方案
-
 lock = asyncio.Lock()
-prev_task: Optional[asyncio.Task] = None
 
 
 def get_base_url(url):
     if not re.match(r"$(http|https|ws)://", url):
         url = "http://" + url
     parsed_url = urlparse(url)
     hostname = parsed_url.hostname
@@ -876,35 +866,47 @@
     #             admins = [member for member in members if member["GroupAdmin"] == 1]
     #         return admins
     #
     async def getClusterInfo(self) -> dict:
         """获取当前集群信息"""
         return await self.get("", path="v1/clusterinfo", params={"isShow": 1, "qq": 1})  # type: ignore
 
+    async def getQrCode(self, qq="", devicename="") -> str:
+        """获取登录二维码base64
+        :param qq: 复用设备信息登录需填写 首次登录会随机设备信息
+        :param devicename: 登录的设备名称
+        """
+        resp = await self.get(
+            "",
+            path=f"/v1/login/getqrcode",
+            params={"qq": qq, "devicename": devicename, "json": 1},
+        )
+        return resp["BQrpic"]  # type: ignore
+
     async def getGroupList(self) -> List[dict]:
         """获取群列表"""
         data = await self.post(self.build_request(request={}, cmd="GetGroupLists"))
-        return data["GroupLists"]
+        return data["GroupLists"]  # type: ignore
 
     async def getGroupMembers(self, group: int) -> List[dict]:
         """获取群成员列表"""
         members = []
         LastBuffer = ""
         while True:
             data = await self.post(
                 self.build_request(
                     request={"Uin": group, "LastBuffer": LastBuffer},
                     cmd="GetGroupMemberLists",
                 )
             )
-            if "MemberLists" in data:
-                members.extend(data["MemberLists"])
-            if "LastBuffer" not in data or data["LastBuffer"] == "":
+            if "MemberLists" in data:  # type: ignore
+                members.extend(data["MemberLists"])  # type: ignore
+            if "LastBuffer" not in data or data["LastBuffer"] == "":  # type:ignore
                 break
-            LastBuffer = data["LastBuffer"]
+            LastBuffer = data["LastBuffer"]  # type: ignore
         return members
 
     async def getGroupAdminList(self, group: int, include_owner=True) -> List[dict]:
         """获取群管理员列表
         :param group: 群号
         :param include_owner: 是否包括群主
         """
@@ -1151,97 +1153,54 @@
         method: str,
         funcname: str,
         path: str,
         payload: Optional[dict] = None,
         params: Optional[dict] = None,
         timeout: Optional[int] = None,
     ):
-        global lock, prev_task
         """基础请求方法, 提供部分提示信息，出错返回空字典，其他返回服务端响应结果"""
+
         async with lock:
-            if prev_task:
-                try:
-                    await asyncio.wait_for(prev_task, 2)
-                except TimeoutError:
-                    pass
-                else:
-                    await asyncio.sleep(0.5)
+            await asyncio.sleep(0.5)
+
         params = params or {}
         params["funcname"] = funcname
-        if not params.get("qq"):
+        if "qq" not in params:
             params["qq"] = await self.qq
 
         try:
-            # 发送请求
-            prev_task = asyncio.ensure_future(
+            request_task = asyncio.ensure_future(
                 self.c.request(
                     method,
                     httpx.URL(url=path, params=params),
                     json=payload,
-                    **({"timeout": timeout} if timeout else {}),
+                    timeout=timeout,
                 )
             )
-            resp = await prev_task
+
+            resp = None
+            async with lock:
+                try:
+                    resp = await asyncio.wait_for(request_task, 2)
+                except TimeoutError:
+                    pass
+            if resp is None or not request_task.done():
+                resp = await request_task
+
+            # TODO: 处理更多细节
             resp_model = Response.parse_obj(resp.json())
             if resp_model.CgiBaseResponse.ErrMsg:
                 if resp_model.CgiBaseResponse.Ret == 0:
                     logger.success(resp_model.CgiBaseResponse.ErrMsg)
                 else:
                     logger.error(resp_model.CgiBaseResponse.ErrMsg)
             return resp_model.ResponseData
         except Exception as e:
             logger.error(e)
             return None
-        # try:
-        #     resp = await self.c.request(
-        #         method, httpx.URL(url=path, params=params), json=payload
-        #     )
-        #     resp.raise_for_status()
-        # except httpx.TimeoutException:
-        #     logger.warning(f"响应超时，但不代表处理未成功, 结果未知!")
-        #     return {}
-        # except httpx.HTTPStatusError:
-        #     logger.error(
-        #         f"响应码出错 => {resp.status_code}，大概率是因为账号已离线或者qq号错误",  # type:ignore
-        #     )
-        #     return {}
-        # except Exception:
-        #     logger.error(f"请求出错: {traceback.format_exc()}")
-        #     return {}
-        #
-        # # 处理数据
-        # try:
-        #     data = resp.json()
-        # except Exception:
-        #     logger.error("API响应结果非json格式")
-        #     return {}
-        #
-        # if data is None:
-        #     logger.error("返回为null, 该类情况多数是因为响应超时或者该API不存在，或服务端操作超时(此时不代表未成功)")
-        #     return {}
-        #
-        # # 返回码提示
-        # if "Ret" in data:
-        #     ret = data.get("Ret")
-        #     if ret == 0:
-        #         pass
-        #     elif ret == 34:
-        #         logger.error(f"未知错误，跟消息长度似乎无关，可以尝试分段重新发送 => {data}")
-        #     elif ret == 110:
-        #         logger.error(f"发送失败，你已被移出该群，请重新加群 => {data}")
-        #     elif ret == 120:
-        #         logger.error(f"机器人被禁言 => {data}")
-        #     elif ret == 241:
-        #         logger.error(f"消息发送频率过高，对同一个群或好友，建议发消息的最小间隔控制在1100ms以上 => {data}")
-        #     elif ret == 299:
-        #         logger.error(f"超过群发言频率限制 => {data}")
-        #     else:
-        #         logger.error(f"请求发送成功, 但处理失败 => {data}")
-        #
-        # return data
 
     #
     async def post(
         self,
         payload: dict,
         funcname: str = "MagicCgiCmd",
         params: Optional[dict] = None,
```

### Comparing `botoy-9.0/botoy/_internal/cli.py` & `botoy-9.1/botoy/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/client.py` & `botoy-9.1/botoy/_internal/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,27 +109,27 @@
         info = getattr(callback, RECEIVER_INFO, ReceiverInfo())
 
         receiver = Receiver(callback, info, pool=self.pool)
         self.receivers.append(receiver)
 
     __call__ = attach
 
-    async def _packet_handler(self, pkt, __available_names: Optional[List[str]] = None):
+    async def _packet_handler(self, pkt, _available_names: Optional[List[str]] = None):
         # __available_names 用于mahiro管理
         # 当前的实现，副作用：增加一项要求: 接收函数有 name 并且 name 唯一
         # TODO: 在mark_recv中处理好name
         # 由botoy注册的框架名自动添加 BOTOY前缀如："name" => "BOTOY name"
         token = current_ctx.set(Context(pkt))
-        if __available_names is not None:
-            __available_names = [i[6:] for i in __available_names]
+        if _available_names is not None:
+            _available_names = [i[6:] for i in _available_names]
             await asyncio.gather(
                 *(
                     self._start_task(receiver)
                     for receiver in self.receivers
-                    if receiver.info.name in __available_names
+                    if receiver.info.name in _available_names
                 ),
                 return_exceptions=True,
             )
         else:
             await asyncio.gather(
                 *(self._start_task(receiver) for receiver in self.receivers),
                 return_exceptions=True,
```

### Comparing `botoy-9.0/botoy/_internal/config/config.py` & `botoy-9.1/botoy/_internal/config/config.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/config/util.py` & `botoy-9.1/botoy/_internal/config/util.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/context.py` & `botoy-9.1/botoy/_internal/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,22 +248,25 @@
 class EventMsg:
     def __init__(self, data):
         model = models.EventMsg.parse_raw(data)  # type: ignore
         self.model = model
 
 
 class Context:
-    def __init__(self, data: str) -> None:
+    def __init__(self, data: Union[str, dict]) -> None:
         """
         :param data: websokets收到的原始包数据
         """
-        self.__data = json.loads(data)
+        if isinstance(data, dict):
+            self.__data = data
+        else:
+            self.__data = json.loads(data)
 
     @property
-    def data(self) -> str:
+    def data(self) -> dict:
         """websokets收到的原始包数据"""
         return self.__data
 
     @property
     def bot_qq(self) -> int:
         """当前机器人QQ"""
         return self.data["CurrentQQ"]  # type: ignore
```

### Comparing `botoy-9.0/botoy/_internal/contrib.py` & `botoy-9.1/botoy/_internal/contrib.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/log.py` & `botoy-9.1/botoy/_internal/log.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/mahiro.py` & `botoy-9.1/botoy/_internal/mahiro.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     async def __message_handler(self, req: Request):
         await self.__ensure_token()
         data = await req.json()
         self._start_task(
             self._packet_handler,
             data["raw"],
-            __available_names=data.get("configs", {}).get("availablePlugins", []),
+            _available_names=data.get("configs", {}).get("availablePlugins", []),
         )
         return {"code": 200}
 
     async def __exchange_authentication(self, req: Request):
         data = await req.json()
         self.set_token(data["token"])
         for receiver in self.receivers:
```

### Comparing `botoy-9.0/botoy/_internal/models/friend_msg.py` & `botoy-9.1/botoy/_internal/models/friend_msg.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/models/group_msg.py` & `botoy-9.1/botoy/_internal/models/group_msg.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/pool.py` & `botoy-9.1/botoy/_internal/pool.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/receiver.py` & `botoy-9.1/botoy/_internal/receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,17 +282,17 @@
         :param text: 需要确认的问题
         :param default: 如果回复超时则返回该默认值
         :param timeout: 超时时间，单位为秒。超时返回`None`。默认30s，可通过`set_default_timeout`修改。
         :param show_default: 在问题后显示超时默认值
         """
         timeout = timeout or self.__s__.default_timeout
         if show_default:
-            prompt = f"[y/N] {timeout}超时，默认为{default and 'yes' or 'no'}"
+            prompt = f"[y/N] {timeout}秒超时，默认为{default and 'yes' or 'no'}"
         else:
-            prompt = f"[y/N] {timeout}超时"
+            prompt = f"[y/N] {timeout}秒超时"
         user_text, _ = await self.text(f"{text}\n\n{prompt}", timeout)
         while True:
             if user_text is None:
                 return default
             elif user_text.lower() == "y":
                 return True
             elif user_text.lower() == "n":
@@ -515,15 +515,15 @@
             self._waiting_group = True
         the_ctx = await self.get_ctx(timeout)
         async with self.lock:
             self._waiting_group = False
         if the_ctx:
             self.prev_s = S.bind(the_ctx)
             return the_ctx.g, self.prev_s
-        return None, S
+        return None, self.prev_s or S
 
     async def next_f(
         self, info: str = "", timeout: Optional[float] = None
     ) -> Tuple[Optional[T_FriendMsg], T_S]:
         """获取下一条好友消息
         如果该会话不支持捕捉好友消息，将报错。
         :param info: 可选的提示信息
@@ -537,15 +537,15 @@
             self._waiting_friend = True
         the_ctx = await self.get_ctx(timeout)
         async with self.lock:
             self._waiting_friend = False
         if the_ctx:
             self.prev_s = S.bind(the_ctx)
             return the_ctx.f, self.prev_s
-        return None, S
+        return None, self.prev_s or S
 
     async def next_ctx(
         self, info: str = "", timeout: Optional[float] = None
     ) -> Tuple[Optional[T_Context], T_S]:
         """获取下一个ctx
         :param info: 可选的提示信息
         :param timeout: 超时时间，单位为秒。超时返回`None`。默认30s，可通过`set_default_timeout`修改。
@@ -558,15 +558,15 @@
         the_ctx = await self.get_ctx(timeout or self.default_timeout)
         async with self.lock:
             self._waiting_group = False
             self._waiting_friend = False
         if the_ctx:
             self.prev_s = S.bind(the_ctx)
             return the_ctx, self.prev_s
-        return None, S
+        return None, self.prev_s or S
 
     def __repr__(self) -> str:
         return f"<Session[sid={self.sid}]>"
 
 
 class ReceiverMarker:
     def __init__(self) -> None:
```

### Comparing `botoy-9.0/botoy/_internal/runner.py` & `botoy-9.1/botoy/_internal/runner.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/schedule.py` & `botoy-9.1/botoy/_internal/schedule.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/sugar.py` & `botoy-9.1/botoy/_internal/sugar.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy/_internal/utils.py` & `botoy-9.1/botoy/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `botoy-9.0/botoy.egg-info/PKG-INFO` & `botoy-9.1/botoy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: botoy
-Version: 9.0
+Version: 9.1
 Summary: OPQBot/IOTQQ/IOTBot的Python开发助手
 Home-page: https://github.com/xiyaowong/botoy
 Author: wongxy
 Author-email: xiyao.wong@foxmail.com
 License: MIT
 Description: # botoy
         
         [![QQ Group](https://img.shields.io/badge/QQ%E7%BE%A4-856337734-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=K8iQy7i7)
         
         [![pypi](https://img.shields.io/pypi/v/botoy?style=flat-square 'pypi')](https://pypi.org/project/botoy/)
         [![python](https://img.shields.io/badge/python-3.8+-blue 'python')](https://pypi.org/project/botoy/)
+        [![Lines of code](https://img.shields.io/tokei/lines/github/opq-osc/botoy?label=lines&style=flat-square)](https://github.com/opq-osc/botoy)
+        [![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy)
         [![LICENSE](https://img.shields.io/github/license/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy/blob/main/LICENSE)
         
         对机器人框架[OPQ](https://github.com/OPQBOT/OPQ/)接口的 Python 封装,
         因为功能模块耦合度低, 所以你可以完全使用该框架开发，也可以选取需要的内容到自己的项目中
         
         ---
         
@@ -81,9 +83,9 @@
         
         ## V0.0.1
         
         初次发布
         
 Keywords: iotbot,iotqq,OPQ,OPQBot,botoy
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `botoy-9.0/botoy.egg-info/SOURCES.txt` & `botoy-9.1/botoy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botoy-9.0/setup.py` & `botoy-9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     keywords=["iotbot", "iotqq", "OPQ", "OPQBot", "botoy"],
     packages=find_packages(),
     install_requires=read_files(["requirements.txt"]),
     entry_points="""
         [console_scripts]
         botoy=botoy._internal.cli:cli
     """,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

