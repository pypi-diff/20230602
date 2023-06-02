# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.904.tar", last modified: Thu Jun  1 02:47:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.905.tar", last modified: Fri Jun  2 00:40:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.904.tar` & `tencentcloud-sdk-python-tcss-3.0.905.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1041280 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:47:25.000000 tencentcloud-sdk-python-tcss-3.0.904/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   317082 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1046148 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:40:19.000000 tencentcloud-sdk-python-tcss-3.0.905/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/README.rst` & `tencentcloud-sdk-python-tcss-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6189,14 +6189,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeVulRegistryImageList(self, request):
+        """查询漏洞影响的仓库镜像列表
+
+        :param request: Request instance for DescribeVulRegistryImageList.
+        :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulRegistryImageListRequest`
+        :rtype: :class:`tencentcloud.tcss.v20201101.models.DescribeVulRegistryImageListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeVulRegistryImageList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeVulRegistryImageListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeVulScanAuthorizedImageSummary(self, request):
         """统计漏洞扫描页已授权和未扫描镜像数
 
         :param request: Request instance for DescribeVulScanAuthorizedImageSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulScanAuthorizedImageSummaryRequest`
         :rtype: :class:`tencentcloud.tcss.v20201101.models.DescribeVulScanAuthorizedImageSummaryResponse`
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.905/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -20708,14 +20708,101 @@
         self.HighLevelVulCount = params.get("HighLevelVulCount")
         self.MediumLevelVulCount = params.get("MediumLevelVulCount")
         self.LowLevelVulCount = params.get("LowLevelVulCount")
         self.CriticalLevelVulCount = params.get("CriticalLevelVulCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeVulRegistryImageListRequest(AbstractModel):
+    """DescribeVulRegistryImageList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PocID: 漏洞ID
+        :type PocID: str
+        :param Limit: 需要返回的数量，默认为10，最大值为100
+        :type Limit: int
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        :param Filters: 过滤条件。
+OnlyAffectedNewestImage bool 是否影响最新镜像
+ImageDigest 镜像Digest，支持模糊查询
+ImageId 镜像ID，支持模糊查询
+Namespace 命名空间，支持模糊查询
+ImageTag 镜像版本，支持模糊查询
+InstanceName 实例名称，支持模糊查询
+ImageName 镜像名，支持模糊查询
+ImageRepoAddress 镜像地址，支持模糊查询
+        :type Filters: list of AssetFilters
+        :param Order: 排序方式
+        :type Order: str
+        :param By: 排序字段
+        :type By: str
+        """
+        self.PocID = None
+        self.Limit = None
+        self.Offset = None
+        self.Filters = None
+        self.Order = None
+        self.By = None
+
+
+    def _deserialize(self, params):
+        self.PocID = params.get("PocID")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = AssetFilters()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.Order = params.get("Order")
+        self.By = params.get("By")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeVulRegistryImageListResponse(AbstractModel):
+    """DescribeVulRegistryImageList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 镜像总数
+        :type TotalCount: int
+        :param List: 仓库镜像列表
+        :type List: list of VulAffectedRegistryImageInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.List = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("List") is not None:
+            self.List = []
+            for item in params.get("List"):
+                obj = VulAffectedRegistryImageInfo()
+                obj._deserialize(item)
+                self.List.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeVulScanAuthorizedImageSummaryRequest(AbstractModel):
     """DescribeVulScanAuthorizedImageSummary请求参数结构体
 
     """
 
 
 class DescribeVulScanAuthorizedImageSummaryResponse(AbstractModel):
@@ -29412,14 +29499,71 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class VulAffectedRegistryImageInfo(AbstractModel):
+    """漏洞影响的仓库镜像列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageID: 镜像ID
+        :type ImageID: str
+        :param ImageName: 镜像名称
+        :type ImageName: str
+        :param ImageTag: 镜像版本
+        :type ImageTag: str
+        :param Namespace: 镜像命名空间
+        :type Namespace: str
+        :param ImageRepoAddress: 镜像地址
+        :type ImageRepoAddress: str
+        :param ComponentList: 组件列表
+        :type ComponentList: list of VulAffectedImageComponentInfo
+        :param IsLatestImage: 是否为镜像的最新版本
+        :type IsLatestImage: bool
+        :param ImageAssetId: 内部镜像资产ID
+        :type ImageAssetId: int
+        """
+        self.ImageID = None
+        self.ImageName = None
+        self.ImageTag = None
+        self.Namespace = None
+        self.ImageRepoAddress = None
+        self.ComponentList = None
+        self.IsLatestImage = None
+        self.ImageAssetId = None
+
+
+    def _deserialize(self, params):
+        self.ImageID = params.get("ImageID")
+        self.ImageName = params.get("ImageName")
+        self.ImageTag = params.get("ImageTag")
+        self.Namespace = params.get("Namespace")
+        self.ImageRepoAddress = params.get("ImageRepoAddress")
+        if params.get("ComponentList") is not None:
+            self.ComponentList = []
+            for item in params.get("ComponentList"):
+                obj = VulAffectedImageComponentInfo()
+                obj._deserialize(item)
+                self.ComponentList.append(obj)
+        self.IsLatestImage = params.get("IsLatestImage")
+        self.ImageAssetId = params.get("ImageAssetId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class VulDefenceEvent(AbstractModel):
     """漏洞防御事件详情
 
     """
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.905/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.905/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.904/setup.py` & `tencentcloud-sdk-python-tcss-3.0.905/setup.py`

 * *Files identical despite different names*

