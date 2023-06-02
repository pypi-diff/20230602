# Comparing `tmp/nonebot_plugin_rename-1.3.5.tar.gz` & `tmp/nonebot_plugin_rename-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.3.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.3.7.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.3.5.tar` & `nonebot_plugin_rename-1.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/LICENSE
--rw-r--r--   0        0        0     5286 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/README.md
--rw-r--r--   0        0        0      363 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      293 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      844 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      893 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/starrail_time.py
--rw-r--r--   0        0        0      604 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      376 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8894 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      151 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      838 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1529 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      644 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/LICENSE
+-rw-r--r--   0        0        0     5286 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/README.md
+-rw-r--r--   0        0        0      495 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      903 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      893 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/starrail_time.py
+-rw-r--r--   0        0        0      604 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      377 2023-06-02 01:25:50.926933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8740 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      151 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      838 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1529 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      574 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.7/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.3.5/LICENSE` & `nonebot_plugin_rename-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/README.md` & `nonebot_plugin_rename-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/starrail_time.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# Description: 获取高考倒计时
-
+# Description: 获取星穹铁道版本剩余时间
 from datetime import datetime
 
 
-def gk() -> str:
-    # 基准时间
-    year = 2023
+def starrail_version_time() -> str:
+    # 基准版本
+    Version = 1.0
     baseTime = (
-        datetime.strptime("2023-6-7 9:00:00", "%Y-%m-%d %H:%M:%S").timestamp() * 1000
+        datetime.strptime("2023-4-26 10:00:00", "%Y-%m-%d %H:%M:%S").timestamp() * 1000
     )
     nowTime = datetime.now().timestamp() * 1000
     # 获取持续时间
     duringTime = baseTime - nowTime
     while duringTime <= 0:
-        # 时间+365天 年份+1年
-        duringTime += 365 * 24 * 60 * 60 * 1000
-        year += 1
+        # 版本+0.1 同时时间+42天
+        duringTime += 42 * 24 * 60 * 60 * 1000
+        Version += 0.1
     # 获取天数并取整
     days = int(duringTime / (24 * 3600 * 1000))
     leave1 = duringTime % (24 * 3600 * 1000)
     # 获取小时数并取整
     hours = int(leave1 / (3600 * 1000))
     leave2 = leave1 % (3600 * 1000)
     # 获取分钟数并取整
     minutes = int(leave2 / (60 * 1000))
-    return f"离{year}年高考还有{days}天{hours}小时{minutes}分钟"
+    return f"离崩铁{Version:.1f}还有{days}天{hours}小时{minutes}分钟"
```

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,23 @@
     choice_card,
     generate_card_image,
     read_yaml,
     write_yaml,
 )
 
 require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler # noqa
+from nonebot_plugin_apscheduler import scheduler  # noqa
 
 driver: Driver = get_driver()
 env_config = Config.parse_obj(get_driver().config.dict())
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
-    NICKNAME = (
-        env_config.self_name
-        if env_config.self_name
-        else list(driver.config.nickname)[0]
-    )
+    NICKNAME = env_config.self_name or list(driver.config.nickname)[0]
 else:
-    NICKNAME = env_config.self_name if env_config.self_name else "bot"
+    NICKNAME = env_config.self_name or "bot"
 yml_file = Path.cwd() / "data" / "group_card"
 permissions = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
 
 group_card = on_command(
     "设置群名片",
     aliases={"更改群名片", "修改群名片"},
     permission=permissions,
@@ -96,41 +92,38 @@
     nicks = " ".join(group_nicknames)
     if not group_nicknames:
         await group_card.finish("请输入你想要设置的群名片序号")
     group_id = str(event.group_id)
     bot_id = bot.self_id
     # 读取群名片数据
     group_data = read_yaml(yml_file / "group_card.yaml") or {}
-    group_nicknames_valid = not any(
+    group_nicknames_valid = any(
         int(gn) > len(card_list) for gn in group_nicknames
     )  # 判断用户输入的群名片序号是否有效
     # 更新群名片数据
     if group_nicknames_valid:
-        group_data.setdefault(bot_id, {})
-        group_data[bot_id].setdefault(group_id, {})
-        group_data[bot_id][group_id] = group_nicknames
-        write_yaml(yml_file / "group_card.yaml", group_data)
-        await group_card.finish(f"已为你更改该群群名片序号为{nicks}")
-    else:
         await group_card.finish("没有这种群名片哦")
+    group_data.setdefault(bot_id, {})
+    group_data[bot_id].setdefault(group_id, {})
+    group_data[bot_id][group_id] = group_nicknames
+    write_yaml(yml_file / "group_card.yaml", group_data)
+    await group_card.finish(f"已为你更改该群群名片序号为{nicks}")
 
 
 # 定时任务执行函数
 async def set_group_card(is_handle: bool = False):
     tasks = []
     set_wrong = []
     bots = get_bots()
     group_data = read_yaml(yml_file / "group_card.yaml") or {}
     if not group_data:
         return
     for bot_id, bot_case in bots.items():
-        group_info = group_data.get(bot_id, {})
-        if not group_info:
-            continue
-        tasks.extend(await set_card(group_info, bot_id, bot_case))
+        if group_info := group_data.get(bot_id, {}):
+            tasks.extend(await set_card(group_info, bot_id, bot_case))
     results = await asyncio.gather(*tasks, return_exceptions=True)
     for group_info, result in zip(group_data.values(), results):
         group_id = next(iter(group_info))
         if isinstance(result, Exception):
             logger.warning(f"群{group_id}名片更改失败，错误信息：{result}")
             set_wrong.append(group_id)
     if is_handle:
@@ -160,15 +153,15 @@
 
 # on_command "立即更改群名片"
 @set_card_now.handle()
 async def _(bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()):
     card_number = arg.extract_plain_text().strip()
     if not card_number:
         await set_card_now.finish("请输入序号或序号输入错误")
-    elif card_number not in map(str, range(1, len(card_list)+1)):
+    elif card_number not in map(str, range(1, len(card_list) + 1)):
         await set_card_now.finish("没有这种类型的群名片哦，可以发送[查看群名片列表]命令查看吧")
     card_names = await choice_card(card_number)
     if env_config.use_nickname_front:
         card_names = f"{NICKNAME}|{card_names}"
     try:
         await bot.set_group_card(
             group_id=event.group_id, user_id=int(bot.self_id), card=card_names
```

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.5/pyproject.toml` & `nonebot_plugin_rename-1.3.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.3.5"
+version = "1.3.7"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
-[[tool.poetry.source]]
-name = "ali"
-default = true
-url = "https://mirrors.aliyun.com/pypi/simple/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.23.3"
+httpx = ">=0.20.0, <1.0.0"
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-plugin-apscheduler = "^0.2.0"
 psutil = "^5.9.5"
 pyyaml = "^6.0"
 pillow = "^9.5.0"
+nonebot2 = "^2.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_rename-1.3.5/PKG-INFO` & `nonebot_plugin_rename-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.3.5
+Version: 1.3.7
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.7 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-
+Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-
-Dist: psutil (>=5.9.5,<6.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Description-
-Content-Type: text/markdown
+apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-
+Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: psutil (>=5.9.5,<6.0.0) Requires-
+Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                          # nonebot-plugin-rename _â¨
 éè¿å®æ¶ä»»å¡æ´æ¹botæå¨ç¾¤èªå·±çç¾¤åç,åç½®äºå ç§å¸¸è§çç¾¤åçå¹¶ä¸åæ­¥æ¯æäºå¤bot,æ¬¢è¿**pr**æ°çç¾¤åç!
                         â¨_ [license] [pypi] [python]
  * [nonebot-plugin-rename](#nonebot-plugin-rename) * [ðç®ä»](#ç®ä») *
 [ðè®¸å¯](#è®¸å¯) * [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) *
```

