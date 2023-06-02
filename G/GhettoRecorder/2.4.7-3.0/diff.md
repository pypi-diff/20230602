# Comparing `tmp/GhettoRecorder-2.4.7.tar.gz` & `tmp/GhettoRecorder-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GhettoRecorder-2.4.7.tar", last modified: Tue Apr  4 17:01:31 2023, max compression
+gzip compressed data, was "GhettoRecorder-3.0.tar", last modified: Fri Jun  2 16:28:12 2023, max compression
```

## Comparing `GhettoRecorder-2.4.7.tar` & `GhettoRecorder-3.0.tar`

### file list

```diff
@@ -1,41 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 17:01:31.851373 GhettoRecorder-2.4.7/
-drwxrwxrwx   0        0        0        0 2023-04-04 17:01:31.804554 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/
--rw-rw-rw-   0        0        0     7581 2023-04-04 17:01:31.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      924 2023-04-04 17:01:31.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 17:01:31.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-04 17:01:31.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      153 2023-04-04 17:01:31.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-04 17:01:31.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-04 17:01:30.000000 GhettoRecorder-2.4.7/GhettoRecorder.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1106 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/LICENSE.rst
--rw-rw-rw-   0        0        0      627 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7581 2023-04-04 17:01:31.851373 GhettoRecorder-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     5388 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-04 17:01:31.808455 GhettoRecorder-2.4.7/docs/
--rw-rw-rw-   0        0        0      756 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/Makefile
--rwxrwxrwx   0        0        0      804 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-04 17:01:31.822109 GhettoRecorder-2.4.7/docs/source/
--rw-rw-rw-   0        0        0     5301 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-04 17:01:31.824062 GhettoRecorder-2.4.7/docs/source/_static/
--rw-rw-rw-   0        0        0      458 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/_static/css-style.css
--rw-rw-rw-   0        0        0     1951 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/conf.py
--rw-rw-rw-   0        0        0    14278 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/ghetto_logo.png
--rw-rw-rw-   0        0        0     1969 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/ghettorecorder.rst
--rw-rw-rw-   0        0        0      313 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/index.rst
--rw-rw-rw-   0        0        0       86 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-04-04 17:01:31.849466 GhettoRecorder-2.4.7/ghettorecorder/
--rw-rw-rw-   0        0        0       99 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/__init__.py
--rw-rw-rw-   0        0        0     5720 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/api.py
--rw-rw-rw-   0        0        0      339 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/cmd.py
--rw-rw-rw-   0        0        0     3236 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_blacklist.py
--rw-rw-rw-   0        0        0     3235 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_container.py
--rw-rw-rw-   0        0        0     1741 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_http_srv.py
--rw-rw-rw-   0        0        0     7541 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_ini.py
--rw-rw-rw-   0        0        0    17119 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_menu.py
--rw-rw-rw-   0        0        0     7339 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_meta.py
--rw-rw-rw-   0        0        0     4520 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_net.py
--rw-rw-rw-   0        0        0      398 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_recorder.ascii
--rw-rw-rw-   0        0        0    53113 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/ghetto_recorder.py
--rw-rw-rw-   0        0        0     1407 2023-04-04 16:25:49.000000 GhettoRecorder-2.4.7/ghettorecorder/settings.ini
--rw-rw-rw-   0        0        0     1496 2023-04-04 16:58:16.000000 GhettoRecorder-2.4.7/pyproject.toml
--rw-rw-rw-   0        0        0      432 2023-04-04 17:01:31.854297 GhettoRecorder-2.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:12.000936 GhettoRecorder-3.0/
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:11.941444 GhettoRecorder-3.0/GhettoRecorder.egg-info/
+-rw-rw-rw-   0        0        0     8439 2023-06-02 16:28:11.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1322 2023-06-02 16:28:11.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 16:28:11.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-02 16:28:11.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-06-02 16:28:11.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 16:28:11.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 16:18:39.000000 GhettoRecorder-3.0/GhettoRecorder.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1106 2023-05-07 15:30:09.000000 GhettoRecorder-3.0/LICENSE.rst
+-rw-rw-rw-   0        0        0      183 2023-05-25 14:50:20.000000 GhettoRecorder-3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8439 2023-06-02 16:28:12.000936 GhettoRecorder-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7619 2023-06-02 13:28:21.000000 GhettoRecorder-3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:11.987282 GhettoRecorder-3.0/ghettorecorder/
+-rw-rw-rw-   0        0        0    21445 2023-05-31 16:23:59.000000 GhettoRecorder-3.0/ghettorecorder/__init__.py
+-rw-rw-rw-   0        0        0    17147 2023-06-02 08:54:28.000000 GhettoRecorder-3.0/ghettorecorder/__main__.py
+-rw-rw-rw-   0        0        0     2496 2023-05-07 15:30:09.000000 GhettoRecorder-3.0/ghettorecorder/audio_conf.py
+-rw-rw-rw-   0        0        0     6507 2023-05-30 15:07:54.000000 GhettoRecorder-3.0/ghettorecorder/cmd.py
+-rw-rw-rw-   0        0        0     3515 2023-05-07 15:30:09.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_agents.py
+-rw-rw-rw-   0        0        0     3808 2023-05-22 16:47:10.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_api.py
+-rw-rw-rw-   0        0        0     8980 2023-06-02 08:20:30.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_blacklist.py
+-rw-rw-rw-   0        0        0     3838 2023-05-25 21:14:12.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_container.py
+-rw-rw-rw-   0        0        0     9396 2023-05-08 18:06:02.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_db_worker.py
+-rw-rw-rw-   0        0        0     7174 2023-05-07 15:30:09.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_header_aac.py
+-rw-rw-rw-   0        0        0     6538 2023-05-22 16:53:15.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_header_mp3.py
+-rw-rw-rw-   0        0        0     2350 2023-05-12 11:00:55.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_http_simple.py
+-rw-rw-rw-   0        0        0     8116 2023-06-02 07:03:27.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_ini.py
+-rw-rw-rw-   0        0        0    17323 2023-06-02 08:42:22.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_menu.py
+-rw-rw-rw-   0        0        0     8141 2023-05-19 09:30:01.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_meta.py
+-rw-rw-rw-   0        0        0     6212 2023-05-22 08:01:54.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_net.py
+-rw-rw-rw-   0        0        0     6609 2023-05-30 14:57:57.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_procenv.py
+-rw-rw-rw-   0        0        0      398 2023-05-07 15:30:09.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_recorder.ascii
+-rw-rw-rw-   0        0        0      305 2023-06-02 07:07:24.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_recorder.menu_info
+-rw-rw-rw-   0        0        0     7354 2023-05-19 23:12:25.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_recorder.py
+-rw-rw-rw-   0        0        0     2762 2023-05-22 16:54:40.000000 GhettoRecorder-3.0/ghettorecorder/ghetto_utils.py
+-rw-rw-rw-   0        0        0     5839 2023-05-31 12:20:18.000000 GhettoRecorder-3.0/ghettorecorder/index.html
+-rw-rw-rw-   0        0        0      601 2023-05-08 04:06:45.000000 GhettoRecorder-3.0/ghettorecorder/schema.sql
+-rw-rw-rw-   0        0        0      887 2023-06-02 12:24:01.000000 GhettoRecorder-3.0/ghettorecorder/settings.ini
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:11.912180 GhettoRecorder-3.0/ghettorecorder/static/
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:11.989233 GhettoRecorder-3.0/ghettorecorder/static/css/
+-rw-rw-rw-   0        0        0     3767 2023-05-27 17:07:19.000000 GhettoRecorder-3.0/ghettorecorder/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:11.995086 GhettoRecorder-3.0/ghettorecorder/static/images/
+-rw-rw-rw-   0        0        0     8911 2023-06-02 06:20:19.000000 GhettoRecorder-3.0/ghettorecorder/static/images/ghetto_url.svg
+-rw-rw-rw-   0        0        0   102936 2023-05-13 13:12:09.000000 GhettoRecorder-3.0/ghettorecorder/static/images/gr_sky.svg
+-rw-rw-rw-   0        0        0     2485 2023-05-17 01:24:22.000000 GhettoRecorder-3.0/ghettorecorder/static/images/gr_sky_basket.svg
+drwxrwxrwx   0        0        0        0 2023-06-02 16:28:11.998987 GhettoRecorder-3.0/ghettorecorder/static/js/
+-rw-rw-rw-   0        0        0     3151 2023-05-27 16:36:57.000000 GhettoRecorder-3.0/ghettorecorder/static/js/animate.js
+-rw-rw-rw-   0        0        0    12737 2023-05-28 19:30:29.000000 GhettoRecorder-3.0/ghettorecorder/static/js/index.js
+-rw-rw-rw-   0        0        0     1021 2023-05-26 08:22:55.000000 GhettoRecorder-3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      457 2023-06-02 16:28:12.002888 GhettoRecorder-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-05-26 07:57:23.000000 GhettoRecorder-3.0/setup.py
```

### Comparing `GhettoRecorder-2.4.7/GhettoRecorder.egg-info/PKG-INFO` & `GhettoRecorder-3.0/GhettoRecorder.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: GhettoRecorder
-Version: 2.4.7
-Summary: command line internet radio grabber with listen capabilities
+Version: 3.0
+Summary: multiprocessor capable internet radio grabber
+Home-page: 
 Author: René Horn
-Author-email: rene_horn@gmx.net
-License: MIT License
-        ===========
-        
-        Copyright (c) [2022] [René Horn]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+Author-email: René Horn <rene_horn@gmx.net>
+License: MIT
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://GhettoRecorder.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/GhettoRecorder
-Keywords: aac recovery,aac repair
+Keywords: internet radio grabber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 License-File: LICENSE.rst
 
 Documentation - GhettoRecorder
 ==============================
-command line internet radio grabber with listen capabilities
+![alt logo of ghettorecorder](https://github.com/44xtc44/ghettorecorder/raw/dev/docs/source/_static/ghetto_url.svg)
+Grab hundreds of radio stations `simultaneously`.
 
-Info
-----
-| Can read and write removable, network and local storage.
-| Professional AAC Audio File Recovery during operation.
-| Type ``$ ghettorecorder`` to display the menu.
-| Package folder can be copied elsewhere, run ``cmd.py`` from there.
-|
-| Multiple menu options are available:
-|   * Custom save path (written to config)
-|   * Blacklist, grab only once (written to config)
-|   * Store config file elsewhere and store grabbed content in 'Custom save path' (elsewhere)
-|   * Offline AACP repair, AAC repair files https://aacrepair.readthedocs.io/
+How to run installed package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+GhettoRecorder
+class module (example in ghetto_procenv).::
+
+    from ghettorecorder import GhettoRecorder
+
+    ghetto_01 = GhettoRecorder(radio, url)
+    ghetto_01.com_in = mp.Queue(maxsize=1)  # eval exec communication for multiprocessing
+    ghetto_01.audio_out = mp.Queue(maxsize=1)  # can also be normal queue.Queue()
+
+Commandline
+option (calls cmd.py).::
+
+    ghetto_cmd or
+    python3 -m ghettorecorder.cmd
+
+Client Server
+option (calls __main__.py).::
+
+    ghetto_url or
+    python3 -m ghettorecorder
+
+Overview
+~~~~~~~~~
+* Queue communication. Multiprocessor ready.
+* GhettoRecorder class has connector attributes for external modules.
+* External modul *Blacklisting recorded titles* is already included.
+* Optional Browser Frontend on Python multithreading HTTP server.
 
 Links
-^^^^^
+~~~~~
 * Snap: https://snapcraft.io/ghettorecorder
 * GitHub: https://github.com/44xtc44/GhettoRecorder
 * Issues to fix: https://github.com/44xtc44/GhettoRecorder/issues
 * ReadTheDocs: https://ghettorecorder.readthedocs.io/ (see module index)
 
 Configuration File
 ------------------
 'Settings.ini' is the config file for GhettoRecorder.
-INI files consist of sections to divide different settings.
+INI files consist of sections to divide different settings.::
 
+    [STATIONS]
+    anime_jp = http://streamingv2.shoutcast.com/japanimradio-tokyo
 
-| [STATIONS] is used for radio connection information
-| anime_jp = ``http://streamingv2.shoutcast.com/japanimradio-tokyo``
+    [GLOBAL]
+    blacklist_enable = True
+    save_to_dir = f:\54321
 
-| [GLOBAL] stores blacklist status and the parent save directory location
-| blacklist_enable = ``True``
-| save_to_dir = ``f:\31``
+
+| [STATIONS]
+| custom radio name and radio connection information (can be pls or m3u playlist)
+
+| [GLOBAL]
+| stores blacklist status and the *custom* parent directory location
 
 Usage
 -----
 Main Menu
 ^^^^^^^^^
 ::
 
@@ -211,7 +212,41 @@
 
 remove::
 
    >$ pip3 show ghettorecorder
    >$ pip3 uninstall ghettorecorder
 
 Location: ... /python310/site-packages
+
+GhettoRecorder module
+~~~~~~~~~~~~~~~~~~~~~~
+Communication with the GhettoRecorder instance
+
+       ========= ================= ======================================================
+       port      action            description
+       ========= ================= ======================================================
+       com_in    commands input    tuple (radio, [str 'eval' or 'exec'], str 'command')
+       com_out   status, err msg   (radio, [str 'eval' or 'exec'], response)
+       audio_out copy of html resp server can loop through to a browser
+       ========= ================= ======================================================
+
+Feature attributes to switch on/off
+
+       ========================== ==================================================================================
+       attribute                  description
+       ========================== ==================================================================================
+       runs_meta                  call metadata periodically, create path for rec out; False: recorder is the file
+       runs_record                disable writing to recorder file at all
+       recorder_file_write        allow dumping current recorder file
+       runs_listen                disable write to audio output queue; 3rd party can grab it. (listen blacklist)
+       ========================== ==================================================================================
+
+Snapcraft package
+~~~~~~~~~~~~~~~~~~
+The installer creates an icon with the name "GhettoRecorder".
+You can use two command line options.::
+
+    ghettorecorder.url
+    ghettorecorder.cmd
+
+First is Client, Server connection.
+Second is command line menu.
```

### Comparing `GhettoRecorder-2.4.7/LICENSE.rst` & `GhettoRecorder-3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `GhettoRecorder-2.4.7/PKG-INFO` & `GhettoRecorder-3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: GhettoRecorder
-Version: 2.4.7
-Summary: command line internet radio grabber with listen capabilities
+Version: 3.0
+Summary: multiprocessor capable internet radio grabber
+Home-page: 
 Author: René Horn
-Author-email: rene_horn@gmx.net
-License: MIT License
-        ===========
-        
-        Copyright (c) [2022] [René Horn]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+Author-email: René Horn <rene_horn@gmx.net>
+License: MIT
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://GhettoRecorder.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/GhettoRecorder
-Keywords: aac recovery,aac repair
+Keywords: internet radio grabber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 License-File: LICENSE.rst
 
 Documentation - GhettoRecorder
 ==============================
-command line internet radio grabber with listen capabilities
+![alt logo of ghettorecorder](https://github.com/44xtc44/ghettorecorder/raw/dev/docs/source/_static/ghetto_url.svg)
+Grab hundreds of radio stations `simultaneously`.
 
-Info
-----
-| Can read and write removable, network and local storage.
-| Professional AAC Audio File Recovery during operation.
-| Type ``$ ghettorecorder`` to display the menu.
-| Package folder can be copied elsewhere, run ``cmd.py`` from there.
-|
-| Multiple menu options are available:
-|   * Custom save path (written to config)
-|   * Blacklist, grab only once (written to config)
-|   * Store config file elsewhere and store grabbed content in 'Custom save path' (elsewhere)
-|   * Offline AACP repair, AAC repair files https://aacrepair.readthedocs.io/
+How to run installed package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+GhettoRecorder
+class module (example in ghetto_procenv).::
+
+    from ghettorecorder import GhettoRecorder
+
+    ghetto_01 = GhettoRecorder(radio, url)
+    ghetto_01.com_in = mp.Queue(maxsize=1)  # eval exec communication for multiprocessing
+    ghetto_01.audio_out = mp.Queue(maxsize=1)  # can also be normal queue.Queue()
+
+Commandline
+option (calls cmd.py).::
+
+    ghetto_cmd or
+    python3 -m ghettorecorder.cmd
+
+Client Server
+option (calls __main__.py).::
+
+    ghetto_url or
+    python3 -m ghettorecorder
+
+Overview
+~~~~~~~~~
+* Queue communication. Multiprocessor ready.
+* GhettoRecorder class has connector attributes for external modules.
+* External modul *Blacklisting recorded titles* is already included.
+* Optional Browser Frontend on Python multithreading HTTP server.
 
 Links
-^^^^^
+~~~~~
 * Snap: https://snapcraft.io/ghettorecorder
 * GitHub: https://github.com/44xtc44/GhettoRecorder
 * Issues to fix: https://github.com/44xtc44/GhettoRecorder/issues
 * ReadTheDocs: https://ghettorecorder.readthedocs.io/ (see module index)
 
 Configuration File
 ------------------
 'Settings.ini' is the config file for GhettoRecorder.
-INI files consist of sections to divide different settings.
+INI files consist of sections to divide different settings.::
 
+    [STATIONS]
+    anime_jp = http://streamingv2.shoutcast.com/japanimradio-tokyo
 
-| [STATIONS] is used for radio connection information
-| anime_jp = ``http://streamingv2.shoutcast.com/japanimradio-tokyo``
+    [GLOBAL]
+    blacklist_enable = True
+    save_to_dir = f:\54321
 
-| [GLOBAL] stores blacklist status and the parent save directory location
-| blacklist_enable = ``True``
-| save_to_dir = ``f:\31``
+
+| [STATIONS]
+| custom radio name and radio connection information (can be pls or m3u playlist)
+
+| [GLOBAL]
+| stores blacklist status and the *custom* parent directory location
 
 Usage
 -----
 Main Menu
 ^^^^^^^^^
 ::
 
@@ -211,7 +212,41 @@
 
 remove::
 
    >$ pip3 show ghettorecorder
    >$ pip3 uninstall ghettorecorder
 
 Location: ... /python310/site-packages
+
+GhettoRecorder module
+~~~~~~~~~~~~~~~~~~~~~~
+Communication with the GhettoRecorder instance
+
+       ========= ================= ======================================================
+       port      action            description
+       ========= ================= ======================================================
+       com_in    commands input    tuple (radio, [str 'eval' or 'exec'], str 'command')
+       com_out   status, err msg   (radio, [str 'eval' or 'exec'], response)
+       audio_out copy of html resp server can loop through to a browser
+       ========= ================= ======================================================
+
+Feature attributes to switch on/off
+
+       ========================== ==================================================================================
+       attribute                  description
+       ========================== ==================================================================================
+       runs_meta                  call metadata periodically, create path for rec out; False: recorder is the file
+       runs_record                disable writing to recorder file at all
+       recorder_file_write        allow dumping current recorder file
+       runs_listen                disable write to audio output queue; 3rd party can grab it. (listen blacklist)
+       ========================== ==================================================================================
+
+Snapcraft package
+~~~~~~~~~~~~~~~~~~
+The installer creates an icon with the name "GhettoRecorder".
+You can use two command line options.::
+
+    ghettorecorder.url
+    ghettorecorder.cmd
+
+First is Client, Server connection.
+Second is command line menu.
```

### Comparing `GhettoRecorder-2.4.7/README.rst` & `GhettoRecorder-3.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,67 @@
 Documentation - GhettoRecorder
 ==============================
-command line internet radio grabber with listen capabilities
+![alt logo of ghettorecorder](https://github.com/44xtc44/ghettorecorder/raw/dev/docs/source/_static/ghetto_url.svg)
+Grab hundreds of radio stations `simultaneously`.
 
-Info
-----
-| Can read and write removable, network and local storage.
-| Professional AAC Audio File Recovery during operation.
-| Type ``$ ghettorecorder`` to display the menu.
-| Package folder can be copied elsewhere, run ``cmd.py`` from there.
-|
-| Multiple menu options are available:
-|   * Custom save path (written to config)
-|   * Blacklist, grab only once (written to config)
-|   * Store config file elsewhere and store grabbed content in 'Custom save path' (elsewhere)
-|   * Offline AACP repair, AAC repair files https://aacrepair.readthedocs.io/
+How to run installed package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+GhettoRecorder
+class module (example in ghetto_procenv).::
+
+    from ghettorecorder import GhettoRecorder
+
+    ghetto_01 = GhettoRecorder(radio, url)
+    ghetto_01.com_in = mp.Queue(maxsize=1)  # eval exec communication for multiprocessing
+    ghetto_01.audio_out = mp.Queue(maxsize=1)  # can also be normal queue.Queue()
+
+Commandline
+option (calls cmd.py).::
+
+    ghetto_cmd or
+    python3 -m ghettorecorder.cmd
+
+Client Server
+option (calls __main__.py).::
+
+    ghetto_url or
+    python3 -m ghettorecorder
+
+Overview
+~~~~~~~~~
+* Queue communication. Multiprocessor ready.
+* GhettoRecorder class has connector attributes for external modules.
+* External modul *Blacklisting recorded titles* is already included.
+* Optional Browser Frontend on Python multithreading HTTP server.
 
 Links
-^^^^^
+~~~~~
 * Snap: https://snapcraft.io/ghettorecorder
 * GitHub: https://github.com/44xtc44/GhettoRecorder
 * Issues to fix: https://github.com/44xtc44/GhettoRecorder/issues
 * ReadTheDocs: https://ghettorecorder.readthedocs.io/ (see module index)
 
 Configuration File
 ------------------
 'Settings.ini' is the config file for GhettoRecorder.
-INI files consist of sections to divide different settings.
+INI files consist of sections to divide different settings.::
 
+    [STATIONS]
+    anime_jp = http://streamingv2.shoutcast.com/japanimradio-tokyo
 
-| [STATIONS] is used for radio connection information
-| anime_jp = ``http://streamingv2.shoutcast.com/japanimradio-tokyo``
+    [GLOBAL]
+    blacklist_enable = True
+    save_to_dir = f:\54321
 
-| [GLOBAL] stores blacklist status and the parent save directory location
-| blacklist_enable = ``True``
-| save_to_dir = ``f:\31``
+
+| [STATIONS]
+| custom radio name and radio connection information (can be pls or m3u playlist)
+
+| [GLOBAL]
+| stores blacklist status and the *custom* parent directory location
 
 Usage
 -----
 Main Menu
 ^^^^^^^^^
 ::
 
@@ -166,7 +190,41 @@
 
 remove::
 
    >$ pip3 show ghettorecorder
    >$ pip3 uninstall ghettorecorder
 
 Location: ... /python310/site-packages
+
+GhettoRecorder module
+~~~~~~~~~~~~~~~~~~~~~~
+Communication with the GhettoRecorder instance
+
+       ========= ================= ======================================================
+       port      action            description
+       ========= ================= ======================================================
+       com_in    commands input    tuple (radio, [str 'eval' or 'exec'], str 'command')
+       com_out   status, err msg   (radio, [str 'eval' or 'exec'], response)
+       audio_out copy of html resp server can loop through to a browser
+       ========= ================= ======================================================
+
+Feature attributes to switch on/off
+
+       ========================== ==================================================================================
+       attribute                  description
+       ========================== ==================================================================================
+       runs_meta                  call metadata periodically, create path for rec out; False: recorder is the file
+       runs_record                disable writing to recorder file at all
+       recorder_file_write        allow dumping current recorder file
+       runs_listen                disable write to audio output queue; 3rd party can grab it. (listen blacklist)
+       ========================== ==================================================================================
+
+Snapcraft package
+~~~~~~~~~~~~~~~~~~
+The installer creates an icon with the name "GhettoRecorder".
+You can use two command line options.::
+
+    ghettorecorder.url
+    ghettorecorder.cmd
+
+First is Client, Server connection.
+Second is command line menu.
```

### Comparing `GhettoRecorder-2.4.7/ghettorecorder/ghetto_container.py` & `GhettoRecorder-3.0/ghettorecorder/ghetto_container.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,57 +8,76 @@
    container_setup  - decide to set up a container env
    container_config_dir - get path for new folder creation
    create_config_env    - overwrite base dir for ghetto, copy config file to that dir
 """
 import os
 import shutil
 import getpass
-from ghettorecorder.api import ghettoApi
+from ghettorecorder.ghetto_api import ghettoApi
 
 
 def container_setup():
     """ return False if no package specific env variable is set
 
      Info
         variable must be set in package config file Dockerfile or snapcraft.yaml
         change and create the default (parent) record path
         copy settings.ini to that path
+
+    :returns: True if container
     """
-    is_container = False
-    is_snap_container = 'GHETTORECORDER_SNAP' in os.environ   # var must be set in package config, some value
-    is_docker_container = 'DOCKER' in os.environ              # var must be set in package config, some value
-
-    if is_snap_container:
-        print('Snap Container')
-        is_container = True
-        container_config_dir('SNAP')
-        return is_container
-
-    if is_docker_container:
-        print('Docker Container')
-        is_container = True
-        container_config_dir('DOCKER')
-        return is_container
-    return is_container
+    folder = False
+    is_snap = 'SNAP' in os.environ
+    is_docker = 'DOCKER' in os.environ
+
+    if is_snap:
+        get_env_snap()
+        folder = container_config_dir('SNAP')
+
+    if is_docker:
+        get_env_docker()
+        folder = container_config_dir('DOCKER')
+
+    return folder
+
+
+def get_env_snap():
+    print('GhettoRecorder App in Snap Container, check environment:\n')
+    print('SNAP_USER_COMMON: ' + os.environ["SNAP_USER_COMMON"])
+    print('SNAP_LIBRARY_PATH: ' + os.environ["SNAP_LIBRARY_PATH"])
+    print('SNAP_COMMON: ' + os.environ["SNAP_COMMON"])
+    print('SNAP_USER_DATA: ' + os.environ["SNAP_USER_DATA"])
+    print('SNAP_DATA: ' + os.environ["SNAP_DATA"])
+    print('SNAP_REVISION: ' + os.environ["SNAP_REVISION"])
+    print('SNAP_NAME: ' + os.environ["SNAP_NAME"])
+    print('SNAP_ARCH: ' + os.environ["SNAP_ARCH"])
+    print('SNAP_VERSION: ' + os.environ["SNAP_VERSION"])
+    print('SNAP: ' + os.environ["SNAP"])
+
+
+def get_env_docker():
+    print('\n\tGhettoRecorder App in Docker Container\n')
 
 
 def container_config_dir(container):
     """ assemble the path to new config dir (settings.ini and blacklist)
+    | 'get user' - create dir under home folder for snap
+    | save path for caller to read later
 
-    variable
-       get user - create dir under home folder for snap
-     """
+    :params: container: either snap or docker
+    """
     if container == 'SNAP':                                   # SNAP
         username = getpass.getuser()
         print('Hello, ' + username)
         ghetto_folder = os.path.join('/home', username, 'GhettoRecorder')
     else:
         ghetto_folder = os.path.join('/tmp', 'GhettoRecorder')  # DOCKER
 
     create_config_env(ghetto_folder)
+    return ghetto_folder
 
 
 def create_config_env(ghetto_folder):
     """ copy config files outside the default package folder /site-settings/ghettorecorder
 
     statements
        create new parent record folder
```

### Comparing `GhettoRecorder-2.4.7/ghettorecorder/ghetto_ini.py` & `GhettoRecorder-3.0/ghettorecorder/ghetto_ini.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,180 +1,216 @@
 """ GhettoRecorder config
 settings.ini file
 """
 import os
 import configparser
 from pathlib import Path as Pathlib_path
-from ghettorecorder.api import ghettoApi
+from ghettorecorder.ghetto_api import ghettoApi
 
 
-class GIni:
-    """ ONLY command line; 'settings.ini' config
-    choice of radios can be made via list index number or name of the radio
-
-    Dictionaries
-       radio_names_list = []  . list to search radio name via character
-       config_stations = {}          . radio, url pairs from [STATIONS] section
-       config_global = {}            . extra infos from [GLOBAL] section, SAVE_TO_DIR = f:\2, BLACKLIST_ENABLE = True
-
-    Methods
-       show_items_ini_file() . show the content of the ini file to choose from, fill radio_names_list,radio_names_dict
-       config_path_test()    . look if we can read the config file
-       blacklist_path_set()  . config_path_test success, set blacklist path to settings.ini path
-       global_config_show(print_config=False) . extract GLOBAL section from settings.ini
-       global_record_path_write(custom_path) . SAVE_TO_DIR = f:/2
-       global_blacklist_enable_write(option) . BLACKLIST_ENABLE = True
-       config_path_set(config_files_dir)     . on config path change (menu) set blacklist path to settings.ini path
+class Gini:
+    """Configparser stores most found setting in itself.
+    | config.read_file() returns nothing
+    """
+    def __init__(self):
+        self.config_name = "settings.ini"
+        self.radio_names_list = []  # search radio name via character, from ghetto_menu
+        self.dir_name = os.path.dirname(os.path.abspath(__file__))  # print ghettorecorder logo to screen
+        self.config_stations_dct = {}  # config section [STATIONS] radio, url pairs
+        self.config_global_dct = {}    # config section [GLOBAL]  info SAVE_TO_DIR = f:\2, BLACKLIST_ENABLE = True
+
+
+gini = Gini()
+
+
+def global_config_get():
+    """Fills the 'config_global_dct', if [GLOBAL] section has members.
+    """
+    config = config_file_read()
+    try:
+        gini.config_global_dct = dict(config.items('GLOBAL'))
+    except Exception as error:
+        print(f'Config found, minor error [GLOBAL]: {error} - proceed')
+    return gini.config_global_dct
+
+
+def global_config_show():
+    """ extract [GLOBAL] section from settings.ini, if available
+    GLOBAL can be - not there, empty, or with values (test case)
+
+    Method
+       config_parse_get() - exit if no path
+
+    Raise
+       show that there is no config, but can proceed without (config_parse_get(), ok)
+    """
+    if not len(gini.config_global_dct):
+        print("--> section [GLOBAL] is empty. No blacklist, or record path set.")
+        return False
+    else:
+        print(f'.. settings.ini [GLOBAL] section: {gini.config_global_dct}')
+        return True
+
+
+def stations_config_get():
+    """Fills the 'config_stations_dct', if [STATIONS] section has members.
+    """
+    config = config_file_read()
+    try:
+        gini.config_stations_dct = dict(config.items('STATIONS'))
+    except AttributeError:
+        print("--> gini.setting_config_show(), can not find configuration section [STATIONS] - proceed")
+        return False
+
+    for name in dict(config.items('STATIONS')):
+        gini.radio_names_list.append(name)
+
+    return True
+
+
+def stations_config_show():
+    """ show the content of the ini file to choose from
+    fill radio_names_list and radio_names_dict to later validate the choice
      """
+    with open(os.path.join(gini.dir_name, "ghetto_recorder.ascii"), "r") as reader:
+        print(reader.read())
 
-    radio_names_list = []  # search radio name via character
-    logo_path = os.path.dirname(os.path.abspath(__file__))  # print ghettorecorder logo to screen
-    config_stations = {}  # config section [STATIONS] radio, url pairs
-    config_global = {}    # config section [STATIONS] extra infos SAVE_TO_DIR = f:\2, BLACKLIST_ENABLE = True
-
-    @staticmethod
-    def show_items_ini_file():
-        """ show the content of the ini file to choose from
-        fill radio_names_list and radio_names_dict to later validate the choice
-         """
-        config = GIni.config_path_test()
-        try:
-            GIni.config_stations = dict(config.items('STATIONS'))
-        except AttributeError:
-            print("--> GIni.show_items_ini_file(), can not find configuration section [STATIONS] - proceed")
-            return
-
-        with open(os.path.join(GIni.logo_path, "ghetto_recorder.ascii"), "r") as reader:
-            print(reader.read())
-
-        GIni.radio_names_list = []
-        for name in dict(config.items('STATIONS')):
-            GIni.radio_names_list.append(name)
-
-        for index, name in enumerate(GIni.radio_names_list):
-            print(f'\t{index} \t>> %-20s <<' % name)
-
-        print(' \n Radio stations in your list. --> CHANGED: 42 to 12345')
-        print(' Please use "Ctrl + C" to stop the app.\n')
-        print('\tCopy/Paste a Radio from >> settings.ini <<, \n\tor type the leading number and press Enter\n')
-        print("\t http://localhost:1242/" + " listen to local recorded stream (saves bandwidth)")
-        print("\t If blacklist is ON, file: blacklist.json in the same folder as settings.ini")
-
-        return
-
-    @staticmethod
-    def config_path_test():
-        config = configparser.ConfigParser()  # instantiate imported library to work with .ini files
+    for index, name in enumerate(gini.radio_names_list):
+        print(f'\t{index} \t>> %-20s <<' % name)
+
+    with open(os.path.join(gini.dir_name, "ghetto_recorder.menu_info"), "r") as reader:
+        print(reader.read())
+    # print(' \n Radio stations in your list. --> CHANGED: 42 to 12345')
+    # print(' Please use "Ctrl + C" to stop the app.\n')
+    # print('\tCopy/Paste a Radio from >> settings.ini <<, \n\tor type the leading number and press Enter\n')
+    # print("\tType: 'ghetto_url' in a terminal to start the User Interface at " + "http://localhost:1242/")
+    # print("\t If blacklist is ON, file: blacklist.json in the same folder as settings.ini")
+
+
+def config_file_read():
+    """Error if configparser fails.
+    Path can be local module path or remote.
+    """
+    config = configparser.ConfigParser()
+    try:
+        config_file_path = os.path.join(ghettoApi.path.config_dir, ghettoApi.path.config_name)
+        config.read_file(open(config_file_path))
+        return config
+    except OSError:
         try:
-            config_file_path = os.path.join(ghettoApi.config_dir, ghettoApi.config_name)
+            config_file_path = os.path.join(gini.dir_name, gini.config_name)
             config.read_file(open(config_file_path))
+            return config
         except OSError:
+            print(f'OSError in config_parse_get not avail.')
+            return False
+
+
+def global_config_to_api():
+    """ return True if [GLOBAL] section exists and has settings
+    push setting of [GLOBAL] section from settings.ini in variables,
+
+    Raise
+       show that there is no config, but can proceed without (config_parse_get(), ok)
+    """
+    config = config_file_read()
+    if config:
+        try:
+            gini.config_global_dct = dict(config.items('GLOBAL'))
+        except Exception as error:
+            print(f'Config found, minor error: {error} - proceed')
+            return False
+
+        if not len(gini.config_global_dct):
+            print("--> section [GLOBAL] is empty. No blacklist, or record path set.")
             return False
         else:
-            # GIni.blacklist_path_set()
-            return config
+            for key, val in gini.config_global_dct.items():
+                if key == "SAVE_TO_DIR".lower():
+                    # push path from [GLOBAL]
+                    ghettoApi.path.save_to_dir = val
+                if key == "BLACKLIST_ENABLE".lower():
+                    ghettoApi.blacklist.blacklist_enable = val
+            return True
+
+
+def global_record_path_write(custom_path):
+    """ ini config write SAVE_TO_DIR 'remote' from modules path.
+    We have already tried to read the global section.
+    ["GLOBAL"]
+    SAVE_TO_DIR = f:/2
+
+    :params: custom_path: can be a remote path of an .ini in Alaska, not the dir where module is located
+    """
+    # the magic happens here
+    config_file_path = os.path.join(ghettoApi.path.config_dir, ghettoApi.path.config_name)
+
+    config = configparser.ConfigParser()
+    config.read_file(open(config_file_path))
+    config.sections()
+    if "GLOBAL" not in config:
+        config.add_section('GLOBAL')
+    config.set('GLOBAL', 'SAVE_TO_DIR', str(Pathlib_path(custom_path)))  # help to write path for OS
+    with open(config_file_path, 'w') as configfile:
+        config.write(configfile)
+
+
+def global_blacklist_enable_write(option):
+    """ ini config write
+    ["GLOBAL"]
+    BLACKLIST_ENABLE = True
+    """
+    # the magic happens here
+    config_file_path = os.path.join(ghettoApi.path.config_dir, ghettoApi.path.config_name)
+
+    config = configparser.ConfigParser()
+    config.read_file(open(config_file_path))
+    config.sections()
+    if "GLOBAL" not in config:
+        config.add_section('GLOBAL')
+    config.set('GLOBAL', 'BLACKLIST_ENABLE', option)
+    with open(config_file_path, 'w') as configfile:
+        config.write(configfile)
+
+
+def config_path_api_set(config_files_dir):
+    """ Menu 'Set path to config, settings.ini'
+    set path blacklist,
+    set path to a 'remote' config file (local fs, writable network location)
+
+    Hint
+       can have config somewhere and write to save_to_dir path elsewhere, if this option is used
+    """
+    ghettoApi.blacklist.blacklist_dir = ghettoApi.path.config_dir = str(Pathlib_path(config_files_dir))
+
+
+def main():
+    """Show what we are doing here and
+    function test module.
+    """
+
+    global_config_get()  # read [GLOBAL] section to dict
+    global_config_show()
+    stations_config_get()  # read [STATIONS] section to dict
+    stations_config_show()
+    # write new record path to either local ini or remote ini (custom_path)
+    import ghetto_utils
+    custom_path = os.path.join(gini.dir_name, "home_of_the_grinch")
+    ghetto_utils.make_dirs(custom_path)
+    import shutil
+    src_ini, dst_ini = os.path.join(gini.dir_name, gini.config_name), os.path.join(custom_path, gini.config_name)
+    shutil.copy(src_ini, dst_ini)
+    ghettoApi.path.config_dir, ghettoApi.path.config_name = custom_path, gini.config_name
+    global_record_path_write(custom_path)  # save_to_dir custom path
+    global_blacklist_enable_write('False')  # write False to blacklist
+    global_config_get()  # read [GLOBAL] section to dict
+    global_config_show()
+    ghetto_utils.delete_dirs(custom_path)
+
+    global_config_to_api()  # blacklist_enable should be True
+    print('to_api: save_to_dir, blacklist_enable', ghettoApi.path.save_to_dir, ghettoApi.blacklist.blacklist_enable)
+    config_path_api_set(custom_path)
+    print('to_api: config_dir, blacklist_dir', ghettoApi.path.config_dir, ghettoApi.blacklist.blacklist_dir)
 
-    @staticmethod
-    def blacklist_path_set():
-        """ set path to blacklist for blacklist writer
-
-        Info:
-           store info of config folder path, prevent writing blacklist in SAVE_TO_DIR folder
-        """
-        ghettoApi.blacklist_dir = ghettoApi.config_dir
-
-    @staticmethod
-    def global_config_show():
-        """ extract [GLOBAL] section from settings.ini, if available
-        GLOBAL can be - not there, empty, or with values (test case)
-
-        Method
-           GIni.config_path_test() - exit if no path
-
-        Raise
-           show that there is no config, but can proceed without (GIni.config_path_test(), ok)
-        """
-        config = GIni.config_path_test()
-        if config:
-            try:
-                GIni.config_global = dict(config.items('GLOBAL'))
-            except Exception as error:
-                print(f'Config found, minor error: {error} - proceed')
-                return True
-
-            if not len(GIni.config_global):
-                print("--> section [GLOBAL] is empty. No blacklist, or record path set.")
-                return True
-            else:
-                print(f'.. settings.ini [GLOBAL] section: {GIni.config_global}')
-                return True
-
-    @staticmethod
-    def global_config_push():
-        """ return True if [GLOBAL] section exists and has settings
-        push setting of [GLOBAL] section from settings.ini in variables,
-
-        Raise
-           show that there is no config, but can proceed without (GIni.config_path_test(), ok)
-        """
-        config = GIni.config_path_test()
-        if config:
-            try:
-                GIni.config_global = dict(config.items('GLOBAL'))
-            except Exception as error:
-                print(f'Config found, minor error: {error} - proceed')
-                return False
-
-            if not len(GIni.config_global):
-                print("--> section [GLOBAL] is empty. No blacklist, or record path set.")
-                return False
-            else:
-                for key, val in GIni.config_global.items():
-                    if key == "SAVE_TO_DIR".lower():
-                        # push path from [GLOBAL]
-                        ghettoApi.save_to_dir = val
-                    if key == "BLACKLIST_ENABLE".lower():
-                        ghettoApi.blacklist_enable = val
-                return True
-
-    @staticmethod
-    def global_record_path_write(custom_path):
-        """ ini config write
-        ["GLOBAL"]
-        SAVE_TO_DIR = f:/2
-        """
-        config = configparser.ConfigParser()
-        config_file_path = os.path.join(ghettoApi.config_dir, ghettoApi.config_name)
-        config.read_file(open(config_file_path))
-        config.sections()
-        if "GLOBAL" not in config:
-            config.add_section('GLOBAL')
-        config.set('GLOBAL', 'SAVE_TO_DIR', str(Pathlib_path(custom_path)))  # help to write path for OS
-        with open(config_file_path, 'w') as configfile:
-            config.write(configfile)
-
-    @staticmethod
-    def global_blacklist_enable_write(option):
-        """ ini config write
-        ["GLOBAL"]
-        BLACKLIST_ENABLE = True
-        """
-        config = configparser.ConfigParser()
-        config_file_path = os.path.join(ghettoApi.config_dir, ghettoApi.config_name)
-        config.read_file(open(config_file_path))
-        config.sections()
-        if "GLOBAL" not in config:
-            config.add_section('GLOBAL')
-        config.set('GLOBAL', 'BLACKLIST_ENABLE', option)
-        with open(config_file_path, 'w') as configfile:
-            config.write(configfile)
-
-    @staticmethod
-    def config_path_set(config_files_dir):
-        """ Menu 'Set path to config, settings.ini'
-        set path to a 'remote' config file (local fs, writable network location)
-
-        Hint
-           can have config somewhere and write to save_to_dir path elsewhere, if this option is used
-        """
-        ghettoApi.config_dir = str(Pathlib_path(config_files_dir))
-        ghettoApi.blacklist_dir = str(Pathlib_path(config_files_dir))
+
+if __name__ == "__main__":
+    main()
```

### Comparing `GhettoRecorder-2.4.7/ghettorecorder/ghetto_menu.py` & `GhettoRecorder-3.0/ghettorecorder/ghetto_menu.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,33 +12,31 @@
    menu_path()      - store custom path in config, default is recorder parent dir in config file folder
    menu_blacklist() - enable blacklist feature, store in config and create json dict file if not exists
    record()         - init all dicts in ghetto_ini.GIni, show the list of radios to choose from
    record_read_radios() - input prompt, get radio name or the choice (index) number of a radio list, create folder
    record_validate_input(radio_name) - True if choice in list, True if index of list is valid, False if not valid
    record_validate_radio_name(radio_name) - change the index number back to radio name, if index was the choice
    record_create_radio_url_dict(radio_name) - need radio name as thread and folder name, url to connect to network
-   record_create_folder_radio_name(radio_name) - create parent folder and radio child folder
    terminal_record_parent_dir_get()  - return GIni.radio_base_dir, parent folder
    terminal_record_custom_path_get() - called by ghetto_recorder module, config is called at radio choice in main menu
    terminal_record_blacklist_enabled_get() - called by ghetto_recorder module, enable api variable
    terminal_record_all_radios_get() - called by ghetto_recorder module to write blacklist beside settings.ini
    path_change() - call menu_path(), Change record parent path
    parent_record_path_change() - store path in [GLOBAL], test if path is writeable
    path_validate_input(custom_path) - return True if path is valid
    blacklist()                      - Enable/disable blacklists
    blacklist_is_enabled()           - Write a new blacklist option to settings.ini file
    blacklist_on()                   - write enabled to config file
    blacklist_off()                  - write disabled to config file
    remove_special_chars(str_name)   - clean radio name to create a folder
 """
 import os
-from pathlib import Path as Pathlib_path
 from aacrepair import AacRepair
-from ghettorecorder.api import ghettoApi
-from ghettorecorder.ghetto_ini import GIni
+from ghettorecorder.ghetto_api import ghettoApi
+import ghettorecorder.ghetto_ini as ghetto_ini
 
 
 def menu_main():
     print('\tmenu \'Main\'')
     menu_options = {
         1: 'Record (local listen option)',
         2: 'Change parent record path',
@@ -91,24 +89,26 @@
 
         try:
             option = int(input('Enter your choice: '))
         except ValueError:
             print('Invalid option. Please enter a number between 1 and 2.')
         if option == 1:
             parent_record_path_change()
+            menu_main()
             break
         elif option == 2:
             menu_main()
             break
         else:
             print('Invalid option. Please enter a number between 1 and 2.')
 
 
 def menu_blacklist():
-    GIni.global_config_show()
+    ghetto_ini.global_config_get()
+    ghetto_ini.global_config_show()
     menu_options = {
         1: "blacklist on (don't write title if already downloaded)",
         2: 'blacklist off',
         3: 'Back to Main Menu',
     }
 
     while 1:
@@ -130,15 +130,15 @@
             menu_main()
             break
         else:
             print('Invalid option. Please enter a number between 1 and 3.')
 
 
 def menu_find_config():
-    GIni.global_config_show()
+    ghetto_ini.global_config_show()
     menu_options = {
         1: 'Path to "setting.ini" and "blacklist.json"',
         2: 'Back to Main Menu',
     }
 
     while 1:
         option = ""
@@ -161,30 +161,26 @@
 
 def record():
     """ show all options if True, else fail brutal to retrieve the error message
     init all dicts in ghetto_ini.GIni, show the list of radios to choose from
 
     Functions
        GIni.config_path_test()    - test if configparser can read config file
-       GIni.global_config_show()  - [GLOBAL] settings.ini vars
-       GIni.global_config_push()  - read in [GLOBAL] settings.ini vars
-       GIni.show_items_ini_file() - show the main menu headline and description
+       ghetto_ini.global_config_show()  - [GLOBAL] settings.ini vars
+       ghetto_ini.global_config_to_api  - read in [GLOBAL] settings.ini vars
+       ghetto_ini.stations_config_show() - show the main menu headline and description
     """
     print('\toption \'record\'')
-    if record_path_get():
-        GIni.show_items_ini_file()
-        print(f'\n.. config file in {ghettoApi.config_dir}')
-        if GIni.global_config_show():
-            GIni.global_config_push()
-
+    if ghetto_ini.stations_config_get():
+        ghetto_ini.stations_config_show()
 
-def record_path_get():
-    if not GIni.config_path_test():
-        return False
-    return True
+        print(f'\n..  config file settings.ini in {ghettoApi.path.config_dir}')
+        ghetto_ini.global_config_get()
+        ghetto_ini.global_config_to_api()
+        ghetto_ini.global_config_show()  # if something is configured
 
 
 def record_read_radios():
     """ return validated 'radio_url_dict' to ghetto_recorder module
 
     input on main menu
        the list index number of a radio (prefix, [6 >> time_machine <<])
@@ -193,32 +189,29 @@
     target
        write radio_url_dict[radioName] = URL
        recognize list index numbers to transform number into radio name
 
     Methods
        record_validate_radio_name() - validate radio name or transform choice (index) number of a radio to name,
        record_create_radio_url_dict(valid_name) - return (name, url) tuple
-       record_create_folder_radio_name(radio_dir_name) - create folder for validated radio
 
     return
        'radio_url_dict'
     """
     radio_list = []  # fill a list, just to see if we get valid input
     radio_url_dict = {}  # return value of the function
     while True:
         line_input = input('Enter to record -->:')
         radio_name = line_input.strip()
 
         if line_input == str(12345):  # all
-            for name in GIni.radio_names_list:
+            for name in ghetto_ini.gini.radio_names_list:
                 name, url = record_create_radio_url_dict(name)
                 radio_url_dict[name] = url
                 print(f"12345...{name}")
-                radio_dir_name = remove_special_chars(name)
-                record_create_folder_radio_name(radio_dir_name)
             break
 
         elif (not len(radio_list)) and (not len(radio_name)):
             print("nothing to do, next try ...")
             menu_main()
         elif (len(radio_list) > 0) and (not len(radio_name)):
             # list is filled with valid inputs, record starts with empty input
@@ -229,90 +222,92 @@
             is_valid = record_validate_input(radio_name)
             if is_valid:
                 # turn list index in element name, choice '0' to Blues_UK,
                 valid_name = record_validate_radio_name(radio_name)
                 name, url = record_create_radio_url_dict(valid_name)
                 radio_url_dict[name] = url
                 radio_dir_name = remove_special_chars(valid_name)
-                record_create_folder_radio_name(radio_dir_name)
                 radio_list.append(radio_dir_name)
                 print(' Hit Enter <---| to RECORD, or paste next radio, write 12345 for all radios ')
     return radio_url_dict
 
 
+def radio_url_dict_create():
+    radio_url_dict = {}
+    for name in ghetto_ini.gini.radio_names_list:
+        name, url = record_create_radio_url_dict(name)
+        radio_url_dict[name] = url
+    return radio_url_dict
+
+
+def settings_ini_to_dict():
+    """"""
+    radio_url_dict = {}
+    for name in ghetto_ini.gini.radio_names_list:
+        name, url = record_create_radio_url_dict(name)
+        radio_url_dict[name] = url
+    return radio_url_dict
+
+
+def settings_ini_global():
+    """"""
+    rv_empty = {}
+    config_global_dct = ghetto_ini.global_config_get()
+    return config_global_dct if config_global_dct else rv_empty
+
+
 def record_validate_input(radio_name) -> bool:
     """ return True if choice is name in list, return True for choice if index of list is a valid integer
     return False if not valid
      """
-    if radio_name in GIni.radio_names_list:
+    if radio_name in ghetto_ini.gini.radio_names_list:
         return True
     try:
         radio_index = abs(int(radio_name))  # 0000 and -1
     except ValueError:
         return False
-    if len(GIni.radio_names_list) < radio_index:
+    if len(ghetto_ini.gini.radio_names_list) < radio_index:
         # input 100 if radio list has only 12 members
         return False
-    if GIni.radio_names_list[radio_index]:
+    if ghetto_ini.gini.radio_names_list[radio_index]:
         return True
 
 
 def record_validate_radio_name(radio_name):
     """ return radio name from 'radio_names_list', else return name by absolute number of index of 'radio_names_list'
     clean false input like 0000 to 0, -12 to 12
     GIni.radio_names_list[abs(int(12))] = 'nachtflug'
     """
-    if radio_name in GIni.radio_names_list:
+    if radio_name in ghetto_ini.gini.radio_names_list:
         return radio_name
     else:
         radio_id = radio_name
-        return GIni.radio_names_list[abs(int(radio_id))]
+        return ghetto_ini.gini.radio_names_list[abs(int(radio_id))]
 
 
 def record_create_radio_url_dict(radio_name):
     """ return tuple radio name, url
     need radio name as thread name and folder name, url to connect to network
     clean the radio name from special chars to make folders
     """
-    url = GIni.config_stations[radio_name]
+    url = ghetto_ini.gini.config_stations_dct[radio_name]
     radio_spec = remove_special_chars(radio_name)
     radio_url_tuple = (radio_spec, url)
     return radio_url_tuple
 
 
-def record_create_folder_radio_name(radio_name):
-    """ create parent folder and radio child folders either in dir with config files or in [GLOBAL] remote dir """
-    remote_dir = ghettoApi.save_to_dir
-    if remote_dir is not None:
-        save_path = str(Pathlib_path(os.path.join(ghettoApi.save_to_dir, ghettoApi.radio_parent)))
-    else:
-        save_path = str(Pathlib_path(os.path.join(ghettoApi.config_dir, ghettoApi.radio_parent)))
-    path = os.path.join(save_path, radio_name)
-    notes = "♫♪"
-    arrow = "-->"
-
-    try:
-        os.makedirs(path, exist_ok=True)
-        try:
-            print(f".. {notes} {path}")
-        except UnicodeEncodeError:
-            print(f".. {arrow} {path}")
-    except OSError:
-        print(f"\t{radio_name} Directory {path} can not be created")
-
-
 def terminal_record_blacklist_enabled_get():
     """ return True/False, called by ghetto_recorder module """
-    GIni.global_config_show()
-    return ghettoApi.blacklist_enable
+    ghetto_ini.global_config_show()
+    return ghettoApi.blacklist.blacklist_enable
 
 
 def terminal_record_all_radios_get():
     """ called by ghetto_recorder module to write blacklist beside settings.ini """
-    return GIni.radio_names_list
+    return ghetto_ini.gini.radio_names_list
 
 
 def path_change():
     """ call menu_path(), Change record parent path """
     print('\toption \'Change record parent path\'')
     menu_path()
 
@@ -324,71 +319,73 @@
         if any, write new one to GLOBAL section, create GLOBAL, if not exists
         test if path is writeable
         show new path, GIni.global_config_show
 
      Exception
         we crash, if config file is not in path, writing will fail
      """
-    print(f'\n\tWrite a new path to store files\n.. config file in {ghettoApi.config_dir}')
-    GIni.global_config_show()
+    print(f'\n\tWrite a new path to store files\n.. config file settings.ini in  {ghettoApi.path.config_dir}')
+    ghetto_ini.global_config_get()
+    ghetto_ini.global_config_show()
     while True:
         line_input = input('Enter a new path, OS syntax (f:\\10 or /home ) -->:')
         custom_path = line_input.strip()  # to validate the name
 
         if not len(custom_path):
             print("nothing to do ...")
             menu_main()
             break
         else:
             is_valid = path_validate_input(custom_path)
             if is_valid:
                 try:
-                    GIni.global_record_path_write(custom_path)
+                    ghetto_ini.global_record_path_write(custom_path)
                 except FileNotFoundError:
                     print("--> error, config file is not there or writeable (check path) - proceed")
-                GIni.global_config_show()
+                ghetto_ini.global_config_get()
+                ghetto_ini.global_config_show()
                 input('Hit Enter to leave -->:')
                 break
             else:
                 input_exit = input('Hit Enter to try again, or "E" to leave -->:')
                 if (input_exit == "E") or (input_exit == "E".lower()):
                     break
 
 
 def config_path_change():
     """ change the path to settings.ini and blacklist.json
 
      show old path
         write new path to [GLOBAL] section, create [GLOBAL], if not exists
         test if path is writeable
-        show new path, GIni.global_config_show()
+        show new path, ghetto_ini.global_config_show()
      """
     print(f'\n\tType path to folder with settings.ini and blacklist.json (used for radio sub directories)'
-          f'\n.. config file in {ghettoApi.config_dir}')
-    GIni.global_config_show()
+          f'\n.. config file settings.ini in  {ghettoApi.path.config_dir}')
+    ghetto_ini.global_config_show()
     while True:
         line_input = input('Enter a new path, OS syntax (f:\\10 or /home ) -->:')
         config_files_dir = line_input.strip()  # to validate the name
 
         if not len(config_files_dir):
             print("nothing to do ...")
             menu_main()
             break
         else:
-            old_config_dir = ghettoApi.config_dir
-            ghettoApi.config_dir = config_files_dir
-            has_config = record_path_get()
+            old_config_dir = ghettoApi.path.config_dir
+            ghettoApi.path.config_dir = config_files_dir
+            has_config = ghetto_ini.config_file_read()
             is_valid = path_validate_input(config_files_dir)
             if is_valid and has_config:
-                GIni.config_path_set(config_files_dir)
-                GIni.global_config_show()
+                ghetto_ini.config_path_api_set(config_files_dir)
+                ghetto_ini.global_config_show()
                 input('Hit Enter to leave -->:')
                 break
             else:
-                ghettoApi.config_dir = old_config_dir
+                ghettoApi.path.config_dir = old_config_dir
                 print(f'Not valid. Directory writeable: {is_valid}, has config: {has_config}')
                 input_exit = input('Hit Enter to try again, or "E" to leave -->:')
                 if (input_exit == "E") or (input_exit == "E".lower()):
                     break
 
 
 def path_validate_input(custom_path):
@@ -407,41 +404,43 @@
     print('\toption \'Enable/disable blacklists\'')
     blacklist_is_enabled()
 
 
 def blacklist_is_enabled():
     """ Write a new blacklist option to settings.ini file """
     print('\n\tWrite a new blacklist option to settings.ini file'
-          f'\n.. config file in {ghettoApi.config_dir}')
+          f'\n.. config file settings.ini in  {ghettoApi.path.config_dir}')
     menu_blacklist()
 
 
 def blacklist_on():
     """ write enabled to config file """
     print('\n\tblacklist is ON: settings.ini file'
           '\n\tExisting titles are not recorded again and again.'
           '\nfile name is "blacklist.json" in the same folder as "settings.ini"')
-    GIni.global_blacklist_enable_write("True")
-    GIni.global_config_show()
+    ghetto_ini.global_blacklist_enable_write("True")
+    ghetto_ini.global_config_get()
+    ghetto_ini.global_config_show()
     input('Hit Enter to leave -->:')
 
 
 def blacklist_off():
     """ write disabled to config file """
     print('\n\tblacklist is OFF: settings.ini file')
-    GIni.global_blacklist_enable_write("False")
-    GIni.global_config_show()
+    ghetto_ini.global_blacklist_enable_write("False")
+    ghetto_ini.global_config_get()
+    ghetto_ini.global_config_show()
     input('Hit Enter to leave -->:')
 
 
 def aac_file_repair():
     """
     """
     print('\n\tWrite a path to aac files. Only aac files will be touched.')
-    GIni.global_config_show()
+    ghetto_ini.global_config_show()
     while True:
         line_input = input('Enter a path, OS syntax (f:\\10 or /home ) -->:')
         aac_path = line_input.strip()  # to validate the name
 
         if not len(aac_path):
             print("nothing to do ...")
             menu_main()
@@ -458,7 +457,18 @@
                 if (input_exit == "E") or (input_exit == "E".lower()):
                     break
 
 
 def remove_special_chars(str_name):
     ret_value = str_name.translate({ord(string): "" for string in '"!@#$%^*()[]{};:,./<>?\\|`~=+"""'})
     return ret_value
+
+
+def main():
+    config_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)))
+    ghettoApi.path.config_dir = config_dir
+    ghettoApi.path.config_name = "settings.ini"
+    menu_main()
+
+
+if __name__ == "__main__":
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `GhettoRecorder-2.4.7/ghettorecorder/settings.ini` & `GhettoRecorder-3.0/ghettorecorder/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,56 @@
 00000000: 5b53 5441 5449 4f4e 535d 0d0a 6161 6363  [STATIONS]..aacc
 00000010: 6869 6c6c 203d 2068 7474 703a 2f2f 7261  hill = http://ra
 00000020: 6469 6f34 2e76 6970 2d72 6164 696f 732e  dio4.vip-radios.
 00000030: 666d 3a38 3032 302f 7374 7265 616d 3132  fm:8020/stream12
 00000040: 386b 2d41 4143 2d43 6869 6c6c 5f61 7574  8k-AAC-Chill_aut
-00000050: 6f64 6a0d 0a38 3069 6573 5f6e 6c20 3d20  odj..80ies_nl = 
-00000060: 6874 7470 3a2f 2f39 342e 3232 382e 3133  http://94.228.13
-00000070: 332e 353a 3830 0d0a 616e 696d 655f 6a70  3.5:80..anime_jp
-00000080: 203d 2068 7474 703a 2f2f 7374 7265 616d   = http://stream
-00000090: 696e 6776 322e 7368 6f75 7463 6173 742e  ingv2.shoutcast.
-000000a0: 636f 6d2f 6a61 7061 6e69 6d72 6164 696f  com/japanimradio
-000000b0: 2d74 6f6b 796f 0d0a 626c 7565 735f 756b  -tokyo..blues_uk
-000000c0: 203d 2068 7474 703a 2f2f 3134 392e 3235   = http://149.25
-000000d0: 352e 3539 2e33 3a38 3233 322f 7374 7265  5.59.3:8232/stre
-000000e0: 616d 0d0a 6272 3234 203d 2068 7474 7073  am..br24 = https
-000000f0: 3a2f 2f64 6973 7061 7463 6865 722e 726e  ://dispatcher.rn
-00000100: 6466 6e6b 2e63 6f6d 2f62 722f 6272 3234  dfnk.com/br/br24
-00000110: 2f6c 6976 652f 6d70 332f 6d69 640d 0a62  /live/mp3/mid..b
-00000120: 726f 636b 656e 203d 2068 7474 703a 2f2f  rocken = http://
-00000130: 7374 7265 616d 2e72 6164 696f 6272 6f63  stream.radiobroc
-00000140: 6b65 6e2e 6465 2f6c 6976 652f 6d70 332d  ken.de/live/mp3-
-00000150: 3235 362f 7261 6469 6f70 6c61 7965 7268  256/radioplayerh
-00000160: 702f 706c 6179 2e6d 3375 0d0a 636c 6173  p/play.m3u..clas
-00000170: 7369 635f 726f 203d 2068 7474 703a 2f2f  sic_ro = http://
-00000180: 3337 2e32 3531 2e31 3436 2e31 3639 3a38  37.251.146.169:8
-00000190: 3030 302f 7374 7265 616d 4844 0d0a 6666  000/streamHD..ff
-000001a0: 6e20 3d20 6874 7470 3a2f 2f70 6c61 7965  n = http://playe
-000001b0: 722e 6666 6e2e 6465 2f72 6164 696f 6666  r.ffn.de/radioff
-000001c0: 6e2e 6d33 750d 0a67 6f61 5f70 7379 203d  n.m3u..goa_psy =
-000001d0: 2068 7474 7073 3a2f 2f61 6d6f 7269 732e   https://amoris.
-000001e0: 736b 6e74 2e72 752f 676f 612e 6d70 330d  sknt.ru/goa.mp3.
-000001f0: 0a68 6d20 3d20 6874 7470 733a 2f2f 6869  .hm = https://hi
-00000200: 7273 6368 6d69 6c63 682e 6465 3a37 3030  rschmilch.de:700
-00000210: 312f 7072 6f67 2d68 6f75 7365 2e6d 7033  1/prog-house.mp3
-00000220: 0d0a 686f 6d65 5f74 6578 6173 203d 2068  ..home_texas = h
-00000230: 7474 703a 2f2f 6865 7374 6961 2e63 646e  ttp://hestia.cdn
-00000240: 7374 7265 616d 2e63 6f6d 3a38 302f 3135  stream.com:80/15
-00000250: 3537 5f36 340d 0a68 7233 203d 2068 7474  57_64..hr3 = htt
-00000260: 703a 2f2f 6d65 7461 6669 6c65 732e 676c  p://metafiles.gl
-00000270: 2d73 7973 7465 6d68 6175 732e 6465 2f68  -systemhaus.de/h
-00000280: 722f 6872 335f 322e 6d33 750d 0a6d 6472  r/hr3_2.m3u..mdr
-00000290: 5f6a 756d 7020 3d20 6874 7470 3a2f 2f61  _jump = http://a
-000002a0: 7677 2e6d 6472 2e64 652f 7374 7265 616d  vw.mdr.de/stream
-000002b0: 732f 3238 3433 3230 2d30 5f6d 7033 5f68  s/284320-0_mp3_h
-000002c0: 6967 682e 6d33 750d 0a6e 6572 642d 736f  igh.m3u..nerd-so
-000002d0: 756e 642d 7472 6163 6b73 203d 2068 7474  und-tracks = htt
-000002e0: 703a 2f2f 3136 372e 3131 342e 3231 302e  p://167.114.210.
-000002f0: 3233 323a 3832 3539 2f73 7472 6561 6d0d  232:8259/stream.
-00000300: 0a6e 6163 6874 666c 7567 203d 2068 7474  .nachtflug = htt
-00000310: 703a 2f2f 3835 2e31 3935 2e38 382e 3134  p://85.195.88.14
-00000320: 393a 3131 3831 300d 0a6e 6472 3220 3d20  9:11810..ndr2 = 
-00000330: 6874 7470 3a2f 2f77 7777 2e6e 6472 2e64  http://www.ndr.d
-00000340: 652f 7265 736f 7572 6365 732f 6d65 7461  e/resources/meta
-00000350: 6461 7465 6e2f 6175 6469 6f2f 6d33 752f  daten/audio/m3u/
-00000360: 6e64 7232 2e6d 3375 0d0a 7061 6c6f 6d61  ndr2.m3u..paloma
-00000370: 203d 2068 7474 7073 3a2f 2f70 6f6f 6c2e   = https://pool.
-00000380: 7261 6469 6f70 616c 6f6d 612e 6465 2f52  radiopaloma.de/R
-00000390: 4144 494f 5041 4c4f 4d41 2e6d 7033 0d0a  ADIOPALOMA.mp3..
-000003a0: 706c 6179 7572 6261 6e20 3d20 6874 7470  playurban = http
-000003b0: 3a2f 2f6c 6976 652e 706c 6179 7261 6469  ://live.playradi
-000003c0: 6f2e 6f72 673a 3930 3930 2f55 7262 616e  o.org:9090/Urban
-000003d0: 4844 0d0a 706f 7032 3420 3d20 6874 7470  HD..pop24 = http
-000003e0: 3a2f 2f72 6f73 6577 656c 6c70 6f70 2e72  ://rosewellpop.r
-000003f0: 6164 696f 6361 2e73 743a 3830 2f73 7472  adioca.st:80/str
-00000400: 6561 6d73 2f33 3230 6b62 7073 3f79 703d  eams/320kbps?yp=
-00000410: 330d 0a72 6567 6761 6520 3d20 6874 7470  3..reggae = http
-00000420: 3a2f 2f68 642e 6c61 6772 6f73 7365 7261  ://hd.lagrossera
-00000430: 6469 6f2e 696e 666f 3a38 3030 302f 6c61  dio.info:8000/la
-00000440: 6772 6f73 7365 7261 6469 6f2d 7265 6767  grosseradio-regg
-00000450: 6165 2d31 3932 2e6d 7033 0d0a 7469 6d65  ae-192.mp3..time
-00000460: 5f6d 6163 6869 6e65 203d 2068 7474 703a  _machine = http:
-00000470: 2f2f 3938 2e32 3131 2e36 382e 393a 3837  //98.211.68.9:87
-00000480: 3635 0d0a 7669 6574 3220 3d20 6874 7470  65..viet2 = http
-00000490: 3a2f 2f6c 6976 6530 322e 7266 692e 6672  ://live02.rfi.fr
-000004a0: 2f72 6669 656e 7669 6574 6e61 6d69 656e  /rfienvietnamien
-000004b0: 2d36 342e 6d70 330d 0a76 6965 7420 3d20  -64.mp3..viet = 
-000004c0: 6874 7470 3a2f 2f6d 6564 6961 2e6b 7974  http://media.kyt
-000004d0: 6875 6174 766f 762e 766e 3a37 3032 312f  huatvov.vn:7021/
-000004e0: 3b73 7472 6561 6d2f 0d0a 7965 6168 6d6f  ;stream/..yeahmo
-000004f0: 6e20 3d20 6874 7470 3a2f 2f63 332e 7261  n = http://c3.ra
-00000500: 6469 6f62 6f73 732e 666d 3a38 3039 352f  dioboss.fm:8095/
-00000510: 6175 746f 646a 0d0a 7a65 6e73 7479 6c65  autodj..zenstyle
-00000520: 203d 2068 7474 7073 3a2f 2f72 6164 696f   = https://radio
-00000530: 342e 6364 6d2d 7261 6469 6f2e 636f 6d3a  4.cdm-radio.com:
-00000540: 3138 3030 342f 7374 7265 616d 2d6d 7033  18004/stream-mp3
-00000550: 2d5a 656e 0d0a 0d0a 5b47 4c4f 4241 4c5d  -Zen....[GLOBAL]
-00000560: 0d0a 626c 6163 6b6c 6973 745f 656e 6162  ..blacklist_enab
-00000570: 6c65 203d 2054 7275 650d 0a0d 0a0d 0a    le = True......
+00000050: 6f64 6a0d 0a61 6e69 6d65 5f6a 7020 3d20  odj..anime_jp = 
+00000060: 6874 7470 3a2f 2f73 7472 6561 6d69 6e67  http://streaming
+00000070: 7632 2e73 686f 7574 6361 7374 2e63 6f6d  v2.shoutcast.com
+00000080: 2f6a 6170 616e 696d 7261 6469 6f2d 746f  /japanimradio-to
+00000090: 6b79 6f0d 0a62 726f 636b 656e 203d 2068  kyo..brocken = h
+000000a0: 7474 703a 2f2f 7374 7265 616d 2e72 6164  ttp://stream.rad
+000000b0: 696f 6272 6f63 6b65 6e2e 6465 2f6c 6976  iobrocken.de/liv
+000000c0: 652f 6d70 332d 3235 362f 7261 6469 6f70  e/mp3-256/radiop
+000000d0: 6c61 7965 7268 702f 706c 6179 2e6d 3375  layerhp/play.m3u
+000000e0: 0d0a 636c 6173 7369 635f 726f 203d 2068  ..classic_ro = h
+000000f0: 7474 703a 2f2f 3337 2e32 3531 2e31 3436  ttp://37.251.146
+00000100: 2e31 3639 3a38 3030 302f 7374 7265 616d  .169:8000/stream
+00000110: 4844 0d0a 6869 7273 6368 6d69 6c63 6820  HD..hirschmilch 
+00000120: 3d20 6874 7470 733a 2f2f 6869 7273 6368  = https://hirsch
+00000130: 6d69 6c63 682e 6465 3a37 3030 312f 7072  milch.de:7001/pr
+00000140: 6f67 2d68 6f75 7365 2e6d 7033 0d0a 6872  og-house.mp3..hr
+00000150: 3320 3d20 6874 7470 3a2f 2f6d 6574 6166  3 = http://metaf
+00000160: 696c 6573 2e67 6c2d 7379 7374 656d 6861  iles.gl-systemha
+00000170: 7573 2e64 652f 6872 2f68 7233 5f32 2e6d  us.de/hr/hr3_2.m
+00000180: 3375 0d0a 6d64 725f 6a75 6d70 203d 2068  3u..mdr_jump = h
+00000190: 7474 703a 2f2f 6176 772e 6d64 722e 6465  ttp://avw.mdr.de
+000001a0: 2f73 7472 6561 6d73 2f32 3834 3332 302d  /streams/284320-
+000001b0: 305f 6d70 335f 6869 6768 2e6d 3375 0d0a  0_mp3_high.m3u..
+000001c0: 6e61 6368 7466 6c75 6720 3d20 6874 7470  nachtflug = http
+000001d0: 3a2f 2f38 352e 3139 352e 3838 2e31 3439  ://85.195.88.149
+000001e0: 3a31 3138 3130 0d0a 7061 6c6f 6d61 203d  :11810..paloma =
+000001f0: 2068 7474 7073 3a2f 2f70 6f6f 6c2e 7261   https://pool.ra
+00000200: 6469 6f70 616c 6f6d 612e 6465 2f52 4144  diopaloma.de/RAD
+00000210: 494f 5041 4c4f 4d41 2e6d 7033 0d0a 706c  IOPALOMA.mp3..pl
+00000220: 6179 7572 6261 6e20 3d20 6874 7470 3a2f  ayurban = http:/
+00000230: 2f6c 6976 652e 706c 6179 7261 6469 6f2e  /live.playradio.
+00000240: 6f72 673a 3930 3930 2f55 7262 616e 4844  org:9090/UrbanHD
+00000250: 0d0a 7265 6767 6165 203d 2068 7474 703a  ..reggae = http:
+00000260: 2f2f 6864 2e6c 6167 726f 7373 6572 6164  //hd.lagrosserad
+00000270: 696f 2e69 6e66 6f3a 3830 3030 2f6c 6167  io.info:8000/lag
+00000280: 726f 7373 6572 6164 696f 2d72 6567 6761  rosseradio-regga
+00000290: 652d 3139 322e 6d70 330d 0a74 696d 655f  e-192.mp3..time_
+000002a0: 6d61 6368 696e 6520 3d20 6874 7470 3a2f  machine = http:/
+000002b0: 2f39 382e 3231 312e 3638 2e39 3a38 3736  /98.211.68.9:876
+000002c0: 350d 0a79 6561 686d 6f6e 203d 2068 7474  5..yeahmon = htt
+000002d0: 703a 2f2f 6333 2e72 6164 696f 626f 7373  p://c3.radioboss
+000002e0: 2e66 6d3a 3830 3935 2f61 7574 6f64 6a0d  .fm:8095/autodj.
+000002f0: 0a7a 656e 7374 796c 6520 3d20 6874 7470  .zenstyle = http
+00000300: 733a 2f2f 7261 6469 6f34 2e63 646d 2d72  s://radio4.cdm-r
+00000310: 6164 696f 2e63 6f6d 3a31 3830 3034 2f73  adio.com:18004/s
+00000320: 7472 6561 6d2d 6d70 332d 5a65 6e0d 0a64  tream-mp3-Zen..d
+00000330: 6576 203d 2068 7474 703a 2f2f 6c6f 6361  ev = http://loca
+00000340: 6c68 6f73 743a 3830 3030 2f72 6164 696f  lhost:8000/radio
+00000350: 0d0a 0d0a 5b47 4c4f 4241 4c5d 0d0a 626c  ....[GLOBAL]..bl
+00000360: 6163 6b6c 6973 745f 656e 6162 6c65 203d  acklist_enable =
+00000370: 2054 7275 650d 0a                         True..
```

