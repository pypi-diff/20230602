# Comparing `tmp/twAuto-0.3.5.tar.gz` & `tmp/twAuto-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twAuto-0.3.5.tar", last modified: Wed May 31 11:12:55 2023, max compression
+gzip compressed data, was "twAuto-0.3.6.tar", last modified: Thu Jun  1 22:05:08 2023, max compression
```

## Comparing `twAuto-0.3.5.tar` & `twAuto-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:55.517353 twAuto-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-31 11:12:40.000000 twAuto-0.3.5/LICENCE.MD
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 11:12:40.000000 twAuto-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-31 11:12:55.517353 twAuto-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-31 11:12:40.000000 twAuto-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:12:55.517353 twAuto-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-31 11:12:40.000000 twAuto-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:55.517353 twAuto-0.3.5/twAuto/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 11:12:40.000000 twAuto-0.3.5/twAuto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31693 2023-05-31 11:12:40.000000 twAuto-0.3.5/twAuto/twauto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:55.517353 twAuto-0.3.5/twAuto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:05:08.675248 twAuto-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 22:04:57.000000 twAuto-0.3.6/LICENCE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 22:04:57.000000 twAuto-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-01 22:05:08.675248 twAuto-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-01 22:04:57.000000 twAuto-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 22:05:08.675248 twAuto-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 22:04:57.000000 twAuto-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:05:08.675248 twAuto-0.3.6/twAuto/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 22:04:57.000000 twAuto-0.3.6/twAuto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27148 2023-06-01 22:04:57.000000 twAuto-0.3.6/twAuto/twauto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:05:08.675248 twAuto-0.3.6/twAuto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-01 22:05:08.000000 twAuto-0.3.6/twAuto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-01 22:05:08.000000 twAuto-0.3.6/twAuto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:05:08.000000 twAuto-0.3.6/twAuto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 22:05:08.000000 twAuto-0.3.6/twAuto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 22:05:08.000000 twAuto-0.3.6/twAuto.egg-info/top_level.txt
```

### Comparing `twAuto-0.3.5/LICENCE.MD` & `twAuto-0.3.6/LICENCE.MD`

 * *Files identical despite different names*

### Comparing `twAuto-0.3.5/PKG-INFO` & `twAuto-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: twAuto
-Version: 0.3.5
+Version: 0.3.6
 Summary: TwAuto is a library for testing your code on pre-Twitter API application stage.
 Home-page: https://github.com/EKOzkan/twAuto
 Author: Ekin Kagan Ozkan
 Author-email: ekinkagan@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE.MD
 
-# twAuto - Twitter Automation Tool v0.3.4 🦆
+# twAuto - Twitter Automation Tool v0.3.6 🦆
 
 twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
 
 <br/>
 
 Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
 
@@ -51,15 +51,15 @@
 tw = twAuto.twAuto(
   username="Your Twitter Username",
   email="Your Twitter E-Mail",
   password="Your Twitter Password",
   chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
                                        #if you use the manual option, you need to provide the driver path in driverPath parameter.
   driverPath="your drivers path", #use only if you are using the chromeDriverMode in manual mode 
-  pathType="testId" or "xPath", #It is xPath by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
+  pathType="testId" or "xPath", #It is testId by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
   headless=True/False, #Headless is true by default.
   debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
                         #It is not reliable right now but you can give it a try if you want to.
 )
 
 ```
```

### Comparing `twAuto-0.3.5/README.md` & `twAuto-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# twAuto - Twitter Automation Tool v0.3.4 🦆
+# twAuto - Twitter Automation Tool v0.3.6 🦆
 
 twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
 
 <br/>
 
 Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
 
@@ -40,15 +40,15 @@
 tw = twAuto.twAuto(
   username="Your Twitter Username",
   email="Your Twitter E-Mail",
   password="Your Twitter Password",
   chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
                                        #if you use the manual option, you need to provide the driver path in driverPath parameter.
   driverPath="your drivers path", #use only if you are using the chromeDriverMode in manual mode 
-  pathType="testId" or "xPath", #It is xPath by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
+  pathType="testId" or "xPath", #It is testId by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
   headless=True/False, #Headless is true by default.
   debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
                         #It is not reliable right now but you can give it a try if you want to.
 )
 
 ```
```

### Comparing `twAuto-0.3.5/setup.py` & `twAuto-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='twAuto',
-    version='0.3.5',
+    version='0.3.6',
     packages=find_packages(exclude=['tests*']),
     license='MIT',
     description='TwAuto is a library for testing your code on pre-Twitter API application stage.',
     long_description=open('README.md',  encoding="utf8").read(),
     long_description_content_type='text/markdown',
     install_requires=['selenium', 'bs4', 'webdriver-manager'],
     url='https://github.com/EKOzkan/twAuto',
```

### Comparing `twAuto-0.3.5/twAuto/twauto.py` & `twAuto-0.3.6/twAuto/twauto.py`

 * *Files 23% similar despite different names*

```diff
@@ -150,34 +150,18 @@
             sleep(3)
             self.close()
 
     # tweet text
     def tweet(self, imgpath=None, text=""):
         # load tweeting page
         twAuto.driver.get("https://twitter.com/home")
-        twAuto.driver.get('https://twitter.com/compose/tweet')
-
-
+        urlWithText = "https://twitter.com/compose/tweet?text="+text
+        twAuto.driver.get(urlWithText)
         if self.pathType=="xPath":
             try:
-                # try finding tweet inbox
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div[2]/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")))
-                except TimeoutException:
-                    print('Couldnt tweet.')
-
-                # modify tweet text
-                full_text = text
-
-                input_field = twAuto.driver.find_element(
-                    'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div[2]/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")
-                input_field.send_keys(full_text)
-
                 try:
                     wait = WebDriverWait(twAuto.driver, 120)
                     wait.until(EC.presence_of_element_located(
                         (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[4]")))
                 except TimeoutException:
                     print('Couldnt tweet.')
                     
@@ -224,29 +208,14 @@
             except Exception as e:
                 if self.debugMode:
                     print("twAuto Error: ", e)
                 return False
 
         if self.pathType == "testId":
             try:
-                # try finding tweet inbox
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, '//div[@data-testid="tweetTextarea_0"]')))
-                except TimeoutException:
-                    print('Couldnt tweet.')
-                
-                # modify tweet text
-                full_text = text
-                
-                input_field = twAuto.driver.find_element(
-                    'xpath', '//div[@data-testid="tweetTextarea_0"]')
-                input_field.send_keys(full_text)
-                
                 try:
                     wait = WebDriverWait(twAuto.driver, 120)
                     wait.until(EC.presence_of_element_located((By.XPATH, '//div[@data-testid="tweetButton"]')))
                     
                 except TimeoutException:
                     print('Couldnt tweet.' )
                 
@@ -298,14 +267,15 @@
                 if self.debugMode:
                     print("twAuto Error: ", e)
                 return False
 
         
     # quote tweet. this function uses the "adding the quoted tweets url to end of the text method" but maybe i will add the another version of this function that uses the quote tweet function later
     def quoteTweet(self, url="", imgpath="", text=""):
+        
         try:
             twAuto.driver.get("https://twitter.com/home")
             fixUrl=url+"?s=20"
             twAuto.driver.get(fixUrl)
             container_element = self.findTweet(url=url)
             
             if self.pathType == "testId":
@@ -456,107 +426,54 @@
             if self.debugMode:
                 print("twAuto Error: ", e)
             return False
     # reply to a tweet
     def reply(self, url="", imgpath="", text=""):
         try:
             twAuto.driver.get("https://twitter.com/home")
-            fixUrl=url+"?s=20"
-            twAuto.driver.get(fixUrl)
-            container_element = self.findTweet(url=url)
-            """ if self.pathType == "xPath":
-                try:
-                    try:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[8]/div/div[1]/div')
-                    except Exception as e:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[7]/div/div[1]/div')
-                        if self.debugMode : print("twAuto Error: ", e)
-                    body_element.click()
-                    try:
-                        wait = WebDriverWait(twAuto.driver, 5)
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")))
-                        twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div").send_keys(text+" ")
-                        if imgpath != "":
-                            element = twAuto.driver.find_element(
-                                By.XPATH, "//input[@type='file']")
-
-                            twAuto.driver.execute_script(
-                                "arguments[0].style.display = 'block';", element)
-
-                            element.send_keys(imgpath)
-                        tweetReplyButton = twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[2]")
-                        tweetReplyButton.click()
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a")))
-                        replyURL = twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a").get_attribute("href")
-                        return replyURL
-                    except Exception as e:
-                        if self.debugMode : print("twAuto Error: ", e)
-                        return False
-                except Exception as e:
-                    if self.debugMode : print("twAuto Error: ", e)
-                    return False """
+            tweet_id = self.extract_tweet_id(url)
+            urlWithText = "https://twitter.com/intent/tweet?in_reply_to="+tweet_id+"&text="+text
+            twAuto.driver.get(urlWithText)
             if self.pathType == "testId" or self.pathType == "xPath":
                 #data-testid="tweetTextarea_0_label"]tweetButton
                 try:
                     try:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[8]/div/div[1]/div')
-                    except Exception as e:
-                        body_element = container_element.find_element(
-                            By.XPATH, '//div[@data-testid="tweetTextarea_0RichTextInputContainer"]')
-                    body_element.click()
-                    try:
-                        #tweetTextarea_0
-                        wait = WebDriverWait(twAuto.driver, 5)
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, '//div[@data-testid="tweetTextarea_0"]')))
-                        
-                        input_field = twAuto.driver.find_element(
-                            'xpath', '//div[@data-testid="tweetTextarea_0"]')
-                        if text=="":
-                            input_field.send_keys(text)
-                        else:
-                            input_field.send_keys(text)
-                            
-                        #imgbutton = container_element.find_element(
-                        #    By.XPATH, './/div/div/div[2]/div/div[2]/div[2]/div/div/div/div[2]/div[3]/div/div/div[1]/div[1]')
-                        
                         if imgpath != "":
                             element = twAuto.driver.find_element(
                                 By.XPATH, "//input[@type='file']")
 
                             twAuto.driver.execute_script(
                                 "arguments[0].style.display = 'block';", element)
 
                             element.send_keys(imgpath)
-                        time.sleep(1)
+                        
                         #check if there is a mask
                         try:
                             maskClose = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="app-bar-close"]')
                             twAuto.driver.execute_script("arguments[0].click()", maskClose)
                         except:
                             pass
                         #find tweet button
+                        time.sleep(1)
+                        wait = WebDriverWait(twAuto.driver, 120)
+                      
                         try:
+                            wait.until(EC.presence_of_element_located(
+                                (By.XPATH, '//div[@data-testid="tweetButton"]')))
                             tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
                             #click tweet button
                             twAuto.driver.execute_script("arguments[0].click()", tweetButton)
-                        except:
-                            tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButtonInline"]')
+                        except Exception as e:
+                            wait.until(EC.presence_of_element_located(
+                                (By.XPATH, '//div[@data-testid="tweetButton"]')))
+                            
+                            tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
                             #click tweet button
                             twAuto.driver.execute_script("arguments[0].click()", tweetButton)
-
-                    
+                        wait = WebDriverWait(twAuto.driver, 120)
                         wait.until(EC.presence_of_element_located(
                             (By.XPATH, '//div[@data-testid="toast"]')))
                         replyURLButton = twAuto.driver.find_element(
                             By.XPATH, '//div[@data-testid="toast"]')
                         replyURLElement = replyURLButton.find_element(By.XPATH, './/div[2]/a[1]').get_attribute("href")
                         return replyURLElement
                     except Exception as e:
@@ -631,7 +548,15 @@
             'xpath', "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div[2]/div[1]").click()
         os.remove("cookies.pkl")
         print("Succesfully logged out")
         
     # closes selenium driver
     def close(self):
         twAuto.driver.quit()
+    def extract_tweet_id(self, url):
+        url = url.replace("https://", "")  # Remove "https://"
+        url = url.replace("http://", "")  # Remove "http://"
+        print("url:", url)
+        url_parts = url.split("/")
+        if "twitter.com" in url_parts:
+            url_parts.remove("twitter.com")
+        return url_parts[2] if len(url_parts) >= 3 else None
```

### Comparing `twAuto-0.3.5/twAuto.egg-info/PKG-INFO` & `twAuto-0.3.6/twAuto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: twAuto
-Version: 0.3.5
+Version: 0.3.6
 Summary: TwAuto is a library for testing your code on pre-Twitter API application stage.
 Home-page: https://github.com/EKOzkan/twAuto
 Author: Ekin Kagan Ozkan
 Author-email: ekinkagan@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE.MD
 
-# twAuto - Twitter Automation Tool v0.3.4 🦆
+# twAuto - Twitter Automation Tool v0.3.6 🦆
 
 twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
 
 <br/>
 
 Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
 
@@ -51,15 +51,15 @@
 tw = twAuto.twAuto(
   username="Your Twitter Username",
   email="Your Twitter E-Mail",
   password="Your Twitter Password",
   chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
                                        #if you use the manual option, you need to provide the driver path in driverPath parameter.
   driverPath="your drivers path", #use only if you are using the chromeDriverMode in manual mode 
-  pathType="testId" or "xPath", #It is xPath by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
+  pathType="testId" or "xPath", #It is testId by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
   headless=True/False, #Headless is true by default.
   debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
                         #It is not reliable right now but you can give it a try if you want to.
 )
 
 ```
```

