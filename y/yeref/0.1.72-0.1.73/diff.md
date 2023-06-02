# Comparing `tmp/yeref-0.1.72.tar.gz` & `tmp/yeref-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.72.tar", last modified: Thu Jun  1 11:57:39 2023, max compression
+gzip compressed data, was "yeref-0.1.73.tar", last modified: Fri Jun  2 12:28:12 2023, max compression
```

## Comparing `yeref-0.1.72.tar` & `yeref-0.1.73.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-01 11:57:39.092430 yeref-0.1.72/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-01 11:57:39.092668 yeref-0.1.72/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-01 11:57:39.093507 yeref-0.1.72/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-01 11:57:12.000000 yeref-0.1.72/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-01 11:57:39.089486 yeref-0.1.72/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.72/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489747 2023-05-30 14:52:13.000000 yeref-0.1.72/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   207128 2023-06-01 11:53:54.000000 yeref-0.1.72/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-01 11:57:39.092039 yeref-0.1.72/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 12:28:12.064344 yeref-0.1.73/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 12:28:12.064496 yeref-0.1.73/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-02 12:28:12.065116 yeref-0.1.73/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-02 12:27:53.000000 yeref-0.1.73/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 12:28:12.057676 yeref-0.1.73/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.73/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   490632 2023-06-02 12:19:49.000000 yeref-0.1.73/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   208414 2023-06-02 10:26:58.000000 yeref-0.1.73/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 12:28:12.063953 yeref-0.1.73/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.72/setup.py` & `yeref-0.1.73/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.72',
+      version='0.1.73',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.71-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.72-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.72/yeref/l_.py` & `yeref-0.1.73/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -6982,8 +6982,58 @@
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
 # endregion
 
 
+# region html
+l_trg_add = {
+    'ru': '+ Добавить Триггер',
+    'en': '+ Add Trigger',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_trg_cmd = {
+    'ru': '+ команда',
+    'en': '+ command',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_trg_txt = {
+    'ru': '+ текст',
+    'en': '+ text',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_trg_btn = {
+    'ru': '+ кнопка',
+    'en': '+ button',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_trg_var = {
+    'ru': '+ переменная',
+    'en': '+ variable',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_trg_lst = {
+    'ru': '+ список',
+    'en': '+ list',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+# endregion
 # endregion
```

### Comparing `yeref-0.1.72/yeref/yeref.py` & `yeref-0.1.73/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,14 +488,21 @@
 
                 timestamp_ = str(utils.datetime_to_timestamp(datetime.datetime.utcnow()))
                 content_json[timestamp_] = json_
                 post_dumps = json.dumps(content_json, ensure_ascii=False)
                 await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content=post_dumps)
                 return 1
         except Exception as e:
+            if 'Flood control exceeded' in str(e):
+                try:
+                    secs = int(str(e).split(' seconds')[0].split()[-1])
+                    if secs < 10: await asyncio.sleep(secs+1)
+                except Exception as e:
+                    logger.info(log_ % str(e))
+                    await asyncio.sleep(round(random.uniform(1, 2), 2))
             logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(1, 2), 2))
         finally:
             retry -= 1
     return 0
 
 
@@ -677,22 +684,22 @@
 
         access_token = TGPH_TOKENS[access_key]
         telegraph_ = Telegraph(access_token=access_token)
         pages = await telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
-                if item['url'] == access_key:
-                    page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
-                    try:
-                        content_json = json.loads(str(page['content'][0]))
-                    except:
-                        content_json = {}
+                if item['url'] != access_key: continue
+                page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
+                try:
+                    content_json = json.loads(str(page['content'][0]))
+                except:
+                    content_json = {}
 
-                    for OFFER_USERTID, v in content_json.items():
+                for OFFER_USERTID, v in content_json.items():
                         OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
                             OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
                             OFFER_DT, OFFER_TZ = v
 
                         sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
                               "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
                               "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
@@ -704,14 +711,16 @@
                                               v[OFFER_DT], v[OFFER_TZ],), BASE_D)
 
                         del content_json[str(OFFER_USERTID)]
                         post_dumps = json.dumps(content_json, ensure_ascii=False)
                         await telegraph_.edit_page(path=item['path'], title=access_key, html_content=post_dumps)
                         return
             except Exception as e:
+                if 'Flood control exceeded' in str(e):
+                    await run_shell(f'/usr/bin/pm2 restart {bot_username}')
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
@@ -2197,14 +2206,40 @@
     finally:
         return result
 
 # endregion
 
 
 # region functions
+async def run_shell(cmd):
+    result = None
+    try:
+        proc = await asyncio.create_subprocess_shell(
+            cmd,
+            stderr=asyncio.subprocess.PIPE,
+            stdout=asyncio.subprocess.PIPE
+        )
+        stdout, stderr = await proc.communicate()
+
+        logger.info(log_ % f'[{cmd!r} exited with {proc.returncode}]')
+        if stdout:
+            logger.info(log_ % f'{stdout.decode()}')
+            result = f'[stdout]\n{stdout.decode()}'
+        if stderr:
+            logger.info(log_ % f'{stderr.decode()}')
+            result = f'[stderr]\n{stderr.decode()}'
+        else:
+            result = str(proc.returncode)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return result
+
+
 def escape_md(*content, sep=" ") -> str:
     """
     Escape markdown text
 
     E.g. for usernames
 
     :param content:
```

