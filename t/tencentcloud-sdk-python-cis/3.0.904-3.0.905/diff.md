# Comparing `tmp/tencentcloud-sdk-python-cis-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-cis-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cis-3.0.904.tar", last modified: Thu Jun  1 02:30:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cis-3.0.905.tar", last modified: Fri Jun  2 00:24:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cis-3.0.904.tar` & `tencentcloud-sdk-python-cis-3.0.905.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/
--rw-r--r--   0 root         (0) root         (0)     7698 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/cis_client.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24442 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud_sdk_python_cis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud_sdk_python_cis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud_sdk_python_cis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud_sdk_python_cis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/tencentcloud_sdk_python_cis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:30:01.000000 tencentcloud-sdk-python-cis-3.0.904/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/cis_client.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24442 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud_sdk_python_cis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud_sdk_python_cis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud_sdk_python_cis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud_sdk_python_cis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/tencentcloud_sdk_python_cis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:24:04.000000 tencentcloud-sdk-python-cis-3.0.905/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cis-3.0.904/README.rst` & `tencentcloud-sdk-python-cis-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/cis_client.py` & `tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/cis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/errorcodes.py` & `tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.904/tencentcloud/cis/v20180408/models.py` & `tencentcloud-sdk-python-cis-3.0.905/tencentcloud/cis/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cis-3.0.905/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.904'
+__version__ = '3.0.905'
```

### Comparing `tencentcloud-sdk-python-cis-3.0.904/tencentcloud_sdk_python_cis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cis-3.0.905/tencentcloud_sdk_python_cis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cis
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Cis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cis-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-cis-3.0.905/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cis
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Cis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cis-3.0.904/setup.py` & `tencentcloud-sdk-python-cis-3.0.905/setup.py`

 * *Files identical despite different names*

