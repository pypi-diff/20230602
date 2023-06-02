# Comparing `tmp/caqui-1.0.4.tar.gz` & `tmp/caqui-1.0.5.tar.gz`

## Comparing `caqui-1.0.4.tar` & `caqui-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,33 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 caqui-1.0.4/sample.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 caqui-1.0.4/test-requirements.txt
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.4/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.4/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/exceptions.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/constants.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/fake_responses.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/test_sniffer.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/feature/test_functions.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/html/playground.html
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/unit/__initi__.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/unit/test_sync_unit.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.4/LICENSE
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 caqui-1.0.4/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 caqui-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 caqui-1.0.5/sample.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 caqui-1.0.5/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/helper.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/constants.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/fake_responses.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/test_sniffer.py
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/feature/test_functions.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/html/playground.html
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/test_sync_unit.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.5/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.5/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10402 2020-02-02 00:00:00.000000 caqui-1.0.5/PKG-INFO
```

### Comparing `caqui-1.0.4/CODE_OF_CONDUCT.md` & `caqui-1.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/.github/workflows/python-app.yml` & `caqui-1.0.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/.github/workflows/python-publish.yml` & `caqui-1.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/caqui/__init__.py` & `caqui-1.0.5/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/caqui/asynchronous.py` & `caqui-1.0.5/caqui/synchronous.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,134 @@
-import aiohttp
+import requests
 import json
-from caqui.constants import HEADERS
 from caqui.exceptions import WebDriverError
+from caqui.helper import get_element
 
+HEADERS = {
+    "Accept-Encoding": "identity",
+    "Accept": "application/json",
+    "Content-Type": "application/json;charset=UTF-8",
+    "Connection": "keep-alive",
+}
 
-async def __post(url, payload):
+
+def __get(url, payload):
+    try:
+        return requests.request("GET", url, headers=HEADERS, data=payload).json()
+    except Exception as error:
+        raise WebDriverError("'GET' request failed.") from error
+
+
+def __post(url, payload):
     try:
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url, data=payload, headers=HEADERS) as resp:
-                response = await resp.json()
-                return response
+        return requests.request("POST", url, headers=HEADERS, data=payload).json()
     except Exception as error:
         raise WebDriverError("'POST' request failed.") from error
 
 
-async def find_elements(driver_url, session, locator_type, locator_value):
+def __delete(url):
+    try:
+        return requests.request("DELETE", url, headers={}, data={}).json()
+    except Exception as error:
+        raise WebDriverError("'DELETE' request failed.") from error
+
+
+def find_elements(driver_url, session, locator_type, locator_value):
     try:
-        payload = json.dumps({"using": locator_type, "value": locator_value})
         url = f"{driver_url}/session/{session}/elements"
-        response = await __post(url, payload)
+        payload = json.dumps({"using": locator_type, "value": locator_value})
+        response = __post(url, payload)
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
         raise WebDriverError(
-            f"Failed to find element by '{locator_type}'-'{locator_value}'."
+            f"Failed to find elements by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
-async def get_property(driver_url, session, element, property):
+def get_property(driver_url, session, element, property):
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=HEADERS) as resp:
-                response = await resp.json()
-                return response.get("value")
+        response = __get(url, {})
+        return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
 
-async def get_text(driver_url, session, element):
+def go_to_page(driver_url, session, page_url):
     try:
-        url = f"{driver_url}/session/{session}/element/{element}/text"
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=HEADERS) as resp:
-                response = await resp.json()
-                return response.get("value")
+        url = f"{driver_url}/session/{session}/url"
+        payload = json.dumps({"url": page_url})
+        __post(url, payload)
+        return True
     except Exception as error:
-        raise WebDriverError("Failed to get text from element.") from error
+        raise WebDriverError(f"Failed to navigate to '{page_url}'") from error
 
 
-async def close_session(driver_url, session):
+def close_session(driver_url, session):
     try:
         url = f"{driver_url}/session/{session}"
-        async with aiohttp.ClientSession() as session:
-            async with session.delete(url, headers=HEADERS) as resp:
-                response = await resp.json()
-                return response.get("sessionId")
+        __delete(url)
+        return True
     except Exception as error:
         raise WebDriverError("Failed to close session.") from error
 
 
-async def go_to_page(driver_url, session, page_url):
+def get_text(driver_url, session, element):
     try:
-        url = f"{driver_url}/session/{session}/url"
-        payload = json.dumps({"url": page_url})
-        response = await __post(url, payload)
-        return response.get("sessionId")
+        url = f"{driver_url}/session/{session}/element/{element}/text"
+        response = __get(url, {})
+        return response.get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to navigate to page '{page_url}'.") from error
+        raise WebDriverError("Failed to get text from element.") from error
 
 
-async def send_keys(driver_url, session, element, text):
+def send_keys(driver_url, session, element, text):
     try:
         url = f"{driver_url}/session/{session}/element/{element}/value"
         payload = json.dumps({"text": text, "value": [*text], "id": element})
-        response = await __post(url, payload)
-        return response.get("sessionId")
+        __post(url, payload)
+        return True
     except Exception as error:
         raise WebDriverError(f"Failed to send key '{text}'.") from error
 
 
-async def click(driver_url, session, element):
+def click(driver_url, session, element):
     try:
-        payload = json.dumps({"id": element})
         url = f"{driver_url}/session/{session}/element/{element}/click"
-        response = await __post(url, payload)
-        return response.get("sessionId")
+        payload = json.dumps({"id": element})
+        __post(url, payload)
+        return True
     except Exception as error:
         raise WebDriverError("Failed to click on element.") from error
 
 
-async def find_element(driver_url, session, locator_type, locator_value):
-    try:
-        payload = json.dumps({"using": locator_type, "value": locator_value})
-        url = f"{driver_url}/session/{session}/element"
-        response = await __post(url, payload)
-        return response.get("value").get("ELEMENT")
-    except Exception as error:
-        raise WebDriverError(
-            f"Failed to find element by '{locator_type}'-'{locator_value}'."
-        ) from error
+def __get_session(response):
+    # Firefox response
+    value = response.get("value")
+    session_id = value.get("sessionId")
+    if session_id:
+        return session_id
+
+    # Chrome response
+    return response.get("sessionId")
 
 
-async def get_session(driver_url, capabilities):
+def get_session(driver_url, capabilities):
     try:
-        payload = json.dumps(capabilities)
         url = f"{driver_url}/session"
-        response = await __post(url, payload)
-        return response.get("sessionId")
+        data = json.dumps(capabilities)
+        response = __post(url, payload=data)
+        return __get_session(response)
     except Exception as error:
         raise WebDriverError("Failed to open session.") from error
+
+
+def find_element(driver_url, session, locator_type, locator_value):
+    try:
+        url = f"{driver_url}/session/{session}/element"
+        payload = json.dumps({"using": locator_type, "value": locator_value})
+        response = __post(url, payload)
+        return get_element(response)
+    except Exception as error:
+        raise WebDriverError(
+            f"Failed to find element by '{locator_type}'-'{locator_value}'."
+        ) from error
```

### Comparing `caqui-1.0.4/tests/fake_responses.py` & `caqui-1.0.5/tests/fake_responses.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/tests/test_sniffer.py` & `caqui-1.0.5/tests/test_sniffer.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/tests/feature/test_functions.py` & `caqui-1.0.5/tests/feature/test_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,32 @@
     )
 
     assert len(elements) > 0
     assert len(async_elements) > 0
 
 
 @mark.asyncio
+async def test_find_element(__setup):
+    driver_url, session = __setup
+    locator_type = "xpath"
+    locator_value = "//input"
+
+    assert (
+        synchronous.find_element(driver_url, session, locator_type, locator_value)
+        is not None
+    )
+    assert (
+        await asynchronous.find_element(
+            driver_url, session, locator_type, locator_value
+        )
+        is not None
+    )
+
+
+@mark.asyncio
 async def test_get_property(__setup):
     driver_url, session = __setup
     text = "any_value"
     locator_type = "xpath"
     locator_value = "//input"
     property = "value"
 
@@ -73,29 +91,26 @@
 @mark.asyncio
 async def test_send_keys(__setup):
     driver_url, session = __setup
     text_async = "any_async"
     text_sync = "any_sync"
     locator_type = "xpath"
     locator_value = "//input"
-    expected = session
 
     element = synchronous.find_element(driver_url, session, locator_type, locator_value)
 
     assert (
-        await asynchronous.send_keys(driver_url, session, element, text_async)
-        == expected
+        await asynchronous.send_keys(driver_url, session, element, text_async) is True
     )
-    assert synchronous.send_keys(driver_url, session, element, text_sync) == expected
+    assert synchronous.send_keys(driver_url, session, element, text_sync) is True
 
 
 @mark.asyncio
 async def test_click(__setup):
     driver_url, session = __setup
     locator_type = "xpath"
     locator_value = "//button"
-    expected = session
 
     element = synchronous.find_element(driver_url, session, locator_type, locator_value)
 
-    assert await asynchronous.click(driver_url, session, element) == expected
-    assert synchronous.click(driver_url, session, element) == expected
+    assert await asynchronous.click(driver_url, session, element) is True
+    assert synchronous.click(driver_url, session, element) is True
```

### Comparing `caqui-1.0.4/tests/html/playground.html` & `caqui-1.0.5/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/tests/integration/test_async_scenarios.py` & `caqui-1.0.5/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/tests/integration/test_sync_scenarios.py` & `caqui-1.0.5/tests/integration/test_sync_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/tests/unit/test_async_unit.py` & `caqui-1.0.5/tests/unit/test_async_unit.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/tests/unit/test_sync_unit.py` & `caqui-1.0.5/tests/unit/test_sync_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,22 +54,22 @@
 
 
 @patch("requests.request", return_value=GO_TO_PAGE)
 def test_go_to_page(*args):
     driver_url, session, _ = __setup()
     url = "http://any.com"
 
-    assert go_to_page(driver_url, session, url) == session
+    assert go_to_page(driver_url, session, url) is True
 
 
 @patch("requests.request", return_value=CLOSE_SESSION)
 def test_close_session(*args):
     driver_url, session, _ = __setup()
 
-    assert close_session(driver_url, session) == session
+    assert close_session(driver_url, session) is True
 
 
 @patch("requests.request", return_value=GET_TEXT)
 def test_get_text(*args):
     driver_url, session, element = __setup()
     expected = "any"
 
@@ -77,22 +77,22 @@
 
 
 @patch("requests.request", return_value=SEND_KEYS)
 def test_send_keys(*args):
     driver_url, session, element = __setup()
     text = "any"
 
-    assert send_keys(driver_url, session, element, text) == session
+    assert send_keys(driver_url, session, element, text) is True
 
 
 @patch("requests.request", return_value=CLICK)
 def test_click(*args):
     driver_url, session, element = __setup()
 
-    assert click(driver_url, session, element) == session
+    assert click(driver_url, session, element) is True
 
 
 @patch("requests.request", return_value=GET_SESSION)
 def test_get_session(*args):
     driver_url = "http://any:9999"
     payload = {
         "desiredCapabilities": {
```

### Comparing `caqui-1.0.4/.gitignore` & `caqui-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/LICENSE` & `caqui-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.4/pyproject.toml` & `caqui-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

