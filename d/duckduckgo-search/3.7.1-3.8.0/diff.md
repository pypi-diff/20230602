# Comparing `tmp/duckduckgo_search-3.7.1.tar.gz` & `tmp/duckduckgo_search-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.7.1.tar", last modified: Wed May 31 06:45:29 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.8.0.tar", last modified: Thu Jun  1 23:59:52 2023, max compression
```

## Comparing `duckduckgo_search-3.7.1.tar` & `duckduckgo_search-3.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13701 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13924 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31374 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.7.1/LICENSE.md` & `duckduckgo_search-3.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.1/PKG-INFO` & `duckduckgo_search-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.7.1
+Version: 3.8.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -56,18 +56,22 @@
 or
 ```python3
 python -m duckduckgo_search --help
 ```
 
 CLI examples:
 ```python3
-# download pdf files
+# text search
+ddgs text -k 'ayrton senna'
+# find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
-# download images
-ddgs images -k "lady in red" -m 500 -s off -d
+# find and download xls files from a specific site
+ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
+# find and download images
+ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
@@ -159,18 +163,14 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception.
-In this case, you need repeat again after a while or to use a proxy ([documentation](https://www.python-httpx.org/advanced/#http-proxying)).
-You can set a timeout if the proxy takes a long time to respond (default timeout=10).
-
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 with DDGS(proxies="socks5://localhost:9150", timeout=20) as ddgs:
     for r in ddgs.text("something you need"):
         print(r)
@@ -183,14 +183,21 @@
     for r in ddgs.text("something you need"):
         print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
+`html` and `lite` backend differ from `api`:</br>
+* don't do an extra request first to get vqd,</br>
+* use POST requests,</br>
+* pause 0.75 seconds between paginations.</br>
+
+If you use `html` or `lite` backend, pause at least 0.75 seconds between text() calls. 
+Otherwise the site will return a 403 status code after a few requests and block your ip for a few seconds.
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     backend: str = "api",
```

### Comparing `duckduckgo_search-3.7.1/README.md` & `duckduckgo_search-3.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,22 @@
 or
 ```python3
 python -m duckduckgo_search --help
 ```
 
 CLI examples:
 ```python3
-# download pdf files
+# text search
+ddgs text -k 'ayrton senna'
+# find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
-# download images
-ddgs images -k "lady in red" -m 500 -s off -d
+# find and download xls files from a specific site
+ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
+# find and download images
+ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
@@ -134,18 +138,14 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception.
-In this case, you need repeat again after a while or to use a proxy ([documentation](https://www.python-httpx.org/advanced/#http-proxying)).
-You can set a timeout if the proxy takes a long time to respond (default timeout=10).
-
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 with DDGS(proxies="socks5://localhost:9150", timeout=20) as ddgs:
     for r in ddgs.text("something you need"):
         print(r)
@@ -158,14 +158,21 @@
     for r in ddgs.text("something you need"):
         print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
+`html` and `lite` backend differ from `api`:</br>
+* don't do an extra request first to get vqd,</br>
+* use POST requests,</br>
+* pause 0.75 seconds between paginations.</br>
+
+If you use `html` or `lite` backend, pause at least 0.75 seconds between text() calls. 
+Otherwise the site will return a 403 status code after a few requests and block your ip for a few seconds.
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     backend: str = "api",
```

### Comparing `duckduckgo_search-3.7.1/duckduckgo_search/__init__.py` & `duckduckgo_search-3.8.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.1/duckduckgo_search/cli.py` & `duckduckgo_search-3.8.0/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.1/duckduckgo_search/compat.py` & `duckduckgo_search-3.8.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.1/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.8.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,15 @@
 REGEX_STRIP_TAGS = re.compile("<.*?>")
 
 USERAGENTS = [
     "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
     "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
     "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
     "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13.4; rv:109.0) Gecko/20100101 Firefox/113.0",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13.4; rv:102.0) Gecko/20100101 Firefox/102.0",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Safari/605.1.15",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/113.0.1774.57",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/113.0.1774.57",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
-    "Mozilla/5.0 (Windows NT 10.0; WOW64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
 ]
-HEADERS = {
-    "User-Agent": choice(USERAGENTS),
-    "Referer": "https://duckduckgo.com/",
-}
 
 
 @dataclass
 class MapsResult:
     title: Optional[str] = None
     address: Optional[str] = None
     country_code: Optional[str] = None
@@ -61,16 +48,21 @@
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         proxies: Optional[Union[Dict, str]] = None,
         timeout: int = 10,
     ) -> None:
+        if headers is None:
+            headers = {
+                "User-Agent": choice(USERAGENTS),
+                "Referer": "https://duckduckgo.com/",
+            }
         self._client = httpx.Client(
-            headers=headers if headers else HEADERS,
+            headers=headers,
             proxies=proxies,
             timeout=timeout,
             http2=True,
         )
 
     def __enter__(self):
         return self
@@ -211,29 +203,33 @@
             try:
                 page_data = resp.json().get("results", None)
             except Exception:
                 break
             if page_data is None:
                 break
 
+            result_exists = False
             for row in page_data:
                 href = row.get("u", None)
                 if (
                     href
                     and href not in cache
                     and href != f"http://www.google.com/search?q={keywords}"
                 ):
                     cache.add(href)
                     body = self._normalize(row["a"])
                     if body:
+                        result_exists = True
                         yield {
                             "title": self._normalize(row["t"]),
                             "href": href,
-                            "body": body,
+                            "body": self._normalize(body),
                         }
+            if result_exists is False:
+                break
 
     def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -267,34 +263,36 @@
             if resp is None:
                 break
 
             tree = html.fromstring(resp.content)
             if tree.xpath('//div[@class="no-results"]/text()'):
                 return
 
+            result_exists = False
             for e in tree.xpath('//div[contains(@class, "results_links")]'):
                 href = e.xpath('.//a[contains(@class, "result__a")]/@href')
                 href = href[0] if href else None
                 if (
                     href
                     and href not in cache
                     and href != f"http://www.google.com/search?q={keywords}"
                 ):
                     cache.add(href)
                     title = e.xpath('.//a[contains(@class, "result__a")]/text()')
                     body = e.xpath('.//a[contains(@class, "result__snippet")]//text()')
+                    result_exists = True
                     yield {
                         "title": self._normalize(title[0]) if title else None,
                         "href": href,
                         "body": self._normalize("".join(body)) if body else None,
                     }
 
             next_page = tree.xpath('.//div[@class="nav-link"]')
             next_page = next_page[-1] if next_page else None
-            if next_page is None:
+            if next_page is None or result_exists is False:
                 return
 
             names = next_page.xpath('.//input[@type="hidden"]/@name')
             values = next_page.xpath('.//input[@type="hidden"]/@value')
             payload = {n: v for n, v in zip(names, values)}
             sleep(0.75)
 
@@ -327,29 +325,31 @@
             payload["s"] = s
             resp = self._get_url(
                 "POST", "https://lite.duckduckgo.com/lite/", data=payload
             )
             if resp is None:
                 break
 
-            tree = html.fromstring(resp.content)
-            if "No more results." in tree.xpath("//table[1]//text()"):
+            if b"No more results." in resp.content:
                 return
 
+            tree = html.fromstring(resp.content)
+
             result_exists = False
             for i, e in zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr")):
                 if i == 1:
                     href = e.xpath(".//a//@href")
                     href = href[0] if href else None
                     if (
                         href is None
                         or href in cache
                         or href == f"http://www.google.com/search?q={keywords}"
                     ):
                         continue
+                    cache.add(href)
                     title = e.xpath(".//a//text()")[0]
                 elif i == 2:
                     body = e.xpath(".//td[@class='result-snippet']//text()")
                     body = "".join(body).strip()
                 elif i == 3:
                     result_exists = True
                     yield {
```

### Comparing `duckduckgo_search-3.7.1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.8.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.7.1
+Version: 3.8.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -56,18 +56,22 @@
 or
 ```python3
 python -m duckduckgo_search --help
 ```
 
 CLI examples:
 ```python3
-# download pdf files
+# text search
+ddgs text -k 'ayrton senna'
+# find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
-# download images
-ddgs images -k "lady in red" -m 500 -s off -d
+# find and download xls files from a specific site
+ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
+# find and download images
+ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
@@ -159,18 +163,14 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception.
-In this case, you need repeat again after a while or to use a proxy ([documentation](https://www.python-httpx.org/advanced/#http-proxying)).
-You can set a timeout if the proxy takes a long time to respond (default timeout=10).
-
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 with DDGS(proxies="socks5://localhost:9150", timeout=20) as ddgs:
     for r in ddgs.text("something you need"):
         print(r)
@@ -183,14 +183,21 @@
     for r in ddgs.text("something you need"):
         print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
+`html` and `lite` backend differ from `api`:</br>
+* don't do an extra request first to get vqd,</br>
+* use POST requests,</br>
+* pause 0.75 seconds between paginations.</br>
+
+If you use `html` or `lite` backend, pause at least 0.75 seconds between text() calls. 
+Otherwise the site will return a 403 status code after a few requests and block your ip for a few seconds.
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     backend: str = "api",
```

### Comparing `duckduckgo_search-3.7.1/pyproject.toml` & `duckduckgo_search-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.1/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.8.0/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

