# Comparing `tmp/antchain_iam-3.12.4.tar.gz` & `tmp/antchain_iam-3.12.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_iam-3.12.4.tar", last modified: Mon Mar  8 13:04:54 2021, max compression
+gzip compressed data, was "dist/antchain_iam-3.12.8.tar", last modified: Fri Jun  2 09:48:09 2023, max compression
```

## Comparing `antchain_iam-3.12.4.tar` & `antchain_iam-3.12.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/
--rw-r--r--   0 root         (0) root         (0)      600 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2171 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      812 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      998 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_iam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2171 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_iam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_iam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_iam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_iam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_iam.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_sdk_iam/
--rw-r--r--   0 root         (0) root         (0)       22 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_sdk_iam/__init__.py
--rw-r--r--   0 root         (0) root         (0)   116401 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_sdk_iam/client.py
--rw-r--r--   0 root         (0) root         (0)   207148 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/antchain_sdk_iam/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2021-03-08 13:04:54.000000 antchain_iam-3.12.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_iam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_iam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_iam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_iam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/antchain_sdk_iam/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/antchain_sdk_iam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   169248 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/antchain_sdk_iam/client.py
+-rw-r--r--   0 root         (0) root         (0)   334227 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/antchain_sdk_iam/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 09:48:09.000000 antchain_iam-3.12.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-02 09:48:08.000000 antchain_iam-3.12.8/setup.py
```

### Comparing `antchain_iam-3.12.4/LICENSE` & `antchain_iam-3.12.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_iam-3.12.4/PKG-INFO` & `antchain_iam-3.12.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_iam
-Version: 3.12.4
+Version: 3.12.8
 Summary: Ant Chain IAM SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_iam
-        pip install antchain_sdk_iam
+        # Install the antchain-iam
+        pip install antchain-iam
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_iam-3.12.4/README-CN.md` & `antchain_iam-3.12.8/README-CN.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain_sdk_iam
-pip install antchain_sdk_iam
+# 安装 antchain-iam
+pip install antchain-iam
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_iam-3.12.4/README.md` & `antchain_iam-3.12.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain_sdk_iam
-pip install antchain_sdk_iam
+# Install the antchain-iam
+pip install antchain-iam
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_iam-3.12.4/antchain_iam.egg-info/PKG-INFO` & `antchain_iam-3.12.8/antchain_iam.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-iam
-Version: 3.12.4
+Version: 3.12.8
 Summary: Ant Chain IAM SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_iam
-        pip install antchain_sdk_iam
+        # Install the antchain-iam
+        pip install antchain-iam
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_iam-3.12.4/antchain_sdk_iam/client.py` & `antchain_iam-3.12.8/antchain_sdk_iam/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 import time
 
 from Tea.exceptions import TeaException, UnretryableException
 from Tea.request import TeaRequest
 from Tea.core import TeaCore
+from antchain_alipay_util.antchain_utils import AntchainUtils
 from typing import Dict
 
 from antchain_sdk_iam import models as iam_models
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_tea_util import models as util_models
-from antchain_alipay_util.client import Client as AntchainUtilClient
 from alibabacloud_rpc_util.client import Client as RPCUtilClient
 
 
 class Client:
     _endpoint: str = None
     _region_id: str = None
     _access_key_id: str = None
@@ -94,27 +94,26 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
-            'ignoreSSL': runtime.ignore_ssl,
-            # 阿里云资源结构体
+            'ignoreSSL': runtime.ignore_ssl
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -127,39 +126,41 @@
                 _request.protocol = UtilClient.default_string(self._protocol, protocol)
                 _request.method = method
                 _request.pathname = pathname
                 _request.query = {
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
-                    'req_time': AntchainUtilClient.get_timestamp(),
-                    'req_msg_id': AntchainUtilClient.get_nonce(),
+                    'req_time': AntchainUtils.get_timestamp(),
+                    'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '3.12.4'
+                    'sdk_version': '3.12.8',
+                    '_prod_code': 'IAM',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
                 tmp = UtilClient.anyify_map_value(RPCUtilClient.query(request))
                 _request.body = UtilClient.to_form_string(tmp)
                 _request.headers['content-type'] = 'application/x-www-form-urlencoded'
                 signed_param = TeaCore.merge(_request.query,
                     RPCUtilClient.query(request))
-                _request.query['sign'] = AntchainUtilClient.get_signature(signed_param, self._access_key_secret)
+                _request.query['sign'] = AntchainUtils.get_signature(signed_param, self._access_key_secret)
                 _last_request = _request
                 _response = TeaCore.do_action(_request, _runtime)
                 raw = UtilClient.read_as_string(_response.body)
                 obj = UtilClient.parse_json(raw)
                 res = UtilClient.assert_as_map(obj)
                 resp = UtilClient.assert_as_map(res.get('response'))
-                if AntchainUtilClient.has_error(raw, self._access_key_secret):
+                if AntchainUtils.has_error(raw, self._access_key_secret):
                     raise TeaException({
                         'message': resp.get('result_msg'),
                         'data': resp,
                         'code': resp.get('result_code')
                     })
                 return resp
             except Exception as e:
@@ -196,27 +197,26 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
-            'ignoreSSL': runtime.ignore_ssl,
-            # 阿里云资源结构体
+            'ignoreSSL': runtime.ignore_ssl
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -229,39 +229,41 @@
                 _request.protocol = UtilClient.default_string(self._protocol, protocol)
                 _request.method = method
                 _request.pathname = pathname
                 _request.query = {
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
-                    'req_time': AntchainUtilClient.get_timestamp(),
-                    'req_msg_id': AntchainUtilClient.get_nonce(),
+                    'req_time': AntchainUtils.get_timestamp(),
+                    'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '3.12.4'
+                    'sdk_version': '3.12.8',
+                    '_prod_code': 'IAM',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
                 tmp = UtilClient.anyify_map_value(RPCUtilClient.query(request))
                 _request.body = UtilClient.to_form_string(tmp)
                 _request.headers['content-type'] = 'application/x-www-form-urlencoded'
                 signed_param = TeaCore.merge(_request.query,
                     RPCUtilClient.query(request))
-                _request.query['sign'] = AntchainUtilClient.get_signature(signed_param, self._access_key_secret)
+                _request.query['sign'] = AntchainUtils.get_signature(signed_param, self._access_key_secret)
                 _last_request = _request
                 _response = await TeaCore.async_do_action(_request, _runtime)
                 raw = await UtilClient.read_as_string_async(_response.body)
                 obj = UtilClient.parse_json(raw)
                 res = UtilClient.assert_as_map(obj)
                 resp = UtilClient.assert_as_map(res.get('response'))
-                if AntchainUtilClient.has_error(raw, self._access_key_secret):
+                if AntchainUtils.has_error(raw, self._access_key_secret):
                     raise TeaException({
                         'message': resp.get('result_msg'),
                         'data': resp,
                         'code': resp.get('result_code')
                     })
                 return resp
             except Exception as e:
@@ -302,30 +304,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetRoleResponse:
         """
         Description: 获取Role
         Summary: 获取角色
         """
         UtilClient.validate_model(request)
-        return iam_models.GetRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetRoleResponse(),
             self.do_request('1.0', 'antcloud.iam.role.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_role_ex_async(
         self,
         request: iam_models.GetRoleRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetRoleResponse:
         """
         Description: 获取Role
         Summary: 获取角色
         """
         UtilClient.validate_model(request)
-        return iam_models.GetRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetRoleResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_policy(
         self,
         request: iam_models.QueryPolicyRequest,
     ) -> iam_models.QueryPolicyResponse:
@@ -356,30 +360,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryPolicyResponse:
         """
         Description: 查询授权对象在指定租户下的所有授权策略
         Summary: 查询授权
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryPolicyResponse(),
             self.do_request('1.0', 'antcloud.iam.policy.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_policy_ex_async(
         self,
         request: iam_models.QueryPolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryPolicyResponse:
         """
         Description: 查询授权对象在指定租户下的所有授权策略
         Summary: 查询授权
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryPolicyResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.policy.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_group(
         self,
         request: iam_models.QueryGroupRequest,
     ) -> iam_models.QueryGroupResponse:
@@ -410,30 +416,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryGroupResponse:
         """
         Description: 查询租户下的权限组
         Summary: 查询授权组
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryGroupResponse(),
             self.do_request('1.0', 'antcloud.iam.group.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_group_ex_async(
         self,
         request: iam_models.QueryGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryGroupResponse:
         """
         Description: 查询租户下的权限组
         Summary: 查询授权组
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryGroupResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_policy(
         self,
         request: iam_models.CreatePolicyRequest,
     ) -> iam_models.CreatePolicyResponse:
@@ -464,30 +472,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreatePolicyResponse:
         """
         Description: 创建授权策略
         Summary: 创建授权策略
         """
         UtilClient.validate_model(request)
-        return iam_models.CreatePolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreatePolicyResponse(),
             self.do_request('1.0', 'antcloud.iam.policy.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_policy_ex_async(
         self,
         request: iam_models.CreatePolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreatePolicyResponse:
         """
         Description: 创建授权策略
         Summary: 创建授权策略
         """
         UtilClient.validate_model(request)
-        return iam_models.CreatePolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreatePolicyResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.policy.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def delete_policy(
         self,
         request: iam_models.DeletePolicyRequest,
     ) -> iam_models.DeletePolicyResponse:
@@ -518,30 +528,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeletePolicyResponse:
         """
         Description: 删除授权策略
         Summary: 删除授权策略
         """
         UtilClient.validate_model(request)
-        return iam_models.DeletePolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeletePolicyResponse(),
             self.do_request('1.0', 'antcloud.iam.policy.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def delete_policy_ex_async(
         self,
         request: iam_models.DeletePolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeletePolicyResponse:
         """
         Description: 删除授权策略
         Summary: 删除授权策略
         """
         UtilClient.validate_model(request)
-        return iam_models.DeletePolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeletePolicyResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.policy.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def attach_policy(
         self,
         request: iam_models.AttachPolicyRequest,
     ) -> iam_models.AttachPolicyResponse:
@@ -572,30 +584,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AttachPolicyResponse:
         """
         Description: 授权策略赋予某个对象
         Summary: 添加授权
         """
         UtilClient.validate_model(request)
-        return iam_models.AttachPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AttachPolicyResponse(),
             self.do_request('1.0', 'antcloud.iam.policy.attach', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def attach_policy_ex_async(
         self,
         request: iam_models.AttachPolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AttachPolicyResponse:
         """
         Description: 授权策略赋予某个对象
         Summary: 添加授权
         """
         UtilClient.validate_model(request)
-        return iam_models.AttachPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AttachPolicyResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.policy.attach', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def detach_policy(
         self,
         request: iam_models.DetachPolicyRequest,
     ) -> iam_models.DetachPolicyResponse:
@@ -626,30 +640,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DetachPolicyResponse:
         """
         Description: 解除授权对象的授权策略
         Summary: 解除授权
         """
         UtilClient.validate_model(request)
-        return iam_models.DetachPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DetachPolicyResponse(),
             self.do_request('1.0', 'antcloud.iam.policy.detach', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def detach_policy_ex_async(
         self,
         request: iam_models.DetachPolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DetachPolicyResponse:
         """
         Description: 解除授权对象的授权策略
         Summary: 解除授权
         """
         UtilClient.validate_model(request)
-        return iam_models.DetachPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DetachPolicyResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.policy.detach', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def list_policy(
         self,
         request: iam_models.ListPolicyRequest,
     ) -> iam_models.ListPolicyResponse:
@@ -680,30 +696,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListPolicyResponse:
         """
         Description: 查询授权对象在指定租户下的所有授权策略,如果是操作员，包含其所在组的授权
         Summary: 查询授权
         """
         UtilClient.validate_model(request)
-        return iam_models.ListPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListPolicyResponse(),
             self.do_request('1.0', 'antcloud.iam.policy.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def list_policy_ex_async(
         self,
         request: iam_models.ListPolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListPolicyResponse:
         """
         Description: 查询授权对象在指定租户下的所有授权策略,如果是操作员，包含其所在组的授权
         Summary: 查询授权
         """
         UtilClient.validate_model(request)
-        return iam_models.ListPolicyResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListPolicyResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.policy.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def judge_authority(
         self,
         request: iam_models.JudgeAuthorityRequest,
     ) -> iam_models.JudgeAuthorityResponse:
@@ -734,30 +752,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeAuthorityResponse:
         """
         Description: 授权对象的权限校验
         Summary: 校验权限
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeAuthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeAuthorityResponse(),
             self.do_request('1.0', 'antcloud.iam.authority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def judge_authority_ex_async(
         self,
         request: iam_models.JudgeAuthorityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeAuthorityResponse:
         """
         Description: 授权对象的权限校验
         Summary: 校验权限
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeAuthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeAuthorityResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.authority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_product_action(
         self,
         request: iam_models.CreateProductActionRequest,
     ) -> iam_models.CreateProductActionResponse:
@@ -788,30 +808,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateProductActionResponse:
         """
         Description: 添加产品操作元数据
         Summary: 创建产品操作点
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateProductActionResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateProductActionResponse(),
             self.do_request('1.0', 'antcloud.iam.product.action.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_product_action_ex_async(
         self,
         request: iam_models.CreateProductActionRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateProductActionResponse:
         """
         Description: 添加产品操作元数据
         Summary: 创建产品操作点
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateProductActionResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateProductActionResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.product.action.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def verify_oauth_token(
         self,
         request: iam_models.VerifyOauthTokenRequest,
     ) -> iam_models.VerifyOauthTokenResponse:
@@ -842,30 +864,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.VerifyOauthTokenResponse:
         """
         Description: 校验token合法性
         Summary: 校验token合法性
         """
         UtilClient.validate_model(request)
-        return iam_models.VerifyOauthTokenResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.VerifyOauthTokenResponse(),
             self.do_request('1.0', 'antcloud.iam.oauth.token.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def verify_oauth_token_ex_async(
         self,
         request: iam_models.VerifyOauthTokenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.VerifyOauthTokenResponse:
         """
         Description: 校验token合法性
         Summary: 校验token合法性
         """
         UtilClient.validate_model(request)
-        return iam_models.VerifyOauthTokenResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.VerifyOauthTokenResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.oauth.token.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def verify_session_token(
         self,
         request: iam_models.VerifySessionTokenRequest,
     ) -> iam_models.VerifySessionTokenResponse:
@@ -896,30 +920,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.VerifySessionTokenResponse:
         """
         Description: 校验中枢登录态合法性
         Summary: 校验中枢登录态合法性
         """
         UtilClient.validate_model(request)
-        return iam_models.VerifySessionTokenResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.VerifySessionTokenResponse(),
             self.do_request('1.0', 'antcloud.iam.session.token.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def verify_session_token_ex_async(
         self,
         request: iam_models.VerifySessionTokenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.VerifySessionTokenResponse:
         """
         Description: 校验中枢登录态合法性
         Summary: 校验中枢登录态合法性
         """
         UtilClient.validate_model(request)
-        return iam_models.VerifySessionTokenResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.VerifySessionTokenResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.session.token.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def list_role_operator(
         self,
         request: iam_models.ListRoleOperatorRequest,
     ) -> iam_models.ListRoleOperatorResponse:
@@ -950,30 +976,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListRoleOperatorResponse:
         """
         Description: 获取授予角色的操作员列表
         Summary: 授予角色的操作员列表
         """
         UtilClient.validate_model(request)
-        return iam_models.ListRoleOperatorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListRoleOperatorResponse(),
             self.do_request('1.0', 'antcloud.iam.role.operator.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def list_role_operator_ex_async(
         self,
         request: iam_models.ListRoleOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListRoleOperatorResponse:
         """
         Description: 获取授予角色的操作员列表
         Summary: 授予角色的操作员列表
         """
         UtilClient.validate_model(request)
-        return iam_models.ListRoleOperatorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListRoleOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.operator.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def apply_trustlogin_url(
         self,
         request: iam_models.ApplyTrustloginUrlRequest,
     ) -> iam_models.ApplyTrustloginUrlResponse:
@@ -1004,30 +1032,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ApplyTrustloginUrlResponse:
         """
         Description: 申请信任登录URL
         Summary: 申请信任登录URL
         """
         UtilClient.validate_model(request)
-        return iam_models.ApplyTrustloginUrlResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ApplyTrustloginUrlResponse(),
             self.do_request('1.0', 'antcloud.iam.trustlogin.url.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def apply_trustlogin_url_ex_async(
         self,
         request: iam_models.ApplyTrustloginUrlRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ApplyTrustloginUrlResponse:
         """
         Description: 申请信任登录URL
         Summary: 申请信任登录URL
         """
         UtilClient.validate_model(request)
-        return iam_models.ApplyTrustloginUrlResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ApplyTrustloginUrlResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.trustlogin.url.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def assume_sts(
         self,
         request: iam_models.AssumeStsRequest,
     ) -> iam_models.AssumeStsResponse:
@@ -1058,30 +1088,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AssumeStsResponse:
         """
         Description: 扮演虚拟身份，获取安全令牌
         Summary: 扮演虚拟身份，获取安全令牌
         """
         UtilClient.validate_model(request)
-        return iam_models.AssumeStsResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AssumeStsResponse(),
             self.do_request('1.0', 'antcloud.iam.sts.assume', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def assume_sts_ex_async(
         self,
         request: iam_models.AssumeStsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AssumeStsResponse:
         """
         Description: 扮演虚拟身份，获取安全令牌
         Summary: 扮演虚拟身份，获取安全令牌
         """
         UtilClient.validate_model(request)
-        return iam_models.AssumeStsResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AssumeStsResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.sts.assume', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_sts_actor(
         self,
         request: iam_models.CreateStsActorRequest,
     ) -> iam_models.CreateStsActorResponse:
@@ -1112,30 +1144,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateStsActorResponse:
         """
         Description: 创建虚拟身份
         Summary: 创建虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateStsActorResponse(),
             self.do_request('1.0', 'antcloud.iam.sts.actor.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_sts_actor_ex_async(
         self,
         request: iam_models.CreateStsActorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateStsActorResponse:
         """
         Description: 创建虚拟身份
         Summary: 创建虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateStsActorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.sts.actor.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def delete_sts_actor(
         self,
         request: iam_models.DeleteStsActorRequest,
     ) -> iam_models.DeleteStsActorResponse:
@@ -1166,30 +1200,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteStsActorResponse:
         """
         Description: 删除虚拟身份
         Summary: 删除虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteStsActorResponse(),
             self.do_request('1.0', 'antcloud.iam.sts.actor.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def delete_sts_actor_ex_async(
         self,
         request: iam_models.DeleteStsActorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteStsActorResponse:
         """
         Description: 删除虚拟身份
         Summary: 删除虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteStsActorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.sts.actor.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_sts_actor(
         self,
         request: iam_models.GetStsActorRequest,
     ) -> iam_models.GetStsActorResponse:
@@ -1220,30 +1256,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetStsActorResponse:
         """
         Description: 唯一查询虚拟身份
         Summary: 唯一查询虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.GetStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetStsActorResponse(),
             self.do_request('1.0', 'antcloud.iam.sts.actor.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_sts_actor_ex_async(
         self,
         request: iam_models.GetStsActorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetStsActorResponse:
         """
         Description: 唯一查询虚拟身份
         Summary: 唯一查询虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.GetStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetStsActorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.sts.actor.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def list_sts_actor(
         self,
         request: iam_models.ListStsActorRequest,
     ) -> iam_models.ListStsActorResponse:
@@ -1274,30 +1312,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListStsActorResponse:
         """
         Description: 获取租户内的虚拟身份
         Summary: 获取租户内的虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.ListStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListStsActorResponse(),
             self.do_request('1.0', 'antcloud.iam.sts.actor.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def list_sts_actor_ex_async(
         self,
         request: iam_models.ListStsActorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListStsActorResponse:
         """
         Description: 获取租户内的虚拟身份
         Summary: 获取租户内的虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.ListStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListStsActorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.sts.actor.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_sts_actor(
         self,
         request: iam_models.UpdateStsActorRequest,
     ) -> iam_models.UpdateStsActorResponse:
@@ -1328,30 +1368,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateStsActorResponse:
         """
         Description: 更新虚拟身份
         Summary: 更新虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateStsActorResponse(),
             self.do_request('1.0', 'antcloud.iam.sts.actor.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_sts_actor_ex_async(
         self,
         request: iam_models.UpdateStsActorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateStsActorResponse:
         """
         Description: 更新虚拟身份
         Summary: 更新虚拟身份
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateStsActorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateStsActorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.sts.actor.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_role(
         self,
         request: iam_models.QueryRoleRequest,
     ) -> iam_models.QueryRoleResponse:
@@ -1382,30 +1424,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryRoleResponse:
         """
         Description: 查询租户内可见的角色
         Summary: 角色查询
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryRoleResponse(),
             self.do_request('1.0', 'antcloud.iam.role.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_role_ex_async(
         self,
         request: iam_models.QueryRoleRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryRoleResponse:
         """
         Description: 查询租户内可见的角色
         Summary: 角色查询
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryRoleResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_iaasaccount_baseinfo(
         self,
         request: iam_models.GetIaasaccountBaseinfoRequest,
     ) -> iam_models.GetIaasaccountBaseinfoResponse:
@@ -1436,30 +1480,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetIaasaccountBaseinfoResponse:
         """
         Description: 获取租户Iaas账号基本信息
         Summary: 获取租户Iaas账号基本信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetIaasaccountBaseinfoResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetIaasaccountBaseinfoResponse(),
             self.do_request('1.0', 'antcloud.iam.iaasaccount.baseinfo.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_iaasaccount_baseinfo_ex_async(
         self,
         request: iam_models.GetIaasaccountBaseinfoRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetIaasaccountBaseinfoResponse:
         """
         Description: 获取租户Iaas账号基本信息
         Summary: 获取租户Iaas账号基本信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetIaasaccountBaseinfoResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetIaasaccountBaseinfoResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.iaasaccount.baseinfo.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def verify_password(
         self,
         request: iam_models.VerifyPasswordRequest,
     ) -> iam_models.VerifyPasswordResponse:
@@ -1490,30 +1536,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.VerifyPasswordResponse:
         """
         Description: 内部接口，用于校验密码是否正确，公有云环境只适用于操作员
         Summary: 校验密码是否正确
         """
         UtilClient.validate_model(request)
-        return iam_models.VerifyPasswordResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.VerifyPasswordResponse(),
             self.do_request('1.0', 'antcloud.iam.password.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def verify_password_ex_async(
         self,
         request: iam_models.VerifyPasswordRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.VerifyPasswordResponse:
         """
         Description: 内部接口，用于校验密码是否正确，公有云环境只适用于操作员
         Summary: 校验密码是否正确
         """
         UtilClient.validate_model(request)
-        return iam_models.VerifyPasswordResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.VerifyPasswordResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.password.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_operator_status(
         self,
         request: iam_models.UpdateOperatorStatusRequest,
     ) -> iam_models.UpdateOperatorStatusResponse:
@@ -1544,30 +1592,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateOperatorStatusResponse:
         """
         Description: 更显操作员状态，NORMAL为正常状态，FROZEN为冻结状态，INACTIVE为未激活状态
         Summary: 更新操作员状态
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateOperatorStatusResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateOperatorStatusResponse(),
             self.do_request('1.0', 'antcloud.iam.operator.status.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_operator_status_ex_async(
         self,
         request: iam_models.UpdateOperatorStatusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateOperatorStatusResponse:
         """
         Description: 更显操作员状态，NORMAL为正常状态，FROZEN为冻结状态，INACTIVE为未激活状态
         Summary: 更新操作员状态
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateOperatorStatusResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateOperatorStatusResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.operator.status.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def freeze_operator(
         self,
         request: iam_models.FreezeOperatorRequest,
     ) -> iam_models.FreezeOperatorResponse:
@@ -1598,30 +1648,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.FreezeOperatorResponse:
         """
         Description: 冻结操作员
         Summary: 冻结操作员
         """
         UtilClient.validate_model(request)
-        return iam_models.FreezeOperatorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.FreezeOperatorResponse(),
             self.do_request('1.0', 'antcloud.iam.operator.freeze', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def freeze_operator_ex_async(
         self,
         request: iam_models.FreezeOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.FreezeOperatorResponse:
         """
         Description: 冻结操作员
         Summary: 冻结操作员
         """
         UtilClient.validate_model(request)
-        return iam_models.FreezeOperatorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.FreezeOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.operator.freeze', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def unfreeze_operator(
         self,
         request: iam_models.UnfreezeOperatorRequest,
     ) -> iam_models.UnfreezeOperatorResponse:
@@ -1652,30 +1704,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UnfreezeOperatorResponse:
         """
         Description: 解冻操作员
         Summary: 解冻操作员
         """
         UtilClient.validate_model(request)
-        return iam_models.UnfreezeOperatorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UnfreezeOperatorResponse(),
             self.do_request('1.0', 'antcloud.iam.operator.unfreeze', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def unfreeze_operator_ex_async(
         self,
         request: iam_models.UnfreezeOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UnfreezeOperatorResponse:
         """
         Description: 解冻操作员
         Summary: 解冻操作员
         """
         UtilClient.validate_model(request)
-        return iam_models.UnfreezeOperatorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UnfreezeOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.operator.unfreeze', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_internal_master(
         self,
         request: iam_models.GetInternalMasterRequest,
     ) -> iam_models.GetInternalMasterResponse:
@@ -1706,30 +1760,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetInternalMasterResponse:
         """
         Description: 获取主账号信息
         Summary: 获取主账号信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetInternalMasterResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetInternalMasterResponse(),
             self.do_request('1.0', 'antcloud.iam.internal.master.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_internal_master_ex_async(
         self,
         request: iam_models.GetInternalMasterRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetInternalMasterResponse:
         """
         Description: 获取主账号信息
         Summary: 获取主账号信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetInternalMasterResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetInternalMasterResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.internal.master.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_aliyun_user(
         self,
         request: iam_models.GetAliyunUserRequest,
     ) -> iam_models.GetAliyunUserResponse:
@@ -1760,30 +1816,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetAliyunUserResponse:
         """
         Description: 公有云一方化场景下，获取用户信息，内部接口，专为一方化设计
         Summary: 获取阿里云用户信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetAliyunUserResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetAliyunUserResponse(),
             self.do_request('1.0', 'antcloud.iam.aliyun.user.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_aliyun_user_ex_async(
         self,
         request: iam_models.GetAliyunUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetAliyunUserResponse:
         """
         Description: 公有云一方化场景下，获取用户信息，内部接口，专为一方化设计
         Summary: 获取阿里云用户信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetAliyunUserResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetAliyunUserResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.aliyun.user.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def judge_aliyun_authority(
         self,
         request: iam_models.JudgeAliyunAuthorityRequest,
     ) -> iam_models.JudgeAliyunAuthorityResponse:
@@ -1814,30 +1872,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeAliyunAuthorityResponse:
         """
         Description: 阿里云RAM权限校验
         Summary: 阿里云RAM权限校验
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeAliyunAuthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeAliyunAuthorityResponse(),
             self.do_request('1.0', 'antcloud.iam.aliyun.authority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def judge_aliyun_authority_ex_async(
         self,
         request: iam_models.JudgeAliyunAuthorityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeAliyunAuthorityResponse:
         """
         Description: 阿里云RAM权限校验
         Summary: 阿里云RAM权限校验
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeAliyunAuthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeAliyunAuthorityResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.aliyun.authority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_session_accessor(
         self,
         request: iam_models.GetSessionAccessorRequest,
     ) -> iam_models.GetSessionAccessorResponse:
@@ -1868,30 +1928,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetSessionAccessorResponse:
         """
         Description: 根据登录态获取ak
         Summary: 根据登录态获取ak
         """
         UtilClient.validate_model(request)
-        return iam_models.GetSessionAccessorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetSessionAccessorResponse(),
             self.do_request('1.0', 'antcloud.iam.session.accessor.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_session_accessor_ex_async(
         self,
         request: iam_models.GetSessionAccessorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetSessionAccessorResponse:
         """
         Description: 根据登录态获取ak
         Summary: 根据登录态获取ak
         """
         UtilClient.validate_model(request)
-        return iam_models.GetSessionAccessorResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetSessionAccessorResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.session.accessor.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_password(
         self,
         request: iam_models.UpdatePasswordRequest,
     ) -> iam_models.UpdatePasswordResponse:
@@ -1922,30 +1984,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdatePasswordResponse:
         """
         Description: 更新密码
         Summary: 更新密码
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdatePasswordResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdatePasswordResponse(),
             self.do_request('1.0', 'antcloud.iam.password.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_password_ex_async(
         self,
         request: iam_models.UpdatePasswordRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdatePasswordResponse:
         """
         Description: 更新密码
         Summary: 更新密码
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdatePasswordResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdatePasswordResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.password.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def judge_multiauthority(
         self,
         request: iam_models.JudgeMultiauthorityRequest,
     ) -> iam_models.JudgeMultiauthorityResponse:
@@ -1976,30 +2040,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeMultiauthorityResponse:
         """
         Description: 蚂蚁侧批量鉴权
         Summary: 蚂蚁侧批量鉴权
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeMultiauthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeMultiauthorityResponse(),
             self.do_request('1.0', 'antcloud.iam.multiauthority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def judge_multiauthority_ex_async(
         self,
         request: iam_models.JudgeMultiauthorityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeMultiauthorityResponse:
         """
         Description: 蚂蚁侧批量鉴权
         Summary: 蚂蚁侧批量鉴权
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeMultiauthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeMultiauthorityResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.multiauthority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def judge_aliyun_multiauthority(
         self,
         request: iam_models.JudgeAliyunMultiauthorityRequest,
     ) -> iam_models.JudgeAliyunMultiauthorityResponse:
@@ -2030,30 +2096,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeAliyunMultiauthorityResponse:
         """
         Description: 阿里云批量鉴权
         Summary: 阿里云批量鉴权
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeAliyunMultiauthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeAliyunMultiauthorityResponse(),
             self.do_request('1.0', 'antcloud.iam.aliyun.multiauthority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def judge_aliyun_multiauthority_ex_async(
         self,
         request: iam_models.JudgeAliyunMultiauthorityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.JudgeAliyunMultiauthorityResponse:
         """
         Description: 阿里云批量鉴权
         Summary: 阿里云批量鉴权
         """
         UtilClient.validate_model(request)
-        return iam_models.JudgeAliyunMultiauthorityResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.JudgeAliyunMultiauthorityResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.aliyun.multiauthority.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_accessor_current(
         self,
         request: iam_models.GetAccessorCurrentRequest,
     ) -> iam_models.GetAccessorCurrentResponse:
@@ -2084,30 +2152,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetAccessorCurrentResponse:
         """
         Description: 辰霖
         Summary: 获取当前AK关联的用户实体信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetAccessorCurrentResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetAccessorCurrentResponse(),
             self.do_request('1.0', 'antcloud.iam.accessor.current.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_accessor_current_ex_async(
         self,
         request: iam_models.GetAccessorCurrentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetAccessorCurrentResponse:
         """
         Description: 辰霖
         Summary: 获取当前AK关联的用户实体信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetAccessorCurrentResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetAccessorCurrentResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.accessor.current.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_serviceaccount(
         self,
         request: iam_models.GetServiceaccountRequest,
     ) -> iam_models.GetServiceaccountResponse:
@@ -2138,30 +2208,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetServiceaccountResponse:
         """
         Description: 获取单个服务账号信息
         Summary: 获取单个服务账号信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetServiceaccountResponse(),
             self.do_request('1.0', 'antcloud.iam.serviceaccount.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_serviceaccount_ex_async(
         self,
         request: iam_models.GetServiceaccountRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetServiceaccountResponse:
         """
         Description: 获取单个服务账号信息
         Summary: 获取单个服务账号信息
         """
         UtilClient.validate_model(request)
-        return iam_models.GetServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetServiceaccountResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.serviceaccount.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_serviceaccount(
         self,
         request: iam_models.CreateServiceaccountRequest,
     ) -> iam_models.CreateServiceaccountResponse:
@@ -2192,30 +2264,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateServiceaccountResponse:
         """
         Description: 创建服务账号
         Summary: 创建服务账号
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateServiceaccountResponse(),
             self.do_request('1.0', 'antcloud.iam.serviceaccount.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_serviceaccount_ex_async(
         self,
         request: iam_models.CreateServiceaccountRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateServiceaccountResponse:
         """
         Description: 创建服务账号
         Summary: 创建服务账号
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateServiceaccountResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.serviceaccount.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def delete_serviceaccount(
         self,
         request: iam_models.DeleteServiceaccountRequest,
     ) -> iam_models.DeleteServiceaccountResponse:
@@ -2246,30 +2320,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteServiceaccountResponse:
         """
         Description: 删除服务账号
         Summary: 删除服务账号
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteServiceaccountResponse(),
             self.do_request('1.0', 'antcloud.iam.serviceaccount.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def delete_serviceaccount_ex_async(
         self,
         request: iam_models.DeleteServiceaccountRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteServiceaccountResponse:
         """
         Description: 删除服务账号
         Summary: 删除服务账号
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteServiceaccountResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.serviceaccount.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_serviceaccount(
         self,
         request: iam_models.UpdateServiceaccountRequest,
     ) -> iam_models.UpdateServiceaccountResponse:
@@ -2300,30 +2376,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateServiceaccountResponse:
         """
         Description: 更新服务账号信息
         Summary: 更新服务账号信息
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateServiceaccountResponse(),
             self.do_request('1.0', 'antcloud.iam.serviceaccount.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_serviceaccount_ex_async(
         self,
         request: iam_models.UpdateServiceaccountRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateServiceaccountResponse:
         """
         Description: 更新服务账号信息
         Summary: 更新服务账号信息
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateServiceaccountResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateServiceaccountResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.serviceaccount.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def remove_tenant_member(
         self,
         request: iam_models.RemoveTenantMemberRequest,
     ) -> iam_models.RemoveTenantMemberResponse:
@@ -2354,30 +2432,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.RemoveTenantMemberResponse:
         """
         Description: 移除租户成员
         Summary: 移除租户成员
         """
         UtilClient.validate_model(request)
-        return iam_models.RemoveTenantMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.RemoveTenantMemberResponse(),
             self.do_request('1.0', 'antcloud.iam.tenant.member.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def remove_tenant_member_ex_async(
         self,
         request: iam_models.RemoveTenantMemberRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.RemoveTenantMemberResponse:
         """
         Description: 移除租户成员
         Summary: 移除租户成员
         """
         UtilClient.validate_model(request)
-        return iam_models.RemoveTenantMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.RemoveTenantMemberResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.tenant.member.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_group(
         self,
         request: iam_models.CreateGroupRequest,
     ) -> iam_models.CreateGroupResponse:
@@ -2408,30 +2488,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateGroupResponse:
         """
         Description: 创建成员组
         Summary: 创建成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateGroupResponse(),
             self.do_request('1.0', 'antcloud.iam.group.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_group_ex_async(
         self,
         request: iam_models.CreateGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateGroupResponse:
         """
         Description: 创建成员组
         Summary: 创建成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateGroupResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def delete_group(
         self,
         request: iam_models.DeleteGroupRequest,
     ) -> iam_models.DeleteGroupResponse:
@@ -2462,30 +2544,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteGroupResponse:
         """
         Description: 删除成员组
         Summary: 删除成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteGroupResponse(),
             self.do_request('1.0', 'antcloud.iam.group.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def delete_group_ex_async(
         self,
         request: iam_models.DeleteGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteGroupResponse:
         """
         Description: 删除成员组
         Summary: 删除成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteGroupResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_group(
         self,
         request: iam_models.UpdateGroupRequest,
     ) -> iam_models.UpdateGroupResponse:
@@ -2516,30 +2600,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateGroupResponse:
         """
         Description: 更新成员组
         Summary: 更新成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateGroupResponse(),
             self.do_request('1.0', 'antcloud.iam.group.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_group_ex_async(
         self,
         request: iam_models.UpdateGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateGroupResponse:
         """
         Description: 更新成员组
         Summary: 更新成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateGroupResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def add_group_member(
         self,
         request: iam_models.AddGroupMemberRequest,
     ) -> iam_models.AddGroupMemberResponse:
@@ -2570,30 +2656,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AddGroupMemberResponse:
         """
         Description: 添加成员组成员
         Summary: 添加成员组成员
         """
         UtilClient.validate_model(request)
-        return iam_models.AddGroupMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AddGroupMemberResponse(),
             self.do_request('1.0', 'antcloud.iam.group.member.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def add_group_member_ex_async(
         self,
         request: iam_models.AddGroupMemberRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AddGroupMemberResponse:
         """
         Description: 添加成员组成员
         Summary: 添加成员组成员
         """
         UtilClient.validate_model(request)
-        return iam_models.AddGroupMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AddGroupMemberResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.member.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def remove_group_member(
         self,
         request: iam_models.RemoveGroupMemberRequest,
     ) -> iam_models.RemoveGroupMemberResponse:
@@ -2624,30 +2712,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.RemoveGroupMemberResponse:
         """
         Description: 移除成员组成员
         Summary: 移除成员组成员
         """
         UtilClient.validate_model(request)
-        return iam_models.RemoveGroupMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.RemoveGroupMemberResponse(),
             self.do_request('1.0', 'antcloud.iam.group.member.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def remove_group_member_ex_async(
         self,
         request: iam_models.RemoveGroupMemberRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.RemoveGroupMemberResponse:
         """
         Description: 移除成员组成员
         Summary: 移除成员组成员
         """
         UtilClient.validate_model(request)
-        return iam_models.RemoveGroupMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.RemoveGroupMemberResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.member.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_group(
         self,
         request: iam_models.GetGroupRequest,
     ) -> iam_models.GetGroupResponse:
@@ -2678,30 +2768,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetGroupResponse:
         """
         Description: 成员组基本信息查询
         Summary: 成员组基本信息查询
         """
         UtilClient.validate_model(request)
-        return iam_models.GetGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetGroupResponse(),
             self.do_request('1.0', 'antcloud.iam.group.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_group_ex_async(
         self,
         request: iam_models.GetGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.GetGroupResponse:
         """
         Description: 成员组基本信息查询
         Summary: 成员组基本信息查询
         """
         UtilClient.validate_model(request)
-        return iam_models.GetGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.GetGroupResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_group_member(
         self,
         request: iam_models.QueryGroupMemberRequest,
     ) -> iam_models.QueryGroupMemberResponse:
@@ -2732,30 +2824,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryGroupMemberResponse:
         """
         Description: 成员组成员查询
         Summary: 成员组成员查询
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryGroupMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryGroupMemberResponse(),
             self.do_request('1.0', 'antcloud.iam.group.member.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_group_member_ex_async(
         self,
         request: iam_models.QueryGroupMemberRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.QueryGroupMemberResponse:
         """
         Description: 成员组成员查询
         Summary: 成员组成员查询
         """
         UtilClient.validate_model(request)
-        return iam_models.QueryGroupMemberResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.QueryGroupMemberResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.group.member.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def list_operator_group(
         self,
         request: iam_models.ListOperatorGroupRequest,
     ) -> iam_models.ListOperatorGroupResponse:
@@ -2786,30 +2880,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListOperatorGroupResponse:
         """
         Description: 获取用户所在成员组
         Summary: 获取用户所在成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.ListOperatorGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListOperatorGroupResponse(),
             self.do_request('1.0', 'antcloud.iam.operator.group.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def list_operator_group_ex_async(
         self,
         request: iam_models.ListOperatorGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.ListOperatorGroupResponse:
         """
         Description: 获取用户所在成员组
         Summary: 获取用户所在成员组
         """
         UtilClient.validate_model(request)
-        return iam_models.ListOperatorGroupResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.ListOperatorGroupResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.operator.group.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def add_role_action(
         self,
         request: iam_models.AddRoleActionRequest,
     ) -> iam_models.AddRoleActionResponse:
@@ -2840,30 +2936,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AddRoleActionResponse:
         """
         Description: 为角色添加权限码
         Summary: 为角色添加权限码
         """
         UtilClient.validate_model(request)
-        return iam_models.AddRoleActionResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AddRoleActionResponse(),
             self.do_request('1.0', 'antcloud.iam.role.action.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def add_role_action_ex_async(
         self,
         request: iam_models.AddRoleActionRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.AddRoleActionResponse:
         """
         Description: 为角色添加权限码
         Summary: 为角色添加权限码
         """
         UtilClient.validate_model(request)
-        return iam_models.AddRoleActionResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.AddRoleActionResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.action.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def remove_role_action(
         self,
         request: iam_models.RemoveRoleActionRequest,
     ) -> iam_models.RemoveRoleActionResponse:
@@ -2894,30 +2992,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.RemoveRoleActionResponse:
         """
         Description: 移除角色权限
         Summary: 移除角色权限
         """
         UtilClient.validate_model(request)
-        return iam_models.RemoveRoleActionResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.RemoveRoleActionResponse(),
             self.do_request('1.0', 'antcloud.iam.role.action.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def remove_role_action_ex_async(
         self,
         request: iam_models.RemoveRoleActionRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.RemoveRoleActionResponse:
         """
         Description: 移除角色权限
         Summary: 移除角色权限
         """
         UtilClient.validate_model(request)
-        return iam_models.RemoveRoleActionResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.RemoveRoleActionResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.action.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_role(
         self,
         request: iam_models.CreateRoleRequest,
     ) -> iam_models.CreateRoleResponse:
@@ -2948,30 +3048,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateRoleResponse:
         """
         Description: 创建自定义角色
         Summary: 创建自定义角色
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateRoleResponse(),
             self.do_request('1.0', 'antcloud.iam.role.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_role_ex_async(
         self,
         request: iam_models.CreateRoleRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.CreateRoleResponse:
         """
         Description: 创建自定义角色
         Summary: 创建自定义角色
         """
         UtilClient.validate_model(request)
-        return iam_models.CreateRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.CreateRoleResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def delete_role(
         self,
         request: iam_models.DeleteRoleRequest,
     ) -> iam_models.DeleteRoleResponse:
@@ -3002,30 +3104,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteRoleResponse:
         """
         Description: 删除角色
         Summary: 删除角色
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteRoleResponse(),
             self.do_request('1.0', 'antcloud.iam.role.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def delete_role_ex_async(
         self,
         request: iam_models.DeleteRoleRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.DeleteRoleResponse:
         """
         Description: 删除角色
         Summary: 删除角色
         """
         UtilClient.validate_model(request)
-        return iam_models.DeleteRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.DeleteRoleResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_role(
         self,
         request: iam_models.UpdateRoleRequest,
     ) -> iam_models.UpdateRoleResponse:
@@ -3056,25 +3160,1427 @@
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateRoleResponse:
         """
         Description: 更新角色
         Summary: 更新角色
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateRoleResponse(),
             self.do_request('1.0', 'antcloud.iam.role.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_role_ex_async(
         self,
         request: iam_models.UpdateRoleRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> iam_models.UpdateRoleResponse:
         """
         Description: 更新角色
         Summary: 更新角色
         """
         UtilClient.validate_model(request)
-        return iam_models.UpdateRoleResponse().from_map(
+        return TeaCore.from_map(
+            iam_models.UpdateRoleResponse(),
             await self.do_request_async('1.0', 'antcloud.iam.role.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def get_department(
+        self,
+        request: iam_models.GetDepartmentRequest,
+    ) -> iam_models.GetDepartmentResponse:
+        """
+        Description: 获取单个部门信息
+        Summary: 获取单个部门信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_department_ex(request, headers, runtime)
+
+    async def get_department_async(
+        self,
+        request: iam_models.GetDepartmentRequest,
+    ) -> iam_models.GetDepartmentResponse:
+        """
+        Description: 获取单个部门信息
+        Summary: 获取单个部门信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_department_ex_async(request, headers, runtime)
+
+    def get_department_ex(
+        self,
+        request: iam_models.GetDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetDepartmentResponse:
+        """
+        Description: 获取单个部门信息
+        Summary: 获取单个部门信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetDepartmentResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_department_ex_async(
+        self,
+        request: iam_models.GetDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetDepartmentResponse:
+        """
+        Description: 获取单个部门信息
+        Summary: 获取单个部门信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetDepartmentResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_department(
+        self,
+        request: iam_models.CreateDepartmentRequest,
+    ) -> iam_models.CreateDepartmentResponse:
+        """
+        Description: 创建部门
+        Summary: 创建部门
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_department_ex(request, headers, runtime)
+
+    async def create_department_async(
+        self,
+        request: iam_models.CreateDepartmentRequest,
+    ) -> iam_models.CreateDepartmentResponse:
+        """
+        Description: 创建部门
+        Summary: 创建部门
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_department_ex_async(request, headers, runtime)
+
+    def create_department_ex(
+        self,
+        request: iam_models.CreateDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.CreateDepartmentResponse:
+        """
+        Description: 创建部门
+        Summary: 创建部门
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.CreateDepartmentResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_department_ex_async(
+        self,
+        request: iam_models.CreateDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.CreateDepartmentResponse:
+        """
+        Description: 创建部门
+        Summary: 创建部门
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.CreateDepartmentResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_department(
+        self,
+        request: iam_models.UpdateDepartmentRequest,
+    ) -> iam_models.UpdateDepartmentResponse:
+        """
+        Description: 更新部门信息
+        Summary: 更新部门信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_department_ex(request, headers, runtime)
+
+    async def update_department_async(
+        self,
+        request: iam_models.UpdateDepartmentRequest,
+    ) -> iam_models.UpdateDepartmentResponse:
+        """
+        Description: 更新部门信息
+        Summary: 更新部门信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_department_ex_async(request, headers, runtime)
+
+    def update_department_ex(
+        self,
+        request: iam_models.UpdateDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.UpdateDepartmentResponse:
+        """
+        Description: 更新部门信息
+        Summary: 更新部门信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.UpdateDepartmentResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_department_ex_async(
+        self,
+        request: iam_models.UpdateDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.UpdateDepartmentResponse:
+        """
+        Description: 更新部门信息
+        Summary: 更新部门信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.UpdateDepartmentResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def delete_department(
+        self,
+        request: iam_models.DeleteDepartmentRequest,
+    ) -> iam_models.DeleteDepartmentResponse:
+        """
+        Description: 删除部门
+        Summary: 删除部门
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.delete_department_ex(request, headers, runtime)
+
+    async def delete_department_async(
+        self,
+        request: iam_models.DeleteDepartmentRequest,
+    ) -> iam_models.DeleteDepartmentResponse:
+        """
+        Description: 删除部门
+        Summary: 删除部门
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.delete_department_ex_async(request, headers, runtime)
+
+    def delete_department_ex(
+        self,
+        request: iam_models.DeleteDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.DeleteDepartmentResponse:
+        """
+        Description: 删除部门
+        Summary: 删除部门
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.DeleteDepartmentResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def delete_department_ex_async(
+        self,
+        request: iam_models.DeleteDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.DeleteDepartmentResponse:
+        """
+        Description: 删除部门
+        Summary: 删除部门
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.DeleteDepartmentResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_department(
+        self,
+        request: iam_models.PagequeryDepartmentRequest,
+    ) -> iam_models.PagequeryDepartmentResponse:
+        """
+        Description: 分页查询部门信息
+        Summary: 分页查询部门信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_department_ex(request, headers, runtime)
+
+    async def pagequery_department_async(
+        self,
+        request: iam_models.PagequeryDepartmentRequest,
+    ) -> iam_models.PagequeryDepartmentResponse:
+        """
+        Description: 分页查询部门信息
+        Summary: 分页查询部门信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_department_ex_async(request, headers, runtime)
+
+    def pagequery_department_ex(
+        self,
+        request: iam_models.PagequeryDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.PagequeryDepartmentResponse:
+        """
+        Description: 分页查询部门信息
+        Summary: 分页查询部门信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.PagequeryDepartmentResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_department_ex_async(
+        self,
+        request: iam_models.PagequeryDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.PagequeryDepartmentResponse:
+        """
+        Description: 分页查询部门信息
+        Summary: 分页查询部门信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.PagequeryDepartmentResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def batchquery_department(
+        self,
+        request: iam_models.BatchqueryDepartmentRequest,
+    ) -> iam_models.BatchqueryDepartmentResponse:
+        """
+        Description: 批量查询部门
+        Summary: 批量查询部门
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.batchquery_department_ex(request, headers, runtime)
+
+    async def batchquery_department_async(
+        self,
+        request: iam_models.BatchqueryDepartmentRequest,
+    ) -> iam_models.BatchqueryDepartmentResponse:
+        """
+        Description: 批量查询部门
+        Summary: 批量查询部门
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.batchquery_department_ex_async(request, headers, runtime)
+
+    def batchquery_department_ex(
+        self,
+        request: iam_models.BatchqueryDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.BatchqueryDepartmentResponse:
+        """
+        Description: 批量查询部门
+        Summary: 批量查询部门
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.BatchqueryDepartmentResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def batchquery_department_ex_async(
+        self,
+        request: iam_models.BatchqueryDepartmentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.BatchqueryDepartmentResponse:
+        """
+        Description: 批量查询部门
+        Summary: 批量查询部门
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.BatchqueryDepartmentResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def save_department_user(
+        self,
+        request: iam_models.SaveDepartmentUserRequest,
+    ) -> iam_models.SaveDepartmentUserResponse:
+        """
+        Description: 添加或更新部门成员
+        Summary: 添加或更新部门成员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.save_department_user_ex(request, headers, runtime)
+
+    async def save_department_user_async(
+        self,
+        request: iam_models.SaveDepartmentUserRequest,
+    ) -> iam_models.SaveDepartmentUserResponse:
+        """
+        Description: 添加或更新部门成员
+        Summary: 添加或更新部门成员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.save_department_user_ex_async(request, headers, runtime)
+
+    def save_department_user_ex(
+        self,
+        request: iam_models.SaveDepartmentUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.SaveDepartmentUserResponse:
+        """
+        Description: 添加或更新部门成员
+        Summary: 添加或更新部门成员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.SaveDepartmentUserResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.user.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def save_department_user_ex_async(
+        self,
+        request: iam_models.SaveDepartmentUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.SaveDepartmentUserResponse:
+        """
+        Description: 添加或更新部门成员
+        Summary: 添加或更新部门成员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.SaveDepartmentUserResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.user.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def remove_department_user(
+        self,
+        request: iam_models.RemoveDepartmentUserRequest,
+    ) -> iam_models.RemoveDepartmentUserResponse:
+        """
+        Description: 移除部门成员
+        Summary: 移除部门成员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.remove_department_user_ex(request, headers, runtime)
+
+    async def remove_department_user_async(
+        self,
+        request: iam_models.RemoveDepartmentUserRequest,
+    ) -> iam_models.RemoveDepartmentUserResponse:
+        """
+        Description: 移除部门成员
+        Summary: 移除部门成员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.remove_department_user_ex_async(request, headers, runtime)
+
+    def remove_department_user_ex(
+        self,
+        request: iam_models.RemoveDepartmentUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.RemoveDepartmentUserResponse:
+        """
+        Description: 移除部门成员
+        Summary: 移除部门成员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.RemoveDepartmentUserResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.user.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def remove_department_user_ex_async(
+        self,
+        request: iam_models.RemoveDepartmentUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.RemoveDepartmentUserResponse:
+        """
+        Description: 移除部门成员
+        Summary: 移除部门成员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.RemoveDepartmentUserResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.user.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_department_user(
+        self,
+        request: iam_models.QueryDepartmentUserRequest,
+    ) -> iam_models.QueryDepartmentUserResponse:
+        """
+        Description: 分页查询部门成员信息
+        Summary: 分页查询部门成员信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_department_user_ex(request, headers, runtime)
+
+    async def query_department_user_async(
+        self,
+        request: iam_models.QueryDepartmentUserRequest,
+    ) -> iam_models.QueryDepartmentUserResponse:
+        """
+        Description: 分页查询部门成员信息
+        Summary: 分页查询部门成员信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_department_user_ex_async(request, headers, runtime)
+
+    def query_department_user_ex(
+        self,
+        request: iam_models.QueryDepartmentUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.QueryDepartmentUserResponse:
+        """
+        Description: 分页查询部门成员信息
+        Summary: 分页查询部门成员信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.QueryDepartmentUserResponse(),
+            self.do_request('1.0', 'antcloud.iam.department.user.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_department_user_ex_async(
+        self,
+        request: iam_models.QueryDepartmentUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.QueryDepartmentUserResponse:
+        """
+        Description: 分页查询部门成员信息
+        Summary: 分页查询部门成员信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.QueryDepartmentUserResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.department.user.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_loginconfig(
+        self,
+        request: iam_models.GetLoginconfigRequest,
+    ) -> iam_models.GetLoginconfigResponse:
+        """
+        Description: 获取租户级安全设置
+        Summary: 获取租户级安全设置
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_loginconfig_ex(request, headers, runtime)
+
+    async def get_loginconfig_async(
+        self,
+        request: iam_models.GetLoginconfigRequest,
+    ) -> iam_models.GetLoginconfigResponse:
+        """
+        Description: 获取租户级安全设置
+        Summary: 获取租户级安全设置
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_loginconfig_ex_async(request, headers, runtime)
+
+    def get_loginconfig_ex(
+        self,
+        request: iam_models.GetLoginconfigRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetLoginconfigResponse:
+        """
+        Description: 获取租户级安全设置
+        Summary: 获取租户级安全设置
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetLoginconfigResponse(),
+            self.do_request('1.0', 'antcloud.iam.loginconfig.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_loginconfig_ex_async(
+        self,
+        request: iam_models.GetLoginconfigRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetLoginconfigResponse:
+        """
+        Description: 获取租户级安全设置
+        Summary: 获取租户级安全设置
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetLoginconfigResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.loginconfig.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_loginconfig(
+        self,
+        request: iam_models.UpdateLoginconfigRequest,
+    ) -> iam_models.UpdateLoginconfigResponse:
+        """
+        Description: 更新租户级安全设置
+        Summary: 更新租户级安全设置
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_loginconfig_ex(request, headers, runtime)
+
+    async def update_loginconfig_async(
+        self,
+        request: iam_models.UpdateLoginconfigRequest,
+    ) -> iam_models.UpdateLoginconfigResponse:
+        """
+        Description: 更新租户级安全设置
+        Summary: 更新租户级安全设置
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_loginconfig_ex_async(request, headers, runtime)
+
+    def update_loginconfig_ex(
+        self,
+        request: iam_models.UpdateLoginconfigRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.UpdateLoginconfigResponse:
+        """
+        Description: 更新租户级安全设置
+        Summary: 更新租户级安全设置
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.UpdateLoginconfigResponse(),
+            self.do_request('1.0', 'antcloud.iam.loginconfig.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_loginconfig_ex_async(
+        self,
+        request: iam_models.UpdateLoginconfigRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.UpdateLoginconfigResponse:
+        """
+        Description: 更新租户级安全设置
+        Summary: 更新租户级安全设置
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.UpdateLoginconfigResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.loginconfig.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_mfa_status(
+        self,
+        request: iam_models.GetMfaStatusRequest,
+    ) -> iam_models.GetMfaStatusResponse:
+        """
+        Description: 唯一条件查询MFA状态
+        Summary: 唯一条件查询MFA状态
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_mfa_status_ex(request, headers, runtime)
+
+    async def get_mfa_status_async(
+        self,
+        request: iam_models.GetMfaStatusRequest,
+    ) -> iam_models.GetMfaStatusResponse:
+        """
+        Description: 唯一条件查询MFA状态
+        Summary: 唯一条件查询MFA状态
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_mfa_status_ex_async(request, headers, runtime)
+
+    def get_mfa_status_ex(
+        self,
+        request: iam_models.GetMfaStatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetMfaStatusResponse:
+        """
+        Description: 唯一条件查询MFA状态
+        Summary: 唯一条件查询MFA状态
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetMfaStatusResponse(),
+            self.do_request('1.0', 'antcloud.iam.mfa.status.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_mfa_status_ex_async(
+        self,
+        request: iam_models.GetMfaStatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetMfaStatusResponse:
+        """
+        Description: 唯一条件查询MFA状态
+        Summary: 唯一条件查询MFA状态
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetMfaStatusResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.mfa.status.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def enable_mfa(
+        self,
+        request: iam_models.EnableMfaRequest,
+    ) -> iam_models.EnableMfaResponse:
+        """
+        Description: 开启MFA
+        Summary: 开启MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.enable_mfa_ex(request, headers, runtime)
+
+    async def enable_mfa_async(
+        self,
+        request: iam_models.EnableMfaRequest,
+    ) -> iam_models.EnableMfaResponse:
+        """
+        Description: 开启MFA
+        Summary: 开启MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.enable_mfa_ex_async(request, headers, runtime)
+
+    def enable_mfa_ex(
+        self,
+        request: iam_models.EnableMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.EnableMfaResponse:
+        """
+        Description: 开启MFA
+        Summary: 开启MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.EnableMfaResponse(),
+            self.do_request('1.0', 'antcloud.iam.mfa.enable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def enable_mfa_ex_async(
+        self,
+        request: iam_models.EnableMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.EnableMfaResponse:
+        """
+        Description: 开启MFA
+        Summary: 开启MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.EnableMfaResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.mfa.enable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def disable_mfa(
+        self,
+        request: iam_models.DisableMfaRequest,
+    ) -> iam_models.DisableMfaResponse:
+        """
+        Description: 关闭MFA
+        Summary: 关闭MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.disable_mfa_ex(request, headers, runtime)
+
+    async def disable_mfa_async(
+        self,
+        request: iam_models.DisableMfaRequest,
+    ) -> iam_models.DisableMfaResponse:
+        """
+        Description: 关闭MFA
+        Summary: 关闭MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.disable_mfa_ex_async(request, headers, runtime)
+
+    def disable_mfa_ex(
+        self,
+        request: iam_models.DisableMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.DisableMfaResponse:
+        """
+        Description: 关闭MFA
+        Summary: 关闭MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.DisableMfaResponse(),
+            self.do_request('1.0', 'antcloud.iam.mfa.disable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def disable_mfa_ex_async(
+        self,
+        request: iam_models.DisableMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.DisableMfaResponse:
+        """
+        Description: 关闭MFA
+        Summary: 关闭MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.DisableMfaResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.mfa.disable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def init_mfa(
+        self,
+        request: iam_models.InitMfaRequest,
+    ) -> iam_models.InitMfaResponse:
+        """
+        Description: 初始化MFA
+        Summary: 初始化MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.init_mfa_ex(request, headers, runtime)
+
+    async def init_mfa_async(
+        self,
+        request: iam_models.InitMfaRequest,
+    ) -> iam_models.InitMfaResponse:
+        """
+        Description: 初始化MFA
+        Summary: 初始化MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.init_mfa_ex_async(request, headers, runtime)
+
+    def init_mfa_ex(
+        self,
+        request: iam_models.InitMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.InitMfaResponse:
+        """
+        Description: 初始化MFA
+        Summary: 初始化MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.InitMfaResponse(),
+            self.do_request('1.0', 'antcloud.iam.mfa.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def init_mfa_ex_async(
+        self,
+        request: iam_models.InitMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.InitMfaResponse:
+        """
+        Description: 初始化MFA
+        Summary: 初始化MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.InitMfaResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.mfa.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def verify_mfa(
+        self,
+        request: iam_models.VerifyMfaRequest,
+    ) -> iam_models.VerifyMfaResponse:
+        """
+        Description: 校验 MFA
+        Summary: 校验 MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.verify_mfa_ex(request, headers, runtime)
+
+    async def verify_mfa_async(
+        self,
+        request: iam_models.VerifyMfaRequest,
+    ) -> iam_models.VerifyMfaResponse:
+        """
+        Description: 校验 MFA
+        Summary: 校验 MFA
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.verify_mfa_ex_async(request, headers, runtime)
+
+    def verify_mfa_ex(
+        self,
+        request: iam_models.VerifyMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.VerifyMfaResponse:
+        """
+        Description: 校验 MFA
+        Summary: 校验 MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.VerifyMfaResponse(),
+            self.do_request('1.0', 'antcloud.iam.mfa.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def verify_mfa_ex_async(
+        self,
+        request: iam_models.VerifyMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.VerifyMfaResponse:
+        """
+        Description: 校验 MFA
+        Summary: 校验 MFA
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.VerifyMfaResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.mfa.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_mfa(
+        self,
+        request: iam_models.GetMfaRequest,
+    ) -> iam_models.GetMfaResponse:
+        """
+        Description: 唯一条件查询MFA配置
+        Summary: 唯一条件查询MFA配置
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_mfa_ex(request, headers, runtime)
+
+    async def get_mfa_async(
+        self,
+        request: iam_models.GetMfaRequest,
+    ) -> iam_models.GetMfaResponse:
+        """
+        Description: 唯一条件查询MFA配置
+        Summary: 唯一条件查询MFA配置
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_mfa_ex_async(request, headers, runtime)
+
+    def get_mfa_ex(
+        self,
+        request: iam_models.GetMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetMfaResponse:
+        """
+        Description: 唯一条件查询MFA配置
+        Summary: 唯一条件查询MFA配置
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetMfaResponse(),
+            self.do_request('1.0', 'antcloud.iam.mfa.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_mfa_ex_async(
+        self,
+        request: iam_models.GetMfaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetMfaResponse:
+        """
+        Description: 唯一条件查询MFA配置
+        Summary: 唯一条件查询MFA配置
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetMfaResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.mfa.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_operator_password(
+        self,
+        request: iam_models.UpdateOperatorPasswordRequest,
+    ) -> iam_models.UpdateOperatorPasswordResponse:
+        """
+        Description: 更新密码
+        Summary: 更新密码
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_operator_password_ex(request, headers, runtime)
+
+    async def update_operator_password_async(
+        self,
+        request: iam_models.UpdateOperatorPasswordRequest,
+    ) -> iam_models.UpdateOperatorPasswordResponse:
+        """
+        Description: 更新密码
+        Summary: 更新密码
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_operator_password_ex_async(request, headers, runtime)
+
+    def update_operator_password_ex(
+        self,
+        request: iam_models.UpdateOperatorPasswordRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.UpdateOperatorPasswordResponse:
+        """
+        Description: 更新密码
+        Summary: 更新密码
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.UpdateOperatorPasswordResponse(),
+            self.do_request('1.0', 'antcloud.iam.operator.password.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_operator_password_ex_async(
+        self,
+        request: iam_models.UpdateOperatorPasswordRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.UpdateOperatorPasswordResponse:
+        """
+        Description: 更新密码
+        Summary: 更新密码
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.UpdateOperatorPasswordResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operator.password.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def reset_operator_password(
+        self,
+        request: iam_models.ResetOperatorPasswordRequest,
+    ) -> iam_models.ResetOperatorPasswordResponse:
+        """
+        Description: 重置账号密码
+        Summary: 重置账号密码
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.reset_operator_password_ex(request, headers, runtime)
+
+    async def reset_operator_password_async(
+        self,
+        request: iam_models.ResetOperatorPasswordRequest,
+    ) -> iam_models.ResetOperatorPasswordResponse:
+        """
+        Description: 重置账号密码
+        Summary: 重置账号密码
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.reset_operator_password_ex_async(request, headers, runtime)
+
+    def reset_operator_password_ex(
+        self,
+        request: iam_models.ResetOperatorPasswordRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.ResetOperatorPasswordResponse:
+        """
+        Description: 重置账号密码
+        Summary: 重置账号密码
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.ResetOperatorPasswordResponse(),
+            self.do_request('1.0', 'antcloud.iam.operator.password.reset', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def reset_operator_password_ex_async(
+        self,
+        request: iam_models.ResetOperatorPasswordRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.ResetOperatorPasswordResponse:
+        """
+        Description: 重置账号密码
+        Summary: 重置账号密码
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.ResetOperatorPasswordResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operator.password.reset', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def batchquery_operator(
+        self,
+        request: iam_models.BatchqueryOperatorRequest,
+    ) -> iam_models.BatchqueryOperatorResponse:
+        """
+        Description: 批量查询操作员
+        Summary: 批量查询操作员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.batchquery_operator_ex(request, headers, runtime)
+
+    async def batchquery_operator_async(
+        self,
+        request: iam_models.BatchqueryOperatorRequest,
+    ) -> iam_models.BatchqueryOperatorResponse:
+        """
+        Description: 批量查询操作员
+        Summary: 批量查询操作员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.batchquery_operator_ex_async(request, headers, runtime)
+
+    def batchquery_operator_ex(
+        self,
+        request: iam_models.BatchqueryOperatorRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.BatchqueryOperatorResponse:
+        """
+        Description: 批量查询操作员
+        Summary: 批量查询操作员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.BatchqueryOperatorResponse(),
+            self.do_request('1.0', 'antcloud.iam.operator.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def batchquery_operator_ex_async(
+        self,
+        request: iam_models.BatchqueryOperatorRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.BatchqueryOperatorResponse:
+        """
+        Description: 批量查询操作员
+        Summary: 批量查询操作员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.BatchqueryOperatorResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operator.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def push_operation(
+        self,
+        request: iam_models.PushOperationRequest,
+    ) -> iam_models.PushOperationResponse:
+        """
+        Description: 推送操作事件，事件需要事先定义
+        Summary: 推送操作事件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.push_operation_ex(request, headers, runtime)
+
+    async def push_operation_async(
+        self,
+        request: iam_models.PushOperationRequest,
+    ) -> iam_models.PushOperationResponse:
+        """
+        Description: 推送操作事件，事件需要事先定义
+        Summary: 推送操作事件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.push_operation_ex_async(request, headers, runtime)
+
+    def push_operation_ex(
+        self,
+        request: iam_models.PushOperationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.PushOperationResponse:
+        """
+        Description: 推送操作事件，事件需要事先定义
+        Summary: 推送操作事件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.PushOperationResponse(),
+            self.do_request('1.0', 'antcloud.iam.operation.push', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def push_operation_ex_async(
+        self,
+        request: iam_models.PushOperationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.PushOperationResponse:
+        """
+        Description: 推送操作事件，事件需要事先定义
+        Summary: 推送操作事件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.PushOperationResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operation.push', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_operationtype(
+        self,
+        request: iam_models.QueryOperationtypeRequest,
+    ) -> iam_models.QueryOperationtypeResponse:
+        """
+        Description: 查询操作类型
+        Summary: 查询操作类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_operationtype_ex(request, headers, runtime)
+
+    async def query_operationtype_async(
+        self,
+        request: iam_models.QueryOperationtypeRequest,
+    ) -> iam_models.QueryOperationtypeResponse:
+        """
+        Description: 查询操作类型
+        Summary: 查询操作类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_operationtype_ex_async(request, headers, runtime)
+
+    def query_operationtype_ex(
+        self,
+        request: iam_models.QueryOperationtypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.QueryOperationtypeResponse:
+        """
+        Description: 查询操作类型
+        Summary: 查询操作类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.QueryOperationtypeResponse(),
+            self.do_request('1.0', 'antcloud.iam.operationtype.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_operationtype_ex_async(
+        self,
+        request: iam_models.QueryOperationtypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.QueryOperationtypeResponse:
+        """
+        Description: 查询操作类型
+        Summary: 查询操作类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.QueryOperationtypeResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operationtype.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_operationtype(
+        self,
+        request: iam_models.GetOperationtypeRequest,
+    ) -> iam_models.GetOperationtypeResponse:
+        """
+        Description: 唯一查询操作类型
+        Summary: 唯一查询操作类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_operationtype_ex(request, headers, runtime)
+
+    async def get_operationtype_async(
+        self,
+        request: iam_models.GetOperationtypeRequest,
+    ) -> iam_models.GetOperationtypeResponse:
+        """
+        Description: 唯一查询操作类型
+        Summary: 唯一查询操作类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_operationtype_ex_async(request, headers, runtime)
+
+    def get_operationtype_ex(
+        self,
+        request: iam_models.GetOperationtypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetOperationtypeResponse:
+        """
+        Description: 唯一查询操作类型
+        Summary: 唯一查询操作类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetOperationtypeResponse(),
+            self.do_request('1.0', 'antcloud.iam.operationtype.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_operationtype_ex_async(
+        self,
+        request: iam_models.GetOperationtypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetOperationtypeResponse:
+        """
+        Description: 唯一查询操作类型
+        Summary: 唯一查询操作类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetOperationtypeResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operationtype.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def add_tenant_member(
+        self,
+        request: iam_models.AddTenantMemberRequest,
+    ) -> iam_models.AddTenantMemberResponse:
+        """
+        Description: 添加租户成员
+        Summary: 添加租户成员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.add_tenant_member_ex(request, headers, runtime)
+
+    async def add_tenant_member_async(
+        self,
+        request: iam_models.AddTenantMemberRequest,
+    ) -> iam_models.AddTenantMemberResponse:
+        """
+        Description: 添加租户成员
+        Summary: 添加租户成员
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.add_tenant_member_ex_async(request, headers, runtime)
+
+    def add_tenant_member_ex(
+        self,
+        request: iam_models.AddTenantMemberRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.AddTenantMemberResponse:
+        """
+        Description: 添加租户成员
+        Summary: 添加租户成员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.AddTenantMemberResponse(),
+            self.do_request('1.0', 'antcloud.iam.tenant.member.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def add_tenant_member_ex_async(
+        self,
+        request: iam_models.AddTenantMemberRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.AddTenantMemberResponse:
+        """
+        Description: 添加租户成员
+        Summary: 添加租户成员
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.AddTenantMemberResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.tenant.member.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_operator_logintoken(
+        self,
+        request: iam_models.GetOperatorLogintokenRequest,
+    ) -> iam_models.GetOperatorLogintokenResponse:
+        """
+        Description: 获取 logintoken，该 token 为一次性使用，且过期时间短。
+        Summary: 获取操作员 signtoken
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_operator_logintoken_ex(request, headers, runtime)
+
+    async def get_operator_logintoken_async(
+        self,
+        request: iam_models.GetOperatorLogintokenRequest,
+    ) -> iam_models.GetOperatorLogintokenResponse:
+        """
+        Description: 获取 logintoken，该 token 为一次性使用，且过期时间短。
+        Summary: 获取操作员 signtoken
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_operator_logintoken_ex_async(request, headers, runtime)
+
+    def get_operator_logintoken_ex(
+        self,
+        request: iam_models.GetOperatorLogintokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetOperatorLogintokenResponse:
+        """
+        Description: 获取 logintoken，该 token 为一次性使用，且过期时间短。
+        Summary: 获取操作员 signtoken
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetOperatorLogintokenResponse(),
+            self.do_request('1.0', 'antcloud.iam.operator.logintoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_operator_logintoken_ex_async(
+        self,
+        request: iam_models.GetOperatorLogintokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> iam_models.GetOperatorLogintokenResponse:
+        """
+        Description: 获取 logintoken，该 token 为一次性使用，且过期时间短。
+        Summary: 获取操作员 signtoken
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            iam_models.GetOperatorLogintokenResponse(),
+            await self.do_request_async('1.0', 'antcloud.iam.operator.logintoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_iam-3.12.4/antchain_sdk_iam/models.py` & `antchain_iam-3.12.8/antchain_sdk_iam/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         # 每个目标主机的最大连接数（分主机域名的长链接最大总数
         self.max_requests_per_host = max_requests_per_host
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.access_key_id is not None:
             result['accessKeyId'] = self.access_key_id
         if self.access_key_secret is not None:
             result['accessKeySecret'] = self.access_key_secret
         if self.security_token is not None:
             result['securityToken'] = self.security_token
@@ -146,14 +150,47 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
+class Condition(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['key'] = self.key
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
 class AliyunResource(TeaModel):
     def __init__(
         self,
         resource: str = None,
         resource_tenant: str = None,
     ):
         # resource_type/resource_id
@@ -162,14 +199,18 @@
         self.resource_tenant = resource_tenant
 
     def validate(self):
         self.validate_required(self.resource, 'resource')
         self.validate_required(self.resource_tenant, 'resource_tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.resource is not None:
             result['resource'] = self.resource
         if self.resource_tenant is not None:
             result['resource_tenant'] = self.resource_tenant
         return result
 
@@ -178,116 +219,223 @@
         if m.get('resource') is not None:
             self.resource = m.get('resource')
         if m.get('resource_tenant') is not None:
             self.resource_tenant = m.get('resource_tenant')
         return self
 
 
-class Condition(TeaModel):
+class AuthenticateEvent(TeaModel):
     def __init__(
         self,
-        key: str = None,
-        value: str = None,
+        actions: List[str] = None,
+        actor_id: str = None,
+        conditions: List[Condition] = None,
+        id: str = None,
     ):
-        self.key = key
-        self.value = value
+        # 鉴权操作列表
+        self.actions = actions
+        # 鉴权对象ID
+        self.actor_id = actor_id
+        # 鉴权条件
+        self.conditions = conditions
+        # 唯一ID
+        self.id = id
 
     def validate(self):
-        pass
+        self.validate_required(self.actions, 'actions')
+        self.validate_required(self.actor_id, 'actor_id')
+        if self.conditions:
+            for k in self.conditions:
+                if k:
+                    k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.key is not None:
-            result['key'] = self.key
-        if self.value is not None:
-            result['value'] = self.value
+        if self.actions is not None:
+            result['actions'] = self.actions
+        if self.actor_id is not None:
+            result['actor_id'] = self.actor_id
+        result['conditions'] = []
+        if self.conditions is not None:
+            for k in self.conditions:
+                result['conditions'].append(k.to_map() if k else None)
+        if self.id is not None:
+            result['id'] = self.id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('key') is not None:
-            self.key = m.get('key')
-        if m.get('value') is not None:
-            self.value = m.get('value')
+        if m.get('actions') is not None:
+            self.actions = m.get('actions')
+        if m.get('actor_id') is not None:
+            self.actor_id = m.get('actor_id')
+        self.conditions = []
+        if m.get('conditions') is not None:
+            for k in m.get('conditions'):
+                temp_model = Condition()
+                self.conditions.append(temp_model.from_map(k))
+        if m.get('id') is not None:
+            self.id = m.get('id')
         return self
 
 
-class StsActorBinding(TeaModel):
+class OnexExtraInfo(TeaModel):
     def __init__(
         self,
-        actor_id: str = None,
-        bind_id: str = None,
-        bind_type: str = None,
+        path: str = None,
+        method: str = None,
     ):
-        # 虚拟身份ID
-        self.actor_id = actor_id
-        # 受信对象ID
-        self.bind_id = bind_id
-        # 虚拟身份受信类型，可以为TENANT或者ALIYUN_SERVICE
-        self.bind_type = bind_type
+        # Onex接口路径
+        self.path = path
+        # Onex接口的HTTP Method
+        self.method = method
 
     def validate(self):
-        pass
+        self.validate_required(self.path, 'path')
+        self.validate_required(self.method, 'method')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.actor_id is not None:
-            result['actor_id'] = self.actor_id
-        if self.bind_id is not None:
-            result['bind_id'] = self.bind_id
-        if self.bind_type is not None:
-            result['bind_type'] = self.bind_type
+        if self.path is not None:
+            result['path'] = self.path
+        if self.method is not None:
+            result['method'] = self.method
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('actor_id') is not None:
-            self.actor_id = m.get('actor_id')
-        if m.get('bind_id') is not None:
-            self.bind_id = m.get('bind_id')
-        if m.get('bind_type') is not None:
-            self.bind_type = m.get('bind_type')
+        if m.get('path') is not None:
+            self.path = m.get('path')
+        if m.get('method') is not None:
+            self.method = m.get('method')
         return self
 
 
-class Action(TeaModel):
+class AliyunRamAuthContext(TeaModel):
     def __init__(
         self,
-        description: str = None,
+        action: str = None,
+        conditions: List[Condition] = None,
         id: str = None,
-        name: str = None,
+        region_id: str = None,
+        resources: List[AliyunResource] = None,
+        service_name: str = None,
     ):
-        # 操作点描述
-        self.description = description
-        # 操作点ID
+        # 操作名称
+        self.action = action
+        # 条件
+        self.conditions = conditions
+        # 唯一ID
         self.id = id
-        # 操作点名称
-        self.name = name
+        # regionId
+        self.region_id = region_id
+        # 资源
+        self.resources = resources
+        # 服务名称
+        self.service_name = service_name
 
     def validate(self):
-        pass
+        self.validate_required(self.action, 'action')
+        if self.conditions:
+            for k in self.conditions:
+                if k:
+                    k.validate()
+        self.validate_required(self.region_id, 'region_id')
+        self.validate_required(self.resources, 'resources')
+        if self.resources:
+            for k in self.resources:
+                if k:
+                    k.validate()
+        self.validate_required(self.service_name, 'service_name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.description is not None:
-            result['description'] = self.description
+        if self.action is not None:
+            result['action'] = self.action
+        result['conditions'] = []
+        if self.conditions is not None:
+            for k in self.conditions:
+                result['conditions'].append(k.to_map() if k else None)
         if self.id is not None:
             result['id'] = self.id
-        if self.name is not None:
-            result['name'] = self.name
+        if self.region_id is not None:
+            result['region_id'] = self.region_id
+        result['resources'] = []
+        if self.resources is not None:
+            for k in self.resources:
+                result['resources'].append(k.to_map() if k else None)
+        if self.service_name is not None:
+            result['service_name'] = self.service_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('description') is not None:
-            self.description = m.get('description')
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        self.conditions = []
+        if m.get('conditions') is not None:
+            for k in m.get('conditions'):
+                temp_model = Condition()
+                self.conditions.append(temp_model.from_map(k))
         if m.get('id') is not None:
             self.id = m.get('id')
-        if m.get('name') is not None:
-            self.name = m.get('name')
+        if m.get('region_id') is not None:
+            self.region_id = m.get('region_id')
+        self.resources = []
+        if m.get('resources') is not None:
+            for k in m.get('resources'):
+                temp_model = AliyunResource()
+                self.resources.append(temp_model.from_map(k))
+        if m.get('service_name') is not None:
+            self.service_name = m.get('service_name')
+        return self
+
+
+class ScopeEntity(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['key'] = self.key
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('value') is not None:
+            self.value = m.get('value')
         return self
 
 
 class AliyunPopRequestInfo(TeaModel):
     def __init__(
         self,
         access_key_id: str = None,
@@ -361,14 +509,18 @@
         # 版本
         self.version = version
 
     def validate(self):
         self.validate_required(self.caller_type, 'caller_type')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.access_key_id is not None:
             result['access_key_id'] = self.access_key_id
         if self.ak_mfa_present is not None:
             result['ak_mfa_present'] = self.ak_mfa_present
         if self.ak_proxy is not None:
             result['ak_proxy'] = self.ak_proxy
@@ -457,269 +609,334 @@
         if m.get('sts_token_user_id') is not None:
             self.sts_token_user_id = m.get('sts_token_user_id')
         if m.get('version') is not None:
             self.version = m.get('version')
         return self
 
 
-class ScopeEntity(TeaModel):
+class StsActorBinding(TeaModel):
     def __init__(
         self,
-        key: str = None,
-        value: str = None,
+        actor_id: str = None,
+        bind_id: str = None,
+        bind_type: str = None,
     ):
-        self.key = key
-        self.value = value
+        # 虚拟身份ID
+        self.actor_id = actor_id
+        # 受信对象ID
+        self.bind_id = bind_id
+        # 虚拟身份受信类型，可以为TENANT或者ALIYUN_SERVICE
+        self.bind_type = bind_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.key is not None:
-            result['key'] = self.key
-        if self.value is not None:
-            result['value'] = self.value
+        if self.actor_id is not None:
+            result['actor_id'] = self.actor_id
+        if self.bind_id is not None:
+            result['bind_id'] = self.bind_id
+        if self.bind_type is not None:
+            result['bind_type'] = self.bind_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('key') is not None:
-            self.key = m.get('key')
-        if m.get('value') is not None:
-            self.value = m.get('value')
+        if m.get('actor_id') is not None:
+            self.actor_id = m.get('actor_id')
+        if m.get('bind_id') is not None:
+            self.bind_id = m.get('bind_id')
+        if m.get('bind_type') is not None:
+            self.bind_type = m.get('bind_type')
         return self
 
 
-class AliyunRamAuthContext(TeaModel):
+class Action(TeaModel):
     def __init__(
         self,
-        action: str = None,
-        conditions: List[Condition] = None,
+        description: str = None,
         id: str = None,
-        region_id: str = None,
-        resources: List[AliyunResource] = None,
-        service_name: str = None,
+        name: str = None,
     ):
-        # 操作名称
-        self.action = action
-        # 条件
-        self.conditions = conditions
-        # 唯一ID
+        # 操作点描述
+        self.description = description
+        # 操作点ID
         self.id = id
-        # regionId
-        self.region_id = region_id
-        # 资源
-        self.resources = resources
-        # 服务名称
-        self.service_name = service_name
+        # 操作点名称
+        self.name = name
 
     def validate(self):
-        self.validate_required(self.action, 'action')
-        if self.conditions:
-            for k in self.conditions:
-                if k:
-                    k.validate()
-        self.validate_required(self.region_id, 'region_id')
-        self.validate_required(self.resources, 'resources')
-        if self.resources:
-            for k in self.resources:
-                if k:
-                    k.validate()
-        self.validate_required(self.service_name, 'service_name')
+        pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.action is not None:
-            result['action'] = self.action
-        result['conditions'] = []
-        if self.conditions is not None:
-            for k in self.conditions:
-                result['conditions'].append(k.to_map() if k else None)
+        if self.description is not None:
+            result['description'] = self.description
         if self.id is not None:
             result['id'] = self.id
-        if self.region_id is not None:
-            result['region_id'] = self.region_id
-        result['resources'] = []
-        if self.resources is not None:
-            for k in self.resources:
-                result['resources'].append(k.to_map() if k else None)
-        if self.service_name is not None:
-            result['service_name'] = self.service_name
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('action') is not None:
-            self.action = m.get('action')
-        self.conditions = []
-        if m.get('conditions') is not None:
-            for k in m.get('conditions'):
-                temp_model = Condition()
-                self.conditions.append(temp_model.from_map(k))
+        if m.get('description') is not None:
+            self.description = m.get('description')
         if m.get('id') is not None:
             self.id = m.get('id')
-        if m.get('region_id') is not None:
-            self.region_id = m.get('region_id')
-        self.resources = []
-        if m.get('resources') is not None:
-            for k in m.get('resources'):
-                temp_model = AliyunResource()
-                self.resources.append(temp_model.from_map(k))
-        if m.get('service_name') is not None:
-            self.service_name = m.get('service_name')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         return self
 
 
-class AuthenticateEvent(TeaModel):
+class OperationType(TeaModel):
     def __init__(
         self,
-        actions: List[str] = None,
-        actor_id: str = None,
-        conditions: List[Condition] = None,
-        id: str = None,
+        description: str = None,
+        display_name: str = None,
+        enabled: str = None,
+        name: str = None,
+        product: str = None,
+        source: str = None,
+        onex_extra_info: OnexExtraInfo = None,
+        resource_type: str = None,
+        resource_exp: str = None,
     ):
-        # 鉴权操作列表
-        self.actions = actions
-        # 鉴权对象ID
-        self.actor_id = actor_id
-        # 鉴权条件
-        self.conditions = conditions
-        # 唯一ID
-        self.id = id
+        # 操作描述
+        self.description = description
+        # 展示名称
+        self.display_name = display_name
+        # 是否启用
+        self.enabled = enabled
+        # 操作名称
+        self.name = name
+        # 产品码
+        self.product = product
+        # 操作来源
+        self.source = source
+        # Onex接口额外信息
+        self.onex_extra_info = onex_extra_info
+        # 资源类型
+        self.resource_type = resource_type
+        # 资源表达式
+        self.resource_exp = resource_exp
 
     def validate(self):
-        self.validate_required(self.actions, 'actions')
-        self.validate_required(self.actor_id, 'actor_id')
-        if self.conditions:
-            for k in self.conditions:
+        self.validate_required(self.description, 'description')
+        self.validate_required(self.display_name, 'display_name')
+        self.validate_required(self.enabled, 'enabled')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.product, 'product')
+        self.validate_required(self.source, 'source')
+        if self.onex_extra_info:
+            self.onex_extra_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['description'] = self.description
+        if self.display_name is not None:
+            result['display_name'] = self.display_name
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.name is not None:
+            result['name'] = self.name
+        if self.product is not None:
+            result['product'] = self.product
+        if self.source is not None:
+            result['source'] = self.source
+        if self.onex_extra_info is not None:
+            result['onex_extra_info'] = self.onex_extra_info.to_map()
+        if self.resource_type is not None:
+            result['resource_type'] = self.resource_type
+        if self.resource_exp is not None:
+            result['resource_exp'] = self.resource_exp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('display_name') is not None:
+            self.display_name = m.get('display_name')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('product') is not None:
+            self.product = m.get('product')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        if m.get('onex_extra_info') is not None:
+            temp_model = OnexExtraInfo()
+            self.onex_extra_info = temp_model.from_map(m['onex_extra_info'])
+        if m.get('resource_type') is not None:
+            self.resource_type = m.get('resource_type')
+        if m.get('resource_exp') is not None:
+            self.resource_exp = m.get('resource_exp')
+        return self
+
+
+class DepartmentUser(TeaModel):
+    def __init__(
+        self,
+        department_code: str = None,
+        user_id: str = None,
+        type: str = None,
+    ):
+        # 部门唯一码
+        self.department_code = department_code
+        # 用户 id
+        self.user_id = user_id
+        # 部门成员类型，
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_code is not None:
+            result['department_code'] = self.department_code
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('department_code') is not None:
+            self.department_code = m.get('department_code')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class AliyunAuthenticateBatchEvent(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+        ram_auth_contexts: List[AliyunRamAuthContext] = None,
+        request_info: AliyunPopRequestInfo = None,
+    ):
+        # 金融云用户ID
+        self.user_id = user_id
+        # 阿里云鉴权列表
+        self.ram_auth_contexts = ram_auth_contexts
+        # BSB透传下来的阿里云信息
+        self.request_info = request_info
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.ram_auth_contexts, 'ram_auth_contexts')
+        if self.ram_auth_contexts:
+            for k in self.ram_auth_contexts:
                 if k:
                     k.validate()
+        self.validate_required(self.request_info, 'request_info')
+        if self.request_info:
+            self.request_info.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.actions is not None:
-            result['actions'] = self.actions
-        if self.actor_id is not None:
-            result['actor_id'] = self.actor_id
-        result['conditions'] = []
-        if self.conditions is not None:
-            for k in self.conditions:
-                result['conditions'].append(k.to_map() if k else None)
-        if self.id is not None:
-            result['id'] = self.id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        result['ram_auth_contexts'] = []
+        if self.ram_auth_contexts is not None:
+            for k in self.ram_auth_contexts:
+                result['ram_auth_contexts'].append(k.to_map() if k else None)
+        if self.request_info is not None:
+            result['request_info'] = self.request_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('actions') is not None:
-            self.actions = m.get('actions')
-        if m.get('actor_id') is not None:
-            self.actor_id = m.get('actor_id')
-        self.conditions = []
-        if m.get('conditions') is not None:
-            for k in m.get('conditions'):
-                temp_model = Condition()
-                self.conditions.append(temp_model.from_map(k))
-        if m.get('id') is not None:
-            self.id = m.get('id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        self.ram_auth_contexts = []
+        if m.get('ram_auth_contexts') is not None:
+            for k in m.get('ram_auth_contexts'):
+                temp_model = AliyunRamAuthContext()
+                self.ram_auth_contexts.append(temp_model.from_map(k))
+        if m.get('request_info') is not None:
+            temp_model = AliyunPopRequestInfo()
+            self.request_info = temp_model.from_map(m['request_info'])
         return self
 
 
-class Tenant(TeaModel):
+class Judgement(TeaModel):
     def __init__(
         self,
-        ant_account: str = None,
-        ant_uid: str = None,
-        business_owner_id: str = None,
-        create_time: str = None,
-        customer: str = None,
-        description: str = None,
         id: str = None,
-        internal_id: str = None,
-        name: str = None,
-        update_time: str = None,
-        tags: List[str] = None,
+        pass_: bool = None,
+        reason: str = None,
+        solution: str = None,
     ):
-        # 蚂蚁通行证签约账户
-        self.ant_account = ant_account
-        # 蚂蚁通行证uid
-        self.ant_uid = ant_uid
-        # 金融云官网:ANTCLOUD,蚂蚁开放平台：ANTOPEN
-        self.business_owner_id = business_owner_id
-        # 租户创建时间，ISO8601格式
-        self.create_time = create_time
-        # 租户所在的企业的唯一标识
-        self.customer = customer
-        # 租户描述信息
-        self.description = description
-        # 租户唯一标识
+        # 唯一ID
         self.id = id
-        # 租户内部id
-        self.internal_id = internal_id
-        # 租户显示名称
-        self.name = name
-        # 租户最近一次修改时间，ISO8601格式
-        self.update_time = update_time
-        # 标签
-        self.tags = tags
+        # 是否通过
+        self.pass_ = pass_
+        # 失败原因
+        self.reason = reason
+        # 解决方案
+        self.solution = solution
 
     def validate(self):
-        pass
+        self.validate_required(self.pass_, 'pass_')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.ant_account is not None:
-            result['ant_account'] = self.ant_account
-        if self.ant_uid is not None:
-            result['ant_uid'] = self.ant_uid
-        if self.business_owner_id is not None:
-            result['business_owner_id'] = self.business_owner_id
-        if self.create_time is not None:
-            result['create_time'] = self.create_time
-        if self.customer is not None:
-            result['customer'] = self.customer
-        if self.description is not None:
-            result['description'] = self.description
         if self.id is not None:
             result['id'] = self.id
-        if self.internal_id is not None:
-            result['internal_id'] = self.internal_id
-        if self.name is not None:
-            result['name'] = self.name
-        if self.update_time is not None:
-            result['update_time'] = self.update_time
-        if self.tags is not None:
-            result['tags'] = self.tags
+        if self.pass_ is not None:
+            result['pass'] = self.pass_
+        if self.reason is not None:
+            result['reason'] = self.reason
+        if self.solution is not None:
+            result['solution'] = self.solution
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ant_account') is not None:
-            self.ant_account = m.get('ant_account')
-        if m.get('ant_uid') is not None:
-            self.ant_uid = m.get('ant_uid')
-        if m.get('business_owner_id') is not None:
-            self.business_owner_id = m.get('business_owner_id')
-        if m.get('create_time') is not None:
-            self.create_time = m.get('create_time')
-        if m.get('customer') is not None:
-            self.customer = m.get('customer')
-        if m.get('description') is not None:
-            self.description = m.get('description')
         if m.get('id') is not None:
             self.id = m.get('id')
-        if m.get('internal_id') is not None:
-            self.internal_id = m.get('internal_id')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('update_time') is not None:
-            self.update_time = m.get('update_time')
-        if m.get('tags') is not None:
-            self.tags = m.get('tags')
+        if m.get('pass') is not None:
+            self.pass_ = m.get('pass')
+        if m.get('reason') is not None:
+            self.reason = m.get('reason')
+        if m.get('solution') is not None:
+            self.solution = m.get('solution')
         return self
 
 
 class Role(TeaModel):
     def __init__(
         self,
         actions: List[Action] = None,
@@ -751,14 +968,18 @@
     def validate(self):
         if self.actions:
             for k in self.actions:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['actions'] = []
         if self.actions is not None:
             for k in self.actions:
                 result['actions'].append(k.to_map() if k else None)
         if self.create_time is not None:
             result['create_time'] = self.create_time
@@ -817,14 +1038,18 @@
         # 更新时间，ISO8601格式
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.creation_time is not None:
             result['creation_time'] = self.creation_time
         if self.id is not None:
             result['id'] = self.id
         if self.name is not None:
             result['name'] = self.name
@@ -841,14 +1066,70 @@
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('update_time') is not None:
             self.update_time = m.get('update_time')
         return self
 
 
+class AccessKey(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        id: str = None,
+        secret: str = None,
+        status: str = None,
+        update_time: str = None,
+    ):
+        # AccessKey创建时间，ISO8601格式
+        self.create_time = create_time
+        # AccessKey唯一标识
+        self.id = id
+        # AccessKey的秘钥，加密传输，网关返回后，使用调用方的AccesSecret进行解密
+        self.secret = secret
+        # 状态
+        self.status = status
+        # AccessKey最近一次修改时间，ISO8601格式
+        self.update_time = update_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['create_time'] = self.create_time
+        if self.id is not None:
+            result['id'] = self.id
+        if self.secret is not None:
+            result['secret'] = self.secret
+        if self.status is not None:
+            result['status'] = self.status
+        if self.update_time is not None:
+            result['update_time'] = self.update_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('create_time') is not None:
+            self.create_time = m.get('create_time')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('secret') is not None:
+            self.secret = m.get('secret')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('update_time') is not None:
+            self.update_time = m.get('update_time')
+        return self
+
+
 class StsActor(TeaModel):
     def __init__(
         self,
         bindings: List[StsActorBinding] = None,
         description: str = None,
         name: str = None,
         tenant: str = None,
@@ -868,14 +1149,18 @@
             for k in self.bindings:
                 if k:
                     k.validate()
         self.validate_required(self.name, 'name')
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['bindings'] = []
         if self.bindings is not None:
             for k in self.bindings:
                 result['bindings'].append(k.to_map() if k else None)
         if self.description is not None:
             result['description'] = self.description
@@ -946,14 +1231,18 @@
                     k.validate()
         if self.scope_entities:
             for k in self.scope_entities:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.ability_id is not None:
             result['ability_id'] = self.ability_id
         if self.ability_type is not None:
             result['ability_type'] = self.ability_type
         result['conditions'] = []
         if self.conditions is not None:
@@ -1008,96 +1297,193 @@
         if m.get('type') is not None:
             self.type = m.get('type')
         if m.get('update_time') is not None:
             self.update_time = m.get('update_time')
         return self
 
 
-class Judgement(TeaModel):
+class Tenant(TeaModel):
     def __init__(
         self,
+        ant_account: str = None,
+        ant_uid: str = None,
+        business_owner_id: str = None,
+        create_time: str = None,
+        customer: str = None,
+        description: str = None,
         id: str = None,
-        pass_: bool = None,
-        reason: str = None,
-        solution: str = None,
+        internal_id: str = None,
+        name: str = None,
+        update_time: str = None,
+        tags: List[str] = None,
     ):
-        # 唯一ID
+        # 蚂蚁通行证签约账户
+        self.ant_account = ant_account
+        # 蚂蚁通行证uid
+        self.ant_uid = ant_uid
+        # 金融云官网:ANTCLOUD,蚂蚁开放平台：ANTOPEN
+        self.business_owner_id = business_owner_id
+        # 租户创建时间，ISO8601格式
+        self.create_time = create_time
+        # 租户所在的企业的唯一标识
+        self.customer = customer
+        # 租户描述信息
+        self.description = description
+        # 租户唯一标识
         self.id = id
-        # 是否通过
-        self.pass_ = pass_
-        # 失败原因
-        self.reason = reason
-        # 解决方案
-        self.solution = solution
+        # 租户内部id
+        self.internal_id = internal_id
+        # 租户显示名称
+        self.name = name
+        # 租户最近一次修改时间，ISO8601格式
+        self.update_time = update_time
+        # 标签
+        self.tags = tags
 
     def validate(self):
-        self.validate_required(self.pass_, 'pass_')
+        pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.ant_account is not None:
+            result['ant_account'] = self.ant_account
+        if self.ant_uid is not None:
+            result['ant_uid'] = self.ant_uid
+        if self.business_owner_id is not None:
+            result['business_owner_id'] = self.business_owner_id
+        if self.create_time is not None:
+            result['create_time'] = self.create_time
+        if self.customer is not None:
+            result['customer'] = self.customer
+        if self.description is not None:
+            result['description'] = self.description
         if self.id is not None:
             result['id'] = self.id
-        if self.pass_ is not None:
-            result['pass'] = self.pass_
-        if self.reason is not None:
-            result['reason'] = self.reason
-        if self.solution is not None:
-            result['solution'] = self.solution
+        if self.internal_id is not None:
+            result['internal_id'] = self.internal_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.update_time is not None:
+            result['update_time'] = self.update_time
+        if self.tags is not None:
+            result['tags'] = self.tags
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('ant_account') is not None:
+            self.ant_account = m.get('ant_account')
+        if m.get('ant_uid') is not None:
+            self.ant_uid = m.get('ant_uid')
+        if m.get('business_owner_id') is not None:
+            self.business_owner_id = m.get('business_owner_id')
+        if m.get('create_time') is not None:
+            self.create_time = m.get('create_time')
+        if m.get('customer') is not None:
+            self.customer = m.get('customer')
+        if m.get('description') is not None:
+            self.description = m.get('description')
         if m.get('id') is not None:
             self.id = m.get('id')
-        if m.get('pass') is not None:
-            self.pass_ = m.get('pass')
-        if m.get('reason') is not None:
-            self.reason = m.get('reason')
-        if m.get('solution') is not None:
-            self.solution = m.get('solution')
+        if m.get('internal_id') is not None:
+            self.internal_id = m.get('internal_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('update_time') is not None:
+            self.update_time = m.get('update_time')
+        if m.get('tags') is not None:
+            self.tags = m.get('tags')
         return self
 
 
-class Group(TeaModel):
+class Department(TeaModel):
     def __init__(
         self,
-        id: str = None,
+        code: str = None,
         name: str = None,
         description: str = None,
+        parent_code: str = None,
+        parent_path: str = None,
+        customer_id: str = None,
+        is_leaf: bool = None,
+        creation_time: str = None,
+        update_time: str = None,
     ):
-        # 成员组ID
-        self.id = id
-        # 成员组名称
+        # 部门唯一代码
+        self.code = code
+        # 部门名称
         self.name = name
-        # 成员组描述
+        # 部门描述信息
         self.description = description
+        # 父部门 code
+        self.parent_code = parent_code
+        # 父部门一直到根节点的路径，例如：DP0000000001/DP0000000002
+        self.parent_path = parent_path
+        # 企业 id
+        self.customer_id = customer_id
+        # 是否为叶子结点
+        self.is_leaf = is_leaf
+        # 创建时间，ISO8601格式
+        self.creation_time = creation_time
+        # 更新时间，ISO8601格式
+        self.update_time = update_time
 
     def validate(self):
-        self.validate_required(self.id, 'id')
-        self.validate_required(self.name, 'name')
-        self.validate_required(self.description, 'description')
+        pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.id is not None:
-            result['id'] = self.id
+        if self.code is not None:
+            result['code'] = self.code
         if self.name is not None:
             result['name'] = self.name
         if self.description is not None:
             result['description'] = self.description
+        if self.parent_code is not None:
+            result['parent_code'] = self.parent_code
+        if self.parent_path is not None:
+            result['parent_path'] = self.parent_path
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
+        if self.is_leaf is not None:
+            result['is_leaf'] = self.is_leaf
+        if self.creation_time is not None:
+            result['creation_time'] = self.creation_time
+        if self.update_time is not None:
+            result['update_time'] = self.update_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('id') is not None:
-            self.id = m.get('id')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('description') is not None:
             self.description = m.get('description')
+        if m.get('parent_code') is not None:
+            self.parent_code = m.get('parent_code')
+        if m.get('parent_path') is not None:
+            self.parent_path = m.get('parent_path')
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
+        if m.get('is_leaf') is not None:
+            self.is_leaf = m.get('is_leaf')
+        if m.get('creation_time') is not None:
+            self.creation_time = m.get('creation_time')
+        if m.get('update_time') is not None:
+            self.update_time = m.get('update_time')
         return self
 
 
 class AuthenticateBatchEvent(TeaModel):
     def __init__(
         self,
         events: List[AuthenticateEvent] = None,
@@ -1109,14 +1495,18 @@
         self.validate_required(self.events, 'events')
         if self.events:
             for k in self.events:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['events'] = []
         if self.events is not None:
             for k in self.events:
                 result['events'].append(k.to_map() if k else None)
         return result
 
@@ -1126,63 +1516,237 @@
         if m.get('events') is not None:
             for k in m.get('events'):
                 temp_model = AuthenticateEvent()
                 self.events.append(temp_model.from_map(k))
         return self
 
 
-class AliyunAuthenticateBatchEvent(TeaModel):
+class Accessor(TeaModel):
+    def __init__(
+        self,
+        access_key: str = None,
+        access_secret: str = None,
+        account: str = None,
+        create_time: str = None,
+        id: str = None,
+        type: str = None,
+    ):
+        # Accessor关联的AccessKey
+        self.access_key = access_key
+        # Accessor关联的AccessKey的密钥，加密传输，网关返回后，使用调用方的AccessSecret进行解密
+        self.access_secret = access_secret
+        # AccessKey的密钥，加密传输，网关返回后，使用调用方的AccessSecret进行解密
+        self.account = account
+        # AccessKey创建时间，ISO8601格式
+        self.create_time = create_time
+        # Accessor唯一标识
+        self.id = id
+        # Accessor类型(RAM/ACCOUNT)
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_key is not None:
+            result['access_key'] = self.access_key
+        if self.access_secret is not None:
+            result['access_secret'] = self.access_secret
+        if self.account is not None:
+            result['account'] = self.account
+        if self.create_time is not None:
+            result['create_time'] = self.create_time
+        if self.id is not None:
+            result['id'] = self.id
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('access_key') is not None:
+            self.access_key = m.get('access_key')
+        if m.get('access_secret') is not None:
+            self.access_secret = m.get('access_secret')
+        if m.get('account') is not None:
+            self.account = m.get('account')
+        if m.get('create_time') is not None:
+            self.create_time = m.get('create_time')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class Customer(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        id: str = None,
+        name: str = None,
+        update_time: str = None,
+    ):
+        # 企业创建时间，ISO8601格式
+        self.create_time = create_time
+        # 企业ID
+        self.id = id
+        # 企业名称
+        self.name = name
+        # 企业最近一次修改时间，ISO8601格式
+        self.update_time = update_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['create_time'] = self.create_time
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.update_time is not None:
+            result['update_time'] = self.update_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('create_time') is not None:
+            self.create_time = m.get('create_time')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('update_time') is not None:
+            self.update_time = m.get('update_time')
+        return self
+
+
+class MfaConfig(TeaModel):
     def __init__(
         self,
         user_id: str = None,
-        ram_auth_contexts: List[AliyunRamAuthContext] = None,
-        request_info: AliyunPopRequestInfo = None,
+        status: str = None,
+        type: str = None,
+        secret_key: str = None,
+        last_generated_time: str = None,
+        verify_attempts: int = None,
+        first_failure_time: str = None,
     ):
-        # 金融云用户ID
+        # 用户id
         self.user_id = user_id
-        # 阿里云鉴权列表
-        self.ram_auth_contexts = ram_auth_contexts
-        # BSB透传下来的阿里云信息
-        self.request_info = request_info
+        # MFA状态, 取值范围：ENABLED, DISABLED
+        self.status = status
+        # MFA类型，取值范围：SELF(自有MFA), SYMANTEC(赛门铁克MFA)
+        self.type = type
+        # 密钥
+        self.secret_key = secret_key
+        # 最后一次密钥生成时间
+        self.last_generated_time = last_generated_time
+        # (校验失败时)重试校验的次数, 0 代表不限次数
+        self.verify_attempts = verify_attempts
+        # 第一次校验失败时间, ISO8601格式
+        self.first_failure_time = first_failure_time
 
     def validate(self):
-        self.validate_required(self.user_id, 'user_id')
-        self.validate_required(self.ram_auth_contexts, 'ram_auth_contexts')
-        if self.ram_auth_contexts:
-            for k in self.ram_auth_contexts:
-                if k:
-                    k.validate()
-        self.validate_required(self.request_info, 'request_info')
-        if self.request_info:
-            self.request_info.validate()
+        pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.user_id is not None:
             result['user_id'] = self.user_id
-        result['ram_auth_contexts'] = []
-        if self.ram_auth_contexts is not None:
-            for k in self.ram_auth_contexts:
-                result['ram_auth_contexts'].append(k.to_map() if k else None)
-        if self.request_info is not None:
-            result['request_info'] = self.request_info.to_map()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.type is not None:
+            result['type'] = self.type
+        if self.secret_key is not None:
+            result['secret_key'] = self.secret_key
+        if self.last_generated_time is not None:
+            result['last_generated_time'] = self.last_generated_time
+        if self.verify_attempts is not None:
+            result['verify_attempts'] = self.verify_attempts
+        if self.first_failure_time is not None:
+            result['first_failure_time'] = self.first_failure_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
-        self.ram_auth_contexts = []
-        if m.get('ram_auth_contexts') is not None:
-            for k in m.get('ram_auth_contexts'):
-                temp_model = AliyunRamAuthContext()
-                self.ram_auth_contexts.append(temp_model.from_map(k))
-        if m.get('request_info') is not None:
-            temp_model = AliyunPopRequestInfo()
-            self.request_info = temp_model.from_map(m['request_info'])
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('secret_key') is not None:
+            self.secret_key = m.get('secret_key')
+        if m.get('last_generated_time') is not None:
+            self.last_generated_time = m.get('last_generated_time')
+        if m.get('verify_attempts') is not None:
+            self.verify_attempts = m.get('verify_attempts')
+        if m.get('first_failure_time') is not None:
+            self.first_failure_time = m.get('first_failure_time')
+        return self
+
+
+class Group(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+        name: str = None,
+        description: str = None,
+    ):
+        # 成员组ID
+        self.id = id
+        # 成员组名称
+        self.name = name
+        # 成员组描述
+        self.description = description
+
+    def validate(self):
+        self.validate_required(self.id, 'id')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.description, 'description')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.description is not None:
+            result['description'] = self.description
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('description') is not None:
+            self.description = m.get('description')
         return self
 
 
 class Operator(TeaModel):
     def __init__(
         self,
         create_time: str = None,
@@ -1196,14 +1760,15 @@
         mobile: str = None,
         nickname: str = None,
         real_name: str = None,
         status: str = None,
         tenants: List[str] = None,
         update_time: str = None,
         work_no: str = None,
+        department_code: str = None,
     ):
         # 操作员创建时间，ISO8601格式
         self.create_time = create_time
         # 操作员所在的企业
         self.customer = customer
         # 邮箱
         self.email = email
@@ -1227,19 +1792,25 @@
         self.status = status
         # 操作员加入的租户列表
         self.tenants = tenants
         # 操作员最近一次修改时间，ISO8601格式
         self.update_time = update_time
         # 操作员工号
         self.work_no = work_no
+        # 部门唯一码
+        self.department_code = department_code
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.create_time is not None:
             result['create_time'] = self.create_time
         if self.customer is not None:
             result['customer'] = self.customer
         if self.email is not None:
             result['email'] = self.email
@@ -1263,14 +1834,16 @@
             result['status'] = self.status
         if self.tenants is not None:
             result['tenants'] = self.tenants
         if self.update_time is not None:
             result['update_time'] = self.update_time
         if self.work_no is not None:
             result['work_no'] = self.work_no
+        if self.department_code is not None:
+            result['department_code'] = self.department_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('create_time') is not None:
             self.create_time = m.get('create_time')
         if m.get('customer') is not None:
@@ -1297,187 +1870,38 @@
             self.status = m.get('status')
         if m.get('tenants') is not None:
             self.tenants = m.get('tenants')
         if m.get('update_time') is not None:
             self.update_time = m.get('update_time')
         if m.get('work_no') is not None:
             self.work_no = m.get('work_no')
-        return self
-
-
-class AccessKey(TeaModel):
-    def __init__(
-        self,
-        create_time: str = None,
-        id: str = None,
-        secret: str = None,
-        status: str = None,
-        update_time: str = None,
-    ):
-        # AccessKey创建时间，ISO8601格式
-        self.create_time = create_time
-        # AccessKey唯一标识
-        self.id = id
-        # AccessKey的秘钥，加密传输，网关返回后，使用调用方的AccesSecret进行解密
-        self.secret = secret
-        # 状态
-        self.status = status
-        # AccessKey最近一次修改时间，ISO8601格式
-        self.update_time = update_time
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.create_time is not None:
-            result['create_time'] = self.create_time
-        if self.id is not None:
-            result['id'] = self.id
-        if self.secret is not None:
-            result['secret'] = self.secret
-        if self.status is not None:
-            result['status'] = self.status
-        if self.update_time is not None:
-            result['update_time'] = self.update_time
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('create_time') is not None:
-            self.create_time = m.get('create_time')
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('secret') is not None:
-            self.secret = m.get('secret')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('update_time') is not None:
-            self.update_time = m.get('update_time')
-        return self
-
-
-class Accessor(TeaModel):
-    def __init__(
-        self,
-        access_key: str = None,
-        access_secret: str = None,
-        account: str = None,
-        create_time: str = None,
-        id: str = None,
-        type: str = None,
-    ):
-        # Accessor关联的AccessKey
-        self.access_key = access_key
-        # Accessor关联的AccessKey的密钥，加密传输，网关返回后，使用调用方的AccessSecret进行解密
-        self.access_secret = access_secret
-        # AccessKey的密钥，加密传输，网关返回后，使用调用方的AccessSecret进行解密
-        self.account = account
-        # AccessKey创建时间，ISO8601格式
-        self.create_time = create_time
-        # Accessor唯一标识
-        self.id = id
-        # Accessor类型(RAM/ACCOUNT)
-        self.type = type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.access_key is not None:
-            result['access_key'] = self.access_key
-        if self.access_secret is not None:
-            result['access_secret'] = self.access_secret
-        if self.account is not None:
-            result['account'] = self.account
-        if self.create_time is not None:
-            result['create_time'] = self.create_time
-        if self.id is not None:
-            result['id'] = self.id
-        if self.type is not None:
-            result['type'] = self.type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('access_key') is not None:
-            self.access_key = m.get('access_key')
-        if m.get('access_secret') is not None:
-            self.access_secret = m.get('access_secret')
-        if m.get('account') is not None:
-            self.account = m.get('account')
-        if m.get('create_time') is not None:
-            self.create_time = m.get('create_time')
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        return self
-
-
-class Customer(TeaModel):
-    def __init__(
-        self,
-        create_time: str = None,
-        id: str = None,
-        name: str = None,
-        update_time: str = None,
-    ):
-        # 企业创建时间，ISO8601格式
-        self.create_time = create_time
-        # 企业ID
-        self.id = id
-        # 企业名称
-        self.name = name
-        # 企业最近一次修改时间，ISO8601格式
-        self.update_time = update_time
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.create_time is not None:
-            result['create_time'] = self.create_time
-        if self.id is not None:
-            result['id'] = self.id
-        if self.name is not None:
-            result['name'] = self.name
-        if self.update_time is not None:
-            result['update_time'] = self.update_time
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('create_time') is not None:
-            self.create_time = m.get('create_time')
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('update_time') is not None:
-            self.update_time = m.get('update_time')
+        if m.get('department_code') is not None:
+            self.department_code = m.get('department_code')
         return self
 
 
 class GetRoleRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         role_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色ID
         self.role_id = role_id
 
     def validate(self):
         self.validate_required(self.role_id, 'role_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.role_id is not None:
             result['role_id'] = self.role_id
         return result
 
@@ -1501,16 +1925,19 @@
         description: str = None,
         id: str = None,
         name: str = None,
         tenant: str = None,
         type: str = None,
         update_time: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 角色所包含的操作点
         self.actions = actions
         # 创建时间,ISO8601格式
         self.create_time = create_time
         # 角色描述
         self.description = description
@@ -1528,14 +1955,18 @@
     def validate(self):
         if self.actions:
             for k in self.actions:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1595,14 +2026,15 @@
         auth_token: str = None,
         actor_id: str = None,
         actor_type: str = None,
         page_num: int = None,
         page_size: int = None,
         tenant: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 授权对象id
         self.actor_id = actor_id
         # 授权对象类型
         self.actor_type = actor_type
         # 当前页，默认值为1
         self.page_num = page_num
@@ -1613,14 +2045,18 @@
 
     def validate(self):
         self.validate_required(self.actor_id, 'actor_id')
         self.validate_required(self.actor_type, 'actor_type')
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.actor_type is not None:
             result['actor_type'] = self.actor_type
@@ -1656,16 +2092,19 @@
         result_code: str = None,
         result_msg: str = None,
         page_num: int = None,
         page_size: int = None,
         policies: List[AuthPolicy] = None,
         total_count: int = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 传入的页码, 如果没有传入, 则取默认值1
         self.page_num = page_num
         # 传入的页大小, 如果没有传入, 则取默认值10
         self.page_size = page_size
         # 授权策略列表
         self.policies = policies
@@ -1679,14 +2118,18 @@
         if self.policies:
             for k in self.policies:
                 if k:
                     k.validate()
         self.validate_required(self.total_count, 'total_count')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1729,28 +2172,33 @@
         self,
         auth_token: str = None,
         member_id: str = None,
         name: str = None,
         page_num: int = None,
         page_size: int = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 授权组成员ID。授权组成员是操作员
         self.member_id = member_id
         # 授权组名称
         self.name = name
         # 当前页码，默认为1
         self.page_num = page_num
         # 分页大小，默认10
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.member_id is not None:
             result['member_id'] = self.member_id
         if self.name is not None:
             result['name'] = self.name
@@ -1782,16 +2230,19 @@
         result_code: str = None,
         result_msg: str = None,
         groups: List[AuthGroup] = None,
         page_num: int = None,
         page_size: int = None,
         total_count: int = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 授权组列表
         self.groups = groups
         # 当前页码
         self.page_num = page_num
         # 分页大小
         self.page_size = page_size
@@ -1805,14 +2256,18 @@
                 if k:
                     k.validate()
         self.validate_required(self.page_num, 'page_num')
         self.validate_required(self.page_size, 'page_size')
         self.validate_required(self.total_count, 'total_count')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1857,14 +2312,15 @@
         ability_id: str = None,
         ability_type: str = None,
         conditons: List[Condition] = None,
         description: str = None,
         name: str = None,
         tenant: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色Id
         self.ability_id = ability_id
         # 授权能力类型（ROLE：角色)
         self.ability_type = ability_type
         # 授权策略的限制条件
         self.conditons = conditons
@@ -1882,14 +2338,18 @@
             for k in self.conditons:
                 if k:
                     k.validate()
         self.validate_required(self.name, 'name')
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.ability_id is not None:
             result['ability_id'] = self.ability_id
         if self.ability_type is not None:
             result['ability_type'] = self.ability_type
@@ -1931,24 +2391,31 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         policy_id: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 授权策略id
         self.policy_id = policy_id
 
     def validate(self):
         self.validate_required(self.policy_id, 'policy_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1971,22 +2438,27 @@
 
 class DeletePolicyRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         policy_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 授权策略Id
         self.policy_id = policy_id
 
     def validate(self):
         self.validate_required(self.policy_id, 'policy_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.policy_id is not None:
             result['policy_id'] = self.policy_id
         return result
 
@@ -2002,22 +2474,29 @@
 class DeletePolicyResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2037,68 +2516,92 @@
 class AttachPolicyRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         actor_id: str = None,
         actor_type: str = None,
         policy_id: str = None,
+        login_name: str = None,
+        policy_name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 授权对象Id
         self.actor_id = actor_id
         # 授权对象类型
         self.actor_type = actor_type
         # 授权策略Id
         self.policy_id = policy_id
+        # 授权操作员的登录名，当配置actor_id与actor_type时可不填
+        self.login_name = login_name
+        # 授权策略的唯一名称，当配置policy_id时可不填
+        self.policy_name = policy_name
 
     def validate(self):
-        self.validate_required(self.actor_id, 'actor_id')
-        self.validate_required(self.actor_type, 'actor_type')
-        self.validate_required(self.policy_id, 'policy_id')
+        pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.actor_type is not None:
             result['actor_type'] = self.actor_type
         if self.policy_id is not None:
             result['policy_id'] = self.policy_id
+        if self.login_name is not None:
+            result['login_name'] = self.login_name
+        if self.policy_name is not None:
+            result['policy_name'] = self.policy_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('actor_id') is not None:
             self.actor_id = m.get('actor_id')
         if m.get('actor_type') is not None:
             self.actor_type = m.get('actor_type')
         if m.get('policy_id') is not None:
             self.policy_id = m.get('policy_id')
+        if m.get('login_name') is not None:
+            self.login_name = m.get('login_name')
+        if m.get('policy_name') is not None:
+            self.policy_name = m.get('policy_name')
         return self
 
 
 class AttachPolicyResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2118,68 +2621,92 @@
 class DetachPolicyRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         actor_id: str = None,
         actor_type: str = None,
         policy_id: str = None,
+        login_name: str = None,
+        policy_name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 授权对象Id
         self.actor_id = actor_id
         # 授权对象类型
         self.actor_type = actor_type
         # 授权策略Id
         self.policy_id = policy_id
+        # 授权操作员的登录名，当配置actor_id与actor_type时可不填
+        self.login_name = login_name
+        # 授权策略的唯一名称，当配置policy_id时可不填
+        self.policy_name = policy_name
 
     def validate(self):
-        self.validate_required(self.actor_id, 'actor_id')
-        self.validate_required(self.actor_type, 'actor_type')
-        self.validate_required(self.policy_id, 'policy_id')
+        pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.actor_type is not None:
             result['actor_type'] = self.actor_type
         if self.policy_id is not None:
             result['policy_id'] = self.policy_id
+        if self.login_name is not None:
+            result['login_name'] = self.login_name
+        if self.policy_name is not None:
+            result['policy_name'] = self.policy_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('actor_id') is not None:
             self.actor_id = m.get('actor_id')
         if m.get('actor_type') is not None:
             self.actor_type = m.get('actor_type')
         if m.get('policy_id') is not None:
             self.policy_id = m.get('policy_id')
+        if m.get('login_name') is not None:
+            self.login_name = m.get('login_name')
+        if m.get('policy_name') is not None:
+            self.policy_name = m.get('policy_name')
         return self
 
 
 class DetachPolicyResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2200,27 +2727,32 @@
     def __init__(
         self,
         auth_token: str = None,
         actor_id: str = None,
         actor_type: str = None,
         tenant: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 授权对象id
         self.actor_id = actor_id
         # 授权对象类型
         self.actor_type = actor_type
         # 授权策略所属租户
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.actor_id, 'actor_id')
         self.validate_required(self.actor_type, 'actor_type')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.actor_type is not None:
             result['actor_type'] = self.actor_type
@@ -2245,28 +2777,35 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         policies: List[AuthPolicy] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 授权策略列表
         self.policies = policies
 
     def validate(self):
         self.validate_required(self.policies, 'policies')
         if self.policies:
             for k in self.policies:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2296,14 +2835,15 @@
     def __init__(
         self,
         auth_token: str = None,
         action_id: str = None,
         conditions: List[Condition] = None,
         operator_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作点id
         self.action_id = action_id
         # 鉴权条件
         self.conditions = conditions
         # 鉴权对象id
         self.operator_id = operator_id
@@ -2313,14 +2853,18 @@
         if self.conditions:
             for k in self.conditions:
                 if k:
                     k.validate()
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.action_id is not None:
             result['action_id'] = self.action_id
         result['conditions'] = []
         if self.conditions is not None:
@@ -2350,24 +2894,31 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         result: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 判断结果。true：鉴权通过；false：鉴权未通过
         self.result = result
 
     def validate(self):
         self.validate_required(self.result, 'result')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2394,14 +2945,15 @@
         auth_token: str = None,
         action_id: str = None,
         category_id: str = None,
         description: str = None,
         name: str = None,
         product: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作点ID
         self.action_id = action_id
         # 操作点所属功能分类ID
         self.category_id = category_id
         # 操作点描述
         self.description = description
@@ -2412,14 +2964,18 @@
 
     def validate(self):
         self.validate_required(self.action_id, 'action_id')
         self.validate_required(self.name, 'name')
         self.validate_required(self.product, 'product')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.action_id is not None:
             result['action_id'] = self.action_id
         if self.category_id is not None:
             result['category_id'] = self.category_id
@@ -2451,22 +3007,29 @@
 class CreateProductActionResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2487,27 +3050,32 @@
     def __init__(
         self,
         auth_token: str = None,
         access_token: str = None,
         extend: bool = None,
         scene: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # token值
         self.access_token = access_token
         # 是否刷新access_token有限期
         self.extend = extend
         # token应用场景，LOGIN或AUTH
         self.scene = scene
 
     def validate(self):
         self.validate_required(self.access_token, 'access_token')
         self.validate_required(self.scene, 'scene')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.access_token is not None:
             result['access_token'] = self.access_token
         if self.extend is not None:
             result['extend'] = self.extend
@@ -2533,26 +3101,33 @@
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         id: str = None,
         type: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # token关联的用户id
         self.id = id
         # token关联的用户类型
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2579,22 +3154,27 @@
 
 class VerifySessionTokenRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         token: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # token值
         self.token = token
 
     def validate(self):
         self.validate_required(self.token, 'token')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.token is not None:
             result['token'] = self.token
         return result
 
@@ -2615,16 +3195,19 @@
         result_msg: str = None,
         customer: str = None,
         login_name: str = None,
         tenants: List[str] = None,
         user_id: str = None,
         tenant_details: List[Tenant] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 用户所在企业的唯一标识
         self.customer = customer
         # 登录名
         self.login_name = login_name
         # 用户加入的租户ID列表
         self.tenants = tenants
@@ -2636,14 +3219,18 @@
     def validate(self):
         if self.tenant_details:
             for k in self.tenant_details:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2688,25 +3275,30 @@
 class ListRoleOperatorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         role_id: str = None,
         tenant: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色ID
         self.role_id = role_id
         # 租户信息
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.role_id, 'role_id')
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.role_id is not None:
             result['role_id'] = self.role_id
         if self.tenant is not None:
             result['tenant'] = self.tenant
@@ -2727,28 +3319,35 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         operators: List[Operator] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 操作员列表
         self.operators = operators
 
     def validate(self):
         self.validate_required(self.operators, 'operators')
         if self.operators:
             for k in self.operators:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2777,25 +3376,30 @@
 class ApplyTrustloginUrlRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         goto_url: str = None,
         operator_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 跳转地址
         self.goto_url = goto_url
         # 操作员id
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.goto_url, 'goto_url')
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.goto_url is not None:
             result['goto_url'] = self.goto_url
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
@@ -2816,24 +3420,31 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         trust_login_url: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 信登URL
         self.trust_login_url = trust_login_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2859,14 +3470,15 @@
         self,
         auth_token: str = None,
         actor_name: str = None,
         actor_tenant: str = None,
         duration_seconds: int = None,
         session_name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 虚拟身份唯一名称
         self.actor_name = actor_name
         # 虚拟身份所属租户
         self.actor_tenant = actor_tenant
         # 过期时间，单位为秒，范围900-3600，默认为3600
         self.duration_seconds = duration_seconds
@@ -2875,14 +3487,18 @@
 
     def validate(self):
         self.validate_required(self.actor_name, 'actor_name')
         self.validate_required(self.actor_tenant, 'actor_tenant')
         self.validate_required(self.session_name, 'session_name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_name is not None:
             result['actor_name'] = self.actor_name
         if self.actor_tenant is not None:
             result['actor_tenant'] = self.actor_tenant
@@ -2914,30 +3530,37 @@
         result_code: str = None,
         result_msg: str = None,
         access_key: str = None,
         access_secret: str = None,
         expired_time: int = None,
         security_token: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 安全令牌accessKey
         self.access_key = access_key
         # 安全令牌accessSecret
         self.access_secret = access_secret
         # 过期时间戳，单位为毫秒
         self.expired_time = expired_time
         # 安全令牌
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2974,14 +3597,15 @@
     def __init__(
         self,
         auth_token: str = None,
         bindings: List[StsActorBinding] = None,
         description: str = None,
         name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 虚拟身份受信关系集合，通常只包含一个
         self.bindings = bindings
         # 针对虚拟身份的描述
         self.description = description
         # 虚拟身份名称，租户内唯一
         self.name = name
@@ -2991,14 +3615,18 @@
         if self.bindings:
             for k in self.bindings:
                 if k:
                     k.validate()
         self.validate_required(self.name, 'name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         result['bindings'] = []
         if self.bindings is not None:
             for k in self.bindings:
                 result['bindings'].append(k.to_map() if k else None)
@@ -3028,24 +3656,31 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         actor_id: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 虚拟身份ID
         self.actor_id = actor_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3069,24 +3704,29 @@
 class DeleteStsActorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         actor_id: str = None,
         actor_name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 虚拟身份ID，与虚拟身份名称两个参数二选一传入
         self.actor_id = actor_id
         # 虚拟身份名称，与虚拟身份名称两个参数二选一传入
         self.actor_name = actor_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.actor_name is not None:
             result['actor_name'] = self.actor_name
@@ -3106,22 +3746,29 @@
 class DeleteStsActorResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3141,24 +3788,29 @@
 class GetStsActorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         actor_id: str = None,
         actor_name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 虚拟身份ID，与虚拟身份名称两个参数二选一传入
         self.actor_id = actor_id
         # 虚拟身份名称，与虚拟身份名称两个参数二选一传入
         self.actor_name = actor_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.actor_name is not None:
             result['actor_name'] = self.actor_name
@@ -3183,16 +3835,19 @@
         result_msg: str = None,
         bindings: List[StsActorBinding] = None,
         description: str = None,
         id: str = None,
         name: str = None,
         tenant: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 虚拟身份受信关系集合，通常只包含一个
         self.bindings = bindings
         # 针对虚拟身份的描述
         self.description = description
         # 虚拟身份ID
         self.id = id
@@ -3204,14 +3859,18 @@
     def validate(self):
         if self.bindings:
             for k in self.bindings:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3254,20 +3913,25 @@
 
 
 class ListStsActorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -3280,27 +3944,34 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         actors: List[StsActor] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 虚拟身份列表
         self.actors = actors
 
     def validate(self):
         if self.actors:
             for k in self.actors:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3329,24 +4000,29 @@
 class UpdateStsActorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         actor_id: str = None,
         description: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 虚拟身份ID
         self.actor_id = actor_id
         # 针对虚拟身份的描述
         self.description = description
 
     def validate(self):
         self.validate_required(self.actor_id, 'actor_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.actor_id is not None:
             result['actor_id'] = self.actor_id
         if self.description is not None:
             result['description'] = self.description
@@ -3371,16 +4047,19 @@
         result_msg: str = None,
         bindings: List[StsActorBinding] = None,
         description: str = None,
         id: str = None,
         name: str = None,
         tenant: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 虚拟身份受信关系集合，通常只包含一个
         self.bindings = bindings
         # 针对虚拟身份的描述
         self.description = description
         # 虚拟身份ID
         self.id = id
@@ -3392,14 +4071,18 @@
     def validate(self):
         if self.bindings:
             for k in self.bindings:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3447,14 +4130,15 @@
         auth_token: str = None,
         name: str = None,
         page_num: int = None,
         page_size: int = None,
         paging: bool = None,
         type: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色名称
         self.name = name
         # 当前页,默认1
         self.page_num = page_num
         # 分页大小，取值范围[1~50],默认10
         self.page_size = page_size
@@ -3463,14 +4147,18 @@
         # 角色类型，自定义角色为CUSTOM或者系统角色为COMMON
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.name is not None:
             result['name'] = self.name
         if self.page_num is not None:
             result['page_num'] = self.page_num
@@ -3506,16 +4194,19 @@
         result_code: str = None,
         result_msg: str = None,
         page_num: int = None,
         page_size: int = None,
         roles: List[Role] = None,
         total_count: int = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 当前页
         self.page_num = page_num
         # 分页大小
         self.page_size = page_size
         # 角色列表
         self.roles = roles
@@ -3525,14 +4216,18 @@
     def validate(self):
         if self.roles:
             for k in self.roles:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3571,20 +4266,25 @@
 
 
 class GetIaasaccountBaseinfoRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -3599,16 +4299,19 @@
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         account: str = None,
         id: str = None,
         source_type: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 账号名称
         self.account = account
         # 账号ID
         self.id = id
         # iaas账号类型
         # ALIYUN_BID: 阿里云BID类型
@@ -3617,14 +4320,18 @@
         # ALIYUN_LOCALIZATION: 阿里云一方化类型
         self.source_type = source_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3656,25 +4363,30 @@
 class VerifyPasswordRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         encrypted_password: str = None,
         login_name: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 加密过的密码值，使用AccessSecret进行3DES加密
         self.encrypted_password = encrypted_password
         # 登录名
         self.login_name = login_name
 
     def validate(self):
         self.validate_required(self.encrypted_password, 'encrypted_password')
         self.validate_required(self.login_name, 'login_name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.encrypted_password is not None:
             result['encrypted_password'] = self.encrypted_password
         if self.login_name is not None:
             result['login_name'] = self.login_name
@@ -3694,22 +4406,29 @@
 class VerifyPasswordResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3729,25 +4448,30 @@
 class UpdateOperatorStatusRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         operator_id: str = None,
         status: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作员ID
         self.operator_id = operator_id
         # 要更新到的状态，FROZEN为冻结，NORMAL为正常
         self.status = status
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
         self.validate_required(self.status, 'status')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         if self.status is not None:
             result['status'] = self.status
@@ -3767,22 +4491,29 @@
 class UpdateOperatorStatusResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3801,22 +4532,27 @@
 
 class FreezeOperatorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         operator_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作员ID
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         return result
 
@@ -3832,22 +4568,29 @@
 class FreezeOperatorResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3866,22 +4609,27 @@
 
 class UnfreezeOperatorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         operator_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作员ID
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         return result
 
@@ -3897,22 +4645,29 @@
 class UnfreezeOperatorResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3933,26 +4688,31 @@
     def __init__(
         self,
         auth_token: str = None,
         iaas_id: str = None,
         master_id: str = None,
         source_system: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 阿里云PK
         self.iaas_id = iaas_id
         # 主账号ID
         self.master_id = master_id
         # 来源系统，例如MAYI，ALBABACLOUD
         self.source_system = source_system
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.iaas_id is not None:
             result['iaas_id'] = self.iaas_id
         if self.master_id is not None:
             result['master_id'] = self.master_id
@@ -3988,16 +4748,19 @@
         id: str = None,
         login_name: str = None,
         mobile: str = None,
         real_name: str = None,
         source_user_type: str = None,
         industry_label: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 证件ID
         self.cert_no = cert_no
         # 证件类型
         self.cert_type = cert_type
         # 所属客户ID
         self.customer_id = customer_id
@@ -4020,14 +4783,18 @@
         # 主账号行业标签，I表示金融机构，C表示特殊机构，N表示非金融机构
         self.industry_label = industry_label
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4094,22 +4861,27 @@
 
 class GetAliyunUserRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         user_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 阿里云用户ID
         self.user_id = user_id
 
     def validate(self):
         self.validate_required(self.user_id, 'user_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.user_id is not None:
             result['user_id'] = self.user_id
         return result
 
@@ -4132,16 +4904,19 @@
         login_name: str = None,
         name: str = None,
         ram_display_name: str = None,
         tenant: str = None,
         type: str = None,
         display_name: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 阿里云用户ID
         self.id = id
         # 主账号类型下有值，即type为ENTERPRISE和PERSONAL时有值
         self.login_name = login_name
         # 用户名称，ENTERPRISE类型为企业名称，PERSONAL为个人姓名，RAM为唯一名称
         self.name = name
@@ -4154,14 +4929,18 @@
         # 显示名
         self.display_name = display_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4214,14 +4993,15 @@
         aliyun_resources: List[AliyunResource] = None,
         conditions: List[Condition] = None,
         region_id: str = None,
         request_info: AliyunPopRequestInfo = None,
         service_name: str = None,
         user_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 阿里云POP API名称
         self.action = action
         # 阿里云资源描述数组
         self.aliyun_resources = aliyun_resources
         # 自定义条件
         self.conditions = conditions
@@ -4249,14 +5029,18 @@
         self.validate_required(self.request_info, 'request_info')
         if self.request_info:
             self.request_info.validate()
         self.validate_required(self.service_name, 'service_name')
         self.validate_required(self.user_id, 'user_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.action is not None:
             result['action'] = self.action
         result['aliyun_resources'] = []
         if self.aliyun_resources is not None:
@@ -4310,28 +5094,35 @@
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         result: bool = None,
         reason: str = None,
         solution: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 权限校验是否通过
         self.result = result
         # 失败原因
         self.reason = reason
         # 解决方案
         self.solution = solution
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4363,25 +5154,30 @@
 class GetSessionAccessorRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         authorization: str = None,
         user_tenant: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 登录态
         self.authorization = authorization
         # 用户所属租户
         self.user_tenant = user_tenant
 
     def validate(self):
         self.validate_required(self.authorization, 'authorization')
         self.validate_required(self.user_tenant, 'user_tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.authorization is not None:
             result['authorization'] = self.authorization
         if self.user_tenant is not None:
             result['user_tenant'] = self.user_tenant
@@ -4405,30 +5201,37 @@
         result_code: str = None,
         result_msg: str = None,
         access_key: str = None,
         access_secret: str = None,
         tenant: str = None,
         user_id: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # access_key
         self.access_key = access_key
         # access_secret
         self.access_secret = access_secret
         # 关联租户名称
         self.tenant = tenant
         # 用户ID
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4465,14 +5268,15 @@
     def __init__(
         self,
         auth_token: str = None,
         login_name: str = None,
         new_encrypted_password: str = None,
         old_encrypted_password: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 登录名
         self.login_name = login_name
         # 加密过的新密码值，使用AccessSecret进行3DES加密
         # 
         self.new_encrypted_password = new_encrypted_password
         # 加密过的旧密码值，使用AccessSecret进行DES加密
@@ -4481,14 +5285,18 @@
 
     def validate(self):
         self.validate_required(self.login_name, 'login_name')
         self.validate_required(self.new_encrypted_password, 'new_encrypted_password')
         self.validate_required(self.old_encrypted_password, 'old_encrypted_password')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.login_name is not None:
             result['login_name'] = self.login_name
         if self.new_encrypted_password is not None:
             result['new_encrypted_password'] = self.new_encrypted_password
@@ -4512,22 +5320,29 @@
 class UpdatePasswordResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4547,26 +5362,31 @@
 class JudgeMultiauthorityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         batch_event: AuthenticateBatchEvent = None,
         context: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 批量鉴权对象
         self.batch_event = batch_event
         # 上下文信息
         self.context = context
 
     def validate(self):
         self.validate_required(self.batch_event, 'batch_event')
         if self.batch_event:
             self.batch_event.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.batch_event is not None:
             result['batch_event'] = self.batch_event.to_map()
         if self.context is not None:
             result['context'] = self.context
@@ -4588,27 +5408,34 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         judgements: List[Judgement] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 鉴权结果列表
         self.judgements = judgements
 
     def validate(self):
         if self.judgements:
             for k in self.judgements:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4637,26 +5464,31 @@
 class JudgeAliyunMultiauthorityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         batch_event: AliyunAuthenticateBatchEvent = None,
         context: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 阿里云批量鉴权
         self.batch_event = batch_event
         # 上下文信息
         self.context = context
 
     def validate(self):
         self.validate_required(self.batch_event, 'batch_event')
         if self.batch_event:
             self.batch_event.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.batch_event is not None:
             result['batch_event'] = self.batch_event.to_map()
         if self.context is not None:
             result['context'] = self.context
@@ -4678,27 +5510,34 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         judgements: List[Judgement] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 鉴权结果列表
         self.judgements = judgements
 
     def validate(self):
         if self.judgements:
             for k in self.judgements:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4725,20 +5564,25 @@
 
 
 class GetAccessorCurrentRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -4755,16 +5599,19 @@
         result_msg: str = None,
         id: str = None,
         login_name: str = None,
         name: str = None,
         tenant: str = None,
         type: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 一方化链路为阿里云用户ID，蚂蚁链路为金融云用户ID
         self.id = id
         # 登录名
         self.login_name = login_name
         # 一方化链路：
         # 用户名称，ENTERPRISE类型为企业名称，PERSONAL为个人姓名，RAM为唯一名称
@@ -4780,14 +5627,18 @@
         # 主账号为MASTER，操作员为OPERATOR，服务账号为SERVICE
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4827,24 +5678,29 @@
 class GetServiceaccountRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         name: str = None,
         service_account_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 服务账号名称
         self.name = name
         # 服务账号ID
         self.service_account_id = service_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.name is not None:
             result['name'] = self.name
         if self.service_account_id is not None:
             result['service_account_id'] = self.service_account_id
@@ -4869,16 +5725,19 @@
         result_msg: str = None,
         alias: str = None,
         description: str = None,
         id: str = None,
         name: str = None,
         tenant: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 服务账号别名
         self.alias = alias
         # 服务账号描述
         self.description = description
         # 服务账号ID
         self.id = id
@@ -4887,14 +5746,18 @@
         # 服务账号所属租户
         self.tenant = tenant
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -4934,24 +5797,29 @@
 class CreateServiceaccountRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         description: str = None,
         alias: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 服务账号描述
         self.description = description
         # 服务账号别名
         self.alias = alias
 
     def validate(self):
         self.validate_required(self.alias, 'alias')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.description is not None:
             result['description'] = self.description
         if self.alias is not None:
             result['alias'] = self.alias
@@ -4978,16 +5846,19 @@
         access_secret: str = None,
         alias: str = None,
         description: str = None,
         id: str = None,
         name: str = None,
         tenant: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 服务账号AK
         self.access_key = access_key
         # 服务账号SK
         self.access_secret = access_secret
         # 服务账号别名
         self.alias = alias
@@ -5000,14 +5871,18 @@
         # 服务账号所属租户
         self.tenant = tenant
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5055,24 +5930,29 @@
 class DeleteServiceaccountRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         name: str = None,
         service_account_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 服务账号名称
         self.name = name
         # 服务账号ID
         self.service_account_id = service_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.name is not None:
             result['name'] = self.name
         if self.service_account_id is not None:
             result['service_account_id'] = self.service_account_id
@@ -5092,22 +5972,29 @@
 class DeleteServiceaccountResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5129,28 +6016,33 @@
         self,
         auth_token: str = None,
         alias: str = None,
         description: str = None,
         name: str = None,
         service_account_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 服务账号别名
         self.alias = alias
         # 服务账号描述
         self.description = description
         # 服务账号名称，与服务账号ID任选其一传入
         self.name = name
         # 服务账号ID
         self.service_account_id = service_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.alias is not None:
             result['alias'] = self.alias
         if self.description is not None:
             result['description'] = self.description
@@ -5178,22 +6070,29 @@
 class UpdateServiceaccountResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5212,22 +6111,27 @@
 
 class RemoveTenantMemberRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         operator_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作员ID
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         return result
 
@@ -5243,22 +6147,29 @@
 class RemoveTenantMemberResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5278,24 +6189,29 @@
 class CreateGroupRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         name: str = None,
         description: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 名称
         self.name = name
         # 描述
         self.description = description
 
     def validate(self):
         self.validate_required(self.name, 'name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.name is not None:
             result['name'] = self.name
         if self.description is not None:
             result['description'] = self.description
@@ -5316,24 +6232,31 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         id: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 成员组ID
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5356,22 +6279,27 @@
 
 class DeleteGroupRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         group_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 成员组ID
         self.group_id = group_id
 
     def validate(self):
         self.validate_required(self.group_id, 'group_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.group_id is not None:
             result['group_id'] = self.group_id
         return result
 
@@ -5387,22 +6315,29 @@
 class DeleteGroupResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5423,26 +6358,31 @@
     def __init__(
         self,
         auth_token: str = None,
         group_id: str = None,
         name: str = None,
         description: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 成员组ID
         self.group_id = group_id
         # 名称
         self.name = name
         # 描述
         self.description = description
 
     def validate(self):
         self.validate_required(self.group_id, 'group_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.group_id is not None:
             result['group_id'] = self.group_id
         if self.name is not None:
             result['name'] = self.name
@@ -5466,22 +6406,29 @@
 class UpdateGroupResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5501,25 +6448,30 @@
 class AddGroupMemberRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         group_id: str = None,
         operator_ids: List[str] = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 成员组ID
         self.group_id = group_id
         # 操作员ID
         self.operator_ids = operator_ids
 
     def validate(self):
         self.validate_required(self.group_id, 'group_id')
         self.validate_required(self.operator_ids, 'operator_ids')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.group_id is not None:
             result['group_id'] = self.group_id
         if self.operator_ids is not None:
             result['operator_ids'] = self.operator_ids
@@ -5539,22 +6491,29 @@
 class AddGroupMemberResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5574,25 +6533,30 @@
 class RemoveGroupMemberRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         group_id: str = None,
         operator_ids: List[str] = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 成员组ID
         self.group_id = group_id
         # 操作员ID
         self.operator_ids = operator_ids
 
     def validate(self):
         self.validate_required(self.group_id, 'group_id')
         self.validate_required(self.operator_ids, 'operator_ids')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.group_id is not None:
             result['group_id'] = self.group_id
         if self.operator_ids is not None:
             result['operator_ids'] = self.operator_ids
@@ -5612,22 +6576,29 @@
 class RemoveGroupMemberResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5646,22 +6617,27 @@
 
 class GetGroupRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         group_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 成员组ID
         self.group_id = group_id
 
     def validate(self):
         self.validate_required(self.group_id, 'group_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.group_id is not None:
             result['group_id'] = self.group_id
         return result
 
@@ -5680,28 +6656,35 @@
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         id: str = None,
         name: str = None,
         description: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 成员组ID
         self.id = id
         # 名称
         self.name = name
         # 描述
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5734,14 +6717,15 @@
     def __init__(
         self,
         auth_token: str = None,
         group_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 成员组ID
         self.group_id = group_id
         # 页大小
         self.page_size = page_size
         # 当前页
         self.current_page = current_page
@@ -5751,14 +6735,18 @@
         if self.page_size is not None:
             self.validate_maximum(self.page_size, 'page_size', 100)
             self.validate_minimum(self.page_size, 'page_size', 10)
         if self.current_page is not None:
             self.validate_minimum(self.current_page, 'current_page', 1)
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.group_id is not None:
             result['group_id'] = self.group_id
         if self.page_size is not None:
             result['page_size'] = self.page_size
@@ -5786,16 +6774,19 @@
         result_code: str = None,
         result_msg: str = None,
         operators: List[Operator] = None,
         current_page: int = None,
         page_size: int = None,
         total_count: int = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 成员列表
         self.operators = operators
         # 当前页
         self.current_page = current_page
         # 页大小
         self.page_size = page_size
@@ -5805,14 +6796,18 @@
     def validate(self):
         if self.operators:
             for k in self.operators:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5852,22 +6847,27 @@
 
 class ListOperatorGroupRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         operator_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 操作员ID
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         return result
 
@@ -5884,27 +6884,34 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         groups: List[Group] = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 成员组列表
         self.groups = groups
 
     def validate(self):
         if self.groups:
             for k in self.groups:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -5933,25 +6940,30 @@
 class AddRoleActionRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         role_id: str = None,
         actions: List[str] = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色ID
         self.role_id = role_id
         # 权限码
         self.actions = actions
 
     def validate(self):
         self.validate_required(self.role_id, 'role_id')
         self.validate_required(self.actions, 'actions')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.role_id is not None:
             result['role_id'] = self.role_id
         if self.actions is not None:
             result['actions'] = self.actions
@@ -5971,22 +6983,29 @@
 class AddRoleActionResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -6006,25 +7025,30 @@
 class RemoveRoleActionRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         role_id: str = None,
         actions: List[str] = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色ID
         self.role_id = role_id
         # 权限码
         self.actions = actions
 
     def validate(self):
         self.validate_required(self.role_id, 'role_id')
         self.validate_required(self.actions, 'actions')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.role_id is not None:
             result['role_id'] = self.role_id
         if self.actions is not None:
             result['actions'] = self.actions
@@ -6044,22 +7068,29 @@
 class RemoveRoleActionResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -6080,26 +7111,31 @@
     def __init__(
         self,
         auth_token: str = None,
         name: str = None,
         description: str = None,
         actions: List[str] = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 名称
         self.name = name
         # 描述
         self.description = description
         # 权限码列表
         self.actions = actions
 
     def validate(self):
         self.validate_required(self.name, 'name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.name is not None:
             result['name'] = self.name
         if self.description is not None:
             result['description'] = self.description
@@ -6124,24 +7160,31 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         id: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
         # 角色ID
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -6164,22 +7207,27 @@
 
 class DeleteRoleRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         role_id: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色ID
         self.role_id = role_id
 
     def validate(self):
         self.validate_required(self.role_id, 'role_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.role_id is not None:
             result['role_id'] = self.role_id
         return result
 
@@ -6195,22 +7243,29 @@
 class DeleteRoleResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -6231,26 +7286,31 @@
     def __init__(
         self,
         auth_token: str = None,
         role_id: str = None,
         name: str = None,
         description: str = None,
     ):
+        # OAuth模式下的授权token
         self.auth_token = auth_token
         # 角色ID
         self.role_id = role_id
         # 名称
         self.name = name
         # 描述
         self.description = description
 
     def validate(self):
         self.validate_required(self.role_id, 'role_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.role_id is not None:
             result['role_id'] = self.role_id
         if self.name is not None:
             result['name'] = self.name
@@ -6274,35 +7334,2798 @@
 class UpdateRoleResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class GetDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一代码
+        self.code = code
+
+    def validate(self):
+        self.validate_required(self.code, 'code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.code is not None:
+            result['code'] = self.code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        return self
+
+
+class GetDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        code: str = None,
+        name: str = None,
+        description: str = None,
+        parent_code: str = None,
+        customer_id: str = None,
+        is_leaf: bool = None,
+        creation_time: str = None,
+        update_time: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
         self.result_code = result_code
+        # 异常信息的文本描述
         self.result_msg = result_msg
+        # 部门唯一代码
+        self.code = code
+        # 部门名称
+        self.name = name
+        # 部门描述信息
+        self.description = description
+        # 父部门 code
+        self.parent_code = parent_code
+        # 企业 id
+        self.customer_id = customer_id
+        # 是否为叶子结点
+        self.is_leaf = is_leaf
+        # 创建时间，ISO8601格式
+        self.creation_time = creation_time
+        # 更新时间，ISO8601格式
+        self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.code is not None:
+            result['code'] = self.code
+        if self.name is not None:
+            result['name'] = self.name
+        if self.description is not None:
+            result['description'] = self.description
+        if self.parent_code is not None:
+            result['parent_code'] = self.parent_code
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
+        if self.is_leaf is not None:
+            result['is_leaf'] = self.is_leaf
+        if self.creation_time is not None:
+            result['creation_time'] = self.creation_time
+        if self.update_time is not None:
+            result['update_time'] = self.update_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('parent_code') is not None:
+            self.parent_code = m.get('parent_code')
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
+        if m.get('is_leaf') is not None:
+            self.is_leaf = m.get('is_leaf')
+        if m.get('creation_time') is not None:
+            self.creation_time = m.get('creation_time')
+        if m.get('update_time') is not None:
+            self.update_time = m.get('update_time')
+        return self
+
+
+class CreateDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        code: str = None,
+        name: str = None,
+        description: str = None,
+        parent_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一码
+        self.code = code
+        # 部门名称
+        self.name = name
+        # 部门描述信息
+        self.description = description
+        # 父部门 code，如果需要创建根部门，需填：ROOT
+        self.parent_code = parent_code
+
+    def validate(self):
+        self.validate_required(self.code, 'code')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.parent_code, 'parent_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.code is not None:
+            result['code'] = self.code
+        if self.name is not None:
+            result['name'] = self.name
+        if self.description is not None:
+            result['description'] = self.description
+        if self.parent_code is not None:
+            result['parent_code'] = self.parent_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('parent_code') is not None:
+            self.parent_code = m.get('parent_code')
+        return self
+
+
+class CreateDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class UpdateDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        code: str = None,
+        name: str = None,
+        description: str = None,
+        parent_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一码
+        self.code = code
+        # 部门名称
+        self.name = name
+        # 部门描述信息
+        self.description = description
+        # 父部们唯一码
+        self.parent_code = parent_code
+
+    def validate(self):
+        self.validate_required(self.code, 'code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.code is not None:
+            result['code'] = self.code
+        if self.name is not None:
+            result['name'] = self.name
+        if self.description is not None:
+            result['description'] = self.description
+        if self.parent_code is not None:
+            result['parent_code'] = self.parent_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('parent_code') is not None:
+            self.parent_code = m.get('parent_code')
+        return self
+
+
+class UpdateDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class DeleteDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一码
+        self.code = code
+
+    def validate(self):
+        self.validate_required(self.code, 'code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.code is not None:
+            result['code'] = self.code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        return self
+
+
+class DeleteDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class PagequeryDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        code: str = None,
+        name: str = None,
+        description: str = None,
+        parent_code: str = None,
+        page_size: int = None,
+        page_num: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一码
+        self.code = code
+        # 部门名称
+        self.name = name
+        # 部门描述信息
+        self.description = description
+        # 父部门唯一码
+        self.parent_code = parent_code
+        # 分页大小
+        self.page_size = page_size
+        # 当前页
+        self.page_num = page_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.code is not None:
+            result['code'] = self.code
+        if self.name is not None:
+            result['name'] = self.name
+        if self.description is not None:
+            result['description'] = self.description
+        if self.parent_code is not None:
+            result['parent_code'] = self.parent_code
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.page_num is not None:
+            result['page_num'] = self.page_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('parent_code') is not None:
+            self.parent_code = m.get('parent_code')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('page_num') is not None:
+            self.page_num = m.get('page_num')
+        return self
+
+
+class PagequeryDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        departments: List[Department] = None,
+        page_num: int = None,
+        page_size: int = None,
+        total_count: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 部门列表
+        self.departments = departments
+        # 当前页码
+        self.page_num = page_num
+        # 分页大小
+        self.page_size = page_size
+        # 总数
+        self.total_count = total_count
+
+    def validate(self):
+        if self.departments:
+            for k in self.departments:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['departments'] = []
+        if self.departments is not None:
+            for k in self.departments:
+                result['departments'].append(k.to_map() if k else None)
+        if self.page_num is not None:
+            result['page_num'] = self.page_num
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total_count is not None:
+            result['total_count'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.departments = []
+        if m.get('departments') is not None:
+            for k in m.get('departments'):
+                temp_model = Department()
+                self.departments.append(temp_model.from_map(k))
+        if m.get('page_num') is not None:
+            self.page_num = m.get('page_num')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total_count') is not None:
+            self.total_count = m.get('total_count')
+        return self
+
+
+class BatchqueryDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        codes: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一码
+        self.codes = codes
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.codes is not None:
+            result['codes'] = self.codes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('codes') is not None:
+            self.codes = m.get('codes')
+        return self
+
+
+class BatchqueryDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        departments: List[Department] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 部门列表
+        self.departments = departments
+
+    def validate(self):
+        if self.departments:
+            for k in self.departments:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['departments'] = []
+        if self.departments is not None:
+            for k in self.departments:
+                result['departments'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.departments = []
+        if m.get('departments') is not None:
+            for k in m.get('departments'):
+                temp_model = Department()
+                self.departments.append(temp_model.from_map(k))
+        return self
+
+
+class SaveDepartmentUserRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        department_users: List[DepartmentUser] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 待添加或更新的部门成员关系列表
+        self.department_users = department_users
+
+    def validate(self):
+        self.validate_required(self.department_users, 'department_users')
+        if self.department_users:
+            for k in self.department_users:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        result['department_users'] = []
+        if self.department_users is not None:
+            for k in self.department_users:
+                result['department_users'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        self.department_users = []
+        if m.get('department_users') is not None:
+            for k in m.get('department_users'):
+                temp_model = DepartmentUser()
+                self.department_users.append(temp_model.from_map(k))
+        return self
+
+
+class SaveDepartmentUserResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class RemoveDepartmentUserRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        department_users: List[DepartmentUser] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 待删除的部门成员关系列表
+        self.department_users = department_users
+
+    def validate(self):
+        self.validate_required(self.department_users, 'department_users')
+        if self.department_users:
+            for k in self.department_users:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        result['department_users'] = []
+        if self.department_users is not None:
+            for k in self.department_users:
+                result['department_users'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        self.department_users = []
+        if m.get('department_users') is not None:
+            for k in m.get('department_users'):
+                temp_model = DepartmentUser()
+                self.department_users.append(temp_model.from_map(k))
+        return self
+
+
+class RemoveDepartmentUserResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class QueryDepartmentUserRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        department_code: str = None,
+        user_id: str = None,
+        type: str = None,
+        page_size: int = None,
+        page_num: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 部门唯一码
+        self.department_code = department_code
+        # 用户 id
+        self.user_id = user_id
+        # 部门成员类型
+        self.type = type
+        # 分页大小
+        self.page_size = page_size
+        # 当前页
+        self.page_num = page_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.department_code is not None:
+            result['department_code'] = self.department_code
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.type is not None:
+            result['type'] = self.type
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.page_num is not None:
+            result['page_num'] = self.page_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('department_code') is not None:
+            self.department_code = m.get('department_code')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('page_num') is not None:
+            self.page_num = m.get('page_num')
+        return self
+
+
+class QueryDepartmentUserResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        department_users: List[DepartmentUser] = None,
+        page_num: int = None,
+        page_size: int = None,
+        total_count: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 部门成员列表
+        self.department_users = department_users
+        # 当前页码
+        self.page_num = page_num
+        # 分页大小
+        self.page_size = page_size
+        # 总数
+        self.total_count = total_count
+
+    def validate(self):
+        if self.department_users:
+            for k in self.department_users:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['department_users'] = []
+        if self.department_users is not None:
+            for k in self.department_users:
+                result['department_users'].append(k.to_map() if k else None)
+        if self.page_num is not None:
+            result['page_num'] = self.page_num
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total_count is not None:
+            result['total_count'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.department_users = []
+        if m.get('department_users') is not None:
+            for k in m.get('department_users'):
+                temp_model = DepartmentUser()
+                self.department_users.append(temp_model.from_map(k))
+        if m.get('page_num') is not None:
+            self.page_num = m.get('page_num')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total_count') is not None:
+            self.total_count = m.get('total_count')
+        return self
+
+
+class GetLoginconfigRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        return self
+
+
+class GetLoginconfigResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        password_min_length: int = None,
+        password_max_length: int = None,
+        password_lowercase_letter: bool = None,
+        password_uppercase_letter: bool = None,
+        password_letter: bool = None,
+        password_digit: bool = None,
+        password_special_char: bool = None,
+        password_valid_check: bool = None,
+        password_valid_period: int = None,
+        password_expired_login: bool = None,
+        password_history_check: bool = None,
+        password_history_num: int = None,
+        verify_attempts_check: bool = None,
+        verify_attempts_window: int = None,
+        verify_attempts_threshold: int = None,
+        lockout_duration: int = None,
+        active_check: bool = None,
+        active_period: int = None,
+        password_self_manage: bool = None,
+        mfa_self_manage: bool = None,
+        status: str = None,
+        concurrent_ip_count: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 密码最小长度
+        self.password_min_length = password_min_length
+        # 密码最大长度
+        self.password_max_length = password_max_length
+        # 密码是否必须包含小写字母
+        self.password_lowercase_letter = password_lowercase_letter
+        # 密码是否必须包含大写字母
+        self.password_uppercase_letter = password_uppercase_letter
+        # 密码是否必须包含字母
+        self.password_letter = password_letter
+        # 密码是否必须包含数字
+        self.password_digit = password_digit
+        # 密码是否必须包含特殊字符
+        self.password_special_char = password_special_char
+        # 是否检查密码有效
+        self.password_valid_check = password_valid_check
+        # 密码有效期
+        self.password_valid_period = password_valid_period
+        # 密码过期后是否允许登录
+        self.password_expired_login = password_expired_login
+        # 是否检查密码历史
+        self.password_history_check = password_history_check
+        # 密码历史个数
+        self.password_history_num = password_history_num
+        # 重试校验是否触发锁定
+        self.verify_attempts_check = verify_attempts_check
+        # 重试校验窗口
+        self.verify_attempts_window = verify_attempts_window
+        # 重试校验触发锁定阈值
+        self.verify_attempts_threshold = verify_attempts_threshold
+        # 锁定时间
+        self.lockout_duration = lockout_duration
+        # 是否检查账户活跃
+        self.active_check = active_check
+        # 活跃周期，非活跃时锁定登录
+        self.active_period = active_period
+        # 是否允许自主管理密码
+        self.password_self_manage = password_self_manage
+        # 是否允许自主管理MFA
+        self.mfa_self_manage = mfa_self_manage
+        # 状态, 取值范围：NORMAL(正常状态), LOCK(锁定), ONE_PARTY_MIGRATING(一方化迁移中), ONE_PARTY_MIGRATION_LOCK(一方化迁移完成，禁用蚂蚁登录)
+        self.status = status
+        # 并发登录的ip数量，小于1表示不限制
+        self.concurrent_ip_count = concurrent_ip_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.password_min_length is not None:
+            result['password_min_length'] = self.password_min_length
+        if self.password_max_length is not None:
+            result['password_max_length'] = self.password_max_length
+        if self.password_lowercase_letter is not None:
+            result['password_lowercase_letter'] = self.password_lowercase_letter
+        if self.password_uppercase_letter is not None:
+            result['password_uppercase_letter'] = self.password_uppercase_letter
+        if self.password_letter is not None:
+            result['password_letter'] = self.password_letter
+        if self.password_digit is not None:
+            result['password_digit'] = self.password_digit
+        if self.password_special_char is not None:
+            result['password_special_char'] = self.password_special_char
+        if self.password_valid_check is not None:
+            result['password_valid_check'] = self.password_valid_check
+        if self.password_valid_period is not None:
+            result['password_valid_period'] = self.password_valid_period
+        if self.password_expired_login is not None:
+            result['password_expired_login'] = self.password_expired_login
+        if self.password_history_check is not None:
+            result['password_history_check'] = self.password_history_check
+        if self.password_history_num is not None:
+            result['password_history_num'] = self.password_history_num
+        if self.verify_attempts_check is not None:
+            result['verify_attempts_check'] = self.verify_attempts_check
+        if self.verify_attempts_window is not None:
+            result['verify_attempts_window'] = self.verify_attempts_window
+        if self.verify_attempts_threshold is not None:
+            result['verify_attempts_threshold'] = self.verify_attempts_threshold
+        if self.lockout_duration is not None:
+            result['lockout_duration'] = self.lockout_duration
+        if self.active_check is not None:
+            result['active_check'] = self.active_check
+        if self.active_period is not None:
+            result['active_period'] = self.active_period
+        if self.password_self_manage is not None:
+            result['password_self_manage'] = self.password_self_manage
+        if self.mfa_self_manage is not None:
+            result['mfa_self_manage'] = self.mfa_self_manage
+        if self.status is not None:
+            result['status'] = self.status
+        if self.concurrent_ip_count is not None:
+            result['concurrent_ip_count'] = self.concurrent_ip_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('password_min_length') is not None:
+            self.password_min_length = m.get('password_min_length')
+        if m.get('password_max_length') is not None:
+            self.password_max_length = m.get('password_max_length')
+        if m.get('password_lowercase_letter') is not None:
+            self.password_lowercase_letter = m.get('password_lowercase_letter')
+        if m.get('password_uppercase_letter') is not None:
+            self.password_uppercase_letter = m.get('password_uppercase_letter')
+        if m.get('password_letter') is not None:
+            self.password_letter = m.get('password_letter')
+        if m.get('password_digit') is not None:
+            self.password_digit = m.get('password_digit')
+        if m.get('password_special_char') is not None:
+            self.password_special_char = m.get('password_special_char')
+        if m.get('password_valid_check') is not None:
+            self.password_valid_check = m.get('password_valid_check')
+        if m.get('password_valid_period') is not None:
+            self.password_valid_period = m.get('password_valid_period')
+        if m.get('password_expired_login') is not None:
+            self.password_expired_login = m.get('password_expired_login')
+        if m.get('password_history_check') is not None:
+            self.password_history_check = m.get('password_history_check')
+        if m.get('password_history_num') is not None:
+            self.password_history_num = m.get('password_history_num')
+        if m.get('verify_attempts_check') is not None:
+            self.verify_attempts_check = m.get('verify_attempts_check')
+        if m.get('verify_attempts_window') is not None:
+            self.verify_attempts_window = m.get('verify_attempts_window')
+        if m.get('verify_attempts_threshold') is not None:
+            self.verify_attempts_threshold = m.get('verify_attempts_threshold')
+        if m.get('lockout_duration') is not None:
+            self.lockout_duration = m.get('lockout_duration')
+        if m.get('active_check') is not None:
+            self.active_check = m.get('active_check')
+        if m.get('active_period') is not None:
+            self.active_period = m.get('active_period')
+        if m.get('password_self_manage') is not None:
+            self.password_self_manage = m.get('password_self_manage')
+        if m.get('mfa_self_manage') is not None:
+            self.mfa_self_manage = m.get('mfa_self_manage')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('concurrent_ip_count') is not None:
+            self.concurrent_ip_count = m.get('concurrent_ip_count')
+        return self
+
+
+class UpdateLoginconfigRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        password_min_length: int = None,
+        password_max_length: int = None,
+        password_lowercase_letter: bool = None,
+        password_uppercase_letter: bool = None,
+        password_letter: bool = None,
+        password_digit: bool = None,
+        password_special_char: bool = None,
+        password_valid_check: bool = None,
+        password_valid_period: int = None,
+        password_expired_login: bool = None,
+        password_history_check: bool = None,
+        password_history_num: int = None,
+        verify_attempts_check: bool = None,
+        verify_attempts_window: int = None,
+        verify_attempts_threshold: int = None,
+        lockout_duration: int = None,
+        active_check: bool = None,
+        active_period: int = None,
+        password_self_manage: bool = None,
+        mfa_self_manage: bool = None,
+        concurrent_ip_count: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 密码最小长度
+        self.password_min_length = password_min_length
+        # 密码最大长度
+        self.password_max_length = password_max_length
+        # 密码是否必须包含小写字母
+        self.password_lowercase_letter = password_lowercase_letter
+        # 密码是否必须包含大写字母
+        self.password_uppercase_letter = password_uppercase_letter
+        # 密码是否必须包含字母
+        self.password_letter = password_letter
+        # 密码是否必须包含数字
+        self.password_digit = password_digit
+        # 密码是否必须包含特殊字符
+        self.password_special_char = password_special_char
+        # 是否检查密码有效
+        self.password_valid_check = password_valid_check
+        # 密码有效期
+        self.password_valid_period = password_valid_period
+        # 密码过期后是否允许登录
+        self.password_expired_login = password_expired_login
+        # 是否检查密码历史
+        self.password_history_check = password_history_check
+        # 密码历史个数
+        self.password_history_num = password_history_num
+        # 重试校验是否触发锁定
+        self.verify_attempts_check = verify_attempts_check
+        # 重试校验窗口
+        self.verify_attempts_window = verify_attempts_window
+        # 重试校验触发锁定阈值
+        self.verify_attempts_threshold = verify_attempts_threshold
+        # 锁定时间
+        self.lockout_duration = lockout_duration
+        # 是否检查账户活跃
+        self.active_check = active_check
+        # 活跃周期，非活跃时锁定登录
+        self.active_period = active_period
+        # 是否允许自主管理密码
+        self.password_self_manage = password_self_manage
+        # 是否允许自主管理MFA
+        self.mfa_self_manage = mfa_self_manage
+        # 并发登录的ip数量，小于1表示不限制
+        self.concurrent_ip_count = concurrent_ip_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.password_min_length is not None:
+            result['password_min_length'] = self.password_min_length
+        if self.password_max_length is not None:
+            result['password_max_length'] = self.password_max_length
+        if self.password_lowercase_letter is not None:
+            result['password_lowercase_letter'] = self.password_lowercase_letter
+        if self.password_uppercase_letter is not None:
+            result['password_uppercase_letter'] = self.password_uppercase_letter
+        if self.password_letter is not None:
+            result['password_letter'] = self.password_letter
+        if self.password_digit is not None:
+            result['password_digit'] = self.password_digit
+        if self.password_special_char is not None:
+            result['password_special_char'] = self.password_special_char
+        if self.password_valid_check is not None:
+            result['password_valid_check'] = self.password_valid_check
+        if self.password_valid_period is not None:
+            result['password_valid_period'] = self.password_valid_period
+        if self.password_expired_login is not None:
+            result['password_expired_login'] = self.password_expired_login
+        if self.password_history_check is not None:
+            result['password_history_check'] = self.password_history_check
+        if self.password_history_num is not None:
+            result['password_history_num'] = self.password_history_num
+        if self.verify_attempts_check is not None:
+            result['verify_attempts_check'] = self.verify_attempts_check
+        if self.verify_attempts_window is not None:
+            result['verify_attempts_window'] = self.verify_attempts_window
+        if self.verify_attempts_threshold is not None:
+            result['verify_attempts_threshold'] = self.verify_attempts_threshold
+        if self.lockout_duration is not None:
+            result['lockout_duration'] = self.lockout_duration
+        if self.active_check is not None:
+            result['active_check'] = self.active_check
+        if self.active_period is not None:
+            result['active_period'] = self.active_period
+        if self.password_self_manage is not None:
+            result['password_self_manage'] = self.password_self_manage
+        if self.mfa_self_manage is not None:
+            result['mfa_self_manage'] = self.mfa_self_manage
+        if self.concurrent_ip_count is not None:
+            result['concurrent_ip_count'] = self.concurrent_ip_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('password_min_length') is not None:
+            self.password_min_length = m.get('password_min_length')
+        if m.get('password_max_length') is not None:
+            self.password_max_length = m.get('password_max_length')
+        if m.get('password_lowercase_letter') is not None:
+            self.password_lowercase_letter = m.get('password_lowercase_letter')
+        if m.get('password_uppercase_letter') is not None:
+            self.password_uppercase_letter = m.get('password_uppercase_letter')
+        if m.get('password_letter') is not None:
+            self.password_letter = m.get('password_letter')
+        if m.get('password_digit') is not None:
+            self.password_digit = m.get('password_digit')
+        if m.get('password_special_char') is not None:
+            self.password_special_char = m.get('password_special_char')
+        if m.get('password_valid_check') is not None:
+            self.password_valid_check = m.get('password_valid_check')
+        if m.get('password_valid_period') is not None:
+            self.password_valid_period = m.get('password_valid_period')
+        if m.get('password_expired_login') is not None:
+            self.password_expired_login = m.get('password_expired_login')
+        if m.get('password_history_check') is not None:
+            self.password_history_check = m.get('password_history_check')
+        if m.get('password_history_num') is not None:
+            self.password_history_num = m.get('password_history_num')
+        if m.get('verify_attempts_check') is not None:
+            self.verify_attempts_check = m.get('verify_attempts_check')
+        if m.get('verify_attempts_window') is not None:
+            self.verify_attempts_window = m.get('verify_attempts_window')
+        if m.get('verify_attempts_threshold') is not None:
+            self.verify_attempts_threshold = m.get('verify_attempts_threshold')
+        if m.get('lockout_duration') is not None:
+            self.lockout_duration = m.get('lockout_duration')
+        if m.get('active_check') is not None:
+            self.active_check = m.get('active_check')
+        if m.get('active_period') is not None:
+            self.active_period = m.get('active_period')
+        if m.get('password_self_manage') is not None:
+            self.password_self_manage = m.get('password_self_manage')
+        if m.get('mfa_self_manage') is not None:
+            self.mfa_self_manage = m.get('mfa_self_manage')
+        if m.get('concurrent_ip_count') is not None:
+            self.concurrent_ip_count = m.get('concurrent_ip_count')
+        return self
+
+
+class UpdateLoginconfigResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class GetMfaStatusRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户id
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
+class GetMfaStatusResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        status: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # MFA状态, 取值范围：ENABLED, DISABLED
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class EnableMfaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+        verification_code: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户 id
+        self.user_id = user_id
+        # 验证码
+        self.verification_code = verification_code
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.verification_code, 'verification_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.verification_code is not None:
+            result['verification_code'] = self.verification_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('verification_code') is not None:
+            self.verification_code = m.get('verification_code')
+        return self
+
+
+class EnableMfaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class DisableMfaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+        verification_code: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户 id
+        self.user_id = user_id
+        # 验证码
+        self.verification_code = verification_code
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.verification_code is not None:
+            result['verification_code'] = self.verification_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('verification_code') is not None:
+            self.verification_code = m.get('verification_code')
+        return self
+
+
+class DisableMfaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class InitMfaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户 id
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
+class InitMfaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        secret_key: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 密钥
+        self.secret_key = secret_key
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.secret_key is not None:
+            result['secret_key'] = self.secret_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('secret_key') is not None:
+            self.secret_key = m.get('secret_key')
+        return self
+
+
+class VerifyMfaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+        verification_code: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户 id
+        self.user_id = user_id
+        # 验证码
+        self.verification_code = verification_code
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.verification_code, 'verification_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.verification_code is not None:
+            result['verification_code'] = self.verification_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('verification_code') is not None:
+            self.verification_code = m.get('verification_code')
+        return self
+
+
+class VerifyMfaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        result: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 校验结果
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class GetMfaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户 id
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
+class GetMfaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        user_id: str = None,
+        status: str = None,
+        secret_key: str = None,
+        last_generated_time: str = None,
+        verify_attempts: int = None,
+        first_failure_time: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 用户 id
+        self.user_id = user_id
+        # MFA状态, 取值范围：ENABLED, DISABLED
+        self.status = status
+        # 密钥
+        self.secret_key = secret_key
+        # 最后一次密钥生成时间
+        self.last_generated_time = last_generated_time
+        # (校验失败时)重试校验的次数
+        self.verify_attempts = verify_attempts
+        # 第一次校验失败时间
+        self.first_failure_time = first_failure_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.status is not None:
+            result['status'] = self.status
+        if self.secret_key is not None:
+            result['secret_key'] = self.secret_key
+        if self.last_generated_time is not None:
+            result['last_generated_time'] = self.last_generated_time
+        if self.verify_attempts is not None:
+            result['verify_attempts'] = self.verify_attempts
+        if self.first_failure_time is not None:
+            result['first_failure_time'] = self.first_failure_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('secret_key') is not None:
+            self.secret_key = m.get('secret_key')
+        if m.get('last_generated_time') is not None:
+            self.last_generated_time = m.get('last_generated_time')
+        if m.get('verify_attempts') is not None:
+            self.verify_attempts = m.get('verify_attempts')
+        if m.get('first_failure_time') is not None:
+            self.first_failure_time = m.get('first_failure_time')
+        return self
+
+
+class UpdateOperatorPasswordRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        login_name: str = None,
+        new_encrypted_password: str = None,
+        old_encrypted_password: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 登录名
+        self.login_name = login_name
+        # 加密过的新密码值，使用AccessSecret进行3DES加密
+        self.new_encrypted_password = new_encrypted_password
+        # 加密过的旧密码值，使用AccessSecret进行DES加密
+        self.old_encrypted_password = old_encrypted_password
+
+    def validate(self):
+        self.validate_required(self.login_name, 'login_name')
+        self.validate_required(self.new_encrypted_password, 'new_encrypted_password')
+        self.validate_required(self.old_encrypted_password, 'old_encrypted_password')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.login_name is not None:
+            result['login_name'] = self.login_name
+        if self.new_encrypted_password is not None:
+            result['new_encrypted_password'] = self.new_encrypted_password
+        if self.old_encrypted_password is not None:
+            result['old_encrypted_password'] = self.old_encrypted_password
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('login_name') is not None:
+            self.login_name = m.get('login_name')
+        if m.get('new_encrypted_password') is not None:
+            self.new_encrypted_password = m.get('new_encrypted_password')
+        if m.get('old_encrypted_password') is not None:
+            self.old_encrypted_password = m.get('old_encrypted_password')
+        return self
+
+
+class UpdateOperatorPasswordResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class ResetOperatorPasswordRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        login_name: str = None,
+        new_encrypted_password: str = None,
+        status: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 登录名
+        self.login_name = login_name
+        # 加密过的新密码值，使用AccessSecret进行3DES加密
+        self.new_encrypted_password = new_encrypted_password
+        # 登录凭证状态，取值范围：NORMAL, EXPIRED
+        # 
+        # 默认为 NORMAL，设为 EXPIRED 用户登录时会要求重置密码
+        self.status = status
+
+    def validate(self):
+        self.validate_required(self.login_name, 'login_name')
+        self.validate_required(self.new_encrypted_password, 'new_encrypted_password')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.login_name is not None:
+            result['login_name'] = self.login_name
+        if self.new_encrypted_password is not None:
+            result['new_encrypted_password'] = self.new_encrypted_password
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('login_name') is not None:
+            self.login_name = m.get('login_name')
+        if m.get('new_encrypted_password') is not None:
+            self.new_encrypted_password = m.get('new_encrypted_password')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class ResetOperatorPasswordResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class BatchqueryOperatorRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        operator_ids: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户id列表
+        self.operator_ids = operator_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.operator_ids is not None:
+            result['operator_ids'] = self.operator_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('operator_ids') is not None:
+            self.operator_ids = m.get('operator_ids')
+        return self
+
+
+class BatchqueryOperatorResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        operators: List[Operator] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 操作员列表
+        self.operators = operators
+
+    def validate(self):
+        if self.operators:
+            for k in self.operators:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['operators'] = []
+        if self.operators is not None:
+            for k in self.operators:
+                result['operators'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.operators = []
+        if m.get('operators') is not None:
+            for k in m.get('operators'):
+                temp_model = Operator()
+                self.operators.append(temp_model.from_map(k))
+        return self
+
+
+class PushOperationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        operation_code: str = None,
+        params: str = None,
+        region: str = None,
+        resource_id: str = None,
+        resource_type: str = None,
+        response: str = None,
+        source: str = None,
+        source_ip_address: str = None,
+        time: str = None,
+        trace_id: str = None,
+        user_agent: str = None,
+        user_id: str = None,
+        user_tenant: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # {产品}.{资源}.{子资源}.{操作}
+        self.operation_code = operation_code
+        # 操作参数
+        self.params = params
+        # 可用区域信息，非必填
+        self.region = region
+        # 资源ID
+        self.resource_id = resource_id
+        # 资源类型
+        self.resource_type = resource_type
+        # 相应结果
+        self.response = response
+        # 操作来源，由接入方上报自身系统host
+        self.source = source
+        # 操作来源IP，由接入方上报
+        self.source_ip_address = source_ip_address
+        # 触发时间
+        self.time = time
+        # TraceId用于事件追踪
+        self.trace_id = trace_id
+        # agent信息
+        self.user_agent = user_agent
+        # 用户ID
+        self.user_id = user_id
+        # 租户8位ID
+        self.user_tenant = user_tenant
+
+    def validate(self):
+        self.validate_required(self.operation_code, 'operation_code')
+        self.validate_required(self.params, 'params')
+        self.validate_required(self.time, 'time')
+        if self.time is not None:
+            self.validate_pattern(self.time, 'time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.user_tenant, 'user_tenant')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.operation_code is not None:
+            result['operation_code'] = self.operation_code
+        if self.params is not None:
+            result['params'] = self.params
+        if self.region is not None:
+            result['region'] = self.region
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.resource_type is not None:
+            result['resource_type'] = self.resource_type
+        if self.response is not None:
+            result['response'] = self.response
+        if self.source is not None:
+            result['source'] = self.source
+        if self.source_ip_address is not None:
+            result['source_ip_address'] = self.source_ip_address
+        if self.time is not None:
+            result['time'] = self.time
+        if self.trace_id is not None:
+            result['trace_id'] = self.trace_id
+        if self.user_agent is not None:
+            result['user_agent'] = self.user_agent
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.user_tenant is not None:
+            result['user_tenant'] = self.user_tenant
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('operation_code') is not None:
+            self.operation_code = m.get('operation_code')
+        if m.get('params') is not None:
+            self.params = m.get('params')
+        if m.get('region') is not None:
+            self.region = m.get('region')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('resource_type') is not None:
+            self.resource_type = m.get('resource_type')
+        if m.get('response') is not None:
+            self.response = m.get('response')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        if m.get('source_ip_address') is not None:
+            self.source_ip_address = m.get('source_ip_address')
+        if m.get('time') is not None:
+            self.time = m.get('time')
+        if m.get('trace_id') is not None:
+            self.trace_id = m.get('trace_id')
+        if m.get('user_agent') is not None:
+            self.user_agent = m.get('user_agent')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('user_tenant') is not None:
+            self.user_tenant = m.get('user_tenant')
+        return self
+
+
+class PushOperationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        unique_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 事件唯一ID
+        self.unique_id = unique_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.unique_id is not None:
+            result['unique_id'] = self.unique_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('unique_id') is not None:
+            self.unique_id = m.get('unique_id')
+        return self
+
+
+class QueryOperationtypeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product: str = None,
+        source: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 产品码
+        self.product = product
+        # 来源信息
+        self.source = source
+
+    def validate(self):
+        self.validate_required(self.product, 'product')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product is not None:
+            result['product'] = self.product
+        if self.source is not None:
+            result['source'] = self.source
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product') is not None:
+            self.product = m.get('product')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        return self
+
+
+class QueryOperationtypeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        operation_types: List[OperationType] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 操作类型列表
+        self.operation_types = operation_types
+
+    def validate(self):
+        if self.operation_types:
+            for k in self.operation_types:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['operation_types'] = []
+        if self.operation_types is not None:
+            for k in self.operation_types:
+                result['operation_types'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.operation_types = []
+        if m.get('operation_types') is not None:
+            for k in m.get('operation_types'):
+                temp_model = OperationType()
+                self.operation_types.append(temp_model.from_map(k))
+        return self
+
+
+class GetOperationtypeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 操作类型名称
+        self.name = name
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.name is not None:
+            result['name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        return self
+
+
+class GetOperationtypeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: OperationType = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 操作类型
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('data') is not None:
+            temp_model = OperationType()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class AddTenantMemberRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        operator_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 操作员唯一id
+        self.operator_id = operator_id
+
+    def validate(self):
+        self.validate_required(self.operator_id, 'operator_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.operator_id is not None:
+            result['operator_id'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('operator_id') is not None:
+            self.operator_id = m.get('operator_id')
+        return self
+
+
+class AddTenantMemberResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        access_key: str = None,
+        access_secret: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # Accessor关联的AccessKey
+        self.access_key = access_key
+        # Accessor关联的AccessKey的密钥
+        self.access_secret = access_secret
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.access_key is not None:
+            result['access_key'] = self.access_key
+        if self.access_secret is not None:
+            result['access_secret'] = self.access_secret
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('access_key') is not None:
+            self.access_key = m.get('access_key')
+        if m.get('access_secret') is not None:
+            self.access_secret = m.get('access_secret')
+        return self
+
+
+class GetOperatorLogintokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        return self
+
+
+class GetOperatorLogintokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        login_token: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 一次性登录认证 token
+        self.login_token = login_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.login_token is not None:
+            result['login_token'] = self.login_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('login_token') is not None:
+            self.login_token = m.get('login_token')
         return self
```

### Comparing `antchain_iam-3.12.4/setup.py` & `antchain_iam-3.12.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_iam.
 
-Created on 08/03/2021
+Created on 02/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_iam"
 NAME = "antchain_iam" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain IAM SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "antchain_alipay_util>=0.0.6, <1.0.0",
-    "alibabacloud_tea_util>=0.3.3, <1.0.0",
-    "alibabacloud_rpc_util>=0.0.3, <1.0.0"
+    "antchain_alipay_util>=1.0.1, <2.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

