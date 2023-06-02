# Comparing `tmp/yapsygui-1.1.3-py3-none-any.whl.zip` & `tmp/yapsygui-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17456 bytes, number of entries: 28
--rw-rw-r--  2.0 unx      383 b- defN 23-Jun-02 16:34 yapsygui/__init__.py
+Zip file size: 17459 bytes, number of entries: 28
+-rw-rw-r--  2.0 unx      383 b- defN 23-Jun-02 16:39 yapsygui/__init__.py
 -rw-rw-r--  2.0 unx     1107 b- defN 23-Jun-02 15:56 yapsygui/__main__.py
 -rw-rw-r--  2.0 unx     2093 b- defN 23-Jun-02 16:33 yapsygui/dialog.py
 -rw-rw-r--  2.0 unx      257 b- defN 23-Jun-01 19:23 yapsygui/endpoint.py
 -rw-rw-r--  2.0 unx      371 b- defN 23-May-29 18:45 yapsygui/items.py
 -rw-rw-r--  2.0 unx     1648 b- defN 23-Jun-01 00:05 yapsygui/manager.py
 -rw-rw-r--  2.0 unx     1454 b- defN 23-Jun-01 21:54 yapsygui/network_request.py
 -rw-rw-r--  2.0 unx     1096 b- defN 23-Jun-01 21:56 yapsygui/plugin_action.py
@@ -17,14 +17,14 @@
 -rw-rw-r--  2.0 unx      390 b- defN 23-May-29 22:32 yapsygui/ui/alert.py
 -rw-rw-r--  2.0 unx     1068 b- defN 23-Jun-02 15:51 yapsygui/ui/dialog_plugin_base.py
 -rw-rw-r--  2.0 unx      358 b- defN 23-Jun-01 02:12 yapsygui/ui/open_file.py
 -rw-rw-r--  2.0 unx      539 b- defN 23-Jun-01 22:39 yapsygui/ui/panel_description.py
 -rw-rw-r--  2.0 unx      528 b- defN 23-May-28 01:33 yapsygui/ui/panel_plugins.py
 -rw-rw-r--  2.0 unx      781 b- defN 23-Jun-01 02:19 yapsygui/ui/row_buttons.py
 -rw-rw-r--  2.0 unx     1824 b- defN 23-Jun-01 02:46 yapsygui/ui/twin_panel.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-02 16:34 yapsygui-1.1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-02 16:34 yapsygui-1.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 16:34 yapsygui-1.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       52 b- defN 23-Jun-02 16:34 yapsygui-1.1.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-02 16:34 yapsygui-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2248 b- defN 23-Jun-02 16:34 yapsygui-1.1.3.dist-info/RECORD
-28 files, 35378 bytes uncompressed, 13856 bytes compressed:  60.8%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-02 16:41 yapsygui-1.1.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2951 b- defN 23-Jun-02 16:41 yapsygui-1.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 16:41 yapsygui-1.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       52 b- defN 23-Jun-02 16:41 yapsygui-1.1.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-02 16:41 yapsygui-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2248 b- defN 23-Jun-02 16:41 yapsygui-1.1.4.dist-info/RECORD
+28 files, 35383 bytes uncompressed, 13859 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -60,26 +60,26 @@
 
 Filename: yapsygui/ui/row_buttons.py
 Comment: 
 
 Filename: yapsygui/ui/twin_panel.py
 Comment: 
 
-Filename: yapsygui-1.1.3.dist-info/LICENSE
+Filename: yapsygui-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: yapsygui-1.1.3.dist-info/METADATA
+Filename: yapsygui-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: yapsygui-1.1.3.dist-info/WHEEL
+Filename: yapsygui-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: yapsygui-1.1.3.dist-info/entry_points.txt
+Filename: yapsygui-1.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: yapsygui-1.1.3.dist-info/top_level.txt
+Filename: yapsygui-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: yapsygui-1.1.3.dist-info/RECORD
+Filename: yapsygui-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yapsygui/__init__.py

```diff
@@ -1,9 +1,9 @@
 __appname__ = "Yapsy GUI"
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 from .items import PluginItem
 
 from .ui import TwinPanel
 from .ui import RowButtons
 from .ui import OpenFilePlugin
```

## Comparing `yapsygui-1.1.3.dist-info/LICENSE` & `yapsygui-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yapsygui-1.1.3.dist-info/METADATA` & `yapsygui-1.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapsygui
-Version: 1.1.3
+Version: 1.1.4
 Summary: GUI for Yapsy plugin system
 Home-page: https://github.com/leonelhs/yapsy-gui
 Author: leonel hernandez
 Author-email: leonelhs@gmail.com
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -84,15 +84,15 @@
 
 app = QtWidgets.QApplication()
 win = QWidget(None)
 win.setLayout(QVBoxLayout())
 btn_manager = QPushButton("Show Manager")
 win.layout().addWidget(btn_manager)
 
-manager = DialogPlugins("./plugins")
+manager = DialogPlugins(win, "./plugins")
 manager.connect(fetchPlugins)
 manager.loadPlugins()
 
 btn_manager.clicked.connect(manager.show)
 win.output = QTextBrowser(win)
 win.layout().addWidget(win.output)
```

## Comparing `yapsygui-1.1.3.dist-info/RECORD` & `yapsygui-1.1.4.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-yapsygui/__init__.py,sha256=rCYRlv-qgRfn4NVAMmmInTwLsRU8tsfgGEsIAq0G73o,383
+yapsygui/__init__.py,sha256=REM5XAn1IirAG42x4hkjEimS8mkuK2W2BcQis6BvC9Y,383
 yapsygui/__main__.py,sha256=POotSvAjd4ooRicamlZH6sCbCbGsYYyC-THm8sZwilA,1107
 yapsygui/dialog.py,sha256=a0DjqcYJjaqb88zH9brHmhgniBrj1EyZuh2SSLOexCY,2093
 yapsygui/endpoint.py,sha256=HRD7ptDYCpaWBxXkB2EaL9ZqMEJF9R3eODMwCxwexb0,257
 yapsygui/items.py,sha256=XluP0tUgIid9Tv2-qZiUcEt8WN_pI8ebM0FxTSEkyZk,371
 yapsygui/manager.py,sha256=8Arr4Bo452NPTIGZjb4lTitnuP-8GtDPx0z2iE9G9Ek,1648
 yapsygui/network_request.py,sha256=iAsKl3UTRZu6gq6-WLRWIBu6JLpKhNrwe60iQpzkhtY,1454
 yapsygui/plugin_action.py,sha256=PmMpmCHWJJyiVW8aR0l112GqFOa_aVYIFOJSZD2pMZE,1096
@@ -16,13 +16,13 @@
 yapsygui/ui/alert.py,sha256=-dVGKL-IY4EvxtJT7joyoXJhOZ1TUtNiYREkKhmd8XA,390
 yapsygui/ui/dialog_plugin_base.py,sha256=gRL9QDb0BgMYt8RSOA3yKh8_MhKTmVRHaI-zyS2QZHI,1068
 yapsygui/ui/open_file.py,sha256=q3htjtPtd3Wp35HyXvKaoudretVueAO_f6XNHh1JY1o,358
 yapsygui/ui/panel_description.py,sha256=VQv_x9-FlUiEB7xByRAoTradv1zuLeDAdEAcE4b6fTs,539
 yapsygui/ui/panel_plugins.py,sha256=-fJbjoJg-5Ka3XSKQsI0tmr_JJk-VKw0Kmfrtn34BWs,528
 yapsygui/ui/row_buttons.py,sha256=YZr0CMqadjpqzS6DC5mIYTVA8cjvAGltpzG9Cp82GhM,781
 yapsygui/ui/twin_panel.py,sha256=kI_A9ah3CnL9-lPa4C5Unx5HLlo0O3u0Y7rqUZBEmZA,1824
-yapsygui-1.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-yapsygui-1.1.3.dist-info/METADATA,sha256=8L-nkeeT6Y0GM1xb17zS1ep92TTcJgYpJ8OKPfFwYDQ,2946
-yapsygui-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-yapsygui-1.1.3.dist-info/entry_points.txt,sha256=AOdUxNWqkMSfPH546Hb5FuK3kvJBYFgpuLhdtnqF_tA,52
-yapsygui-1.1.3.dist-info/top_level.txt,sha256=fNAHdkKr7kkYdlRuUe58Hqut4Min7VIbvjfNKfxntMc,9
-yapsygui-1.1.3.dist-info/RECORD,,
+yapsygui-1.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+yapsygui-1.1.4.dist-info/METADATA,sha256=g4pXrUkhl4jyYpsI_EFkMPm28LDN5AkC3isfRvp81RY,2951
+yapsygui-1.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+yapsygui-1.1.4.dist-info/entry_points.txt,sha256=AOdUxNWqkMSfPH546Hb5FuK3kvJBYFgpuLhdtnqF_tA,52
+yapsygui-1.1.4.dist-info/top_level.txt,sha256=fNAHdkKr7kkYdlRuUe58Hqut4Min7VIbvjfNKfxntMc,9
+yapsygui-1.1.4.dist-info/RECORD,,
```

