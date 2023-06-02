# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.904.tar", last modified: Thu Jun  1 02:34:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.905.tar", last modified: Fri Jun  2 00:28:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.904.tar` & `tencentcloud-sdk-python-essbasic-3.0.905.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16247 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51460 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   232146 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:34:49.000000 tencentcloud-sdk-python-essbasic-3.0.904/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51460 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   232146 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,20 @@
 
 # 应用号不存在。
 INVALIDPARAMETER_APPLICATION = 'InvalidParameter.Application'
 
 # 参数错误，不合法的签署人类型，请修改后重试。
 INVALIDPARAMETER_APPROVERTYPE = 'InvalidParameter.ApproverType'
 
+# ApproverVerifyType参数值非法
+INVALIDPARAMETER_APPROVERVERIFYTYPE = 'InvalidParameter.ApproverVerifyType'
+
+# 当前仅支持指定上传授权书和法人认证授权, 请重新指定认证方式后发起
+INVALIDPARAMETER_AUTHORIZATIONTYPE = 'InvalidParameter.AuthorizationType'
+
 # 重复添加签署人。
 INVALIDPARAMETER_BIZAPPROVERALREADYEXISTS = 'InvalidParameter.BizApproverAlreadyExists'
 
 # 营业执照格式不合法。
 INVALIDPARAMETER_BUSINESSLICENSE = 'InvalidParameter.BusinessLicense'
 
 # 撤销理由填写格式错误。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.905/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.904/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.905/setup.py`

 * *Files identical despite different names*

