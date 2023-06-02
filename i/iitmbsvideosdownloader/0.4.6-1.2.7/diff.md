# Comparing `tmp/iitmbsvideosdownloader-0.4.6.tar.gz` & `tmp/iitmbsvideosdownloader-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitmbsvideosdownloader-0.4.6.tar", last modified: Mon Mar  6 19:50:55 2023, max compression
+gzip compressed data, was "iitmbsvideosdownloader-1.2.7.tar", last modified: Fri Jun  2 07:44:10 2023, max compression
```

## Comparing `iitmbsvideosdownloader-0.4.6.tar` & `iitmbsvideosdownloader-1.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-03-06 19:50:55.055904 iitmbsvideosdownloader-0.4.6/
--rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-0.4.6/LICENSE.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-03-06 19:50:55.055904 iitmbsvideosdownloader-0.4.6/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-0.4.6/README.md
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-03-06 19:50:54.371123 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      318 2023-02-14 19:22:42.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/SITES.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/SUBJECTS.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/__init__.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7257 2023-02-24 19:05:01.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/_downloader.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7194 2023-03-06 19:44:07.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/_functions.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     5294 2023-02-24 18:59:02.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/_iitm.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     4630 2023-02-24 18:59:02.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/iitmbsvideosdownloader.py
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-03-06 19:50:54.909151 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-03-06 19:50:47.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-03-06 19:50:48.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/SOURCES.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-03-06 19:50:47.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/dependency_links.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       16 2023-03-06 19:50:47.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/requires.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-03-06 19:50:47.000000 iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/top_level.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-03-06 19:50:55.087808 iitmbsvideosdownloader-0.4.6/setup.cfg
--rwxrwxrwx   0 savi      (1000) savi      (1000)      438 2023-03-06 19:48:46.000000 iitmbsvideosdownloader-0.4.6/setup.py
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-06-02 07:44:10.697019 iitmbsvideosdownloader-1.2.7/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-1.2.7/LICENSE.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-06-02 07:44:10.697019 iitmbsvideosdownloader-1.2.7/PKG-INFO
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-1.2.7/README.md
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-06-02 07:44:09.993177 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      318 2023-02-14 19:22:42.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/SITES.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/SUBJECTS.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/__init__.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     7257 2023-02-24 19:05:01.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/_downloader.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     7194 2023-03-06 19:44:07.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/_functions.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     5545 2023-06-02 07:35:29.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/_iitm.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     4630 2023-02-24 18:59:02.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/iitmbsvideosdownloader.py
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-06-02 07:44:10.555683 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-06-02 07:44:02.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/PKG-INFO
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-06-02 07:44:03.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/SOURCES.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-06-02 07:44:02.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/dependency_links.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)       16 2023-06-02 07:44:02.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/requires.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-06-02 07:44:02.000000 iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/top_level.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-06-02 07:44:10.728621 iitmbsvideosdownloader-1.2.7/setup.cfg
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      438 2023-06-02 07:38:49.000000 iitmbsvideosdownloader-1.2.7/setup.py
```

### Comparing `iitmbsvideosdownloader-0.4.6/LICENSE.txt` & `iitmbsvideosdownloader-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-0.4.6/README.md` & `iitmbsvideosdownloader-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/SUBJECTS.py` & `iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/SUBJECTS.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/_downloader.py` & `iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/_downloader.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/_functions.py` & `iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/_functions.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/_iitm.py` & `iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/_iitm.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
         time.sleep(self.SLEEP_TIME)
         side_titles_elements = driver.find_elements(By.CLASS_NAME, "units__items-title")
         side_titles_text = [side_titles_elements[i].text for i in range(len(side_titles_elements))]
 
         self.log(f"Side titles - {side_titles_text}", 3)
 
-        if f"Week {self.WEEK}" not in side_titles_text:
+        if f"Week {self.WEEK} :" not in side_titles_text:
             return None, None
 
-        index_title = side_titles_text.index(f"Week {self.WEEK}")
+        index_title = side_titles_text.index(f"Week {self.WEEK} :")
         self.log(f"Selected side title - {side_titles_text[index_title]}", 3)
 
         side_elements[index_title].click()
 
         units_sublist_test = self.wait_for_element_by_xPath(driver, "//div[contains(@class, 'units__sublist')]/div", 20)
 
         if units_sublist_test is None:
@@ -71,27 +71,32 @@
 
         self.log(f"Sub side titles - {titles}", 3)
 
         # Getting video links
         for i in range(len(sub_items_elements)):
             element = sub_items_elements[i]
             # time.sleep(self.SLEEP_TIME)
-            units_subitem_title_test = self.wait_for_element_by_xPath(element, "div/div[contains(@class, 'units__subitems-title')]/div", 20)
+            units_subitem_title_test = self.wait_for_element_by_xPath(element,
+                                                                      "div/div[contains(@class, 'units__subitems-title')]/div",
+                                                                      20)
 
             if units_subitem_title_test is None:
                 self.log("Finding an element failed, Retrying...", 2)
                 return self.get_video_titles_and_links(driver)
 
             video_text = element.find_element(By.XPATH, "div/div[contains(@class, 'units__subitems-title')]/div")
 
             text = video_text.get_attribute("innerHTML")
             result = re.sub(r'<!(-)+>', '', text)
             if result == "Video":
                 self.log(f"--> Grabbing sub side title ({titles[i]}) details...", 3)
-                element.click()
+                try:
+                    element.click()
+                except:
+                    units_subitem_title_test.click()
 
                 player_test = self.wait_for_element_by_xPath(driver, "//iframe[contains(@id, 'player')]", 20)
 
                 if player_test is None:
                     self.log("Finding an element failed, Retrying...", 2)
                     return self.get_video_titles_and_links(driver)
```

### Comparing `iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader/iitmbsvideosdownloader.py` & `iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader/iitmbsvideosdownloader.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-0.4.6/iitmbsvideosdownloader.egg-info/SOURCES.txt` & `iitmbsvideosdownloader-1.2.7/iitmbsvideosdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

