# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.904.tar", last modified: Thu Jun  1 02:29:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.905.tar", last modified: Fri Jun  2 00:23:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.904.tar` & `tencentcloud-sdk-python-cfw-3.0.905.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    66476 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223068 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:29:26.000000 tencentcloud-sdk-python-cfw-3.0.904/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    66476 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223771 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:23:34.000000 tencentcloud-sdk-python-cfw-3.0.905/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/README.rst` & `tencentcloud-sdk-python-cfw-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/cfw/v20190904/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,34 +413,44 @@
         :type PublicIp: str
         :param Ip: 内网IP
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ip: str
         :param SecurityGroupCount: 关联安全组数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type SecurityGroupCount: int
+        :param SecurityGroupRuleCount: 关联安全组规则数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SecurityGroupRuleCount: int
+        :param CdbId: 关联数据库代理Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CdbId: str
         """
         self.InstanceId = None
         self.InstanceName = None
         self.Type = None
         self.VpcId = None
         self.VpcName = None
         self.PublicIp = None
         self.Ip = None
         self.SecurityGroupCount = None
+        self.SecurityGroupRuleCount = None
+        self.CdbId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.Type = params.get("Type")
         self.VpcId = params.get("VpcId")
         self.VpcName = params.get("VpcName")
         self.PublicIp = params.get("PublicIp")
         self.Ip = params.get("Ip")
         self.SecurityGroupCount = params.get("SecurityGroupCount")
+        self.SecurityGroupRuleCount = params.get("SecurityGroupRuleCount")
+        self.CdbId = params.get("CdbId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3747,14 +3757,17 @@
         :param LeakNum: 漏洞数
         :type LeakNum: str
         :param InsSource: 1，公网 2内网
         :type InsSource: str
         :param ResourcePath: [a,b]
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourcePath: list of str
+        :param Server: 扫描结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Server: list of str
         """
         self.AppId = None
         self.Region = None
         self.VpcId = None
         self.VPCName = None
         self.SubnetId = None
         self.InstanceId = None
@@ -3762,14 +3775,15 @@
         self.InsType = None
         self.PublicIp = None
         self.PrivateIp = None
         self.PortNum = None
         self.LeakNum = None
         self.InsSource = None
         self.ResourcePath = None
+        self.Server = None
 
 
     def _deserialize(self, params):
         self.AppId = params.get("AppId")
         self.Region = params.get("Region")
         self.VpcId = params.get("VpcId")
         self.VPCName = params.get("VPCName")
@@ -3779,14 +3793,15 @@
         self.InsType = params.get("InsType")
         self.PublicIp = params.get("PublicIp")
         self.PrivateIp = params.get("PrivateIp")
         self.PortNum = params.get("PortNum")
         self.LeakNum = params.get("LeakNum")
         self.InsSource = params.get("InsSource")
         self.ResourcePath = params.get("ResourcePath")
+        self.Server = params.get("Server")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.905/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.905/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.905/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.904/setup.py` & `tencentcloud-sdk-python-cfw-3.0.905/setup.py`

 * *Files identical despite different names*

