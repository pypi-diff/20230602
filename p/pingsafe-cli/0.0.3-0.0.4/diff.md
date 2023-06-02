# Comparing `tmp/pingsafe_cli-0.0.3.tar.gz` & `tmp/pingsafe_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingsafe_cli-0.0.3.tar", max compression
+gzip compressed data, was "pingsafe_cli-0.0.4.tar", max compression
```

## Comparing `pingsafe_cli-0.0.3.tar` & `pingsafe_cli-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      223 2023-05-26 11:36:48.516754 pingsafe_cli-0.0.3/LICENSE
--rw-r--r--   0        0        0      453 2023-05-29 09:07:45.887168 pingsafe_cli-0.0.3/README.md
--rw-r--r--   0        0        0      556 2023-05-29 15:00:24.170095 pingsafe_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.371904 pingsafe_cli-0.0.3/src/pingsafe_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.524980 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525045 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525113 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/codescanner/__init__.py
--rw-r--r--   0        0        0     2351 2023-05-26 11:36:48.518444 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py
--rw-r--r--   0        0        0     7746 2023-05-29 14:32:50.518235 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/codescanner/secret.py
--rw-r--r--   0        0        0     5748 2023-05-29 14:32:50.518988 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/command_line_arguments.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525444 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/config/__init__.py
--rw-r--r--   0        0        0      715 2023-05-25 09:26:45.864579 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/config/config.py
--rw-r--r--   0        0        0     2345 2023-05-29 14:32:50.519563 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/main.py
--rw-r--r--   0        0        0     1861 2023-05-29 14:59:04.577636 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/registry.py
--rw-r--r--   0        0        0     9775 2023-05-29 14:32:50.520022 pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/utils.py
--rw-r--r--   0        0        0       17 2023-05-29 15:00:15.922502 pingsafe_cli-0.0.3/src/pingsafe_cli/version.py
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 pingsafe_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-05-30 12:13:13.829681 pingsafe_cli-0.0.4/LICENSE
+-rw-r--r--   0        0        0      453 2023-05-30 12:13:13.829770 pingsafe_cli-0.0.4/README.md
+-rw-r--r--   0        0        0      580 2023-06-02 06:47:26.667234 pingsafe_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 12:13:13.830096 pingsafe_cli-0.0.4/src/pingsafe_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:13:14.021733 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:13:14.021831 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:13:14.021937 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/codescanner/__init__.py
+-rw-r--r--   0        0        0     2351 2023-06-01 12:12:49.368980 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py
+-rw-r--r--   0        0        0     7948 2023-06-01 12:12:49.369119 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/codescanner/secret.py
+-rw-r--r--   0        0        0     5920 2023-06-01 12:12:49.369253 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/command_line_arguments.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:13:14.022393 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/config/__init__.py
+-rw-r--r--   0        0        0      715 2023-05-30 12:13:14.022495 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/config/config.py
+-rw-r--r--   0        0        0     4019 2023-06-02 06:47:26.667544 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/main.py
+-rw-r--r--   0        0        0     2406 2023-06-02 06:47:26.667887 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/registry.py
+-rw-r--r--   0        0        0    11100 2023-06-02 06:47:26.668172 pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/utils.py
+-rw-r--r--   0        0        0     1192 2023-06-02 07:36:37.518077 pingsafe_cli-0.0.4/src/pingsafe_cli/sentry.py
+-rw-r--r--   0        0        0       37 2023-06-01 12:12:54.593214 pingsafe_cli-0.0.4/src/pingsafe_cli/version.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 pingsafe_cli-0.0.4/PKG-INFO
```

### Comparing `pingsafe_cli-0.0.3/pyproject.toml` & `pingsafe_cli-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+
 [tool.poetry]
 name = "pingsafe_cli"
-version = "0.0.3"
+version = "0.0.4"
 authors = ["pingsafe-dev <dev@pingsafe.com>"]
 description = "PingSafe CLI is an extension of our vision to shift-left security with PingSafe."
 readme = "README.md"
 license = "Proprietary"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 jsonschema = "4.17.3"
 requests = "2.29.0"
 toml = "0.10.2"
+sentry-sdk = "^1.24.0"
 
 [tool.poetry.scripts]
 pre-build =  "pre_build.build_script:main"
 pingsafe-cli = "pingsafe_cli.scanner.cli.main:start"
```

### Comparing `pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py` & `pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/codescanner/secret.py` & `pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/codescanner/secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import json
 import logging
 import os.path
 import subprocess
 import uuid
-from pingsafe_cli.scanner.cli.registry import CodeTypeSubParser, BASELINE_FILE, OutputFormat, PACKAGE_NAME, \
-    MissingRequiredFlags
+from pingsafe_cli.scanner.cli.registry import CodeTypeSubParser, BASELINE_FILE, OutputFormat, \
+    MissingRequiredFlags, MissingDependencies
 from pingsafe_cli.scanner.cli.utils import read_from_file, get_config_path, write_json_to_file, write_csv_to_file, \
     get_version
 
 LOGGER = logging.getLogger("cli")
 HASH_STRING = "pingsafe_hashing_string"
 
 
@@ -111,15 +111,19 @@
         args.all_commits = True
 
     workers_count = global_config_data["workers_count"]
     if args.global_workers_count:
         workers_count = args.global_workers_count
 
     version = get_version()
-    command = [f"{cache_directory}/bin/{version}/bin_secret_detector", "--repo-path", args.directory, "--worker-count",
+    secret_detector_binary_path = f"{cache_directory}/bin/{version}/bin_secret_detector"
+    if not os.path.exists(secret_detector_binary_path):
+        raise MissingDependencies(f"Missing bin_secret_detector {version}")
+
+    command = [secret_detector_binary_path, "--repo-path", args.directory, "--worker-count",
                str(workers_count), "--output-path", output_file]
 
     paths_to_skip = args.skip_paths + global_config_data["pathToIgnore"]
     excluded_detectors = get_detectors_to_exclude(secret_config_data, args.excluded_detectors)
 
     if args.verified_only:
         command.extend(["--verified-only"])
```

### Comparing `pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/command_line_arguments.py` & `pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/command_line_arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     parser.add_argument("--workers-count", dest="global_workers_count", metavar="",
                  help="Set worker count")
     parser.add_argument("--output-format", dest="global_output_format", metavar="",
                                    help="Result Output format",
                                    default=OutputFormat.JSON, choices=[OutputFormat.JSON, OutputFormat.CSV])
     parser.add_argument("--output-file", dest="global_output_file", metavar="", default="",
                                    help="Output file location")
+    parser.add_argument("--disable-sentry", dest="disable_sentry", default=False, action="store_true",
+                                   help="Disable sentry monitoring")
 
 
     # Initialized subparser for global parser
     sub_parser = parser.add_subparsers(dest="main_sub_parser", title="Scan Type",
                                        description="PingSafe allows various types of scan.",
                                        help="Scan Type")
```

### Comparing `pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/config/config.py` & `pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/config/config.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.3/src/pingsafe_cli/scanner/cli/utils.py` & `pingsafe_cli-0.0.4/src/pingsafe_cli/scanner/cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import csv
 import json
 import logging
 import os.path
 import platform
+import sys
 import subprocess
-
+from pingsafe_cli import version
+from sentry_sdk import capture_exception, configure_scope
 import requests
 from pingsafe_cli.scanner.cli.registry import CONFIG_FILE_NAME, CodeTypeSubParser, IacConfigData, HttpMethod, \
     PACKAGE_NAME, PIP_COMMAND, PYPI_URL, GET_PRE_SIGNED_URL, BINARY_LIST, DEFAULT_TIMEOUT, LogColors, \
-    DEFAULT_PINGSAFE_DIR, PINGSAFE_LOCAL_CONFIG_PATH, PlatformNotSupported
+    DEFAULT_PINGSAFE_DIR, PINGSAFE_LOCAL_CONFIG_PATH, PlatformNotSupported, HttpConnectionError, RequestTimeout, \
+    SENTRY_TAGS, DownloadException
 from pingsafe_cli import version
 
 LOGGER = logging.getLogger("cli")
 
 
-
 # Custom formatter class
 class ColoredFormatter(logging.Formatter):
     FORMATS = {
         logging.ERROR: LogColors.FAIL + '%(levelname)s\t%(message)s' + LogColors.ENDC,
         logging.WARNING: LogColors.WARNING + '%(levelname)s\t%(message)s' + LogColors.ENDC,
         logging.INFO: '%(levelname)s\t%(message)s',
         logging.DEBUG: '%(levelname)s\t%(message)s',
@@ -31,42 +33,47 @@
         return formatter.format(record)
 
 
 def initialize_logger(name, level):
     logger = logging.getLogger(name)
     logger.setLevel(level)
 
-    handler = logging.StreamHandler()
+    handler = logging.StreamHandler(sys.stdout)
     formatter = ColoredFormatter()
     handler.setFormatter(formatter)
     logger.propagate = False
     logger.addHandler(handler)
 
 
 def get_os_and_architecture():
     operating_system = platform.system().lower()
     arch = platform.machine().lower()
     return operating_system, arch
 
 
 def make_request(method, url, api_token, query_params=None, data={}):
-    request_headers = generate_headers(api_token)
-    response = requests.request(
-        method=method,
-        url=url,
-        data=json.dumps(data),
-        headers=request_headers,
-        params=query_params,
-        timeout=DEFAULT_TIMEOUT,
-    )
-    if response.status_code == 401:
-        raise Exception("Unauthorized 401")
-    if response.status_code == 501:
-        raise PlatformNotSupported(f"Platform {request_headers['x-runtime-arch']} is not supported.")
-    return response
+    try:
+        request_headers = generate_headers(api_token)
+        response = requests.request(
+            method=method,
+            url=url,
+            data=json.dumps(data),
+            headers=request_headers,
+            params=query_params,
+            timeout=DEFAULT_TIMEOUT,
+        )
+        if response.status_code == 401:
+            raise Exception("Unauthorized 401")
+        if response.status_code == 501:
+            raise PlatformNotSupported(f"Platform {request_headers['x-runtime-arch']} is not supported.")
+        return response
+    except requests.ConnectionError as e:
+        raise HttpConnectionError(f"Unable to send request to url: {url} due to connection error")
+    except requests.Timeout as e:
+        raise RequestTimeout(f"Request timed out for url:{url}")
 
 
 def read_from_file(file_path):
     with open(file_path) as infile:
         return json.load(infile)
 
 
@@ -198,15 +205,16 @@
         subprocess.call(f"{PIP_COMMAND}", shell=True)
     else:
         LOGGER.debug("No updates available")
 
 
 def download_file(url, destination):
     with requests.get(url, stream=True) as r:
-        r.raise_for_status()
+        if r.status_code != 200:
+            raise DownloadException(f"Failed to download dependencies, err: {r.text}", r.url, os.path.basename(destination))
         with open(destination, 'wb') as f:
             # Download the file in chunks
             for chunk in r.iter_content(chunk_size=8192):
                 if chunk:
                     f.write(chunk)
     os.chmod(destination, 0o755)
 
@@ -216,15 +224,15 @@
     for binary in binary_list:
         data[binary] = True
     global_config_file_path = get_config_path(cache)
     global_config_data = read_from_file(global_config_file_path)
 
     response = make_request(HttpMethod.POST, GET_PRE_SIGNED_URL, global_config_data["api_token"], None, data)
     if response.status_code != 200:
-        LOGGER.error(f"Failed to get pres-signed urls, err: {response.text}")
+        LOGGER.error(f"Failed to get pre-signed urls, err: {response.text}")
         return {}
     else:
         return response.json()
 
 
 def download(version, binary, url, cache):
     download_path = os.path.join(cache, "bin")
@@ -274,7 +282,28 @@
     if platform.system() == "Windows":
         return os.path.join(os.path.expandvars("$HOME"), directory)
     return os.path.join(os.path.expanduser("~"), directory)
 
 
 def get_version():
     return version.version
+
+
+def add_sentry_tags(scope, cache_directory):
+    scope.set_tag("cli_version", version.version)
+    system_os, arch = get_os_and_architecture()
+    scope.set_tag("os", system_os)
+    scope.set_tag("arch", arch)
+    if cache_directory != "":
+        global_config_data = read_from_file(os.path.join(cache_directory, CONFIG_FILE_NAME))
+        for tag in SENTRY_TAGS:
+            if tag in global_config_data:
+                scope.set_tag(tag, global_config_data[tag])
+
+
+def send_exception_to_sentry(e, cache_directory):
+    try:
+        with configure_scope() as scope:
+            add_sentry_tags(scope, cache_directory)
+            capture_exception(e)
+    except Exception as e:
+        LOGGER.debug(e)
```

### Comparing `pingsafe_cli-0.0.3/PKG-INFO` & `pingsafe_cli-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pingsafe-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: PingSafe CLI is an extension of our vision to shift-left security with PingSafe.
 License: Proprietary
 Author: pingsafe-dev
 Author-email: dev@pingsafe.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: requests (==2.29.0)
+Requires-Dist: sentry-sdk (>=1.24.0,<2.0.0)
 Requires-Dist: toml (==0.10.2)
 Description-Content-Type: text/markdown
 
 # PingSafe CLI
 PingSafe CLI is an extension of our vision to shift-left security with PingSafe. It is the newest edition to the toolset that will help to keep our customer’s cloud infrastructure safe from external threats and ensure the highest quality standard for security while writing and deploying code.
 
 ## LICENSE
```

