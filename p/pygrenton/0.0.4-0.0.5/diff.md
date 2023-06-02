# Comparing `tmp/pygrenton-0.0.4.tar.gz` & `tmp/pygrenton-0.0.5.tar.gz`

## Comparing `pygrenton-0.0.4.tar` & `pygrenton-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pygrenton-0.0.4/requirements.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygrenton-0.0.4/setup.cfg
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pygrenton-0.0.4/pygrenton/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pygrenton-0.0.4/pygrenton/cipher.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 pygrenton-0.0.4/pygrenton/requests.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pygrenton-0.0.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pygrenton-0.0.4/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pygrenton-0.0.4/README.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pygrenton-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pygrenton-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pygrenton-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pygrenton-0.0.5/setup.cfg
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pygrenton-0.0.5/pygrenton/__init__.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pygrenton-0.0.5/pygrenton/cipher.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pygrenton-0.0.5/pygrenton/requests.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pygrenton-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pygrenton-0.0.5/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pygrenton-0.0.5/README.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pygrenton-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pygrenton-0.0.5/PKG-INFO
```

### Comparing `pygrenton-0.0.4/pygrenton/cipher.py` & `pygrenton-0.0.5/pygrenton/cipher.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from cryptography.hazmat.primitives import padding
-from cryptography.hazmat.backends import default_backend
-from base64 import b64decode
-
-class GrentonCypher:
-
-    def __init__(self, key: str, iv: str) -> None:
-        self._key = b64decode(key)
-        self._iv = b64decode(iv)
-        self._padding = padding.PKCS7(128)
-        self._cypher = Cipher(
-            algorithms.AES(self._key), modes.CBC(self._iv), backend=default_backend()
-        )
-
-    def encrypt(self, data: bytes) -> bytes:
-        encryptor = self._cypher.encryptor()
-        padder = self._padding.padder()
-        data = padder.update(data) + padder.finalize()
-        return encryptor.update(data) + encryptor.finalize()
-
-    def decrypt(self, data: bytes) -> bytes:
-        decryptor = self._cypher.decryptor()
-        unpadder = self._padding.unpadder()
-        data = decryptor.update(data) + decryptor.finalize()
-        return unpadder.update(data) + unpadder.finalize()
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.primitives import padding
+from cryptography.hazmat.backends import default_backend
+from base64 import b64decode
+
+class GrentonCypher:
+
+    def __init__(self, key: str, iv: str) -> None:
+        self._key = b64decode(key)
+        self._iv = b64decode(iv)
+        self._padding = padding.PKCS7(128)
+        self._cypher = Cipher(
+            algorithms.AES(self._key), modes.CBC(self._iv), backend=default_backend()
+        )
+
+    def encrypt(self, data: bytes) -> bytes:
+        encryptor = self._cypher.encryptor()
+        padder = self._padding.padder()
+        data = padder.update(data) + padder.finalize()
+        return encryptor.update(data) + encryptor.finalize()
+
+    def decrypt(self, data: bytes) -> bytes:
+        decryptor = self._cypher.decryptor()
+        unpadder = self._padding.unpadder()
+        data = decryptor.update(data) + decryptor.finalize()
+        return unpadder.update(data) + unpadder.finalize()
```

### Comparing `pygrenton-0.0.4/pygrenton/requests.py` & `pygrenton-0.0.5/pygrenton/requests.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from abc import ABC, abstractmethod
-from typing import Any
-import random
-
-class Request(ABC):
-
-    def __init__(self, payload: str) -> None:
-        chars = "01234567890abcdef"
-        self._id = ''.join(random.choices(chars, k=8))
-        self._payload = payload
-
-    @abstractmethod
-    def parse_response(self, response: str):
-        pass
-
-    def id(self) -> str:
-        return self._id
-
-    def payload(self) -> str:
-        return self._payload
-
-    def create_request(self, ip: str) -> str:
-        return "req:" + ip + ':' + self._id + ':' + self._payload
-
-class CheckAlive(Request):
-
-    def __init__(self) -> None:
-        super().__init__("checkAlive()")
-
-    def parse_response(self, response: str) -> str:
-        spl = response.split(":")
-        clu_serial_hex = spl.pop()
-        return int(clu_serial_hex, base=16)
-
-class SetRequest(Request):
-
-    def __init__(self, device_id: str, index: int, val: Any) -> None:
-        if isinstance(val, str):
-            val = '"' + val + '"'
-        elif isinstance(val, bool):
-            val = str(val).lower()
-
-        payload = "{}:set({},{})".format(device_id, index, val)
-        super().__init__(payload)
-
-    def parse_response(self, response: str):
-        return None
-
-class GetRequest(Request):
-
-    def __init__(self, device_id: str, index: int) -> None:
-        payload = "{}:get({})".format(device_id, index)
-        super().__init__(payload)
-
-    def parse_response(self, response: str):
-        resp = response.split(":").pop()
-        if resp.isdecimal():
-            return float(resp)
-        elif resp.startswith("\"") and resp.endswith("\""):
-            return resp[1:len(resp)]
-        elif resp in ["true", "false"]:
-            return resp == "true"
-        else:
-            return None
-
-class ExecuteRequest(Request):
-
-    def __init__(self, device_id: str, intdex: int, *args: Any) -> None:
-        params_str = ''.join([(',' + str(i)) for i in args]) if len(args) > 0 else ", 0"
-        payload = "{}:execute({}{})".format(device_id, intdex, params_str)
-        super().__init__(payload)
-
-    def parse_response(self, response: str):
-        resp = response.split(":").pop()
-        if resp.isdecimal():
-            return float(resp)
-        elif resp.startswith("\"") and resp.endswith("\""):
-            return resp[1:len(resp)]
-        elif resp in ["true", "false"]:
-            return resp == "true"
-        else:
-            return None
-
+from abc import ABC, abstractmethod
+from typing import Any
+import random
+
+class Request(ABC):
+
+    def __init__(self, payload: str) -> None:
+        chars = "01234567890abcdef"
+        self._id = ''.join(random.choices(chars, k=8))
+        self._payload = payload
+
+    @abstractmethod
+    def parse_response(self, response: str):
+        pass
+
+    def id(self) -> str:
+        return self._id
+
+    def payload(self) -> str:
+        return self._payload
+
+    def create_request(self, ip: str) -> str:
+        return "req:" + ip + ':' + self._id + ':' + self._payload
+
+class CheckAlive(Request):
+
+    def __init__(self) -> None:
+        super().__init__("checkAlive()")
+
+    def parse_response(self, response: str) -> str:
+        spl = response.split(":")
+        clu_serial_hex = spl.pop()
+        return int(clu_serial_hex, base=16)
+
+class SetRequest(Request):
+
+    def __init__(self, device_id: str, index: int, val: Any) -> None:
+        if isinstance(val, str):
+            val = '"' + val + '"'
+        elif isinstance(val, bool):
+            val = str(val).lower()
+
+        payload = "{}:set({},{})".format(device_id, index, val)
+        super().__init__(payload)
+
+    def parse_response(self, response: str):
+        return None
+
+class GetRequest(Request):
+
+    def __init__(self, device_id: str, index: int) -> None:
+        payload = "{}:get({})".format(device_id, index)
+        super().__init__(payload)
+
+    def parse_response(self, response: str):
+        resp = response.split(":").pop()
+        if resp.isdecimal():
+            return float(resp)
+        elif resp.startswith("\"") and resp.endswith("\""):
+            return resp[1:len(resp)]
+        elif resp in ["true", "false"]:
+            return resp == "true"
+        else:
+            return None
+
+class ExecuteRequest(Request):
+
+    def __init__(self, device_id: str, intdex: int, *args: Any) -> None:
+        params_str = ''.join([(',' + str(i)) for i in args]) if len(args) > 0 else ", 0"
+        payload = "{}:execute({}{})".format(device_id, intdex, params_str)
+        super().__init__(payload)
+
+    def parse_response(self, response: str):
+        resp = response.split(":").pop()
+        if resp.isdecimal():
+            return float(resp)
+        elif resp.startswith("\"") and resp.endswith("\""):
+            return resp[1:len(resp)]
+        elif resp in ["true", "false"]:
+            return resp == "true"
+        else:
+            return None
+
```

### Comparing `pygrenton-0.0.4/.gitignore` & `pygrenton-0.0.5/.gitignore`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,131 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+/test.py
```

### Comparing `pygrenton-0.0.4/LICENSE` & `pygrenton-0.0.5/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Paweł Rogaliński
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Paweł Rogaliński
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pygrenton-0.0.4/PKG-INFO` & `pygrenton-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pygrenton
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lightweight Python library to interact with grenton smart-home system.
 Author-email: Paweł Rogaliński <progalin55@gmial.com>
 License: MIT License
         
-        Copyright (c) 2022 Paweł Rogaliński
+        Copyright (c) 2023 Paweł Rogaliński
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,14 +20,15 @@
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
 Requires-Python: >=3.7
 Requires-Dist: cryptography
 Description-Content-Type: text/markdown
```

