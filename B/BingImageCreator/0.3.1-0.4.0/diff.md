# Comparing `tmp/BingImageCreator-0.3.1.tar.gz` & `tmp/BingImageCreator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.3.1.tar", last modified: Wed May 31 09:08:00 2023, max compression
+gzip compressed data, was "BingImageCreator-0.4.0.tar", last modified: Fri Jun  2 16:02:18 2023, max compression
```

## Comparing `BingImageCreator-0.3.1.tar` & `BingImageCreator-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.098942 BingImageCreator-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16168 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/test/test_example.py
```

### Comparing `BingImageCreator-0.3.1/LICENSE` & `BingImageCreator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.3.1/PKG-INFO` & `BingImageCreator-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.3.1
+Version: 0.4.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.3.1/README.md` & `BingImageCreator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.3.1/setup.py` & `BingImageCreator-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.3.1",
+    version="0.4.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
     project_urls={
         "Bug Report": "https://github.com/acheong08/BingImageCreator/issues/new",
     },
     install_requires=[
-        "aiohttp",
+        "httpx",
         "regex",
         "requests",
     ],
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["BingImageCreator"],
     classifiers=[
```

### Comparing `BingImageCreator-0.3.1/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.4.0/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.3.1
+Version: 0.4.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.3.1/src/BingImageCreator.py` & `BingImageCreator-0.4.0/src/BingImageCreator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import time
 from functools import partial
 from typing import Dict
 from typing import List
 from typing import Union
 
-import aiohttp
+import httpx
 import pkg_resources
 import regex
 import requests
 
 if os.environ.get("BING_URL") == None:
     BING_URL = "https://www.bing.com"
 else:
@@ -37,17 +37,15 @@
 
 # Error messages
 error_timeout = "Your request has timed out."
 error_redirect = "Redirect failed"
 error_blocked_prompt = (
     "Your prompt has been blocked by Bing. Try to change any bad words and try again."
 )
-error_being_reviewed_prompt = (
-    "Your prompt is being reviewed by Bing. Try to change any sensitive words and try again."
-)
+error_being_reviewed_prompt = "Your prompt is being reviewed by Bing. Try to change any sensitive words and try again."
 error_noresults = "Could not get results"
 error_unsupported_lang = "\nthis language is currently not supported by bing"
 error_bad_images = "Bad images"
 error_no_images = "No images"
 #
 sending_message = "Sending request..."
 wait_message = "Waiting for results..."
@@ -97,15 +95,15 @@
             self.debug(sending_message)
         url_encoded_prompt = requests.utils.quote(prompt)
         payload = f"q={url_encoded_prompt}&qs=ds"
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
         response = self.session.post(
             url,
-            allow_redirects=False,
+            follow_redirects=False,
             data=payload,
             timeout=200,
         )
         # check for content waring message
         if "this prompt is being reviewed" in response.text.lower():
             if self.debug_file:
                 self.debug(f"ERROR: {error_being_reviewed_prompt}")
@@ -124,15 +122,15 @@
         ):
             if self.debug_file:
                 self.debug(f"ERROR: {error_unsupported_lang}")
             raise Exception(error_unsupported_lang)
         if response.status_code != 302:
             # if rt4 fails, try rt3
             url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
-            response3 = self.session.post(url, allow_redirects=False, timeout=200)
+            response3 = self.session.post(url, follow_redirects=False, timeout=200)
             if response3.status_code != 302:
                 if self.debug_file:
                     self.debug(f"ERROR: {error_redirect}")
                 print(f"ERROR: {response3.text}")
                 raise Exception(error_redirect)
             response = response3
         # Get redirect URL
@@ -217,102 +215,97 @@
             ) from url_exception
 
 
 class ImageGenAsync:
     """
     Image generation by Microsoft Bing
     Parameters:
-        auth_cookie: str
     """
 
     def __init__(
         self,
         auth_cookie: str = None,
         debug_file: Union[str, None] = None,
         quiet: bool = False,
         all_cookies: List[Dict] = None,
     ) -> None:
         if auth_cookie is None and not all_cookies:
             raise Exception("No auth cookie provided")
-        self.session = aiohttp.ClientSession(
+        self.session = httpx.AsyncClient(
             headers=HEADERS,
-            cookies={"_U": auth_cookie},
             trust_env=True,
         )
+        if auth_cookie:
+            self.session.cookies.update({"_U": auth_cookie})
         if all_cookies:
             for cookie in all_cookies:
-                self.session.cookie_jar.update_cookies(
+                self.session.cookies.update(
                     {cookie["name"]: cookie["value"]},
                 )
-        if auth_cookie:
-            self.session.cookie_jar.update_cookies({"_U": auth_cookie})
         self.quiet = quiet
         self.debug_file = debug_file
         if self.debug_file:
             self.debug = partial(debug, self.debug_file)
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *excinfo) -> None:
-        await self.session.close()
+        await self.session.aclose()
 
     async def get_images(self, prompt: str) -> list:
         """
         Fetches image links from Bing
         Parameters:
             prompt: str
         """
         if not self.quiet:
             print("Sending request...")
         url_encoded_prompt = requests.utils.quote(prompt)
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
-        url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
+        url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
         payload = f"q={url_encoded_prompt}&qs=ds"
-        async with self.session.post(
+        response = await self.session.post(
             url,
-            allow_redirects=False,
+            follow_redirects=False,
             data=payload,
-        ) as response:
-            content = await response.text()
-            if "this prompt has been blocked" in content.lower():
-                raise Exception(
-                    "Your prompt has been blocked by Bing. Try to change any bad words and try again.",
-                )
-            if response.status != 302:
-                # if rt4 fails, try rt3
-                url = (
-                    f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
-                )
-                async with self.session.post(
-                    url,
-                    allow_redirects=False,
-                    timeout=200,
-                ) as response3:
-                    if response3.status != 302:
-                        print(f"ERROR: {await response3.text()}")
-                        raise Exception("Redirect failed")
-                    response = response3
+        )
+        content = response.text
+        if "this prompt has been blocked" in content.lower():
+            raise Exception(
+                "Your prompt has been blocked by Bing. Try to change any bad words and try again.",
+            )
+        if response.status_code != 302:
+            # if rt4 fails, try rt3
+            url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
+            response = await self.session.post(
+                url,
+                follow_redirects=False,
+                timeout=200,
+            )
+            if response.status_code != 302:
+                print(f"ERROR: {response.text}")
+                raise Exception("Redirect failed")
         # Get redirect URL
         redirect_url = response.headers["Location"].replace("&nfy=1", "")
         request_id = redirect_url.split("id=")[-1]
         await self.session.get(f"{BING_URL}{redirect_url}")
         # https://www.bing.com/images/create/async/results/{ID}?q={PROMPT}
         polling_url = f"{BING_URL}/images/create/async/results/{request_id}?q={url_encoded_prompt}"
         # Poll for results
         if not self.quiet:
             print("Waiting for results...")
         while True:
             if not self.quiet:
                 print(".", end="", flush=True)
             # By default, timeout is 300s, change as needed
             response = await self.session.get(polling_url)
-            if response.status != 200:
+            if response.status_code != 200:
                 raise Exception("Could not get results")
-            content = await response.text()
+            content = response.text
             if content and content.find("errorMessage") == -1:
                 break
 
             await asyncio.sleep(1)
             continue
         # Use regex to search for src=""
         image_links = regex.findall(r'src="([^"]+)"', content)
@@ -353,23 +346,24 @@
             fn = f"{file_name}_" if file_name else ""
             jpeg_index = 0
             for link in links:
                 while os.path.exists(
                     os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
                 ):
                     jpeg_index += 1
-                async with self.session.get(link, raise_for_status=True) as response:
-                    # save response to file
-                    with open(
-                        os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
-                        "wb",
-                    ) as output_file:
-                        async for chunk in response.content.iter_chunked(8192):
-                            output_file.write(chunk)
-        except aiohttp.client_exceptions.InvalidURL as url_exception:
+                response = await self.session.get(link)
+                if response.status_code != 200:
+                    raise Exception("Could not download image")
+                # save response to file
+                with open(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
+                    "wb",
+                ) as output_file:
+                    output_file.write(response.content)
+        except httpx.InvalidURL as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt.",
             ) from url_exception
 
 
 async def async_image_gen(
     prompt: str,
```

### Comparing `BingImageCreator-0.3.1/test/test_example.py` & `BingImageCreator-0.4.0/test/test_example.py`

 * *Files identical despite different names*

