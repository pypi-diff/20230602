# Comparing `tmp/yeref-0.1.73.tar.gz` & `tmp/yeref-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.73.tar", last modified: Fri Jun  2 12:28:12 2023, max compression
+gzip compressed data, was "yeref-0.1.74.tar", last modified: Fri Jun  2 13:26:11 2023, max compression
```

## Comparing `yeref-0.1.73.tar` & `yeref-0.1.74.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 12:28:12.064344 yeref-0.1.73/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 12:28:12.064496 yeref-0.1.73/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-02 12:28:12.065116 yeref-0.1.73/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-02 12:27:53.000000 yeref-0.1.73/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 12:28:12.057676 yeref-0.1.73/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.73/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   490632 2023-06-02 12:19:49.000000 yeref-0.1.73/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   208414 2023-06-02 10:26:58.000000 yeref-0.1.73/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 12:28:12.063953 yeref-0.1.73/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-02 12:28:12.000000 yeref-0.1.73/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 13:26:11.810033 yeref-0.1.74/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 13:26:11.810283 yeref-0.1.74/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-02 13:26:11.811228 yeref-0.1.74/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-02 13:26:00.000000 yeref-0.1.74/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 13:26:11.802521 yeref-0.1.74/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.74/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   495236 2023-06-02 13:25:19.000000 yeref-0.1.74/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   208414 2023-06-02 10:26:58.000000 yeref-0.1.74/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 13:26:11.809322 yeref-0.1.74/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 13:26:11.000000 yeref-0.1.74/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-02 13:26:11.000000 yeref-0.1.74/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-02 13:26:11.000000 yeref-0.1.74/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-02 13:26:11.000000 yeref-0.1.74/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.73/setup.py` & `yeref-0.1.74/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.73',
+      version='0.1.74',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.73/yeref/l_.py` & `yeref-0.1.74/yeref/l_.py`

 * *Files 2% similar despite different names*

```diff
@@ -6983,14 +6983,144 @@
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
 # endregion
 
 
 # region html
+l_burger_save = {
+    'ru': 'Сохранить',
+    'en': 'Save',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_gen = {
+    'ru': 'Сгенерировать бота',
+    'en': 'Generate Bot',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_import = {
+    'ru': 'Импортировать .bot',
+    'en': 'Import .bot',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_export = {
+    'ru': 'Экспортировать как >',
+    'en': 'Export as >',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_clear = {
+    'ru': 'Очистка',
+    'en': 'Clear',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_gen_alert = {
+    'ru': 'Создать нового бота?',
+    'en': 'Create a new bot?',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_import_alert = {
+    'ru': 'Загрузка..',
+    'en': 'Loading..',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_burger_clear_alert = {
+    'ru': 'Очистить сцену?',
+    'en': 'Clear the stage?',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+
+l_ent_close = {
+    'ru': 'Закрыть',
+    'en': 'Close',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_ent_save = {
+    'ru': 'Сохранить',
+    'en': 'Save',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_copied = {
+    'ru': 'Скопировано',
+    'en': 'Copied',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_web_gen_img = {
+    'ru': 'Сгенерировать Образ',
+    'en': 'Generate Image',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_web_gen_txt = {
+    'ru': 'Сгенерировать Текст',
+    'en': 'Generate Text',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_all_trg = {
+    'ru': ': все триггеры',
+    'en': ': all triggers',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_one_trg = {
+    'ru': ': 1 триггер',
+    'en': ': 1 trigger',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_actions = {
+    'ru': ': действия',
+    'en': ': actions',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+
 l_trg_add = {
     'ru': '+ Добавить Триггер',
     'en': '+ Add Trigger',
     'es': 'Save',
     'fr': 'Save',
     'zh': 'Save',
     'ar': 'Save',
@@ -7031,9 +7161,132 @@
     'ru': '+ список',
     'en': '+ list',
     'es': 'Save',
     'fr': 'Save',
     'zh': 'Save',
     'ar': 'Save',
 }
+
+l_act_add = {
+    'ru': '+ Добавить Действие',
+    'en': '+ Add Action',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_act_dly = {
+    'ru': '+ задержка',
+    'en': '+ delay',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_act_wait = {
+    'ru': '+ ожидание',
+    'en': '+ wait',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_act_req = {
+    'ru': '+ запрос',
+    'en': '+ request',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+
+l_msg_text = {
+    'ru': ': text',
+    'en': ': text',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_photo = {
+    'ru': ': фото',
+    'en': ': photo',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_gif = {
+    'ru': ': гиф',
+    'en': ': gif',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_video = {
+    'ru': ': видео',
+    'en': ': video',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_video_note = {
+    'ru': ': телескоп',
+    'en': ': video note',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_audio = {
+    'ru': ': аудио',
+    'en': ': audio',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_voice = {
+    'ru': ': голосовое',
+    'en': ': voice',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_document = {
+    'ru': ': документ',
+    'en': ': document',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_sticker = {
+    'ru': ': стикер',
+    'en': ': sticker',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_quiz = {
+    'ru': ': опрос',
+    'en': ': quiz',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_msg_dice = {
+    'ru': ': игра',
+    'en': ': dice',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+
 # endregion
 # endregion
```

### Comparing `yeref-0.1.73/yeref/yeref.py` & `yeref-0.1.74/yeref/yeref.py`

 * *Files identical despite different names*

