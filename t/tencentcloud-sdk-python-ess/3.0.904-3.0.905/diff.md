# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.904.tar", last modified: Thu Jun  1 02:34:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.905.tar", last modified: Fri Jun  2 00:28:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.904.tar` & `tencentcloud-sdk-python-ess-3.0.905.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24243 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   225454 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:34:42.000000 tencentcloud-sdk-python-ess-3.0.904/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24243 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   225854 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.904/README.rst` & `tencentcloud-sdk-python-ess-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.904/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,15 @@
 
     def __init__(self):
         r"""
         :param ApplicationId: 应用号
         :type ApplicationId: str
         :param OrganizationId: 主机构ID
         :type OrganizationId: str
-        :param OperatorId: 经办人的用户ID
+        :param OperatorId: 经办人的用户ID，同UserId
         :type OperatorId: str
         :param SubOrganizationId: 下属机构ID
         :type SubOrganizationId: str
         """
         self.ApplicationId = None
         self.OrganizationId = None
         self.OperatorId = None
@@ -3901,17 +3901,17 @@
 class FileUrl(AbstractModel):
     """下载文件的URL信息
 
     """
 
     def __init__(self):
         r"""
-        :param Url: 下载文件的URL
+        :param Url: 下载文件的URL，有效期为输入的UrlTtl，默认5分钟
         :type Url: str
-        :param Option: 下载文件的附加信息
+        :param Option: 下载文件的附加信息。如果是pdf文件，会返回pdf文件每页的有效高宽
 注意：此字段可能返回 null，表示取不到有效值。
         :type Option: str
         """
         self.Url = None
         self.Option = None
 
 
@@ -3930,20 +3930,20 @@
 class FillApproverInfo(AbstractModel):
     """补充签署人信息
 
     """
 
     def __init__(self):
         r"""
-        :param RecipientId: 签署人签署Id
+        :param RecipientId: 对应模板中的参与方ID
         :type RecipientId: str
         :param ApproverSource: 签署人来源
 WEWORKAPP: 企业微信
         :type ApproverSource: str
-        :param CustomUserId: 企业自定义账号Id
+        :param CustomUserId: 企业自定义账号ID
 WEWORKAPP场景下指企业自有应用获取企微明文的userid
         :type CustomUserId: str
         """
         self.RecipientId = None
         self.ApproverSource = None
         self.CustomUserId = None
 
@@ -3992,55 +3992,58 @@
 class FlowApproverDetail(AbstractModel):
     """签署人详情信息
 
     """
 
     def __init__(self):
         r"""
-        :param ApproveMessage: 签署人信息
+        :param ApproveMessage: 签署时的相关信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveMessage: str
-        :param ApproveName: 签署人名字
+        :param ApproveName: 签署方姓名
         :type ApproveName: str
-        :param ApproveStatus: 签署人的状态
+        :param ApproveStatus: 签署方的签署状态
 0：还没有发起
 1：流程中 没有开始处理
-2：待处理
-3：签署态
-4：拒绝态
-5：过期没人处理
-6：取消态
+2：待签署
+3：已签署
+4：已拒绝
+5：已过期
+6：已撤销
 7：还没有预发起
 8：待填写
 9：因为各种原因而终止
+10：填写完成
+15：已解除
+19：转他人处理
         :type ApproveStatus: int
-        :param ReceiptId: 模板配置时候的签署人id,与控件绑定
+        :param ReceiptId: 模板配置中的参与方ID,与控件绑定
         :type ReceiptId: str
-        :param CustomUserId: 客户自定义userId
+        :param CustomUserId: 客户自定义的用户ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type CustomUserId: str
         :param Mobile: 签署人手机号
         :type Mobile: str
-        :param SignOrder: 签署顺序
+        :param SignOrder: 签署顺序，如果是有序签署，签署顺序从小到大
         :type SignOrder: int
-        :param ApproveTime: 签署人签署时间
+        :param ApproveTime: 签署人签署时间，时间戳，单位秒
         :type ApproveTime: int
-        :param ApproveType: 参与者类型
+        :param ApproveType: 签署方类型，ORGANIZATION-企业员工，PERSON-个人，ENTERPRISESERVER-企业静默签
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveType: str
-        :param ApproverSource: 签署人侧用户来源
+        :param ApproverSource: 签署方侧用户来源，如WEWORKAPP-企业微信等
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproverSource: str
-        :param CustomApproverTag: 客户自定义签署人标识
+        :param CustomApproverTag: 客户自定义签署方标识
 注意：此字段可能返回 null，表示取不到有效值。
         :type CustomApproverTag: str
-        :param OrganizationId: 签署人企业Id
+        :param OrganizationId: 签署方企业Id
 注意：此字段可能返回 null，表示取不到有效值。
         :type OrganizationId: str
-        :param OrganizationName: 签署人企业名称
+        :param OrganizationName: 签署方企业名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type OrganizationName: str
         """
         self.ApproveMessage = None
         self.ApproveName = None
         self.ApproveStatus = None
         self.ReceiptId = None
@@ -4126,38 +4129,39 @@
 class FlowBrief(AbstractModel):
     """流程信息摘要
 
     """
 
     def __init__(self):
         r"""
-        :param FlowId: 流程的编号
+        :param FlowId: 流程的编号ID
         :type FlowId: str
         :param FlowName: 流程的名称
         :type FlowName: str
-        :param FlowDescription: 流程的描述
+        :param FlowDescription: 流程的描述信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowDescription: str
         :param FlowType: 流程的类型
         :type FlowType: str
         :param FlowStatus: 流程状态
-- `0`  还没有发起
-- `1`  未签署
-- `2`  部分签署
-- `3`  已退回
-- `4`  完成签署
-- `5`  已过期
-- `6`  已取消
-- `7`  还没有预发起
-- `8`  等待填写
-- `9`  部分填写
-- `10`  拒填
+- 0 还没有发起
+- 1 待签署
+- 2 部分签署
+- 3 已拒签
+- 4 已签署
+- 5 已过期
+- 6 已撤销
+- 7 还没有预发起
+- 8 等待填写
+- 9 部分填写
+- 10 拒填
+- 21 已解除
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowStatus: int
-        :param CreatedOn: 流程创建的时间戳
+        :param CreatedOn: 流程创建的时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreatedOn: int
         :param FlowMessage: 拒签或者取消的原因描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowMessage: str
         :param Creator:  合同发起人userId
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4203,29 +4207,29 @@
 
     def __init__(self):
         r"""
         :param ApproverType: 参与者类型：
 0：企业
 1：个人
 3：企业静默签署
-注：类型为3（企业静默签署）时，此接口会默认完成该签署方的签署。静默签署仅进行盖章操作，不能自动签名。
+注：类型为3（企业静默签署）时，会默认完成该签署方的签署。静默签署仅进行盖章操作，不能是手写签名。
         :type ApproverType: int
         :param OrganizationName: 如果签署方为企业，需要填入企业全称
         :type OrganizationName: str
         :param ApproverName: 签署方经办人姓名
         :type ApproverName: str
         :param ApproverMobile: 签署方经办人手机号码
         :type ApproverMobile: str
         :param ApproverIdCardType: 签署方经办人证件类型ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
         :type ApproverIdCardType: str
         :param ApproverIdCardNumber: 签署方经办人证件号码
         :type ApproverIdCardNumber: str
-        :param RecipientId: 签署方经办人在模板中的角色ID
+        :param RecipientId: 签署方经办人在模板中的参与方ID
         :type RecipientId: str
         :param VerifyChannel: 签署意愿确认渠道,WEIXINAPP:人脸识别
         :type VerifyChannel: list of str
         :param NotifyType: 是否发送短信，sms--短信通知，none--不通知，默认为sms；发起方=签署方时不发送短信
         :type NotifyType: str
         :param IsFullText: 合同强制需要阅读全文，无需传此参数
         :type IsFullText: bool
@@ -4301,43 +4305,44 @@
 class FlowDetailInfo(AbstractModel):
     """此结构体(FlowDetailInfo)描述的是合同(流程)的详细信息
 
     """
 
     def __init__(self):
         r"""
-        :param FlowId: 合同(流程)的Id
+        :param FlowId: 合同(流程)的ID
         :type FlowId: str
         :param FlowName: 合同(流程)的名字
         :type FlowName: str
         :param FlowType: 合同(流程)的类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowType: str
         :param FlowStatus: 流程状态
 - 0 还没有发起
-- 1 未签署
+- 1 待签署
 - 2 部分签署
-- 3 已退回
-- 4 完成签署
+- 3 已拒签
+- 4 已签署
 - 5 已过期
-- 6 已取消
+- 6 已撤销
 - 7 还没有预发起
 - 8 等待填写
 - 9 部分填写
 - 10 拒填
+- 21 已解除
         :type FlowStatus: int
         :param FlowMessage: 合同(流程)的信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowMessage: str
         :param FlowDescription: 流程的描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowDescription: str
-        :param CreatedOn: 合同(流程)的创建时间戳
+        :param CreatedOn: 合同(流程)的创建时间戳，单位秒
         :type CreatedOn: int
-        :param FlowApproverInfos: 合同(流程)的签署人数组
+        :param FlowApproverInfos: 合同(流程)的签署方数组
         :type FlowApproverInfos: list of FlowApproverDetail
         :param CcInfos: 合同(流程)的关注方信息列表
         :type CcInfos: list of FlowApproverDetail
         :param Creator: 合同发起人UserId
 注意：此字段可能返回 null，表示取不到有效值。
         :type Creator: str
         """
```

### Comparing `tencentcloud-sdk-python-ess-3.0.904/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.905/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.904/setup.py` & `tencentcloud-sdk-python-ess-3.0.905/setup.py`

 * *Files identical despite different names*

