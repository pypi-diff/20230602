# Comparing `tmp/google_news_feed-1.0.0.tar.gz` & `tmp/google_news_feed-1.1.0.tar.gz`

## Comparing `google_news_feed-1.0.0.tar` & `google_news_feed-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/requirements.txt
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/.github/workflows/pip-publish.yml
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/src/google_news_feed/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/tests/test_GoogleNewsFeed.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/LICENSE
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/README.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 google_news_feed-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/.github/workflows/pip-publish.yml
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/src/google_news_feed/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/tests/test_GoogleNewsFeed.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 google_news_feed-1.1.0/PKG-INFO
```

### Comparing `google_news_feed-1.0.0/.github/workflows/pip-publish.yml` & `google_news_feed-1.1.0/.github/workflows/pip-publish.yml`

 * *Files identical despite different names*

### Comparing `google_news_feed-1.0.0/.github/workflows/python-package.yml` & `google_news_feed-1.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `google_news_feed-1.0.0/src/google_news_feed/__init__.py` & `google_news_feed-1.1.0/src/google_news_feed/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 import urllib.parse
-import httpx
 from lxml import etree
 from lxml.etree import _Element
 from datetime import datetime,date
 from dateparser import parse
 import asyncio
 import logging
+from typing import Optional
+from dataclasses import dataclass
+import requests
+from bs4 import BeautifulSoup
+import aiohttp
 
 
-GOOGLE_INTERNAL_URL = "https://news.google.com/__i/rss"    
+GOOGLE_INTERNAL_URL = set(["https://news.google.com/__i/rss","https://news.google.com/rss"])   
 BASE_URL = 'https://news.google.com/rss'
 PARSER = etree.HTMLParser(recover=True)
-MOVED_STATUS_CODE = 301
+
+HEADERS = {
+    'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36'
+}
+
+COOKIES = {
+    'CONSENT': 'YES+cb.20220419-08-p0.cs+FX+111'
+}
 
 KNOWN_TOPICS={
     "BUSINESS":"CAAqKggKIiRDQkFTRlFvSUwyMHZNRGx6TVdZU0JXVnVMVlZUR2dKVlV5Z0FQAQ",
     "NATION":"CAAqKggKIiRDQkFTRlFvSUwyMHZNRGx6TVdZU0JXVnVMVlZUR2dKVlV5Z0FQAQ",
     "WORLD":"CAAqJggKIiBDQkFTRWdvSkwyMHZNRGxqTjNjd0VnVmxiaTFWVXlnQVAB",
     "TECHNOLOGY":"CAAqKggKIiRDQkFTRlFvSUwyMHZNRGx1YlY4U0JXVnVMVlZUR2dKVlV5Z0FQAQ",
     "ENTERTAINMENT":"CAAqKggKIiRDQkFTRlFvSUwyMHZNREpxYW5RU0JXVnVMVlZUR2dKVlV5Z0FQAQ",
     "SCIENCE":"CAAqKggKIiRDQkFTRlFvSUwyMHZNREpxYW5RU0JXVnVMVlZUR2dKVlV5Z0FQAQ",
     "SPORTS":"CAAqKggKIiRDQkFTRlFvSUwyMHZNRFp1ZEdvU0JXVnVMVlZUR2dKVlV5Z0FQAQ",
     "HEALTH":"CAAqJQgKIh9DQkFTRVFvSUwyMHZNR3QwTlRFU0JXVnVMVlZUS0FBUAE"
 }
     
+@dataclass
 class NewsItem(object):
-    title:str
-    link:str
-    pubDate:datetime
-    description:str
-    source:str
-    def __init__(self,title:str=None,link:str=None,pubDate:datetime=None,description:str=None,source:str=None) -> None:
-        self.title = title
-        self.link = link
-        self.pubDate = pubDate
-        self.description = description
-        self.source = source
-        
+    title:Optional[str]=None
+    link:Optional[str]=None
+    pubDate:Optional[datetime]=None
+    description:Optional[str]=None
+    source:Optional[str]=None
+
     def __repr__(self) -> str:
         return f'{self.title}'
     
     @property
-    def is_google_internal_link(self)->bool:
-        return self.link.startswith(GOOGLE_INTERNAL_URL)
+    def is_internal_google_link(self)->bool:
+        for internal_link in GOOGLE_INTERNAL_URL:
+            if self.link.startswith(internal_link):
+                return True
+        return False
     
 class GoogleNewsFeed:
-    def __init__(self,language:str='en',country:str='US',client:httpx.Client=None,resolve_internal_links:bool=True,run_async:bool=True)->None:
+    def __init__(self,language:str='en',country:str='US',client:Optional[requests.Session]=None,resolve_internal_links:bool=True,run_async:bool=True)->None:
         self.language = language.lower()
         self.country = country.upper()
-        self.client = client if client else httpx.Client()
+        if client:
+            self.client = client
+        else:
+            self.client = requests.Session()
+            self.client.headers.update(HEADERS)
+            self.client.cookies.update(COOKIES)
+
         self.resolve_internal_links = resolve_internal_links
         self.run_async = run_async
         
         
     @staticmethod
     def _build_ceid(country:str,language:str)->str:
         return f'hl={language}-{country}&gl={country}&ceid={country}:{language}'
@@ -106,38 +121,45 @@
     def _parse_feed(content:str)->list[NewsItem]:
         root = etree.fromstring(content,parser=PARSER)
         
         parsed_items = []
         for item in root.iter('item'):
             try:
                 parsed_items.append(GoogleNewsFeed._parse_item(item))
-            except:
-                logging.debug(f"Failed to parse item: {item}")
+            except Exception as e:
+                logging.debug(f"Failed to parse item: {item}! Exception: {e}")
             
         return parsed_items
         
     async def _async_resolve_internal_links(self,items:list[NewsItem])->list[NewsItem]:
-        async with httpx.AsyncClient() as client:
+        async with aiohttp.ClientSession() as session:
+            session.headers.update(HEADERS)
+            session.cookie_jar.update_cookies(COOKIES)
             for item in items:
                 try:
-                    if item.is_google_internal_link:
-                        response = await client.get(item.link)
-                        if response.status_code == MOVED_STATUS_CODE:
-                            item.link = response.headers['Location']
+                    if item.is_internal_google_link:
+                        async with session.get(item.link) as response:
+                            content = await response.text()
+                            if content:
+                                soup = BeautifulSoup(content, 'html.parser')
+                                item.link = soup.a['href']
+                                del soup
                 except:
                     logging.debug(f"Failed to resolve internal link: {item.link}")
         return items
     
     def _resolve_internal_links(self,items:list[NewsItem])->list[NewsItem]:
         for item in items:
             try:
-                if item.is_google_internal_link:
+                if item.is_internal_google_link:
                     response = self.client.get(item.link)
-                    if response.status_code == MOVED_STATUS_CODE:
-                        item.link = response.headers['Location']
+                    if response.text:
+                        soup = BeautifulSoup(response.text, 'html.parser')
+                        item.link = soup.a['href']
+                        del soup
             except:
                     logging.debug(f"Failed to resolve internal link: {item.link}")
         return items
         
     def _get_feed(self,url:str)->list[NewsItem]:
         result = self.client.get(url)
         if result.status_code == 200:
```

### Comparing `google_news_feed-1.0.0/tests/test_GoogleNewsFeed.py` & `google_news_feed-1.1.0/tests/test_GoogleNewsFeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,11 +64,17 @@
     
 def test_top_headlines_should_return_news_items():
     news_items = GoogleNewsFeed(resolve_internal_links=False).top_headlines()
     assert len(news_items) > 0
     assert isinstance(news_items[0], NewsItem)
     
 def test_internal_link_are_resolved():
+    news_items = GoogleNewsFeed(run_async=False).top_headlines()
+    assert len(news_items) > 0
+    for news_item in news_items:
+        assert not news_item.is_internal_google_link
+
+def test_internal_link_are_resolved_async():
     news_items = GoogleNewsFeed().top_headlines()
     assert len(news_items) > 0
     for news_item in news_items:
-        assert not news_item.is_google_internal_link
+        assert not news_item.is_internal_google_link
```

### Comparing `google_news_feed-1.0.0/.gitignore` & `google_news_feed-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `google_news_feed-1.0.0/LICENSE` & `google_news_feed-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_news_feed-1.0.0/README.md` & `google_news_feed-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Google-News-Feed
 A simple python library to consume the google news rss feed.
 
-Inspired by [pygooglenews](https://github.com/kotartemiy/pygooglenews) and implemented using [httpx](https://pypi.org/project/httpx/) and [lxml](https://pypi.org/project/lxml/).
+Inspired by [pygooglenews](https://github.com/kotartemiy/pygooglenews) and implemented using [aiohttp](https://pypi.org/project/aiohttp/) and [lxml](https://pypi.org/project/lxml/).
 
 
 ## Installation
 Via pip: <code>pip install google-news-feed</code>
 
 ## How to use
 ```python
```

### Comparing `google_news_feed-1.0.0/pyproject.toml` & `google_news_feed-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "google_news_feed"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Lukas Kreussel"},
 ]
 description = "A simple python library to consume the google news rss feed"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies=["httpx>=0.23.0","dateparser>=1.1.1","lxml>=4.9.0"]
+dependencies=["aiohttp>=3.8.4","dateparser>=1.1.1","lxml>=4.9.0","requests>=2.31.0","beautifulsoup4>=4.12.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/LLukas22/Google-News-RSS"
 "Bug Tracker" = "https://github.com/LLukas22/Google-News-RSS/issues"
```

### Comparing `google_news_feed-1.0.0/PKG-INFO` & `google_news_feed-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_news_feed
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple python library to consume the google news rss feed
 Project-URL: Homepage, https://github.com/LLukas22/Google-News-RSS
 Project-URL: Bug Tracker, https://github.com/LLukas22/Google-News-RSS/issues
 Author: Lukas Kreussel
 License: MIT License
         
         Copyright (c) 2022 LLukas22
@@ -22,27 +22,30 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: dateparser>=1.1.1
-Requires-Dist: httpx>=0.23.0
 Requires-Dist: lxml>=4.9.0
+Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # Google-News-Feed
 A simple python library to consume the google news rss feed.
 
-Inspired by [pygooglenews](https://github.com/kotartemiy/pygooglenews) and implemented using [httpx](https://pypi.org/project/httpx/) and [lxml](https://pypi.org/project/lxml/).
+Inspired by [pygooglenews](https://github.com/kotartemiy/pygooglenews) and implemented using [aiohttp](https://pypi.org/project/aiohttp/) and [lxml](https://pypi.org/project/lxml/).
 
 
 ## Installation
 Via pip: <code>pip install google-news-feed</code>
 
 ## How to use
 ```python
```

