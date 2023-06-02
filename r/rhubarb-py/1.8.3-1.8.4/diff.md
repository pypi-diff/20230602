# Comparing `tmp/rhubarb_py-1.8.3.tar.gz` & `tmp/rhubarb_py-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhubarb_py-1.8.3.tar", max compression
+gzip compressed data, was "rhubarb_py-1.8.4.tar", max compression
```

## Comparing `rhubarb_py-1.8.3.tar` & `rhubarb_py-1.8.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1079 2023-06-01 18:37:38.783184 rhubarb_py-1.8.3/LICENSE
--rw-r--r--   0        0        0     7269 2023-06-01 18:37:38.783184 rhubarb_py-1.8.3/README.md
--rw-r--r--   0        0        0     3651 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/pyproject.toml
--rw-r--r--   0        0        0      570 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/__init__.py
--rw-r--r--   0        0        0    16069 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/_core.py
--rw-r--r--   0        0        0     3131 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/base.py
--rw-r--r--   0        0        0       40 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/exceptions.py
--rw-r--r--   0        0        0     7555 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/kafka.py
--rw-r--r--   0        0        0     2483 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/memory.py
--rw-r--r--   0        0        0     3094 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/postgres.py
--rw-r--r--   0        0        0     4360 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/rabbitmq.py
--rw-r--r--   0        0        0    13779 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/redis.py
--rw-r--r--   0        0        0      210 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/event.py
--rw-r--r--   0        0        0        0 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/py.typed
--rw-r--r--   0        0        0     8517 1970-01-01 00:00:00.000000 rhubarb_py-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-02 10:39:01.423738 rhubarb_py-1.8.4/LICENSE
+-rw-r--r--   0        0        0     7567 2023-06-02 10:39:01.423738 rhubarb_py-1.8.4/README.md
+-rw-r--r--   0        0        0     3669 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0      570 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/__init__.py
+-rw-r--r--   0        0        0    16069 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/_core.py
+-rw-r--r--   0        0        0     3131 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/base.py
+-rw-r--r--   0        0        0       40 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/exceptions.py
+-rw-r--r--   0        0        0     7555 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/kafka.py
+-rw-r--r--   0        0        0     2483 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/memory.py
+-rw-r--r--   0        0        0     3094 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/postgres.py
+-rw-r--r--   0        0        0     4360 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/rabbitmq.py
+-rw-r--r--   0        0        0    13779 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/redis.py
+-rw-r--r--   0        0        0      210 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/event.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/py.typed
+-rw-r--r--   0        0        0     8816 1970-01-01 00:00:00.000000 rhubarb_py-1.8.4/PKG-INFO
```

### Comparing `rhubarb_py-1.8.3/LICENSE` & `rhubarb_py-1.8.4/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
-OR OTHER DEALINGS IN THE SOFTWARE.
+OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `rhubarb_py-1.8.3/README.md` & `rhubarb_py-1.8.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Rhubarb
 
 <div align="center">
 
-[![Build status](https://github.com/mopeyjellyfish/rhubarb/workflows/build/badge.svg?branch=main&event=push)](https://github.com/mopeyjellyfish/rhubarb/actions?query=workflow%3Abuild)
+[![Release](https://img.shields.io/github/v/release/mopeyjellyfish/rhubarb)](https://img.shields.io/github/v/release/mopeyjellyfish/rhubarb)
+[![Build](https://github.com/mopeyjellyfish/rhubarb/workflows/build/badge.svg?branch=main&event=push)](https://github.com/mopeyjellyfish/rhubarb/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/rhubarb-py.svg)](https://pypi.org/project/rhubarb-py)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/mopeyjellyfish/rhubarb/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 [![codecov](https://codecov.io/gh/mopeyjellyfish/rhubarb/branch/main/graph/badge.svg?token=E8F5LMKDBK)](https://codecov.io/gh/mopeyjellyfish/rhubarb)
 [![Documentation Status](https://readthedocs.org/projects/rhubarb-py/badge/?version=latest)](https://rhubarb-py.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/mopeyjellyfish/rhubarb/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/mopeyjellyfish/rhubarb/releases)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/rhubarb)](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/rhubarb)
 [![License](https://img.shields.io/github/license/mopeyjellyfish/rhubarb)](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE)
 
 Rhubarb is a library that simplifies realtime streaming of events for a number of backends in to a single API. Currently supports [`Postgres`](https://github.com/MagicStack/asyncpg), [`kafka`](https://github.com/aio-libs/aiokafka), [`RabbitMQ`](https://github.com/mosquito/aio-pika), [`redis`](https://github.com/aio-libs/aioredis-py) as well as an internal memory backend useful for testing.
 
 </div>
 
 ## Installation
@@ -51,15 +53,15 @@
 async with Rhubarb("redis://localhost:6379/0") as events:
     await events.publish("test message")
 ```
 
 ### History retrieval
 
 ```python
-async with Rhubarb("redis://localhost:6379/0") as events: 
+async with Rhubarb("redis://localhost:6379/0") as events:
     async with events.subscribe(channel="CHATROOM", history=10) as subscriber: # read the last 10 events published to the channel
         async for event in subscriber:
             await websocket.send_text(event.message)
 ```
 
 ### Custom serializer & deserializer
```

### Comparing `rhubarb_py-1.8.3/pyproject.toml` & `rhubarb_py-1.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rhubarb-py"
 packages = [{ include = "rhubarb" }]
-version = "1.8.3"
+version = "1.8.4"
 description = "Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API"
 readme = "README.md"
 authors = ["mopeyjellyfish <dev@davidhall.tech>"]
 license = "MIT"
 repository = "https://github.com/mopeyjellyfish/rhubarb"
 homepage = "https://github.com/mopeyjellyfish/rhubarb"
 
@@ -27,46 +27,46 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiokafka = "^0.7.2"
-asyncpg = ">=0.24,<0.27"
-aio-pika = ">=6.8,<9.0"
+aiokafka = ">=0.7.2,<0.9.0"
+asyncpg = ">=0.24,<0.28"
+aio-pika = ">=6.8,<10.0"
 anyio = "^3.4.0"
 redis = "^4.3.4"
 
 [tool.poetry.extras]
 redis = ["redis"]
 kafka = ["aiokafka"]
 postgres = ["asyncpg"]
 rabbitmq = ["aio-pika"]
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
-black = { version = "^22.6", allow-prereleases = true }
+black = { version = "^23.3", allow-prereleases = true }
 darglint = "^1.8.0"
 isort = { extras = ["colors"], version = "^5.9.3" }
 mypy = "^0.971"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.20.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.14.5"
 pytest = "^7.3.1"
 pyupgrade = "^2.37.3"
 safety = "^2.1.1"
-pytest-asyncio = "^0.19.0"
+pytest-asyncio = "^0.21.0"
 Sphinx = "^5.1.1"
 sphinx-rtd-theme = "^1.0.0"
-pytest-cov = "^3.0.0"
-asyncpg = ">=0.24,<0.27"
-aiokafka = "^0.7.2"
-aio-pika = ">=6.8,<9.0"
+pytest-cov = "^4.1.0"
+asyncpg = ">=0.24,<0.28"
+aiokafka = ">=0.7.2,<0.9.0"
+aio-pika = ">=6.8,<10.0"
 hypothesis = "^6.53.0"
 
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
```

### Comparing `rhubarb_py-1.8.3/rhubarb/__init__.py` & `rhubarb_py-1.8.4/rhubarb/__init__.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/_core.py` & `rhubarb_py-1.8.4/rhubarb/_core.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/backends/base.py` & `rhubarb_py-1.8.4/rhubarb/backends/base.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/backends/kafka.py` & `rhubarb_py-1.8.4/rhubarb/backends/kafka.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/backends/memory.py` & `rhubarb_py-1.8.4/rhubarb/backends/memory.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/backends/postgres.py` & `rhubarb_py-1.8.4/rhubarb/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/backends/rabbitmq.py` & `rhubarb_py-1.8.4/rhubarb/backends/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/rhubarb/backends/redis.py` & `rhubarb_py-1.8.4/rhubarb/backends/redis.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.3/PKG-INFO` & `rhubarb_py-1.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhubarb-py
-Version: 1.8.3
+Version: 1.8.4
 Summary: Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API
 Home-page: https://github.com/mopeyjellyfish/rhubarb
 License: MIT
 Author: mopeyjellyfish
 Author-email: dev@davidhall.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,35 +16,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: kafka
 Provides-Extra: postgres
 Provides-Extra: rabbitmq
 Provides-Extra: redis
-Requires-Dist: aio-pika (>=6.8,<9.0) ; extra == "rabbitmq"
-Requires-Dist: aiokafka (>=0.7.2,<0.8.0) ; extra == "kafka"
+Requires-Dist: aio-pika (>=6.8,<10.0) ; extra == "rabbitmq"
+Requires-Dist: aiokafka (>=0.7.2,<0.9.0) ; extra == "kafka"
 Requires-Dist: anyio (>=3.4.0,<4.0.0)
-Requires-Dist: asyncpg (>=0.24,<0.27) ; extra == "postgres"
+Requires-Dist: asyncpg (>=0.24,<0.28) ; extra == "postgres"
 Requires-Dist: redis (>=4.3.4,<5.0.0) ; extra == "redis"
 Project-URL: Repository, https://github.com/mopeyjellyfish/rhubarb
 Description-Content-Type: text/markdown
 
 # Rhubarb
 
 <div align="center">
 
-[![Build status](https://github.com/mopeyjellyfish/rhubarb/workflows/build/badge.svg?branch=main&event=push)](https://github.com/mopeyjellyfish/rhubarb/actions?query=workflow%3Abuild)
+[![Release](https://img.shields.io/github/v/release/mopeyjellyfish/rhubarb)](https://img.shields.io/github/v/release/mopeyjellyfish/rhubarb)
+[![Build](https://github.com/mopeyjellyfish/rhubarb/workflows/build/badge.svg?branch=main&event=push)](https://github.com/mopeyjellyfish/rhubarb/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/rhubarb-py.svg)](https://pypi.org/project/rhubarb-py)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/mopeyjellyfish/rhubarb/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 [![codecov](https://codecov.io/gh/mopeyjellyfish/rhubarb/branch/main/graph/badge.svg?token=E8F5LMKDBK)](https://codecov.io/gh/mopeyjellyfish/rhubarb)
 [![Documentation Status](https://readthedocs.org/projects/rhubarb-py/badge/?version=latest)](https://rhubarb-py.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/mopeyjellyfish/rhubarb/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/mopeyjellyfish/rhubarb/releases)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/rhubarb)](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/rhubarb)
 [![License](https://img.shields.io/github/license/mopeyjellyfish/rhubarb)](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE)
 
 Rhubarb is a library that simplifies realtime streaming of events for a number of backends in to a single API. Currently supports [`Postgres`](https://github.com/MagicStack/asyncpg), [`kafka`](https://github.com/aio-libs/aiokafka), [`RabbitMQ`](https://github.com/mosquito/aio-pika), [`redis`](https://github.com/aio-libs/aioredis-py) as well as an internal memory backend useful for testing.
 
 </div>
 
 ## Installation
@@ -81,15 +83,15 @@
 async with Rhubarb("redis://localhost:6379/0") as events:
     await events.publish("test message")
 ```
 
 ### History retrieval
 
 ```python
-async with Rhubarb("redis://localhost:6379/0") as events: 
+async with Rhubarb("redis://localhost:6379/0") as events:
     async with events.subscribe(channel="CHATROOM", history=10) as subscriber: # read the last 10 events published to the channel
         async for event in subscriber:
             await websocket.send_text(event.message)
 ```
 
 ### Custom serializer & deserializer
```

