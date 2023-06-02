# Comparing `tmp/nonebot_plugin_servicestate-0.1.9.tar.gz` & `tmp/nonebot_plugin_servicestate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_servicestate-0.1.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_servicestate-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_servicestate-0.1.9.tar` & `nonebot_plugin_servicestate-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0     1089 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/LICENSE
--rw-r--r--   0        0        0       57 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/__init__.py
--rw-r--r--   0        0        0     6776 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/adapter_nonebot.py
--rw-r--r--   0        0        0      964 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/compatible.py
--rw-r--r--   0        0        0      750 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/exception.py
--rw-r--r--   0        0        0      422 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/logger.py
--rw-r--r--   0        0        0     6250 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/manager.py
--rw-r--r--   0        0        0      210 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/__init__.py
--rw-r--r--   0        0        0     2341 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/demo.py
--rw-r--r--   0        0        0     1130 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/http.py
--rw-r--r--   0        0        0     2094 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/protocol.py
--rw-r--r--   0        0        0      728 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/tcp.py
--rw-r--r--   0        0        0     6412 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/service.py
--rw-r--r--   0        0        0     1304 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/utils.py
--rw-r--r--   0        0        0      805 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     6373 2023-03-08 16:56:07.632431 nonebot_plugin_servicestate-0.1.9/README.md
--rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 nonebot_plugin_servicestate-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6378 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/exception.py
+-rw-r--r--   0        0        0     6257 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/manager.py
+-rw-r--r--   0        0        0      210 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/__init__.py
+-rw-r--r--   0        0        0     2341 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/demo.py
+-rw-r--r--   0        0        0     1130 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/http.py
+-rw-r--r--   0        0        0     2094 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/protocol.py
+-rw-r--r--   0        0        0      728 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/tcp.py
+-rw-r--r--   0        0        0     6489 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/service.py
+-rw-r--r--   0        0        0     1354 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/utils.py
+-rw-r--r--   0        0        0      805 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6373 2023-06-02 12:37:15.263086 nonebot_plugin_servicestate-0.2.0/README.md
+-rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 nonebot_plugin_servicestate-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_servicestate-0.1.9/LICENSE` & `nonebot_plugin_servicestate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/adapter_nonebot.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,42 @@
-from typing import Dict, List, Any, Tuple
-from pathlib import Path
+from typing import List, Tuple
 from pydantic import ValidationError
 
 from nonebot.plugin.on import on_command
 from nonebot.params import CommandArg, Depends
 from nonebot.adapters.onebot.v11 import Message
-import nonebot.log as nb_log
 from nonebot.permission import SUPERUSER
 
-from .logger import set_logger, logger
-
-set_logger(nb_log.logger)
-logger = nb_log.logger
+from nonebot.log import logger
 
 from .service import SupportProtocol
 from .exception import (
     ProtocolUnsopportError,
     NameConflictError,
     ParamCountInvalidError,
     NameEscapeCharacterCountError,
     NameNotFoundError,
 )
 from .manager import manager
 from .utils import Escharacter
-from . import compatible
 
 service_status_matcher = on_command("服务状态")
 
 
 @service_status_matcher.handle()
 async def _():
     result_dict = await manager.get_detect_result()
     if result_dict == {}:
         await service_status_matcher.finish("您未绑定任何服务！")
     pretty_text = ""
     for name, result in result_dict.items():
-        pretty_text += "O" if result else "X"
-        pretty_text += "" if result else " "  # QQ字符O和X宽度不一致
-        pretty_text += " "
-        pretty_text += "正常" if result else "故障"
-        pretty_text += " | "
-        pretty_text += name
-        pretty_text += "\n"
+        if result:
+            pretty_text += f"O 正常 | {name}\n"
+        else:
+            pretty_text += f"X 故障 | {name}\n"
     pretty_text = pretty_text[:-1]
     await service_status_matcher.finish(pretty_text)
 
 
 def extract_str_list(command_arg: Message = CommandArg()):
     return command_arg.extract_plain_text().split()
 
@@ -81,16 +72,14 @@
 service_del_matcher = on_command("服务删除", aliases={"删除服务"}, permission=SUPERUSER)
 
 
 @service_del_matcher.handle()
 async def _(command_arg: Message = CommandArg()):
     try:
         manager.unbind_service_by_name(command_arg.extract_plain_text())
-    except KeyError:
-        await service_del_matcher.finish("操作失败：未找到该服务名称！")
     except NameNotFoundError:
         await service_del_matcher.finish("操作失败：未找到该服务名称！")
     manager.save()
     await service_del_matcher.finish("已删除服务：" + command_arg)
 
 
 service_group_matcher = on_command("服务合并", aliases={"合并服务", "群组服务", "服务群组"}, permission=SUPERUSER)
@@ -100,29 +89,29 @@
 async def _(command_arg_list: List[str] = Depends(extract_str_list)):
     if len(command_arg_list) < 3:
         await service_group_matcher.finish(f"参数不足\n合并服务 <名称1> <名称2> <群组名称>")
     bind_service_name_list = command_arg_list[:-1]
     name = command_arg_list[-1]
     try:
         manager.bind_group_by_name(bind_service_name_list, name)
-    except KeyError:
+    except NameNotFoundError:
         await service_group_matcher.finish("操作失败：合并的服务名称中有一个或多个无法找到！")
     manager.save()
     await service_group_matcher.finish(f"已成功合并 {len(bind_service_name_list)} 个服务")
 
 
 service_ungroup_matcher = on_command("服务解散", aliases={"解散服务"}, permission=SUPERUSER)
 
 
 @service_ungroup_matcher.handle()
 async def _(name_msg: Message = CommandArg()):
     name = name_msg.extract_plain_text()
     try:
         manager.unbind_group_by_name(name)
-    except KeyError:
+    except NameNotFoundError:
         await service_ungroup_matcher.finish("操作失败：无法找到该名称的群组服务")
     except NameConflictError:
         await service_ungroup_matcher.finish("操作失败：即将解散的群组服务中与现有名称重复")
     except:
         await service_ungroup_matcher.finish("操作失败：内部错误")
     manager.save()
     await service_ungroup_matcher.finish(f"已成功解散群组")
@@ -145,15 +134,15 @@
     settings_list: List[Tuple[str, str]] = []
     for i in range(0, len(command_arg_list) - 1, 2):
         settings_list.append((command_arg_list[i], command_arg_list[i + 1]))
     logger.debug(f"Modifying settings: {name} @ {settings_list}")
     try:
         for key, value in settings_list:
             manager.modify_service_param(name.auto_name, key, value)
-    except KeyError:
+    except NameNotFoundError:
         await service_set_matcher.finish("操作失败：修改的服务名或参数名未找到")
     except ValidationError:
         await service_set_matcher.finish("操作失败：参数格式或类型不正确")
     except:
         await service_set_matcher.finish("操作失败：内部错误")
     manager.save()
     await service_set_matcher.finish(f"服务 {name} 参数修改成功")
```

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/exception.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/exception.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,52 @@
 class ProtocolUnsopportError(Exception):
+    """
+    不支持该协议
+    """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class NameConflictError(Exception):
+    """
+    名称冲突
+    """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class NameNotFoundError(Exception):
+    """
+    未找到该名称
+    """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class ParamInvalidError(Exception):
+    """
+    参数类型或范围不正确
+    """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class ParamCountInvalidError(Exception):
+    """
+    参数个数不正确
+    """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class NameEscapeCharacterCountError(Exception):
+    """
+    转义符个数不正确
+    """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/manager.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .exception import (
     ProtocolUnsopportError,
     NameConflictError,
     NameNotFoundError,
     ParamInvalidError,
 )
 
-plugin_config_file_path = Path(store.get_data_file("nonebot-plugin-servicestate", "protocol_settings.json"))
+PLUGIN_CONFIG_FILE_PATH = Path(store.get_data_file("nonebot-plugin-servicestate", "protocol_settings.json"))
 
 
 def modify_exception_recovery(func):
     def inner(*args, **kw):
         try:
             manager.save()
             return func(*args, **kw)
@@ -38,26 +38,26 @@
 class CommandManager:
     __service_status: ServiceStatus = ServiceStatus()
     __service_status_group: ServiceStatusGroup = ServiceStatusGroup()
 
     def __init__(self) -> None:
         pass
 
-    def load(self, path: Path = plugin_config_file_path) -> None:
+    def load(self, path: Path = PLUGIN_CONFIG_FILE_PATH) -> None:
         with open(path, "r", encoding="utf-8") as f:
             load_dict = json.loads(f.read())
         self.__service_status = ServiceStatus.load(load_dict["service"])
         self.__service_status_group = ServiceStatusGroup.load(load_dict["service_group"])
 
-    def save(self, path: Path = plugin_config_file_path) -> None:
+    def save(self, path: Path = PLUGIN_CONFIG_FILE_PATH) -> None:
         save_dict = {
             "service": self.__service_status.export(),
             "service_group": self.__service_status_group.export(),
         }
-        if not path.exists():
+        if not path.parent.is_dir():
             logger.debug("Creating plugin folder")
             path.parent.mkdir(parents=True)
         with open(path, "w", encoding="utf-8") as f:
             f.write(
                 json.dumps(
                     save_dict,
                     ensure_ascii=False,
@@ -146,11 +146,11 @@
         group_service_count = 0
         for i in self.__service_status_group:
             group_service_count += len(i)
         return single_count, group_count, group_service_count
 
 
 manager = CommandManager()
-if not plugin_config_file_path.is_file():
+if not PLUGIN_CONFIG_FILE_PATH.is_file():
     logger.info("Creating config file")
     manager.save()
-manager.load(plugin_config_file_path)
+manager.load(PLUGIN_CONFIG_FILE_PATH)
```

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/demo.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/demo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/http.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/http.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/protocol.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/protocol/tcp.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/protocol/tcp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/service.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Union, Dict, List, Any, Tuple
 from asyncio import gather
 
 from .protocol import BaseProtocol, SupportProtocol
-from .exception import ProtocolUnsopportError, NameConflictError
-from .logger import logger
+from .exception import ProtocolUnsopportError, NameConflictError,NameNotFoundError
+from nonebot.log import logger
 
 
 class ServiceStatus:
     def __init__(self) -> None:
         self.__bind_services: List[BaseProtocol] = []
 
     def __contains__(self, item) -> bool:
@@ -28,22 +28,22 @@
     def __next__(self) -> BaseProtocol:
         return self.__iterator.__next__()
 
     def __getitem__(self, key: Union[str, BaseProtocol]) -> BaseProtocol:
         for i in self:
             if i == key:
                 return i
-        raise KeyError(key)
+        raise NameNotFoundError(key)
 
     def __setitem__(self, key: Union[str, BaseProtocol], value: BaseProtocol) -> None:
         for i, j in enumerate(self.__bind_services):
             if key == j:
                 self.__bind_services[i] = value
                 return
-        raise KeyError(key)
+        raise NameNotFoundError(key)
 
     def __len__(self) -> int:
         return len(self.__bind_services)
 
     def register_service(self, protocol: str, *args, **kw) -> BaseProtocol:
         if protocol not in SupportProtocol.get():
             raise ProtocolUnsopportError
@@ -55,15 +55,15 @@
         if service in self:
             raise NameConflictError
         self.__bind_services.append(service)
         return service
 
     def unbind_service(self, unbind_service: Union[BaseProtocol, str]) -> BaseProtocol:
         if unbind_service not in self:
-            raise KeyError
+            raise NameNotFoundError
         if isinstance(unbind_service, str):
             unbind_service = self[unbind_service]
         self.__bind_services.pop(self.__bind_services.index(unbind_service))
         return unbind_service
 
     async def get_detect_result(self) -> Dict[str, bool]:
         tasks = [service.detect() for service in self]
@@ -118,24 +118,24 @@
 
     def __getitem__(self, key: Union[str, ServiceStatus]) -> ServiceStatus:
         if isinstance(key, str):
             return self.__bind_services_group[key]
         for i in self:
             if i == key:
                 return i
-        raise KeyError(key)
+        raise NameNotFoundError(key)
 
     def __setitem__(self, key: Union[str, ServiceStatus], value: ServiceStatus) -> None:
         if isinstance(key, str):
             key = self[key]
         for i, j in self.items():
             if key == j:
                 self.__bind_services_group[i] = value
                 return
-        raise KeyError(key)
+        raise NameNotFoundError (key)
 
     def __len__(self):
         return len(self.__bind_services_group)
 
     def items(self):
         return self.__bind_services_group.items()
 
@@ -146,15 +146,15 @@
     ) -> None:
         self.__bind_services_group[name] = ServiceStatus()
         for this_service in services:
             self.__bind_services_group[name].bind_service(this_service)
 
     def unbind_group(self, key: str) -> ServiceStatus:
         if key not in self:
-            raise KeyError
+            raise NameNotFoundError
         temp_ret = self.__bind_services_group[key]
         del self.__bind_services_group[key]
         return temp_ret
 
     async def get_detect_result(self) -> Dict[str, bool]:
         ret_result = {}
         for name, this_service_group in self.items():
```

### Comparing `nonebot_plugin_servicestate-0.1.9/nonebot_plugin_servicestate/utils.py` & `nonebot_plugin_servicestate-0.2.0/nonebot_plugin_servicestate/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 
 class Escharacter:
     def __init__(self, keywords: str, max_count: int = 2) -> None:
         self.__raw_content = keywords
         self.__extract_content = list(
             map(
-                lambda i: i.replace("^_^", "@"),
-                keywords.replace("@@", "^_^").split("@"),
+                lambda i: i.replace("__BUTLTIN_ESCAPE_CHARACTER__", "@"),
+                keywords.replace("@@", "__BUTLTIN_ESCAPE_CHARACTER__").split("@"),
             )
         )
         self.is_group = False
         if len(self.__extract_content) != 1:
             self.is_group = True
         if self.is_group and len(self.__extract_content) > max_count:
             raise NameEscapeCharacterCountError
```

### Comparing `nonebot_plugin_servicestate-0.1.9/pyproject.toml` & `nonebot_plugin_servicestate-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-servicestate"
-version = "0.1.9"
+version = "0.2.0"
 description = "基于NoneBot2的状态监测插件"
 authors = ["OREOCODEDEV <17620745509@126.COM>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OREOCODEDEV/nonebot-plugin-servicestate"
 repository = "https://github.com/OREOCODEDEV/nonebot-plugin-servicestate"
 packages = [{include = "nonebot_plugin_servicestate"}]
```

### Comparing `nonebot_plugin_servicestate-0.1.9/README.md` & `nonebot_plugin_servicestate-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_servicestate-0.1.9/PKG-INFO` & `nonebot_plugin_servicestate-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-servicestate
-Version: 0.1.9
+Version: 0.2.0
 Summary: 基于NoneBot2的状态监测插件
 Home-page: https://github.com/OREOCODEDEV/nonebot-plugin-servicestate
 License: MIT
 Author: OREOCODEDEV
 Author-email: 17620745509@126.COM
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-servicestate Version: 0.1.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-servicestate Version: 0.2.0 Summary:
 åºäºNoneBot2çç¶æçæµæä»¶ Home-page: https://github.com/OREOCODEDEV/
 nonebot-plugin-servicestate License: MIT Author: OREOCODEDEV Author-email:
 17620745509@126.COM Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
```

