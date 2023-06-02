# Comparing `tmp/nonebot_plugin_access_control-0.5.1.tar.gz` & `tmp/nonebot_plugin_access_control-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-0.5.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-0.5.2.tar", max compression
```

## Comparing `nonebot_plugin_access_control-0.5.1.tar` & `nonebot_plugin_access_control-0.5.2.tar`

### file list

```diff
@@ -1,50 +1,48 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.1/LICENSE
--rw-r--r--   0        0        0      949 2023-06-01 01:18:33.536786 nonebot_plugin_access_control-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    18867 2023-05-30 02:55:49.596711 nonebot_plugin_access_control-0.5.1/README.MD
--rw-r--r--   0        0        0     1633 2023-06-01 01:15:34.961098 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/errors.py
--rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/event_bus.py
--rw-r--r--   0        0        0    10794 2023-06-01 01:16:36.463425 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/handle_error.py
--rw-r--r--   0        0        0     3352 2023-06-01 01:13:05.751049 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/parser.py
--rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/permission.py
--rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/rate_limit.py
--rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/plugin_data.py
--rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/base.py
--rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/__init__.py
--rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/permission.py
--rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/rate_limit.py
--rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/base.py
--rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/permission.py
--rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/rate_limit.py
--rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/service.py
--rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/methods.py
--rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/nonebot.py
--rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/permission/__init__.py
--rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/permission/permission.py
--rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/plugin.py
--rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
--rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/rate_limit/rule.py
--rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/rate_limit/token.py
--rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice.py
--rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice_owner.py
--rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/base.py
--rw-r--r--   0        0        0     2954 2023-06-01 01:04:23.797927 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/union.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/session.py
--rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/superuser.py
--rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/__init__.py
--rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
--rw-r--r--   0        0        0     2094 2023-05-31 16:13:35.569687 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
--rw-r--r--   0        0        0     3072 2023-05-31 16:13:35.546685 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
--rw-r--r--   0        0        0    19260 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.2/LICENSE
+-rw-r--r--   0        0        0      876 2023-06-02 02:24:07.049316 nonebot_plugin_access_control-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    19070 2023-06-02 01:51:58.407828 nonebot_plugin_access_control-0.5.2/README.MD
+-rw-r--r--   0        0        0     3318 2023-06-02 02:23:43.755840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/errors.py
+-rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/event_bus.py
+-rw-r--r--   0        0        0    10794 2023-06-01 01:16:36.463425 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/matchers/__init__.py
+-rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/matchers/handle_error.py
+-rw-r--r--   0        0        0     3352 2023-06-01 01:13:05.751049 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/matchers/parser.py
+-rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/models/permission.py
+-rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/models/rate_limit.py
+-rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/plugin_data.py
+-rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/impl/__init__.py
+-rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/impl/permission.py
+-rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/impl/rate_limit.py
+-rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/base.py
+-rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/permission.py
+-rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/service.py
+-rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/methods.py
+-rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/nonebot.py
+-rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/permission/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/permission/permission.py
+-rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/plugin.py
+-rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/rate_limit/rule.py
+-rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/rate_limit/token.py
+-rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/subservice.py
+-rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/subservice_owner.py
+-rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-02 02:16:32.433342 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-02 02:16:32.442340 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/extractor/base.py
+-rw-r--r--   0        0        0     1885 2023-06-02 02:16:32.463343 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/extractor/onebot_v11.py
+-rw-r--r--   0        0        0      590 2023-06-02 02:16:32.446339 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/extractor/onebot_v12.py
+-rw-r--r--   0        0        0     2093 2023-06-02 02:16:32.413738 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/extractor/session.py
+-rw-r--r--   0        0        0      938 2023-06-02 02:16:32.471866 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/subject/extractor/union.py
+-rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/utils/session.py
+-rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/utils/superuser.py
+-rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0    19460 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.2/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-0.5.1/LICENSE` & `nonebot_plugin_access_control-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/pyproject.toml` & `nonebot_plugin_access_control-0.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/ssttkkl/nonebot-plugin-access-control"
 packages = [
-    { include = "nonebot_plugin_access_control", from = "src" },
-    { include = "nonebot_plugin_access_control_onebot", from = "src" }
+    { include = "nonebot_plugin_access_control", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0rc3"
 nonebot-plugin-datastore = "^0.6.0a3"
 nonebot-plugin-apscheduler = "^0.2.0"
```

### Comparing `nonebot_plugin_access_control-0.5.1/README.MD` & `nonebot_plugin_access_control-0.5.2/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,22 @@
 
 回到上面的例子，假设我们对主体”群组G“禁用服务，但是对主体”用户V“启用服务。则用户U在群组G内将无法使用服务，但是用户V在群组G内可以使用。
 
 在插件使用中，我们用一个字符串表示主体，例如`qq:12345678`表示QQ用户12345678、`qq:g87654321`表示QQ群组87654321。
 
 我们约定：`all`表示所有用户、`superuser`表示超级用户、`<平台名>`表示所有此平台的用户、`<协议名>`表示所有此协议的用户、所有与平台相关的主体均以`<平台名>:`开头、所有与协议相关的主体均以`<协议名>:`开头。
 
-各适配器的主体定义如下：
+插件依赖[nonebot-plugin-session](https://github.com/noneplugin/nonebot-plugin-session)提取事件的主体，各适配器的主体定义如下：
 
 - [OneBot V11](docs/onebot_v11.md)
 - [OneBot V12](docs/onebot_v12.md)
 - [Kaiheila](docs/kaiheila.md)
+- [QQ Guild](docs/qqguild.md)
+- Telegram：未测试，参考OneBot V12的定义
 
-如果你能帮助我们进行其他协议适配，欢迎提交PR。
 
 ### 服务
 
 **服务（Service）为一组能够进行权限控制的功能的集合。** 服务可以拥有子服务，通过树形结构组织服务，统一管理权限。
 
 整个NoneBot是一个名为nonebot的服务，为树形结构的根节点，其直接子节点为所有插件。
 
@@ -144,14 +145,16 @@
     - `/ac limit ls --sbj <主体>`：列出主体已配置的限流规则
     - `/ac limit ls --srv <服务>`：列出服务已配置的限流规则
     - `/ac limit ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的限流规则
     - `/ac limit reset`：重置限流计数
 - 服务查看
     - `/ac service ls`：列出所有服务与子服务层级
     - `/ac service ls --srv <服务>`：列出服务的子服务层级
+- 主体测试
+    - `/ac subject`：列出消息发送者的所有主体
 
 其中`<服务>`的格式如下：
 
 - `nonebot`：对整个NoneBot进行开关
 - `<插件名>`：对整个插件进行开关
 - `<插件名>.<子服务名>.<子服务名>.....<子服务名>`：对插件内的某个子服务进行开关（需参照下文对插件进行配置）
```

#### html2text {}

```diff
@@ -12,17 +12,19 @@
 ä¸ä¸ªç¨æ·éå¸¸æ¥æå¤ä¸ªä¸»ä½ãä¸¾ä¸ªä¾å­ï¼QQä¸ç¾¤ç»Gçç¨æ·Uåéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·åæ¶å·æâç¨æ·Uâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãåæ¶QQä¸ç¾¤ç»Gçç¨æ·Vä¹åéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·è¯¥ç¨æ·åæ¶å·æâç¨æ·Vâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ã
 å½è®¾ç½®æéæ¶ï¼æä»¬ç´æ¥éå¯¹ä¸ä¸ªä¸»ä½è¿è¡è®¾ç½®ãå½é´ææ¶ï¼æä»¬å¯¹ç¨æ·çææä¸»ä½**æä¼åçº§ä»é«å°ä½çé¡ºåº**ï¼éä¸æ£æ¥æ¯å¦è®¾ç½®äºæéãä¸æ¦æ£æ¥å°æä¸ªä¸»ä½è®¾ç½®äºæéï¼å°±ä»¥è¯¥ä¸»ä½è®¾ç½®çæéä½ä¸ºè¯¥ç¨æ·çæéã
 åå°ä¸é¢çä¾å­ï¼åè®¾æä»¬å¯¹ä¸»ä½âç¾¤ç»Gâç¦ç¨æå¡ï¼ä½æ¯å¯¹ä¸»ä½âç¨æ·Vâå¯ç¨æå¡ãåç¨æ·Uå¨ç¾¤ç»Gåå°æ æ³ä½¿ç¨æå¡ï¼ä½æ¯ç¨æ·Vå¨ç¾¤ç»Gåå¯ä»¥ä½¿ç¨ã
 å¨æä»¶ä½¿ç¨ä¸­ï¼æä»¬ç¨ä¸ä¸ªå­ç¬¦ä¸²è¡¨ç¤ºä¸»ä½ï¼ä¾å¦`qq:
 12345678`è¡¨ç¤ºQQç¨æ·12345678ã`qq:g87654321`è¡¨ç¤ºQQç¾¤ç»87654321ã
 æä»¬çº¦å®ï¼`all`è¡¨ç¤ºææç¨æ·ã`superuser`è¡¨ç¤ºè¶çº§ç¨æ·ã`<å¹³å°å>`è¡¨ç¤ºæææ­¤å¹³å°çç¨æ·ã`<åè®®å>`è¡¨ç¤ºæææ­¤åè®®çç¨æ·ãææä¸å¹³å°ç¸å³çä¸»ä½åä»¥`<å¹³å°å>:
 `å¼å¤´ãææä¸åè®®ç¸å³çä¸»ä½åä»¥`<åè®®å>:`å¼å¤´ã
-åééå¨çä¸»ä½å®ä¹å¦ä¸ï¼ - [OneBot V11](docs/onebot_v11.md) -
-[OneBot V12](docs/onebot_v12.md) - [Kaiheila](docs/kaiheila.md)
-å¦æä½ è½å¸®å©æä»¬è¿è¡å¶ä»åè®®ééï¼æ¬¢è¿æäº¤PRã ### æå¡
+æä»¶ä¾èµ[nonebot-plugin-session](https://github.com/noneplugin/nonebot-
+plugin-session)æåäºä»¶çä¸»ä½ï¼åééå¨çä¸»ä½å®ä¹å¦ä¸ï¼ -
+[OneBot V11](docs/onebot_v11.md) - [OneBot V12](docs/onebot_v12.md) -
+[Kaiheila](docs/kaiheila.md) - [QQ Guild](docs/qqguild.md) -
+Telegramï¼æªæµè¯ï¼åèOneBot V12çå®ä¹ ### æå¡
 **æå¡ï¼Serviceï¼ä¸ºä¸ç»è½å¤è¿è¡æéæ§å¶çåè½çéåã**
 æå¡å¯ä»¥æ¥æå­æå¡ï¼éè¿æ å½¢ç»æç»ç»æå¡ï¼ç»ä¸ç®¡çæéã
 æ´ä¸ªNoneBotæ¯ä¸ä¸ªåä¸ºnonebotçæå¡ï¼ä¸ºæ å½¢ç»æçæ ¹èç¹ï¼å¶ç´æ¥å­èç¹ä¸ºæææä»¶ã
 ä¸ä¸ªæä»¶æ¯ä¸ä¸ªæå¡ï¼PluginServiceï¼ï¼å¶ç¶èç¹ä¸ºnonebotãå½æä»¶æªè¿è¡ééæ¶ï¼è¯¥æä»¶åªå·æè¿ä¸ä¸ªPluginServiceãå¯¹æä»¶è¿è¡ééï¼åéè¦ä»æä»¶çPluginServiceåå»ºSubServiceï¼ä¸ºæä»¶çMatcherç­åè½å¥å£åºç¨SubServiceãï¼åèä¸ææä»¶ééç« èï¼
 ï¼ä¸ºé²æ­¢æå¤åçï¼nonebot_plugin_access_controlæ¬èº«ä¸å¯ä»¥è¿è¡æéå¼å³ï¼
 å½æä¸»ä½éè¦æ£æ¥ææå¡æ¯å¦å¯ç¨æ¶ï¼å°ä»è¯¥æå¡å¼å§æ£æ¥æ¯å¦ä¸ºè¯¥ä¸»ä½éç½®äºæéï¼è¥æªéç½®åæ£æ¥å¶ç¶æå¡ï¼ä»¥æ­¤ç±»æ¨ç´å°æ£æ¥å°æ ¹èç¹nonebotã
 æ¢å¥è¯è¯´ï¼å½é´ææ¶ï¼æä»¬éä¸å¯¹ç¨æ·çææä¸»ä½**æä¼åçº§ä»é«å°ä½çé¡ºåº**ï¼**ææå¡çèç¹æ·±åº¦ä»æ·±å°æµçé¡ºåº**æ£æ¥è¯¥æå¡åå¶ææç¥åèç¹éç½®çæéãå æ­¤ï¼å¨èç¹æ·±åº¦è¾æµçæå¡éç½®çé«ä¼åçº§çä¸»ä½éç½®ï¼ä¹ä¼è¦çå¨èç¹æ·±åº¦è¾æ·±çæå¡éç½®çä½ä¼åçº§çä¸»ä½éç½®ã
@@ -76,16 +78,17 @@
 ac limit rm <è§åID>`ï¼å é¤éæµè§å - `/ac limit
 ls`ï¼ååºææå·²éç½®çéæµè§å - `/ac limit ls --sbj
 <ä¸»ä½>`ï¼ååºä¸»ä½å·²éç½®çéæµè§å - `/ac limit ls --srv
 <æå¡>`ï¼ååºæå¡å·²éç½®çéæµè§å - `/ac limit ls --sbj <ä¸»ä½>
 --srv <æå¡>`ï¼ååºä¸»ä½ä¸æå¡å·²éç½®çéæµè§å - `/ac limit
 reset`ï¼éç½®éæµè®¡æ° - æå¡æ¥ç - `/ac service
 ls`ï¼ååºæææå¡ä¸å­æå¡å±çº§ - `/ac service ls --srv
-<æå¡>`ï¼ååºæå¡çå­æå¡å±çº§ å¶ä¸­`<æå¡>`çæ ¼å¼å¦ä¸ï¼ -
-`nonebot`ï¼å¯¹æ´ä¸ªNoneBotè¿è¡å¼å³ -
+<æå¡>`ï¼ååºæå¡çå­æå¡å±çº§ - ä¸»ä½æµè¯ - `/ac
+subject`ï¼ååºæ¶æ¯åéèçææä¸»ä½
+å¶ä¸­`<æå¡>`çæ ¼å¼å¦ä¸ï¼ - `nonebot`ï¼å¯¹æ´ä¸ªNoneBotè¿è¡å¼å³ -
 `<æä»¶å>`ï¼å¯¹æ´ä¸ªæä»¶è¿è¡å¼å³ -
 `<æä»¶å>.<å­æå¡å>.<å­æå¡å>.....<å­æå¡å>`ï¼å¯¹æä»¶åçæä¸ªå­æå¡è¿è¡å¼å³ï¼éåç§ä¸æå¯¹æä»¶è¿è¡éç½®ï¼
 ### ç¤ºä¾ é¦åç¼è¾éç½®æä»¶ï¼æå¼å¯¹æªééæä»¶çæ¯æï¼ ```
 ACCESS_CONTROL_AUTO_PATCH_ENABLED=true ``` åè®¾botå è½½äºåç½®æä»¶echo
 ```python nonebot.load_builtin_plugins("echo") ``` #### é´æ
 æ§è¡ä¸é¢çæä»¤åï¼QQç¨æ·12345678å°æ æ³è°ç¨æä»¤`/echo` ``` /ac
 permission deny --sbj qq:12345678 --srv echo ```
```

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/event_bus.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/__init__.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/handle_error.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/matchers/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/parser.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/matchers/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/rate_limit.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/base.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/permission.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/impl/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/rate_limit.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/impl/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/base.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/permission.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/rate_limit.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/service.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/interface/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/methods.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/nonebot.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/plugin.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice_owner.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/session.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/tree.py` & `nonebot_plugin_access_control-0.5.2/src/nonebot_plugin_access_control/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.1/PKG-INFO` & `nonebot_plugin_access_control-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -69,21 +69,22 @@
 
 回到上面的例子，假设我们对主体”群组G“禁用服务，但是对主体”用户V“启用服务。则用户U在群组G内将无法使用服务，但是用户V在群组G内可以使用。
 
 在插件使用中，我们用一个字符串表示主体，例如`qq:12345678`表示QQ用户12345678、`qq:g87654321`表示QQ群组87654321。
 
 我们约定：`all`表示所有用户、`superuser`表示超级用户、`<平台名>`表示所有此平台的用户、`<协议名>`表示所有此协议的用户、所有与平台相关的主体均以`<平台名>:`开头、所有与协议相关的主体均以`<协议名>:`开头。
 
-各适配器的主体定义如下：
+插件依赖[nonebot-plugin-session](https://github.com/noneplugin/nonebot-plugin-session)提取事件的主体，各适配器的主体定义如下：
 
 - [OneBot V11](docs/onebot_v11.md)
 - [OneBot V12](docs/onebot_v12.md)
 - [Kaiheila](docs/kaiheila.md)
+- [QQ Guild](docs/qqguild.md)
+- Telegram：未测试，参考OneBot V12的定义
 
-如果你能帮助我们进行其他协议适配，欢迎提交PR。
 
 ### 服务
 
 **服务（Service）为一组能够进行权限控制的功能的集合。** 服务可以拥有子服务，通过树形结构组织服务，统一管理权限。
 
 整个NoneBot是一个名为nonebot的服务，为树形结构的根节点，其直接子节点为所有插件。
 
@@ -165,14 +166,16 @@
     - `/ac limit ls --sbj <主体>`：列出主体已配置的限流规则
     - `/ac limit ls --srv <服务>`：列出服务已配置的限流规则
     - `/ac limit ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的限流规则
     - `/ac limit reset`：重置限流计数
 - 服务查看
     - `/ac service ls`：列出所有服务与子服务层级
     - `/ac service ls --srv <服务>`：列出服务的子服务层级
+- 主体测试
+    - `/ac subject`：列出消息发送者的所有主体
 
 其中`<服务>`的格式如下：
 
 - `nonebot`：对整个NoneBot进行开关
 - `<插件名>`：对整个插件进行开关
 - `<插件名>.<子服务名>.<子服务名>.....<子服务名>`：对插件内的某个子服务进行开关（需参照下文对插件进行配置）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.1
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.2
 Summary: Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-datastore
@@ -23,17 +23,19 @@
 ä¸ä¸ªç¨æ·éå¸¸æ¥æå¤ä¸ªä¸»ä½ãä¸¾ä¸ªä¾å­ï¼QQä¸ç¾¤ç»Gçç¨æ·Uåéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·åæ¶å·æâç¨æ·Uâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãåæ¶QQä¸ç¾¤ç»Gçç¨æ·Vä¹åéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·è¯¥ç¨æ·åæ¶å·æâç¨æ·Vâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ã
 å½è®¾ç½®æéæ¶ï¼æä»¬ç´æ¥éå¯¹ä¸ä¸ªä¸»ä½è¿è¡è®¾ç½®ãå½é´ææ¶ï¼æä»¬å¯¹ç¨æ·çææä¸»ä½**æä¼åçº§ä»é«å°ä½çé¡ºåº**ï¼éä¸æ£æ¥æ¯å¦è®¾ç½®äºæéãä¸æ¦æ£æ¥å°æä¸ªä¸»ä½è®¾ç½®äºæéï¼å°±ä»¥è¯¥ä¸»ä½è®¾ç½®çæéä½ä¸ºè¯¥ç¨æ·çæéã
 åå°ä¸é¢çä¾å­ï¼åè®¾æä»¬å¯¹ä¸»ä½âç¾¤ç»Gâç¦ç¨æå¡ï¼ä½æ¯å¯¹ä¸»ä½âç¨æ·Vâå¯ç¨æå¡ãåç¨æ·Uå¨ç¾¤ç»Gåå°æ æ³ä½¿ç¨æå¡ï¼ä½æ¯ç¨æ·Vå¨ç¾¤ç»Gåå¯ä»¥ä½¿ç¨ã
 å¨æä»¶ä½¿ç¨ä¸­ï¼æä»¬ç¨ä¸ä¸ªå­ç¬¦ä¸²è¡¨ç¤ºä¸»ä½ï¼ä¾å¦`qq:
 12345678`è¡¨ç¤ºQQç¨æ·12345678ã`qq:g87654321`è¡¨ç¤ºQQç¾¤ç»87654321ã
 æä»¬çº¦å®ï¼`all`è¡¨ç¤ºææç¨æ·ã`superuser`è¡¨ç¤ºè¶çº§ç¨æ·ã`<å¹³å°å>`è¡¨ç¤ºæææ­¤å¹³å°çç¨æ·ã`<åè®®å>`è¡¨ç¤ºæææ­¤åè®®çç¨æ·ãææä¸å¹³å°ç¸å³çä¸»ä½åä»¥`<å¹³å°å>:
 `å¼å¤´ãææä¸åè®®ç¸å³çä¸»ä½åä»¥`<åè®®å>:`å¼å¤´ã
-åééå¨çä¸»ä½å®ä¹å¦ä¸ï¼ - [OneBot V11](docs/onebot_v11.md) -
-[OneBot V12](docs/onebot_v12.md) - [Kaiheila](docs/kaiheila.md)
-å¦æä½ è½å¸®å©æä»¬è¿è¡å¶ä»åè®®ééï¼æ¬¢è¿æäº¤PRã ### æå¡
+æä»¶ä¾èµ[nonebot-plugin-session](https://github.com/noneplugin/nonebot-
+plugin-session)æåäºä»¶çä¸»ä½ï¼åééå¨çä¸»ä½å®ä¹å¦ä¸ï¼ -
+[OneBot V11](docs/onebot_v11.md) - [OneBot V12](docs/onebot_v12.md) -
+[Kaiheila](docs/kaiheila.md) - [QQ Guild](docs/qqguild.md) -
+Telegramï¼æªæµè¯ï¼åèOneBot V12çå®ä¹ ### æå¡
 **æå¡ï¼Serviceï¼ä¸ºä¸ç»è½å¤è¿è¡æéæ§å¶çåè½çéåã**
 æå¡å¯ä»¥æ¥æå­æå¡ï¼éè¿æ å½¢ç»æç»ç»æå¡ï¼ç»ä¸ç®¡çæéã
 æ´ä¸ªNoneBotæ¯ä¸ä¸ªåä¸ºnonebotçæå¡ï¼ä¸ºæ å½¢ç»æçæ ¹èç¹ï¼å¶ç´æ¥å­èç¹ä¸ºæææä»¶ã
 ä¸ä¸ªæä»¶æ¯ä¸ä¸ªæå¡ï¼PluginServiceï¼ï¼å¶ç¶èç¹ä¸ºnonebotãå½æä»¶æªè¿è¡ééæ¶ï¼è¯¥æä»¶åªå·æè¿ä¸ä¸ªPluginServiceãå¯¹æä»¶è¿è¡ééï¼åéè¦ä»æä»¶çPluginServiceåå»ºSubServiceï¼ä¸ºæä»¶çMatcherç­åè½å¥å£åºç¨SubServiceãï¼åèä¸ææä»¶ééç« èï¼
 ï¼ä¸ºé²æ­¢æå¤åçï¼nonebot_plugin_access_controlæ¬èº«ä¸å¯ä»¥è¿è¡æéå¼å³ï¼
 å½æä¸»ä½éè¦æ£æ¥ææå¡æ¯å¦å¯ç¨æ¶ï¼å°ä»è¯¥æå¡å¼å§æ£æ¥æ¯å¦ä¸ºè¯¥ä¸»ä½éç½®äºæéï¼è¥æªéç½®åæ£æ¥å¶ç¶æå¡ï¼ä»¥æ­¤ç±»æ¨ç´å°æ£æ¥å°æ ¹èç¹nonebotã
 æ¢å¥è¯è¯´ï¼å½é´ææ¶ï¼æä»¬éä¸å¯¹ç¨æ·çææä¸»ä½**æä¼åçº§ä»é«å°ä½çé¡ºåº**ï¼**ææå¡çèç¹æ·±åº¦ä»æ·±å°æµçé¡ºåº**æ£æ¥è¯¥æå¡åå¶ææç¥åèç¹éç½®çæéãå æ­¤ï¼å¨èç¹æ·±åº¦è¾æµçæå¡éç½®çé«ä¼åçº§çä¸»ä½éç½®ï¼ä¹ä¼è¦çå¨èç¹æ·±åº¦è¾æ·±çæå¡éç½®çä½ä¼åçº§çä¸»ä½éç½®ã
@@ -87,16 +89,17 @@
 ac limit rm <è§åID>`ï¼å é¤éæµè§å - `/ac limit
 ls`ï¼ååºææå·²éç½®çéæµè§å - `/ac limit ls --sbj
 <ä¸»ä½>`ï¼ååºä¸»ä½å·²éç½®çéæµè§å - `/ac limit ls --srv
 <æå¡>`ï¼ååºæå¡å·²éç½®çéæµè§å - `/ac limit ls --sbj <ä¸»ä½>
 --srv <æå¡>`ï¼ååºä¸»ä½ä¸æå¡å·²éç½®çéæµè§å - `/ac limit
 reset`ï¼éç½®éæµè®¡æ° - æå¡æ¥ç - `/ac service
 ls`ï¼ååºæææå¡ä¸å­æå¡å±çº§ - `/ac service ls --srv
-<æå¡>`ï¼ååºæå¡çå­æå¡å±çº§ å¶ä¸­`<æå¡>`çæ ¼å¼å¦ä¸ï¼ -
-`nonebot`ï¼å¯¹æ´ä¸ªNoneBotè¿è¡å¼å³ -
+<æå¡>`ï¼ååºæå¡çå­æå¡å±çº§ - ä¸»ä½æµè¯ - `/ac
+subject`ï¼ååºæ¶æ¯åéèçææä¸»ä½
+å¶ä¸­`<æå¡>`çæ ¼å¼å¦ä¸ï¼ - `nonebot`ï¼å¯¹æ´ä¸ªNoneBotè¿è¡å¼å³ -
 `<æä»¶å>`ï¼å¯¹æ´ä¸ªæä»¶è¿è¡å¼å³ -
 `<æä»¶å>.<å­æå¡å>.<å­æå¡å>.....<å­æå¡å>`ï¼å¯¹æä»¶åçæä¸ªå­æå¡è¿è¡å¼å³ï¼éåç§ä¸æå¯¹æä»¶è¿è¡éç½®ï¼
 ### ç¤ºä¾ é¦åç¼è¾éç½®æä»¶ï¼æå¼å¯¹æªééæä»¶çæ¯æï¼ ```
 ACCESS_CONTROL_AUTO_PATCH_ENABLED=true ``` åè®¾botå è½½äºåç½®æä»¶echo
 ```python nonebot.load_builtin_plugins("echo") ``` #### é´æ
 æ§è¡ä¸é¢çæä»¤åï¼QQç¨æ·12345678å°æ æ³è°ç¨æä»¤`/echo` ``` /ac
 permission deny --sbj qq:12345678 --srv echo ```
```

