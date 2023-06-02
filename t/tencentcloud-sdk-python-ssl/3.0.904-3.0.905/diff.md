# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.904.tar", last modified: Thu Jun  1 02:45:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.905.tar", last modified: Fri Jun  2 00:38:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.904.tar` & `tencentcloud-sdk-python-ssl-3.0.905.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     8810 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217801 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    48579 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:45:20.000000 tencentcloud-sdk-python-ssl-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:45:21.000000 tencentcloud-sdk-python-ssl-3.0.904/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     9587 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222301 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    49507 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:38:18.000000 tencentcloud-sdk-python-ssl-3.0.905/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/README.rst` & `tencentcloud-sdk-python-ssl-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,14 +172,17 @@
 
 # 角色不存在，请前往授权。
 FAILEDOPERATION_ROLENOTFOUNDAUTHORIZATION = 'FailedOperation.RoleNotFoundAuthorization'
 
 # 系统错误。
 FAILEDOPERATION_SYSTEMERROR = 'FailedOperation.SystemError'
 
+# 计费中心错误。
+FAILEDOPERATION_TRADEERROR = 'FailedOperation.TradeError'
+
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 后端服务响应为空。
 INTERNALERROR_BACKENDRESPONSEEMPTY = 'InternalError.BackendResponseEmpty'
 
 # 后端服务响应错误。
@@ -193,17 +196,38 @@
 
 # 证书数量超出限制。
 INVALIDPARAMETER_CERTIFICATESNUMBEREXCEEDED = 'InvalidParameter.CertificatesNumberExceeded'
 
 # 包含无效的证书ID。
 INVALIDPARAMETER_CONTAINSINVALIDCERTIFICATEID = 'InvalidParameter.ContainsInvalidCertificateId'
 
+# 域名数量无效。
+INVALIDPARAMETER_DOMAINCOUNTINVALID = 'InvalidParameter.DomainCountInvalid'
+
+# 域名无效，请重新输入。
+INVALIDPARAMETER_DOMAININVALID = 'InvalidParameter.DomainInvalid'
+
 # 权益点ID列表无效。
 INVALIDPARAMETER_PACKAGEIDSINVALID = 'InvalidParameter.PackageIdsInvalid'
 
+# 证书期限无效。
+INVALIDPARAMETER_PERIODINVALID = 'InvalidParameter.PeriodInvalid'
+
+# 产品PID无效。
+INVALIDPARAMETER_PRODUCTPIDINVALID = 'InvalidParameter.ProductPidInvalid'
+
+# 算法无效。
+INVALIDPARAMETER_RENEWALGORITHMINVALID = 'InvalidParameter.RenewAlgorithmInvalid'
+
+# CSR无效。
+INVALIDPARAMETER_RENEWCSRINVALID = 'InvalidParameter.RenewCsrInvalid'
+
+# 生成CSR方式无效。
+INVALIDPARAMETER_RENEWGENCSRMETHODINVALID = 'InvalidParameter.RenewGenCsrMethodInvalid'
+
 # 参数有误。
 INVALIDPARAMETER_WITHDETAILREASON = 'InvalidParameter.WithDetailReason'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 单位时间内接口请求频率达到限制。
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -962,14 +962,132 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CreateCertificateByPackageRequest(AbstractModel):
+    """CreateCertificateByPackage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductPid: 证书产品PID。
+        :type ProductPid: int
+        :param PackageIds: 要消耗的权益包ID。
+        :type PackageIds: list of str
+        :param DomainCount: 证书域名数量。
+        :type DomainCount: str
+        :param Period: 多年期证书年限。
+        :type Period: int
+        :param OldCertificateId: 要续费的原证书ID（续费时填写）。
+        :type OldCertificateId: str
+        :param RenewGenCsrMethod: 续费时CSR生成方式（original、upload、online）。
+        :type RenewGenCsrMethod: str
+        :param RenewCsr: 续费时选择上传CSR时填写CSR。
+        :type RenewCsr: str
+        :param RenewAlgorithmType: 续费证书CSR的算法类型。
+        :type RenewAlgorithmType: str
+        :param RenewAlgorithmParam: 续费证书CSR的算法参数。
+        :type RenewAlgorithmParam: str
+        :param ProjectId: 项目ID。
+        :type ProjectId: int
+        :param Tags: 标签。
+        :type Tags: list of Tags
+        :param RenewKeyPass: 续费证书的私钥密码。
+        :type RenewKeyPass: str
+        :param DomainNames: 批量购买证书时预填写的域名。
+        :type DomainNames: str
+        :param CertificateCount: 批量购买证书数量。
+        :type CertificateCount: int
+        :param ManagerId: 预填写的管理人ID。
+        :type ManagerId: int
+        :param CompanyId: 预填写的公司ID。
+        :type CompanyId: int
+        :param VerifyType: 验证方式
+        :type VerifyType: str
+        """
+        self.ProductPid = None
+        self.PackageIds = None
+        self.DomainCount = None
+        self.Period = None
+        self.OldCertificateId = None
+        self.RenewGenCsrMethod = None
+        self.RenewCsr = None
+        self.RenewAlgorithmType = None
+        self.RenewAlgorithmParam = None
+        self.ProjectId = None
+        self.Tags = None
+        self.RenewKeyPass = None
+        self.DomainNames = None
+        self.CertificateCount = None
+        self.ManagerId = None
+        self.CompanyId = None
+        self.VerifyType = None
+
+
+    def _deserialize(self, params):
+        self.ProductPid = params.get("ProductPid")
+        self.PackageIds = params.get("PackageIds")
+        self.DomainCount = params.get("DomainCount")
+        self.Period = params.get("Period")
+        self.OldCertificateId = params.get("OldCertificateId")
+        self.RenewGenCsrMethod = params.get("RenewGenCsrMethod")
+        self.RenewCsr = params.get("RenewCsr")
+        self.RenewAlgorithmType = params.get("RenewAlgorithmType")
+        self.RenewAlgorithmParam = params.get("RenewAlgorithmParam")
+        self.ProjectId = params.get("ProjectId")
+        if params.get("Tags") is not None:
+            self.Tags = []
+            for item in params.get("Tags"):
+                obj = Tags()
+                obj._deserialize(item)
+                self.Tags.append(obj)
+        self.RenewKeyPass = params.get("RenewKeyPass")
+        self.DomainNames = params.get("DomainNames")
+        self.CertificateCount = params.get("CertificateCount")
+        self.ManagerId = params.get("ManagerId")
+        self.CompanyId = params.get("CompanyId")
+        self.VerifyType = params.get("VerifyType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateCertificateByPackageResponse(AbstractModel):
+    """CreateCertificateByPackage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 证书ID。
+        :type CertificateId: str
+        :param CertificateIds: 批量购买证书时返回多个证书ID。
+        :type CertificateIds: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.CertificateId = None
+        self.CertificateIds = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.CertificateIds = params.get("CertificateIds")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateCertificateRequest(AbstractModel):
     """CreateCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.905/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateCertificateByPackage(self, request):
+        """使用权益点创建证书
+
+        :param request: Request instance for CreateCertificateByPackage.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.CreateCertificateByPackageRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.CreateCertificateByPackageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCertificateByPackage", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCertificateByPackageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteCertificate(self, request):
         """本接口（DeleteCertificate）用于删除证书。
 
         :param request: Request instance for DeleteCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DeleteCertificateRequest`
         :rtype: :class:`tencentcloud.ssl.v20191205.models.DeleteCertificateResponse`
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.905/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/setup.py` & `tencentcloud-sdk-python-ssl-3.0.905/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.904/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.905/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

