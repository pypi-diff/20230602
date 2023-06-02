# Comparing `tmp/sentry_dynamic_sampling_lib-1.2.0a2.tar.gz` & `tmp/sentry_dynamic_sampling_lib-1.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_dynamic_sampling_lib-1.2.0a2.tar", max compression
+gzip compressed data, was "sentry_dynamic_sampling_lib-1.2.0a3.tar", max compression
```

## Comparing `sentry_dynamic_sampling_lib-1.2.0a2.tar` & `sentry_dynamic_sampling_lib-1.2.0a3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1303 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/LICENSE
--rw-r--r--   0        0        0     2047 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/README.md
--rw-r--r--   0        0        0     3101 2023-05-28 15:06:39.583538 sentry_dynamic_sampling_lib-1.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     1682 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/__init__.py
--rw-r--r--   0        0        0     5617 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/sampler.py
--rw-r--r--   0        0        0      603 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/settings.py
--rw-r--r--   0        0        0     4089 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/shared.py
--rw-r--r--   0        0        0      507 2023-05-28 15:06:26.423245 sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/utils.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.2.0a2/setup.py
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-06-02 11:19:27.691884 sentry_dynamic_sampling_lib-1.2.0a3/LICENSE
+-rw-r--r--   0        0        0     2047 2023-06-02 11:19:27.691884 sentry_dynamic_sampling_lib-1.2.0a3/README.md
+-rw-r--r--   0        0        0     3101 2023-06-02 11:19:36.343955 sentry_dynamic_sampling_lib-1.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1682 2023-06-02 11:19:27.695884 sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/__init__.py
+-rw-r--r--   0        0        0     5617 2023-06-02 11:19:27.695884 sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/sampler.py
+-rw-r--r--   0        0        0      603 2023-06-02 11:19:27.695884 sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/settings.py
+-rw-r--r--   0        0        0     4089 2023-06-02 11:19:27.695884 sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/shared.py
+-rw-r--r--   0        0        0      507 2023-06-02 11:19:27.695884 sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/utils.py
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.2.0a3/setup.py
+-rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.2.0a3/PKG-INFO
```

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/LICENSE` & `sentry_dynamic_sampling_lib-1.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/README.md` & `sentry_dynamic_sampling_lib-1.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/pyproject.toml` & `sentry_dynamic_sampling_lib-1.2.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentry-dynamic-sampling-lib"
-version = "1.2.0-alpha.2"
+version = "1.2.0-alpha.3"
 description = "This project aims to provide dynamic sampling without relying on Sentry Dynamic Sampling."
 authors = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 maintainers = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 readme = "README.md"
 packages = [{ include = "sentry_dynamic_sampling_lib" }]
 license = "BSD-2-Clause"
 repository = "https://github.com/SpikeeLabs/django-admin-action-tools"
@@ -19,15 +19,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 schedule = "^1.1.0"
 wrapt = "^1.14.1"
 psutil = "^5.9.4"
-requests-cache = "^0.9.7"
+requests-cache = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.4"
 black = "^22.12.0"
 coverage = "^7.0.4"
 pre-commit = "^2.21.0"
 pylama = "^8.4.1"
```

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/__init__.py` & `sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/sampler.py` & `sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/sampler.py`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/settings.py` & `sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/settings.py`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/sentry_dynamic_sampling_lib/shared.py` & `sentry_dynamic_sampling_lib-1.2.0a3/sentry_dynamic_sampling_lib/shared.py`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/setup.py` & `sentry_dynamic_sampling_lib-1.2.0a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 ['sentry_dynamic_sampling_lib']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['psutil>=5.9.4,<6.0.0',
- 'requests-cache>=0.9.7,<0.10.0',
+ 'requests-cache>=1.0.0,<2.0.0',
  'schedule>=1.1.0,<2.0.0',
  'wrapt>=1.14.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'sentry-dynamic-sampling-lib',
-    'version': '1.2.0a2',
+    'version': '1.2.0a3',
     'description': 'This project aims to provide dynamic sampling without relying on Sentry Dynamic Sampling.',
     'long_description': '# Sentry Dynamic Sampling Controller\n\n[![PyPI](https://img.shields.io/pypi/v/sentry-dynamic-sampling-lib?color=blue)](https://pypi.org/project/sentry-dynamic-sampling-lib/)\n![Tests Status](https://github.com/SpikeeLabs/sentry-dynamic-sampling-lib/actions/workflows/.github/workflows/tests.yml/badge.svg)\n[![codecov](https://codecov.io/gh/SpikeeLabs/sentry-dynamic-sampling-lib/branch/main/graph/badge.svg?token=RON7F8QTZX)](https://codecov.io/gh/SpikeeLabs/sentry-dynamic-sampling-lib)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sentry-dynamic-sampling-lib)\n![PyPI - License](https://img.shields.io/pypi/l/sentry-dynamic-sampling-lib)\n\n---\nThis project aims to provide dynamic sampling without relying on Sentry own\'s Dynamic Sampling.\nThis libs works by adding a `traces_sampler` callback to sentry.\nIn the background a thread fetch the data from the [controller](https://github.com/SpikeeLabs/sentry-dynamic-sampling-controller)\nIt\'s also able to ignore WSGI route an Celery task set in controller.\n\n\n\n\n\n## Usage\n```python\nimport sentry_sdk\nfrom sentry_dynamic_sampling_lib import init_wrapper\n\n# init sentry as usual\n# without traces_sampler and sample_rate param\nsentry_sdk.init(  # pylint: disable=E0110\n    dsn=SENTRY_DSN,\n    integrations=[],\n    environment=ENVIRONMENT,\n    release=SENTRY_RELEASE,\n)\n\n# hook sentry_dynamic_sampling_lib into sentry\ninit_wrapper()\n```\n\n\n## Configuration\nThe following environment variables can be used to configure the lib\n\n```bash\nSENTRY_CONTROLLER_HOST=none # (required, no default)\nSENTRY_CONTROLLER_PATH="/sentry/apps/{}/" # (optional, default to example)\nSENTRY_CONTROLLER_METRIC_PATH="/sentry/apps/{}/metrics/{}/" # (optional, default to example)\nSENTRY_CONTROLLER_POLL_INTERVAL=60 # (optional, default to example)\nSENTRY_CONTROLLER_METRIC_INTERVAL=600 # (optional, default to example)\n```\n\n\n\n\n## Development\n```bash\n# install deps\npoetry install\n\n# pre-commit\npoetry run pre-commit install --install-hook\npoetry run pre-commit install --install-hooks --hook-type commit-msg\n```\n',
     'author': 'jeanloup.monnier',
     'author_email': 'jean-loup.monnier@spikeelabs.fr',
     'maintainer': 'jeanloup.monnier',
     'maintainer_email': 'jean-loup.monnier@spikeelabs.fr',
     'url': 'https://github.com/SpikeeLabs/django-admin-action-tools',
```

### Comparing `sentry_dynamic_sampling_lib-1.2.0a2/PKG-INFO` & `sentry_dynamic_sampling_lib-1.2.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-dynamic-sampling-lib
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: This project aims to provide dynamic sampling without relying on Sentry Dynamic Sampling.
 Home-page: https://github.com/SpikeeLabs/django-admin-action-tools
 License: BSD-2-Clause
 Author: jeanloup.monnier
 Author-email: jean-loup.monnier@spikeelabs.fr
 Maintainer: jeanloup.monnier
 Maintainer-email: jean-loup.monnier@spikeelabs.fr
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: requests-cache (>=0.9.7,<0.10.0)
+Requires-Dist: requests-cache (>=1.0.0,<2.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: wrapt (>=1.14.1,<2.0.0)
 Project-URL: Repository, https://github.com/SpikeeLabs/django-admin-action-tools
 Description-Content-Type: text/markdown
 
 # Sentry Dynamic Sampling Controller
```

