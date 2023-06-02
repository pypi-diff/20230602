# Comparing `tmp/pysmart365-0.0.4.tar.gz` & `tmp/pysmart365-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.4.tar", last modified: Tue May 30 15:09:17 2023, max compression
+gzip compressed data, was "pysmart365-0.0.5.tar", last modified: Fri Jun  2 13:27:55 2023, max compression
```

## Comparing `pysmart365-0.0.4.tar` & `pysmart365-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:09:17.659386 pysmart365-0.0.4/
--rw-rw-rw-   0        0        0    35802 2023-05-27 14:51:46.000000 pysmart365-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      467 2023-05-30 15:09:17.643786 pysmart365-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-05-28 11:36:50.000000 pysmart365-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 15:09:17.628186 pysmart365-0.0.4/pysmart365/
--rw-rw-rw-   0        0        0     1103 2023-05-29 17:14:25.000000 pysmart365-0.0.4/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     2319 2023-05-29 11:53:59.000000 pysmart365-0.0.4/pysmart365/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:09:17.643786 pysmart365-0.0.4/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      467 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 15:09:17.659386 pysmart365-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-29 17:53:53.000000 pysmart365-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:27:55.989868 pysmart365-0.0.5/
+-rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      442 2023-06-02 13:27:55.989868 pysmart365-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-02 13:24:19.000000 pysmart365-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 13:27:55.970916 pysmart365-0.0.5/pysmart365/
+-rw-rw-rw-   0        0        0     1028 2023-06-02 13:27:34.000000 pysmart365-0.0.5/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     2218 2023-06-02 13:27:19.000000 pysmart365-0.0.5/pysmart365/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:27:55.988871 pysmart365-0.0.5/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      442 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 13:27:55.989868 pysmart365-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-06-02 13:25:17.000000 pysmart365-0.0.5/setup.py
```

### Comparing `pysmart365-0.0.4/LICENSE` & `pysmart365-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pysmart365-0.0.4/README.md` & `pysmart365-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.4/pysmart365/MicroSoftware.py` & `pysmart365-0.0.5/pysmart365/MicroSoftware.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,22 @@
         sleep = time.sleep(0)
         return sleep
     elif delay:
         sleep1 = time.sleep(delay)
         return sleep1
     else:
         print("Error")
-class center_screen():
-    def init(width, height):
-        try:
-            monitors = get_monitors()
-            if monitors:
-                monitor = monitors[0]
-                screen_width = monitor.width
-                screen_height = monitor.height
-                sw = (screen_width - width) // 2
-                sh = (screen_height - height) // 2
-                text = f'{width}x{height}+{sw}+{sh}'
-                return text
-            else:
-                return None
-        except Exception as error:
-            print('Error: ', error)
+def center_screen(width, height):
+    try:
+        monitors = get_monitors()
+        if monitors:
+            monitor = monitors[0]
+            screen_width = monitor.width
+            screen_height = monitor.height
+            sw = (screen_width - width) // 2
+            sh = (screen_height - height) // 2
+            text = f'{width}x{height}+{sw}+{sh}'
+            return text
+        else:
+            return None
+    except Exception as error:
+        print('Error: ', error)
```

### Comparing `pysmart365-0.0.4/pysmart365/__init__.py` & `pysmart365-0.0.5/pysmart365/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 AUTHOR = 'Runkang'
 COPYRIGHT = '© Copyright 2023 Informatic365 - SmartSoft - MicroSoftware'
 
-class main():
-    print("Welcome to pysmart365 0.0.3")
-
 import subprocess
 import platform
 from customtkinter import *
 from tkinter import messagebox
 import sys
 
 def turn_off(time):
@@ -56,11 +53,9 @@
     '''
     Enter the copyright text that will be displayed with the name that you can customize and the year using the attribute 'company' for the name and 'year' for the year.
     Example if i write copyright_view(year='2022 - 2023', company= 'Informatic365')
     then displays "© Copyright 2022 - 2023 Informatic365".
     '''
     get = f'© Copyright {year} {company}'
     return get
-class close():
-    sys.exit()
-if __name__ == '__main__':
-    main()
+def close():
+    sys.exit()
```

