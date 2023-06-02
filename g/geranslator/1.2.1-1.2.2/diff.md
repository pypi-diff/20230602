# Comparing `tmp/geranslator-1.2.1-py3-none-any.whl.zip` & `tmp/geranslator-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24289 bytes, number of entries: 44
+Zip file size: 24400 bytes, number of entries: 44
 -rw-rw-rw-  2.0 fat       54 b- defN 23-Feb-26 22:40 geranslator/__init__.py
 -rw-rw-rw-  2.0 fat     6413 b- defN 23-Apr-09 01:56 geranslator/geranslator.py
 -rw-rw-rw-  2.0 fat       82 b- defN 23-Feb-07 16:22 geranslator/command_line/__init__.py
 -rw-rw-rw-  2.0 fat     1718 b- defN 23-Apr-02 01:29 geranslator/command_line/command_line.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-21 16:20 geranslator/config/__init__.py
 -rw-rw-rw-  2.0 fat     1441 b- defN 23-Apr-06 18:10 geranslator/config/config.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-06 18:10 geranslator/config/samples/__init__.py
@@ -30,17 +30,17 @@
 -rw-rw-rw-  2.0 fat      699 b- defN 23-Apr-06 18:10 geranslator/guess/guess.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-25 13:08 geranslator/languages/__init__.py
 -rw-rw-rw-  2.0 fat     2034 b- defN 23-Jan-25 13:08 geranslator/languages/dictionary.yml
 -rw-rw-rw-  2.0 fat      414 b- defN 23-Feb-07 16:22 geranslator/languages/languages.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-25 13:08 geranslator/provider/__init__.py
 -rw-rw-rw-  2.0 fat     1368 b- defN 23-Apr-09 01:56 geranslator/provider/provider.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-25 13:08 geranslator/provider/providers/__init__.py
--rw-rw-rw-  2.0 fat     7973 b- defN 23-Apr-09 01:56 geranslator/provider/providers/abstractProvider.py
+-rw-rw-rw-  2.0 fat     7973 b- defN 23-Jun-02 17:50 geranslator/provider/providers/abstractProvider.py
 -rw-rw-rw-  2.0 fat     5573 b- defN 23-Apr-08 01:53 geranslator/provider/providers/deepl.py
--rw-rw-rw-  2.0 fat     4805 b- defN 23-Feb-26 22:40 geranslator/provider/providers/google.py
--rw-rw-rw-  2.0 fat     1095 b- defN 23-Apr-09 02:19 geranslator-1.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4658 b- defN 23-Apr-09 02:19 geranslator-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-09 02:19 geranslator-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       63 b- defN 23-Apr-09 02:19 geranslator-1.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-09 02:19 geranslator-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     4083 b- defN 23-Apr-09 02:19 geranslator-1.2.1.dist-info/RECORD
-44 files, 53582 bytes uncompressed, 17559 bytes compressed:  67.2%
+-rw-rw-rw-  2.0 fat     5340 b- defN 23-Jun-02 19:15 geranslator/provider/providers/google.py
+-rw-rw-rw-  2.0 fat     1095 b- defN 23-Jun-02 19:22 geranslator-1.2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4658 b- defN 23-Jun-02 19:22 geranslator-1.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 19:22 geranslator-1.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       63 b- defN 23-Jun-02 19:22 geranslator-1.2.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-02 19:22 geranslator-1.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     4083 b- defN 23-Jun-02 19:22 geranslator-1.2.2.dist-info/RECORD
+44 files, 54117 bytes uncompressed, 17670 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -108,26 +108,26 @@
 
 Filename: geranslator/provider/providers/deepl.py
 Comment: 
 
 Filename: geranslator/provider/providers/google.py
 Comment: 
 
-Filename: geranslator-1.2.1.dist-info/LICENSE
+Filename: geranslator-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: geranslator-1.2.1.dist-info/METADATA
+Filename: geranslator-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: geranslator-1.2.1.dist-info/WHEEL
+Filename: geranslator-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: geranslator-1.2.1.dist-info/entry_points.txt
+Filename: geranslator-1.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: geranslator-1.2.1.dist-info/top_level.txt
+Filename: geranslator-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: geranslator-1.2.1.dist-info/RECORD
+Filename: geranslator-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geranslator/provider/providers/google.py

```diff
@@ -1,9 +1,10 @@
 import time
 
+from selenium.common.exceptions import WebDriverException
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.ui import WebDriverWait
 from termspark import TermSpark
 
@@ -23,23 +24,37 @@
 
         ActionChains(self.driver).move_to_element(source_text).click().send_keys(
             text
         ).perform()
 
         time.sleep(4)
 
-        WebDriverWait(self.driver, 15).until(
-            expected_conditions.presence_of_element_located(
-                (By.XPATH, "//button[@aria-label='Copy translation']")
+        try:
+            WebDriverWait(self.driver, 15).until(
+                expected_conditions.presence_of_element_located(
+                    (By.XPATH, "//button[@aria-label='Copy translation']")
+                )
             )
-        )
+        except WebDriverException:
+            while True:
+                try_again = self.driver.find_element(
+                    by=By.XPATH,
+                    value="//button[contains(@class, 'VfPpkd-LgbsSe')][contains(.,'Try again')]",
+                )
+
+                if try_again.is_displayed():
+                    try_again.click()
+                    time.sleep(6)
+                else:
+                    break
 
         translated_element = self.driver.find_element(
             by=By.XPATH, value="//span[@class='HwtZe']"
         )
+
         translation = translated_element.text.lower()
 
         self.clear_source_text()
 
         return translation
 
     def choose_origin_language(self, origin_lang: str) -> bool:
@@ -91,17 +106,17 @@
                 ActionChains(self.driver).move_to_element(
                     search_language_element
                 ).click().send_keys(language).perform()
                 time.sleep(2)
                 unexisted_language = self.driver.find_element(
                     by=By.XPATH,
                     value="//div[@class='G3Fn7c'][contains(.,'No results')]",
-                ).is_displayed()
+                )
 
-                if unexisted_language:
+                if unexisted_language.is_displayed():
                     TermSpark().spark_left([f"{language} "]).spark_right(
                         [" language not supported by google", "red"]
                     ).set_separator(".").spark()
                     ActionChains(self.driver).send_keys(Keys.ESCAPE).perform()
                     return False
                 else:
                     ActionChains(self.driver).send_keys(
```

## Comparing `geranslator-1.2.1.dist-info/LICENSE` & `geranslator-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `geranslator-1.2.1.dist-info/METADATA` & `geranslator-1.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geranslator
-Version: 1.2.1
+Version: 1.2.2
 Summary: Translate your translation files
 Home-page: https://github.com/faissaloux/geranslator
 Author: Faissal Wahabali
 Author-email: fwahabali@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/faissaloux/geranslator
 Project-URL: Documentation, https://geranslator.faissaloux.com
```

## Comparing `geranslator-1.2.1.dist-info/RECORD` & `geranslator-1.2.2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 geranslator/languages/dictionary.yml,sha256=6xOZm_jdDOjssBFAm-loQmyoBLZTAvXBFgXDVN-sUME,2034
 geranslator/languages/languages.py,sha256=2-Bmyw12Wb6KvcPM9b0mFFIvMWeZmzvPgSH3KKBnejg,414
 geranslator/provider/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 geranslator/provider/provider.py,sha256=ciZ-Rn10RswA6lzfSjO7bXXMCo_CFY-UZORRWIy13G8,1368
 geranslator/provider/providers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 geranslator/provider/providers/abstractProvider.py,sha256=zXa4eG7Q4TG5IESxVQem3Odv3GcJgdsJ6K84iC9m39I,7973
 geranslator/provider/providers/deepl.py,sha256=2YEO3H2K75p9vE6QwUm0Ok8q3azj366wxGGGHhuvwro,5573
-geranslator/provider/providers/google.py,sha256=2s5WN3qU42AMXvtZE6mfGiMJ_SiPVfMoau7eNiRnVIo,4805
-geranslator-1.2.1.dist-info/LICENSE,sha256=ufRWIjJ80YIm0Rz89CaBkd-qiRDmJnlJkslV3RyYi8g,1095
-geranslator-1.2.1.dist-info/METADATA,sha256=JdTayOYRzQP8fJmlg32B1oJS_sdDHhRr7xjcrH_XWtc,4658
-geranslator-1.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-geranslator-1.2.1.dist-info/entry_points.txt,sha256=y9pYeUjbjPSN0zYJuwf3nGEMwJmy5QpLE8Y5S4JJvK4,63
-geranslator-1.2.1.dist-info/top_level.txt,sha256=Hyel09eLis3mqtcpyt3phrv8gr_HoDOwCNsGWAqqJHo,12
-geranslator-1.2.1.dist-info/RECORD,,
+geranslator/provider/providers/google.py,sha256=26_lNP4Up4wz2aDFowKe21iFVBc2KCHoIoDW7yilKEI,5340
+geranslator-1.2.2.dist-info/LICENSE,sha256=ufRWIjJ80YIm0Rz89CaBkd-qiRDmJnlJkslV3RyYi8g,1095
+geranslator-1.2.2.dist-info/METADATA,sha256=fv7j0ki5DxCxAx0bQdOR6mStOS_yGo8f-n-85EAuQd4,4658
+geranslator-1.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+geranslator-1.2.2.dist-info/entry_points.txt,sha256=y9pYeUjbjPSN0zYJuwf3nGEMwJmy5QpLE8Y5S4JJvK4,63
+geranslator-1.2.2.dist-info/top_level.txt,sha256=Hyel09eLis3mqtcpyt3phrv8gr_HoDOwCNsGWAqqJHo,12
+geranslator-1.2.2.dist-info/RECORD,,
```

