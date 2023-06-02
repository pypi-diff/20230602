# Comparing `tmp/SeleCrawler-0.0.2.tar.gz` & `tmp/SeleCrawler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeleCrawler-0.0.2.tar", last modified: Fri Mar 24 11:50:43 2023, max compression
+gzip compressed data, was "SeleCrawler-1.0.1.tar", last modified: Fri Jun  2 19:23:56 2023, max compression
```

## Comparing `SeleCrawler-0.0.2.tar` & `SeleCrawler-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 11:50:42.952289 SeleCrawler-0.0.2/
--rw-rw-rw-   0        0        0      271 2023-03-24 11:50:42.936663 SeleCrawler-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-24 11:50:41.947081 SeleCrawler-0.0.2/SeleCrawler/
--rw-rw-rw-   0        0        0       37 2023-03-24 07:37:15.000000 SeleCrawler-0.0.2/SeleCrawler/__init__.py
--rw-rw-rw-   0        0        0     9590 2023-03-24 11:11:49.000000 SeleCrawler-0.0.2/SeleCrawler/selenium_controller.py
-drwxrwxrwx   0        0        0        0 2023-03-24 11:50:42.936663 SeleCrawler-0.0.2/SeleCrawler.egg-info/
--rw-rw-rw-   0        0        0      271 2023-03-24 11:50:38.000000 SeleCrawler-0.0.2/SeleCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-03-24 11:50:38.000000 SeleCrawler-0.0.2/SeleCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 11:50:38.000000 SeleCrawler-0.0.2/SeleCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-03-24 11:50:38.000000 SeleCrawler-0.0.2/SeleCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-24 11:50:38.000000 SeleCrawler-0.0.2/SeleCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 11:50:42.952289 SeleCrawler-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-03-24 11:50:15.000000 SeleCrawler-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:23:56.481648 SeleCrawler-1.0.1/
+-rw-rw-rw-   0        0        0      393 2023-06-02 19:23:56.481648 SeleCrawler-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 19:23:56.403524 SeleCrawler-1.0.1/SeleCrawler.egg-info/
+-rw-rw-rw-   0        0        0      393 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-06-02 19:23:55.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 19:23:56.466028 SeleCrawler-1.0.1/selecrawler/
+-rw-rw-rw-   0        0        0       37 2023-03-24 07:37:15.000000 SeleCrawler-1.0.1/selecrawler/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-06-02 19:22:35.000000 SeleCrawler-1.0.1/selecrawler/browsing.py
+-rw-rw-rw-   0        0        0     7871 2023-06-02 19:12:37.000000 SeleCrawler-1.0.1/selecrawler/controller.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:23:56.512895 SeleCrawler-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      680 2023-06-02 18:19:24.000000 SeleCrawler-1.0.1/setup.py
```

### Comparing `SeleCrawler-0.0.2/SeleCrawler/selenium_controller.py` & `SeleCrawler-1.0.1/selecrawler/controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,61 +28,28 @@
 
 def log_name():
     current_debug_time = datetime.now()
     log_str = str(current_debug_time.hour) + '.' + str(current_debug_time.minute) + '.' + str(current_debug_time.second) + ' ' + str(current_debug_time.day) + '-' + str(current_debug_time.month)  + '-' + str(current_debug_time.year)
     logs_name = 'logs_' + log_str + '.log'
     return logs_name
 
-def debg(e):
+def filelog(e):
     logs_name = log_name()
     with open(logs_name, 'a+') as file:
         contents = file.write(str(e))
         contents = file.write('\n')
     pass
 
 
 def logg(msg, color):
     # debg('='*50)
-    debg(msg)
+    # debg(msg)
     # debg('='*50)
 
 
-def human_delay():
-    global driver
-    mean_delay = random.choice(range(2,7))
-    delay = random.normalvariate(mean_delay, mean_delay/4)
-    time.sleep(delay)
-
-
-def human_typing(text, typing_area):
-    global driver
-    for char in text:
-        start = 0.1 
-        stop = 0.3
-        step = 0.2
-        precision = 0.1
-        f = 1 / precision
-        n = random.randrange(1, 3, 2) / f
-        typo_chance = random.choice(range(0, 99))
-        if typo_chance >= random.choice(range(80,95)):
-            typo_keys = random.choice(range(1, 4))
-            letters = list(string.ascii_lowercase)
-            for _ in range(typo_keys):
-                letter = random.choice(letters)
-                typing_area.send_keys(letter)
-                time.sleep(n)
-
-            for removal in range(typo_keys):
-                typing_area.send_keys(Keys.BACKSPACE)
-                time.sleep(n)
-
-        time.sleep(n)
-        typing_area.send_keys(char)
-
-
 def proxies_plugin(username, proxypass, endpoint, port):
     manifest_json = """
     {
         "version": "1.0.0",
         "manifest_version": 2,
         "name": "Proxies",
         "permissions": [
@@ -125,41 +92,39 @@
     chrome.webRequest.onAuthRequired.addListener(
                 callbackFn,
                 {urls: ["<all_urls>"]},
                 ['blocking']
     );
     """ % (endpoint, port, username, proxypass)
 
-    extension_id = ''.join(random.choices(string.ascii_letters, k=8))
-    extension = 'proxies_extension_' + extension_id + '.zip'
+    # extension_id = ''.join(random.choices(string.ascii_letters, k=8))
+    extension = 'proxies_extension.zip' # + extension_id + '.zip'
     
     with zipfile.ZipFile(extension, 'w') as zp:
         zp.writestr("manifest.json", manifest_json)
         zp.writestr("background.js", background_js)
 
     return extension
 
-def proxy:
-    global PROXY
-    PROXY = ''
 
-def configure_chromedriver(use_proxy=False, user_agent=None, proxy=PROXY, headless_mode=False, change_resolutions=False, undetected_chrome=False, to_detach=False):
+def configure_chromedriver(proxy=None, user_agent=None, headless_mode=False, change_resolutions=False, undetected_chrome=False, detach=False):
     global pluginfile
+    proxy_address = proxy
     if undetected_chrome == False:
         chrome_options = webdriver.ChromeOptions()
         
         if change_resolutions == True:
             resolutions = [[1366, 768], [1920, 1080], [1536, 864], [1440, 900], [1280, 720], [768, 1024], [1280, 800]]
             resolution = random.choice(resolutions)
                 
             width = resolution[0]
             height = resolution[1]
-            debg('Chosen Dimensions Are:')
-            debg('Width: ' + str(width))
-            debg('Height: ' + str(height))
+            # debg('Chosen Dimensions Are:')
+            # debg('Width: ' + str(width))
+            # debg('Height: ' + str(height))
             window_size_param = 'window-size=' + str(width) + ', ' + str(height)
             chrome_options.add_argument(str(window_size_param))
         else:
             pass
 
         if headless_mode == True:
             chrome_options.add_argument("--headless=new")
@@ -179,36 +144,37 @@
         # Exclude the collection of enable-automation switches 
         chrome_options.add_experimental_option("excludeSwitches", ["enable-automation"]) 
         chrome_options.add_experimental_option("excludeSwitches", ["enable-logging"]) 
         
         # Turn-off userAutomationExtension 
         chrome_options.add_experimental_option("useAutomationExtension", False)
 
-        if use_proxy == True:
-            proxy_full = PROXY.strip('\n')
+        if proxy != None:
+            proxy_full = proxy_address.strip('\n')
             proxy_full = proxy_full.split(':')
-            debg(proxy_full)
+            # debg(proxy_full)
             if len(proxy_full) <= 2:
                 PROXY_HOST = proxy_full[0]
                 PROXY_PORT = proxy_full[1]
                 no_authentication = True
             elif len(proxy_full) == 4:
                 PROXY_HOST = proxy_full[0]
                 PROXY_PORT = proxy_full[1]
                 PROXY_USER = proxy_full[2]
                 PROXY_PASS = proxy_full[3]
                 no_authentication = False
         else:
-            debg('Not Using Proxy')
+            # debg('Not Using Proxy')
+            pass
         
 
-        if use_proxy and no_authentication == True:
-            PROXY = str(PROXY_HOST.strip('\n')) + ':' + str(PROXY_PORT.strip('\n'))
-            chrome_options.add_argument('--proxy-server=%s' % PROXY)
-        elif use_proxy and no_authentication == False:
+        if proxy and no_authentication == True:
+            unauthenticated_proxy = str(PROXY_HOST.strip('\n')) + ':' + str(PROXY_PORT.strip('\n'))
+            chrome_options.add_argument('--proxy-server=%s' % unauthenticated_proxy)
+        elif proxy and no_authentication == False:
             pluginfile = proxies_plugin(PROXY_USER, PROXY_PASS, PROXY_HOST, PROXY_PORT)
             chrome_options.add_extension(pluginfile)
             
         if user_agent:
             user_agent = user_agent.strip('\n')
             chrome_options.add_argument('--user-agent=%s' % user_agent)
 
@@ -221,51 +187,34 @@
         
         try:
             # Open the file with the list of User Agents
             driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)
             # Changing the property of the navigator value for webdriver to undefined 
         except Exception as e:            
             # Pick emy
-            debg('Chrome Failed Loading With Error:')
-            debg(e)
+            # debg('Chrome Failed Loading With Error:')
+            # debg(e)
             logg('Error Loading Chrome.', '#f9600f')
 
             # Open the file with the list of User Agents
             # driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)
         
     else:
         chrome_options = uc.ChromeOptions()
         
         try:
             # Open the file with the list of User Agents
             if headless_mode == True:
-                debg('Using Headless Undetected Chromedriver!')
+                # debg('Using Headless Undetected Chromedriver!')
                 driver = uc.Chrome(chrome_options=chrome_options, headless=True)
             else:
-                debg('Using Headfull Undetected Chromedriver!')
+                # debg('Using Headfull Undetected Chromedriver!')
                 driver = uc.Chrome(chrome_options=chrome_options)
             # Changing the property of the navigator value for webdriver to undefined 
         except Exception as e:            
             # Pick emy
-            debg('Chrome Failed Loading With Error:')
-            debg(e)
+            # debg('Chrome Failed Loading With Error:')
+            # debg(e)
             logg('Error Loading Chrome.', '#f9600f')
             
         
     return driver
-
-
-def wait_for_element(driver, time, by_attribute, attribute_value):
-    """
-    Wait for an element to be present in the DOM using the specified WebDriver By attribute and attribute value.
-    
-    Args:
-        driver: a Selenium WebDriver object
-        time (int): the time in seconds to wait for the element to be present
-        by_attribute (str): the By attribute to search for the element by (e.g. By.ID, By.XPATH)
-        attribute_value (str): the value of the attribute to search for
-        
-    Returns:
-        A WebDriverWait object that can be used in a Selenium WebDriver statement
-    """
-    by_method = getattr(By, by_attribute)
-    return WebDriverWait(driver, time).until(EC.presence_of_element_located((by_method, attribute_value)))
```

### Comparing `SeleCrawler-0.0.2/setup.py` & `SeleCrawler-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 
 setup_args = dict(
     name='SeleCrawler',
-    version='0.0.2',
+    version='1.0.1',
     description='Collection Of Tools To Ease Selenium Operation',
     packages=find_packages(),
     author='Gee Tech Labs',
     author_email='geetechlabs@gmail.com',
-    keywords=['SeleCrawler', 'Sele Crawler', 'Selenium Crawler', 'Selenium', 'Crawler', 'Browser', 'BrowserAutomation']
+    keywords=['SeleCrawler', 'Sele Crawler', 'Selenium Crawler', 'Selenium', 'Crawler', 'Browser', 'BrowserAutomation', 'Automation', 'Webdriver', 'web', 'driver', 'web driver']
 )
 
 install_requires = [
     'webdriver-manager==3.8.5',
     'selenium==4.8.2',
     'undetected-chromedriver==3.4.6'
 ]
```

