# Comparing `tmp/alibabacloud_aligeniessp_1_0-1.0.9.tar.gz` & `tmp/alibabacloud_aligeniessp_1_0-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligeniessp_1_0-1.0.9.tar", last modified: Mon Aug 22 08:53:16 2022, max compression
+gzip compressed data, was "dist/alibabacloud_aligeniessp_1_0-2.0.0.tar", last modified: Fri Jun  2 03:06:26 2023, max compression
```

## Comparing `alibabacloud_aligeniessp_1_0-1.0.9.tar` & `alibabacloud_aligeniessp_1_0-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      389 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2353 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1035 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1120 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   314162 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   742718 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2353 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2634 2022-08-22 08:53:16.000000 alibabacloud_aligeniessp_1_0-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   364870 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   842921 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/setup.py
```

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/LICENSE` & `alibabacloud_aligeniessp_1_0-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/PKG-INFO` & `alibabacloud_aligeniessp_1_0-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligeniessp_1_0
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud AliGenie (ssp_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/README-CN.md` & `alibabacloud_aligeniessp_1_0-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/README.md` & `alibabacloud_aligeniessp_1_0-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0/client.py` & `alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,45 +37,29 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def add_and_remove_favorite_content(
-        self,
-        request: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentRequest,
-    ) -> ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.AddAndRemoveFavoriteContentHeaders()
-        return self.add_and_remove_favorite_content_with_options(request, headers, runtime)
-
-    async def add_and_remove_favorite_content_async(
-        self,
-        request: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentRequest,
-    ) -> ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.AddAndRemoveFavoriteContentHeaders()
-        return await self.add_and_remove_favorite_content_with_options_async(request, headers, runtime)
-
     def add_and_remove_favorite_content_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentRequest,
         headers: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.AddAndRemoveFavoriteContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_add_and_remove_favorite_content_request):
-            request.open_add_and_remove_favorite_content_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_add_and_remove_favorite_content_request), 'OpenAddAndRemoveFavoriteContentRequest', 'json')
+            request.open_add_and_remove_favorite_content_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_add_and_remove_favorite_content_request, 'OpenAddAndRemoveFavoriteContentRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_add_and_remove_favorite_content_request_shrink):
@@ -114,19 +98,19 @@
         headers: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.AddAndRemoveFavoriteContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_add_and_remove_favorite_content_request):
-            request.open_add_and_remove_favorite_content_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_add_and_remove_favorite_content_request), 'OpenAddAndRemoveFavoriteContentRequest', 'json')
+            request.open_add_and_remove_favorite_content_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_add_and_remove_favorite_content_request, 'OpenAddAndRemoveFavoriteContentRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_add_and_remove_favorite_content_request_shrink):
@@ -155,45 +139,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def add_sub(
+    def add_and_remove_favorite_content(
         self,
-        request: ali_geniessp__1__0_models.AddSubRequest,
-    ) -> ali_geniessp__1__0_models.AddSubResponse:
+        request: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentRequest,
+    ) -> ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.AddSubHeaders()
-        return self.add_sub_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.AddAndRemoveFavoriteContentHeaders()
+        return self.add_and_remove_favorite_content_with_options(request, headers, runtime)
 
-    async def add_sub_async(
+    async def add_and_remove_favorite_content_async(
         self,
-        request: ali_geniessp__1__0_models.AddSubRequest,
-    ) -> ali_geniessp__1__0_models.AddSubResponse:
+        request: ali_geniessp__1__0_models.AddAndRemoveFavoriteContentRequest,
+    ) -> ali_geniessp__1__0_models.AddAndRemoveFavoriteContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.AddSubHeaders()
-        return await self.add_sub_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.AddAndRemoveFavoriteContentHeaders()
+        return await self.add_and_remove_favorite_content_with_options_async(request, headers, runtime)
 
     def add_sub_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.AddSubRequest,
         headers: ali_geniessp__1__0_models.AddSubHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.AddSubResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.AddSubShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.add_subscription_info_request):
-            request.add_subscription_info_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.add_subscription_info_request), 'AddSubscriptionInfoRequest', 'json')
+            request.add_subscription_info_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.add_subscription_info_request, 'AddSubscriptionInfoRequest', 'json')
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.add_subscription_info_request_shrink):
             query['AddSubscriptionInfoRequest'] = request.add_subscription_info_request_shrink
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -230,19 +214,19 @@
         headers: ali_geniessp__1__0_models.AddSubHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.AddSubResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.AddSubShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.add_subscription_info_request):
-            request.add_subscription_info_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.add_subscription_info_request), 'AddSubscriptionInfoRequest', 'json')
+            request.add_subscription_info_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.add_subscription_info_request, 'AddSubscriptionInfoRequest', 'json')
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.add_subscription_info_request_shrink):
             query['AddSubscriptionInfoRequest'] = request.add_subscription_info_request_shrink
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -269,41 +253,547 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.AddSubResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def check_auth_code_bind_for_ext(
+    def add_sub(
         self,
-        request: ali_geniessp__1__0_models.CheckAuthCodeBindForExtRequest,
-    ) -> ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse:
+        request: ali_geniessp__1__0_models.AddSubRequest,
+    ) -> ali_geniessp__1__0_models.AddSubResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CheckAuthCodeBindForExtHeaders()
-        return self.check_auth_code_bind_for_ext_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.AddSubHeaders()
+        return self.add_sub_with_options(request, headers, runtime)
 
-    async def check_auth_code_bind_for_ext_async(
+    async def add_sub_async(
         self,
-        request: ali_geniessp__1__0_models.CheckAuthCodeBindForExtRequest,
-    ) -> ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse:
+        request: ali_geniessp__1__0_models.AddSubRequest,
+    ) -> ali_geniessp__1__0_models.AddSubResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CheckAuthCodeBindForExtHeaders()
-        return await self.check_auth_code_bind_for_ext_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.AddSubHeaders()
+        return await self.add_sub_with_options_async(request, headers, runtime)
+
+    def auth_login_with_aligenie_user_info_with_options(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.encrypted_aligenie_user_identifier):
+            body['EncryptedAligenieUserIdentifier'] = request.encrypted_aligenie_user_identifier
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithAligenieUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithAligenieUserInfo',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def auth_login_with_aligenie_user_info_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.encrypted_aligenie_user_identifier):
+            body['EncryptedAligenieUserIdentifier'] = request.encrypted_aligenie_user_identifier
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithAligenieUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithAligenieUserInfo',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def auth_login_with_aligenie_user_info(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoHeaders()
+        return self.auth_login_with_aligenie_user_info_with_options(request, headers, runtime)
+
+    async def auth_login_with_aligenie_user_info_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoHeaders()
+        return await self.auth_login_with_aligenie_user_info_with_options_async(request, headers, runtime)
+
+    def auth_login_with_aligenie_user_info_generated_by_phone_number_with_options(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithAligenieUserInfoGeneratedByPhoneNumber',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithAligenieUserInfoGeneratedByPhoneNumber',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def auth_login_with_aligenie_user_info_generated_by_phone_number_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithAligenieUserInfoGeneratedByPhoneNumber',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithAligenieUserInfoGeneratedByPhoneNumber',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def auth_login_with_aligenie_user_info_generated_by_phone_number(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberHeaders()
+        return self.auth_login_with_aligenie_user_info_generated_by_phone_number_with_options(request, headers, runtime)
+
+    async def auth_login_with_aligenie_user_info_generated_by_phone_number_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberHeaders()
+        return await self.auth_login_with_aligenie_user_info_generated_by_phone_number_with_options_async(request, headers, runtime)
+
+    def auth_login_with_taobao_user_info_with_options(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.encrypted_taobao_user_identifier):
+            body['EncryptedTaobaoUserIdentifier'] = request.encrypted_taobao_user_identifier
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithTaobaoUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithTaobaoUserInfo',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def auth_login_with_taobao_user_info_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.encrypted_taobao_user_identifier):
+            body['EncryptedTaobaoUserIdentifier'] = request.encrypted_taobao_user_identifier
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithTaobaoUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithTaobaoUserInfo',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def auth_login_with_taobao_user_info(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoHeaders()
+        return self.auth_login_with_taobao_user_info_with_options(request, headers, runtime)
+
+    async def auth_login_with_taobao_user_info_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithTaobaoUserInfoHeaders()
+        return await self.auth_login_with_taobao_user_info_with_options_async(request, headers, runtime)
+
+    def auth_login_with_third_user_info_with_options(
+        self,
+        tmp_req: ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.ext_info):
+            request.ext_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ext_info, 'ExtInfo', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.ext_info_shrink):
+            body['ExtInfo'] = request.ext_info_shrink
+        if not UtilClient.is_unset(request.scene_code):
+            body['SceneCode'] = request.scene_code
+        if not UtilClient.is_unset(request.third_user_identifier):
+            body['ThirdUserIdentifier'] = request.third_user_identifier
+        if not UtilClient.is_unset(request.third_user_type):
+            body['ThirdUserType'] = request.third_user_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithThirdUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithThirdUserInfo',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def auth_login_with_third_user_info_with_options_async(
+        self,
+        tmp_req: ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoRequest,
+        headers: ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.ext_info):
+            request.ext_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ext_info, 'ExtInfo', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.ext_info_shrink):
+            body['ExtInfo'] = request.ext_info_shrink
+        if not UtilClient.is_unset(request.scene_code):
+            body['SceneCode'] = request.scene_code
+        if not UtilClient.is_unset(request.third_user_identifier):
+            body['ThirdUserIdentifier'] = request.third_user_identifier
+        if not UtilClient.is_unset(request.third_user_type):
+            body['ThirdUserType'] = request.third_user_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AuthLoginWithThirdUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/authLoginWithThirdUserInfo',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def auth_login_with_third_user_info(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoHeaders()
+        return self.auth_login_with_third_user_info_with_options(request, headers, runtime)
+
+    async def auth_login_with_third_user_info_async(
+        self,
+        request: ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.AuthLoginWithThirdUserInfoHeaders()
+        return await self.auth_login_with_third_user_info_with_options_async(request, headers, runtime)
+
+    def check_and_do_voip_call_for_hotel_with_options(
+        self,
+        tmp_req: ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelRequest,
+        headers: ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.device_info):
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
+        if not UtilClient.is_unset(tmp_req.user_info):
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.biz_data):
+            body['BizData'] = request.biz_data
+        if not UtilClient.is_unset(request.callee_nick):
+            body['CalleeNick'] = request.callee_nick
+        if not UtilClient.is_unset(request.callee_phone_num):
+            body['CalleePhoneNum'] = request.callee_phone_num
+        if not UtilClient.is_unset(request.device_info_shrink):
+            body['DeviceInfo'] = request.device_info_shrink
+        if not UtilClient.is_unset(request.user_info_shrink):
+            body['UserInfo'] = request.user_info_shrink
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CheckAndDoVoipCallForHotel',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/checkAndDoVoipCallForHotel',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def check_and_do_voip_call_for_hotel_with_options_async(
+        self,
+        tmp_req: ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelRequest,
+        headers: ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.device_info):
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
+        if not UtilClient.is_unset(tmp_req.user_info):
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.biz_data):
+            body['BizData'] = request.biz_data
+        if not UtilClient.is_unset(request.callee_nick):
+            body['CalleeNick'] = request.callee_nick
+        if not UtilClient.is_unset(request.callee_phone_num):
+            body['CalleePhoneNum'] = request.callee_phone_num
+        if not UtilClient.is_unset(request.device_info_shrink):
+            body['DeviceInfo'] = request.device_info_shrink
+        if not UtilClient.is_unset(request.user_info_shrink):
+            body['UserInfo'] = request.user_info_shrink
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CheckAndDoVoipCallForHotel',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/checkAndDoVoipCallForHotel',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def check_and_do_voip_call_for_hotel(
+        self,
+        request: ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelRequest,
+    ) -> ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelHeaders()
+        return self.check_and_do_voip_call_for_hotel_with_options(request, headers, runtime)
+
+    async def check_and_do_voip_call_for_hotel_async(
+        self,
+        request: ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelRequest,
+    ) -> ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.CheckAndDoVoipCallForHotelHeaders()
+        return await self.check_and_do_voip_call_for_hotel_with_options_async(request, headers, runtime)
 
     def check_auth_code_bind_for_ext_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.CheckAuthCodeBindForExtRequest,
         headers: ali_geniessp__1__0_models.CheckAuthCodeBindForExtHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CheckAuthCodeBindForExtShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.auth_code):
             query['AuthCode'] = request.auth_code
         if not UtilClient.is_unset(request.encode_key):
             query['EncodeKey'] = request.encode_key
         if not UtilClient.is_unset(request.encode_type):
             query['EncodeType'] = request.encode_type
@@ -342,15 +832,15 @@
         headers: ali_geniessp__1__0_models.CheckAuthCodeBindForExtHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CheckAuthCodeBindForExtShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.auth_code):
             query['AuthCode'] = request.auth_code
         if not UtilClient.is_unset(request.encode_key):
             query['EncodeKey'] = request.encode_key
         if not UtilClient.is_unset(request.encode_type):
             query['EncodeType'] = request.encode_type
@@ -379,45 +869,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_alarm(
+    def check_auth_code_bind_for_ext(
         self,
-        request: ali_geniessp__1__0_models.CreateAlarmRequest,
-    ) -> ali_geniessp__1__0_models.CreateAlarmResponse:
+        request: ali_geniessp__1__0_models.CheckAuthCodeBindForExtRequest,
+    ) -> ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CreateAlarmHeaders()
-        return self.create_alarm_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CheckAuthCodeBindForExtHeaders()
+        return self.check_auth_code_bind_for_ext_with_options(request, headers, runtime)
 
-    async def create_alarm_async(
+    async def check_auth_code_bind_for_ext_async(
         self,
-        request: ali_geniessp__1__0_models.CreateAlarmRequest,
-    ) -> ali_geniessp__1__0_models.CreateAlarmResponse:
+        request: ali_geniessp__1__0_models.CheckAuthCodeBindForExtRequest,
+    ) -> ali_geniessp__1__0_models.CheckAuthCodeBindForExtResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CreateAlarmHeaders()
-        return await self.create_alarm_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CheckAuthCodeBindForExtHeaders()
+        return await self.check_auth_code_bind_for_ext_with_options_async(request, headers, runtime)
 
     def create_alarm_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.CreateAlarmRequest,
         headers: ali_geniessp__1__0_models.CreateAlarmHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CreateAlarmResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CreateAlarmShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -454,19 +944,19 @@
         headers: ali_geniessp__1__0_models.CreateAlarmHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CreateAlarmResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CreateAlarmShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -493,45 +983,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.CreateAlarmResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_playing_list(
+    def create_alarm(
         self,
-        request: ali_geniessp__1__0_models.CreatePlayingListRequest,
-    ) -> ali_geniessp__1__0_models.CreatePlayingListResponse:
+        request: ali_geniessp__1__0_models.CreateAlarmRequest,
+    ) -> ali_geniessp__1__0_models.CreateAlarmResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CreatePlayingListHeaders()
-        return self.create_playing_list_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CreateAlarmHeaders()
+        return self.create_alarm_with_options(request, headers, runtime)
 
-    async def create_playing_list_async(
+    async def create_alarm_async(
         self,
-        request: ali_geniessp__1__0_models.CreatePlayingListRequest,
-    ) -> ali_geniessp__1__0_models.CreatePlayingListResponse:
+        request: ali_geniessp__1__0_models.CreateAlarmRequest,
+    ) -> ali_geniessp__1__0_models.CreateAlarmResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CreatePlayingListHeaders()
-        return await self.create_playing_list_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CreateAlarmHeaders()
+        return await self.create_alarm_with_options_async(request, headers, runtime)
 
     def create_playing_list_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.CreatePlayingListRequest,
         headers: ali_geniessp__1__0_models.CreatePlayingListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CreatePlayingListResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CreatePlayingListShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_create_playing_list_request):
-            request.open_create_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_create_playing_list_request), 'OpenCreatePlayingListRequest', 'json')
+            request.open_create_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_create_playing_list_request, 'OpenCreatePlayingListRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_create_playing_list_request_shrink):
@@ -570,19 +1060,19 @@
         headers: ali_geniessp__1__0_models.CreatePlayingListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CreatePlayingListResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CreatePlayingListShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_create_playing_list_request):
-            request.open_create_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_create_playing_list_request), 'OpenCreatePlayingListRequest', 'json')
+            request.open_create_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_create_playing_list_request, 'OpenCreatePlayingListRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_create_playing_list_request_shrink):
@@ -611,45 +1101,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.CreatePlayingListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_schedule_task(
+    def create_playing_list(
         self,
-        request: ali_geniessp__1__0_models.CreateScheduleTaskRequest,
-    ) -> ali_geniessp__1__0_models.CreateScheduleTaskResponse:
+        request: ali_geniessp__1__0_models.CreatePlayingListRequest,
+    ) -> ali_geniessp__1__0_models.CreatePlayingListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CreateScheduleTaskHeaders()
-        return self.create_schedule_task_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CreatePlayingListHeaders()
+        return self.create_playing_list_with_options(request, headers, runtime)
 
-    async def create_schedule_task_async(
+    async def create_playing_list_async(
         self,
-        request: ali_geniessp__1__0_models.CreateScheduleTaskRequest,
-    ) -> ali_geniessp__1__0_models.CreateScheduleTaskResponse:
+        request: ali_geniessp__1__0_models.CreatePlayingListRequest,
+    ) -> ali_geniessp__1__0_models.CreatePlayingListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.CreateScheduleTaskHeaders()
-        return await self.create_schedule_task_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CreatePlayingListHeaders()
+        return await self.create_playing_list_with_options_async(request, headers, runtime)
 
     def create_schedule_task_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.CreateScheduleTaskRequest,
         headers: ali_geniessp__1__0_models.CreateScheduleTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CreateScheduleTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CreateScheduleTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -686,19 +1176,19 @@
         headers: ali_geniessp__1__0_models.CreateScheduleTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.CreateScheduleTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.CreateScheduleTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -725,45 +1215,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.CreateScheduleTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_alarms(
+    def create_schedule_task(
         self,
-        request: ali_geniessp__1__0_models.DeleteAlarmsRequest,
-    ) -> ali_geniessp__1__0_models.DeleteAlarmsResponse:
+        request: ali_geniessp__1__0_models.CreateScheduleTaskRequest,
+    ) -> ali_geniessp__1__0_models.CreateScheduleTaskResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeleteAlarmsHeaders()
-        return self.delete_alarms_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CreateScheduleTaskHeaders()
+        return self.create_schedule_task_with_options(request, headers, runtime)
 
-    async def delete_alarms_async(
+    async def create_schedule_task_async(
         self,
-        request: ali_geniessp__1__0_models.DeleteAlarmsRequest,
-    ) -> ali_geniessp__1__0_models.DeleteAlarmsResponse:
+        request: ali_geniessp__1__0_models.CreateScheduleTaskRequest,
+    ) -> ali_geniessp__1__0_models.CreateScheduleTaskResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeleteAlarmsHeaders()
-        return await self.delete_alarms_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.CreateScheduleTaskHeaders()
+        return await self.create_schedule_task_with_options_async(request, headers, runtime)
 
     def delete_alarms_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.DeleteAlarmsRequest,
         headers: ali_geniessp__1__0_models.DeleteAlarmsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeleteAlarmsResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.DeleteAlarmsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -800,19 +1290,19 @@
         headers: ali_geniessp__1__0_models.DeleteAlarmsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeleteAlarmsResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.DeleteAlarmsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -839,45 +1329,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.DeleteAlarmsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_schedule_task(
+    def delete_alarms(
         self,
-        request: ali_geniessp__1__0_models.DeleteScheduleTaskRequest,
-    ) -> ali_geniessp__1__0_models.DeleteScheduleTaskResponse:
+        request: ali_geniessp__1__0_models.DeleteAlarmsRequest,
+    ) -> ali_geniessp__1__0_models.DeleteAlarmsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeleteScheduleTaskHeaders()
-        return self.delete_schedule_task_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeleteAlarmsHeaders()
+        return self.delete_alarms_with_options(request, headers, runtime)
 
-    async def delete_schedule_task_async(
+    async def delete_alarms_async(
         self,
-        request: ali_geniessp__1__0_models.DeleteScheduleTaskRequest,
-    ) -> ali_geniessp__1__0_models.DeleteScheduleTaskResponse:
+        request: ali_geniessp__1__0_models.DeleteAlarmsRequest,
+    ) -> ali_geniessp__1__0_models.DeleteAlarmsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeleteScheduleTaskHeaders()
-        return await self.delete_schedule_task_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeleteAlarmsHeaders()
+        return await self.delete_alarms_with_options_async(request, headers, runtime)
 
     def delete_schedule_task_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.DeleteScheduleTaskRequest,
         headers: ali_geniessp__1__0_models.DeleteScheduleTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeleteScheduleTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.DeleteScheduleTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -914,19 +1404,19 @@
         headers: ali_geniessp__1__0_models.DeleteScheduleTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeleteScheduleTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.DeleteScheduleTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -953,29 +1443,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.DeleteScheduleTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_sub(
+    def delete_schedule_task(
         self,
-        request: ali_geniessp__1__0_models.DeleteSubRequest,
-    ) -> ali_geniessp__1__0_models.DeleteSubResponse:
+        request: ali_geniessp__1__0_models.DeleteScheduleTaskRequest,
+    ) -> ali_geniessp__1__0_models.DeleteScheduleTaskResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeleteSubHeaders()
-        return self.delete_sub_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeleteScheduleTaskHeaders()
+        return self.delete_schedule_task_with_options(request, headers, runtime)
 
-    async def delete_sub_async(
+    async def delete_schedule_task_async(
         self,
-        request: ali_geniessp__1__0_models.DeleteSubRequest,
-    ) -> ali_geniessp__1__0_models.DeleteSubResponse:
+        request: ali_geniessp__1__0_models.DeleteScheduleTaskRequest,
+    ) -> ali_geniessp__1__0_models.DeleteScheduleTaskResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeleteSubHeaders()
-        return await self.delete_sub_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeleteScheduleTaskHeaders()
+        return await self.delete_schedule_task_with_options_async(request, headers, runtime)
 
     def delete_sub_with_options(
         self,
         request: ali_geniessp__1__0_models.DeleteSubRequest,
         headers: ali_geniessp__1__0_models.DeleteSubHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeleteSubResponse:
@@ -1043,43 +1533,43 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.DeleteSubResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def device_control(
+    def delete_sub(
         self,
-        request: ali_geniessp__1__0_models.DeviceControlRequest,
-    ) -> ali_geniessp__1__0_models.DeviceControlResponse:
+        request: ali_geniessp__1__0_models.DeleteSubRequest,
+    ) -> ali_geniessp__1__0_models.DeleteSubResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeviceControlHeaders()
-        return self.device_control_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeleteSubHeaders()
+        return self.delete_sub_with_options(request, headers, runtime)
 
-    async def device_control_async(
+    async def delete_sub_async(
         self,
-        request: ali_geniessp__1__0_models.DeviceControlRequest,
-    ) -> ali_geniessp__1__0_models.DeviceControlResponse:
+        request: ali_geniessp__1__0_models.DeleteSubRequest,
+    ) -> ali_geniessp__1__0_models.DeleteSubResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.DeviceControlHeaders()
-        return await self.device_control_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeleteSubHeaders()
+        return await self.delete_sub_with_options_async(request, headers, runtime)
 
     def device_control_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.DeviceControlRequest,
         headers: ali_geniessp__1__0_models.DeviceControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeviceControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.DeviceControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.control_request):
-            request.control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.control_request), 'ControlRequest', 'json')
+            request.control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.control_request, 'ControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         body = {}
         if not UtilClient.is_unset(request.control_request_shrink):
             body['ControlRequest'] = request.control_request_shrink
         real_headers = {}
@@ -1116,17 +1606,17 @@
         headers: ali_geniessp__1__0_models.DeviceControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.DeviceControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.DeviceControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.control_request):
-            request.control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.control_request), 'ControlRequest', 'json')
+            request.control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.control_request, 'ControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         body = {}
         if not UtilClient.is_unset(request.control_request_shrink):
             body['ControlRequest'] = request.control_request_shrink
         real_headers = {}
@@ -1153,45 +1643,343 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.DeviceControlResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_alarm(
+    def device_control(
         self,
-        request: ali_geniessp__1__0_models.GetAlarmRequest,
-    ) -> ali_geniessp__1__0_models.GetAlarmResponse:
+        request: ali_geniessp__1__0_models.DeviceControlRequest,
+    ) -> ali_geniessp__1__0_models.DeviceControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetAlarmHeaders()
-        return self.get_alarm_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeviceControlHeaders()
+        return self.device_control_with_options(request, headers, runtime)
 
-    async def get_alarm_async(
+    async def device_control_async(
         self,
-        request: ali_geniessp__1__0_models.GetAlarmRequest,
-    ) -> ali_geniessp__1__0_models.GetAlarmResponse:
+        request: ali_geniessp__1__0_models.DeviceControlRequest,
+    ) -> ali_geniessp__1__0_models.DeviceControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetAlarmHeaders()
-        return await self.get_alarm_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.DeviceControlHeaders()
+        return await self.device_control_with_options_async(request, headers, runtime)
+
+    def ecology_openness_authenticate_with_options(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessAuthenticateRequest,
+        headers: ali_geniessp__1__0_models.EcologyOpennessAuthenticateHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessAuthenticateResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.encode_key):
+            body['EncodeKey'] = request.encode_key
+        if not UtilClient.is_unset(request.encode_type):
+            body['EncodeType'] = request.encode_type
+        if not UtilClient.is_unset(request.login_state_access_token):
+            body['LoginStateAccessToken'] = request.login_state_access_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='EcologyOpennessAuthenticate',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/ecologyOpennessAuthenticate',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.EcologyOpennessAuthenticateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def ecology_openness_authenticate_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessAuthenticateRequest,
+        headers: ali_geniessp__1__0_models.EcologyOpennessAuthenticateHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessAuthenticateResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.encode_key):
+            body['EncodeKey'] = request.encode_key
+        if not UtilClient.is_unset(request.encode_type):
+            body['EncodeType'] = request.encode_type
+        if not UtilClient.is_unset(request.login_state_access_token):
+            body['LoginStateAccessToken'] = request.login_state_access_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='EcologyOpennessAuthenticate',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/ecologyOpennessAuthenticate',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.EcologyOpennessAuthenticateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def ecology_openness_authenticate(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessAuthenticateRequest,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessAuthenticateResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.EcologyOpennessAuthenticateHeaders()
+        return self.ecology_openness_authenticate_with_options(request, headers, runtime)
+
+    async def ecology_openness_authenticate_async(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessAuthenticateRequest,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessAuthenticateResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.EcologyOpennessAuthenticateHeaders()
+        return await self.ecology_openness_authenticate_with_options_async(request, headers, runtime)
+
+    def ecology_openness_send_verification_code_with_options(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeRequest,
+        headers: ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.phone_number):
+            body['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.region):
+            body['Region'] = request.region
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='EcologyOpennessSendVerificationCode',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/ecologyOpennessSendVerificationCode',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def ecology_openness_send_verification_code_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeRequest,
+        headers: ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.phone_number):
+            body['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.region):
+            body['Region'] = request.region
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='EcologyOpennessSendVerificationCode',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/ecologyOpennessSendVerificationCode',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def ecology_openness_send_verification_code(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeRequest,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeHeaders()
+        return self.ecology_openness_send_verification_code_with_options(request, headers, runtime)
+
+    async def ecology_openness_send_verification_code_async(
+        self,
+        request: ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeRequest,
+    ) -> ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.EcologyOpennessSendVerificationCodeHeaders()
+        return await self.ecology_openness_send_verification_code_with_options_async(request, headers, runtime)
+
+    def find_userlist_to_auth_login_with_phone_number_with_options(
+        self,
+        request: ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberRequest,
+        headers: ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.code):
+            query['Code'] = request.code
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.session_id):
+            query['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='FindUserlistToAuthLoginWithPhoneNumber',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/findUserlistToAuthLoginWithPhoneNumber',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def find_userlist_to_auth_login_with_phone_number_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberRequest,
+        headers: ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.code):
+            query['Code'] = request.code
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.session_id):
+            query['SessionId'] = request.session_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='FindUserlistToAuthLoginWithPhoneNumber',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/findUserlistToAuthLoginWithPhoneNumber',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def find_userlist_to_auth_login_with_phone_number(
+        self,
+        request: ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberRequest,
+    ) -> ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberHeaders()
+        return self.find_userlist_to_auth_login_with_phone_number_with_options(request, headers, runtime)
+
+    async def find_userlist_to_auth_login_with_phone_number_async(
+        self,
+        request: ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberRequest,
+    ) -> ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.FindUserlistToAuthLoginWithPhoneNumberHeaders()
+        return await self.find_userlist_to_auth_login_with_phone_number_with_options_async(request, headers, runtime)
 
     def get_alarm_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetAlarmRequest,
         headers: ali_geniessp__1__0_models.GetAlarmHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetAlarmResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetAlarmShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -1228,19 +2016,19 @@
         headers: ali_geniessp__1__0_models.GetAlarmHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetAlarmResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetAlarmShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -1267,29 +2055,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetAlarmResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_album(
+    def get_alarm(
         self,
-        request: ali_geniessp__1__0_models.GetAlbumRequest,
-    ) -> ali_geniessp__1__0_models.GetAlbumResponse:
+        request: ali_geniessp__1__0_models.GetAlarmRequest,
+    ) -> ali_geniessp__1__0_models.GetAlarmResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetAlbumHeaders()
-        return self.get_album_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetAlarmHeaders()
+        return self.get_alarm_with_options(request, headers, runtime)
 
-    async def get_album_async(
+    async def get_alarm_async(
         self,
-        request: ali_geniessp__1__0_models.GetAlbumRequest,
-    ) -> ali_geniessp__1__0_models.GetAlbumResponse:
+        request: ali_geniessp__1__0_models.GetAlarmRequest,
+    ) -> ali_geniessp__1__0_models.GetAlarmResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetAlbumHeaders()
-        return await self.get_album_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetAlarmHeaders()
+        return await self.get_alarm_with_options_async(request, headers, runtime)
 
     def get_album_with_options(
         self,
         request: ali_geniessp__1__0_models.GetAlbumRequest,
         headers: ali_geniessp__1__0_models.GetAlbumHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetAlbumResponse:
@@ -1361,29 +2149,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetAlbumResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_album_detail_by_id(
+    def get_album(
         self,
-        request: ali_geniessp__1__0_models.GetAlbumDetailByIdRequest,
-    ) -> ali_geniessp__1__0_models.GetAlbumDetailByIdResponse:
+        request: ali_geniessp__1__0_models.GetAlbumRequest,
+    ) -> ali_geniessp__1__0_models.GetAlbumResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetAlbumDetailByIdHeaders()
-        return self.get_album_detail_by_id_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetAlbumHeaders()
+        return self.get_album_with_options(request, headers, runtime)
 
-    async def get_album_detail_by_id_async(
+    async def get_album_async(
         self,
-        request: ali_geniessp__1__0_models.GetAlbumDetailByIdRequest,
-    ) -> ali_geniessp__1__0_models.GetAlbumDetailByIdResponse:
+        request: ali_geniessp__1__0_models.GetAlbumRequest,
+    ) -> ali_geniessp__1__0_models.GetAlbumResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetAlbumDetailByIdHeaders()
-        return await self.get_album_detail_by_id_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetAlbumHeaders()
+        return await self.get_album_with_options_async(request, headers, runtime)
 
     def get_album_detail_by_id_with_options(
         self,
         request: ali_geniessp__1__0_models.GetAlbumDetailByIdRequest,
         headers: ali_geniessp__1__0_models.GetAlbumDetailByIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetAlbumDetailByIdResponse:
@@ -1451,43 +2239,133 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetAlbumDetailByIdResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_code_enhance(
+    def get_album_detail_by_id(
         self,
-        request: ali_geniessp__1__0_models.GetCodeEnhanceRequest,
-    ) -> ali_geniessp__1__0_models.GetCodeEnhanceResponse:
+        request: ali_geniessp__1__0_models.GetAlbumDetailByIdRequest,
+    ) -> ali_geniessp__1__0_models.GetAlbumDetailByIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetCodeEnhanceHeaders()
-        return self.get_code_enhance_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetAlbumDetailByIdHeaders()
+        return self.get_album_detail_by_id_with_options(request, headers, runtime)
 
-    async def get_code_enhance_async(
+    async def get_album_detail_by_id_async(
         self,
-        request: ali_geniessp__1__0_models.GetCodeEnhanceRequest,
-    ) -> ali_geniessp__1__0_models.GetCodeEnhanceResponse:
+        request: ali_geniessp__1__0_models.GetAlbumDetailByIdRequest,
+    ) -> ali_geniessp__1__0_models.GetAlbumDetailByIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetCodeEnhanceHeaders()
-        return await self.get_code_enhance_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetAlbumDetailByIdHeaders()
+        return await self.get_album_detail_by_id_with_options_async(request, headers, runtime)
+
+    def get_aligenie_user_info_with_options(
+        self,
+        request: ali_geniessp__1__0_models.GetAligenieUserInfoRequest,
+        headers: ali_geniessp__1__0_models.GetAligenieUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.GetAligenieUserInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.login_state_access_token):
+            query['LoginStateAccessToken'] = request.login_state_access_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAligenieUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/getAligenieUserInfo',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.GetAligenieUserInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_aligenie_user_info_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.GetAligenieUserInfoRequest,
+        headers: ali_geniessp__1__0_models.GetAligenieUserInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.GetAligenieUserInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.login_state_access_token):
+            query['LoginStateAccessToken'] = request.login_state_access_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAligenieUserInfo',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/getAligenieUserInfo',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.GetAligenieUserInfoResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_aligenie_user_info(
+        self,
+        request: ali_geniessp__1__0_models.GetAligenieUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.GetAligenieUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.GetAligenieUserInfoHeaders()
+        return self.get_aligenie_user_info_with_options(request, headers, runtime)
+
+    async def get_aligenie_user_info_async(
+        self,
+        request: ali_geniessp__1__0_models.GetAligenieUserInfoRequest,
+    ) -> ali_geniessp__1__0_models.GetAligenieUserInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.GetAligenieUserInfoHeaders()
+        return await self.get_aligenie_user_info_with_options_async(request, headers, runtime)
 
     def get_code_enhance_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetCodeEnhanceRequest,
         headers: ali_geniessp__1__0_models.GetCodeEnhanceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetCodeEnhanceResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetCodeEnhanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.channel_info):
-            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel_info), 'ChannelInfo', 'json')
+            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.channel_info, 'ChannelInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.channel_info_shrink):
             query['ChannelInfo'] = request.channel_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -1522,17 +2400,17 @@
         headers: ali_geniessp__1__0_models.GetCodeEnhanceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetCodeEnhanceResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetCodeEnhanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.channel_info):
-            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel_info), 'ChannelInfo', 'json')
+            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.channel_info, 'ChannelInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.channel_info_shrink):
             query['ChannelInfo'] = request.channel_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -1557,29 +2435,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetCodeEnhanceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_content(
+    def get_code_enhance(
         self,
-        request: ali_geniessp__1__0_models.GetContentRequest,
-    ) -> ali_geniessp__1__0_models.GetContentResponse:
+        request: ali_geniessp__1__0_models.GetCodeEnhanceRequest,
+    ) -> ali_geniessp__1__0_models.GetCodeEnhanceResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetContentHeaders()
-        return self.get_content_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetCodeEnhanceHeaders()
+        return self.get_code_enhance_with_options(request, headers, runtime)
 
-    async def get_content_async(
+    async def get_code_enhance_async(
         self,
-        request: ali_geniessp__1__0_models.GetContentRequest,
-    ) -> ali_geniessp__1__0_models.GetContentResponse:
+        request: ali_geniessp__1__0_models.GetCodeEnhanceRequest,
+    ) -> ali_geniessp__1__0_models.GetCodeEnhanceResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetContentHeaders()
-        return await self.get_content_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetCodeEnhanceHeaders()
+        return await self.get_code_enhance_with_options_async(request, headers, runtime)
 
     def get_content_with_options(
         self,
         request: ali_geniessp__1__0_models.GetContentRequest,
         headers: ali_geniessp__1__0_models.GetContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetContentResponse:
@@ -1651,43 +2529,43 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetContentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_current_playing_item(
+    def get_content(
         self,
-        request: ali_geniessp__1__0_models.GetCurrentPlayingItemRequest,
-    ) -> ali_geniessp__1__0_models.GetCurrentPlayingItemResponse:
+        request: ali_geniessp__1__0_models.GetContentRequest,
+    ) -> ali_geniessp__1__0_models.GetContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetCurrentPlayingItemHeaders()
-        return self.get_current_playing_item_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetContentHeaders()
+        return self.get_content_with_options(request, headers, runtime)
 
-    async def get_current_playing_item_async(
+    async def get_content_async(
         self,
-        request: ali_geniessp__1__0_models.GetCurrentPlayingItemRequest,
-    ) -> ali_geniessp__1__0_models.GetCurrentPlayingItemResponse:
+        request: ali_geniessp__1__0_models.GetContentRequest,
+    ) -> ali_geniessp__1__0_models.GetContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetCurrentPlayingItemHeaders()
-        return await self.get_current_playing_item_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetContentHeaders()
+        return await self.get_content_with_options_async(request, headers, runtime)
 
     def get_current_playing_item_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetCurrentPlayingItemRequest,
         headers: ali_geniessp__1__0_models.GetCurrentPlayingItemHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetCurrentPlayingItemResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetCurrentPlayingItemShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -1722,17 +2600,17 @@
         headers: ali_geniessp__1__0_models.GetCurrentPlayingItemHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetCurrentPlayingItemResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetCurrentPlayingItemShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -1757,45 +2635,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetCurrentPlayingItemResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_current_playing_list(
+    def get_current_playing_item(
         self,
-        request: ali_geniessp__1__0_models.GetCurrentPlayingListRequest,
-    ) -> ali_geniessp__1__0_models.GetCurrentPlayingListResponse:
+        request: ali_geniessp__1__0_models.GetCurrentPlayingItemRequest,
+    ) -> ali_geniessp__1__0_models.GetCurrentPlayingItemResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetCurrentPlayingListHeaders()
-        return self.get_current_playing_list_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetCurrentPlayingItemHeaders()
+        return self.get_current_playing_item_with_options(request, headers, runtime)
 
-    async def get_current_playing_list_async(
+    async def get_current_playing_item_async(
         self,
-        request: ali_geniessp__1__0_models.GetCurrentPlayingListRequest,
-    ) -> ali_geniessp__1__0_models.GetCurrentPlayingListResponse:
+        request: ali_geniessp__1__0_models.GetCurrentPlayingItemRequest,
+    ) -> ali_geniessp__1__0_models.GetCurrentPlayingItemResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetCurrentPlayingListHeaders()
-        return await self.get_current_playing_list_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetCurrentPlayingItemHeaders()
+        return await self.get_current_playing_item_with_options_async(request, headers, runtime)
 
     def get_current_playing_list_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetCurrentPlayingListRequest,
         headers: ali_geniessp__1__0_models.GetCurrentPlayingListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetCurrentPlayingListResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetCurrentPlayingListShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_query_play_list_request):
-            request.open_query_play_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_query_play_list_request), 'OpenQueryPlayListRequest', 'json')
+            request.open_query_play_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_query_play_list_request, 'OpenQueryPlayListRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_query_play_list_request_shrink):
@@ -1834,19 +2712,19 @@
         headers: ali_geniessp__1__0_models.GetCurrentPlayingListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetCurrentPlayingListResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetCurrentPlayingListShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_query_play_list_request):
-            request.open_query_play_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_query_play_list_request), 'OpenQueryPlayListRequest', 'json')
+            request.open_query_play_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_query_play_list_request, 'OpenQueryPlayListRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_query_play_list_request_shrink):
@@ -1875,41 +2753,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetCurrentPlayingListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_device_basic_info(
+    def get_current_playing_list(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceBasicInfoRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceBasicInfoResponse:
+        request: ali_geniessp__1__0_models.GetCurrentPlayingListRequest,
+    ) -> ali_geniessp__1__0_models.GetCurrentPlayingListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceBasicInfoHeaders()
-        return self.get_device_basic_info_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetCurrentPlayingListHeaders()
+        return self.get_current_playing_list_with_options(request, headers, runtime)
 
-    async def get_device_basic_info_async(
+    async def get_current_playing_list_async(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceBasicInfoRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceBasicInfoResponse:
+        request: ali_geniessp__1__0_models.GetCurrentPlayingListRequest,
+    ) -> ali_geniessp__1__0_models.GetCurrentPlayingListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceBasicInfoHeaders()
-        return await self.get_device_basic_info_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetCurrentPlayingListHeaders()
+        return await self.get_current_playing_list_with_options_async(request, headers, runtime)
 
     def get_device_basic_info_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetDeviceBasicInfoRequest,
         headers: ali_geniessp__1__0_models.GetDeviceBasicInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceBasicInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceBasicInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -1942,15 +2820,15 @@
         headers: ali_geniessp__1__0_models.GetDeviceBasicInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceBasicInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceBasicInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -1973,29 +2851,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetDeviceBasicInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_device_id_by_identity(
+    def get_device_basic_info(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceIdByIdentityRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceIdByIdentityResponse:
+        request: ali_geniessp__1__0_models.GetDeviceBasicInfoRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceBasicInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceIdByIdentityHeaders()
-        return self.get_device_id_by_identity_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceBasicInfoHeaders()
+        return self.get_device_basic_info_with_options(request, headers, runtime)
 
-    async def get_device_id_by_identity_async(
+    async def get_device_basic_info_async(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceIdByIdentityRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceIdByIdentityResponse:
+        request: ali_geniessp__1__0_models.GetDeviceBasicInfoRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceBasicInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceIdByIdentityHeaders()
-        return await self.get_device_id_by_identity_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceBasicInfoHeaders()
+        return await self.get_device_basic_info_with_options_async(request, headers, runtime)
 
     def get_device_id_by_identity_with_options(
         self,
         request: ali_geniessp__1__0_models.GetDeviceIdByIdentityRequest,
         headers: ali_geniessp__1__0_models.GetDeviceIdByIdentityHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceIdByIdentityResponse:
@@ -2079,41 +2957,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetDeviceIdByIdentityResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_device_setting(
+    def get_device_id_by_identity(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceSettingRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceSettingResponse:
+        request: ali_geniessp__1__0_models.GetDeviceIdByIdentityRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceIdByIdentityResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceSettingHeaders()
-        return self.get_device_setting_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceIdByIdentityHeaders()
+        return self.get_device_id_by_identity_with_options(request, headers, runtime)
 
-    async def get_device_setting_async(
+    async def get_device_id_by_identity_async(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceSettingRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceSettingResponse:
+        request: ali_geniessp__1__0_models.GetDeviceIdByIdentityRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceIdByIdentityResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceSettingHeaders()
-        return await self.get_device_setting_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceIdByIdentityHeaders()
+        return await self.get_device_id_by_identity_with_options_async(request, headers, runtime)
 
     def get_device_setting_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetDeviceSettingRequest,
         headers: ali_geniessp__1__0_models.GetDeviceSettingHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceSettingResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceSettingShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.keys):
             request.keys_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.keys, 'Keys', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.keys_shrink):
             query['Keys'] = request.keys_shrink
@@ -2150,15 +3028,15 @@
         headers: ali_geniessp__1__0_models.GetDeviceSettingHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceSettingResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceSettingShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.keys):
             request.keys_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.keys, 'Keys', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.keys_shrink):
             query['Keys'] = request.keys_shrink
@@ -2185,41 +3063,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetDeviceSettingResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_device_status_detail(
+    def get_device_setting(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceStatusDetailRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceStatusDetailResponse:
+        request: ali_geniessp__1__0_models.GetDeviceSettingRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceSettingResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceStatusDetailHeaders()
-        return self.get_device_status_detail_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceSettingHeaders()
+        return self.get_device_setting_with_options(request, headers, runtime)
 
-    async def get_device_status_detail_async(
+    async def get_device_setting_async(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceStatusDetailRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceStatusDetailResponse:
+        request: ali_geniessp__1__0_models.GetDeviceSettingRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceSettingResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceStatusDetailHeaders()
-        return await self.get_device_status_detail_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceSettingHeaders()
+        return await self.get_device_setting_with_options_async(request, headers, runtime)
 
     def get_device_status_detail_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetDeviceStatusDetailRequest,
         headers: ali_geniessp__1__0_models.GetDeviceStatusDetailHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceStatusDetailResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceStatusDetailShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.keys):
             request.keys_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.keys, 'Keys', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.keys_shrink):
             query['Keys'] = request.keys_shrink
@@ -2256,15 +3134,15 @@
         headers: ali_geniessp__1__0_models.GetDeviceStatusDetailHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceStatusDetailResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceStatusDetailShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.keys):
             request.keys_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.keys, 'Keys', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.keys_shrink):
             query['Keys'] = request.keys_shrink
@@ -2291,41 +3169,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetDeviceStatusDetailResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_device_status_info(
+    def get_device_status_detail(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceStatusInfoRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceStatusInfoResponse:
+        request: ali_geniessp__1__0_models.GetDeviceStatusDetailRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceStatusDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceStatusInfoHeaders()
-        return self.get_device_status_info_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceStatusDetailHeaders()
+        return self.get_device_status_detail_with_options(request, headers, runtime)
 
-    async def get_device_status_info_async(
+    async def get_device_status_detail_async(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceStatusInfoRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceStatusInfoResponse:
+        request: ali_geniessp__1__0_models.GetDeviceStatusDetailRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceStatusDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceStatusInfoHeaders()
-        return await self.get_device_status_info_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceStatusDetailHeaders()
+        return await self.get_device_status_detail_with_options_async(request, headers, runtime)
 
     def get_device_status_info_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetDeviceStatusInfoRequest,
         headers: ali_geniessp__1__0_models.GetDeviceStatusInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceStatusInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceStatusInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2358,15 +3236,15 @@
         headers: ali_geniessp__1__0_models.GetDeviceStatusInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceStatusInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceStatusInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2389,41 +3267,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetDeviceStatusInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_device_tag(
+    def get_device_status_info(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceTagRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceTagResponse:
+        request: ali_geniessp__1__0_models.GetDeviceStatusInfoRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceStatusInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceTagHeaders()
-        return self.get_device_tag_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceStatusInfoHeaders()
+        return self.get_device_status_info_with_options(request, headers, runtime)
 
-    async def get_device_tag_async(
+    async def get_device_status_info_async(
         self,
-        request: ali_geniessp__1__0_models.GetDeviceTagRequest,
-    ) -> ali_geniessp__1__0_models.GetDeviceTagResponse:
+        request: ali_geniessp__1__0_models.GetDeviceStatusInfoRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceStatusInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetDeviceTagHeaders()
-        return await self.get_device_tag_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceStatusInfoHeaders()
+        return await self.get_device_status_info_with_options_async(request, headers, runtime)
 
     def get_device_tag_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetDeviceTagRequest,
         headers: ali_geniessp__1__0_models.GetDeviceTagHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceTagResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceTagShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2456,15 +3334,15 @@
         headers: ali_geniessp__1__0_models.GetDeviceTagHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetDeviceTagResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetDeviceTagShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2487,45 +3365,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetDeviceTagResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_schedule_task(
+    def get_device_tag(
         self,
-        request: ali_geniessp__1__0_models.GetScheduleTaskRequest,
-    ) -> ali_geniessp__1__0_models.GetScheduleTaskResponse:
+        request: ali_geniessp__1__0_models.GetDeviceTagRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceTagResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetScheduleTaskHeaders()
-        return self.get_schedule_task_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceTagHeaders()
+        return self.get_device_tag_with_options(request, headers, runtime)
 
-    async def get_schedule_task_async(
+    async def get_device_tag_async(
         self,
-        request: ali_geniessp__1__0_models.GetScheduleTaskRequest,
-    ) -> ali_geniessp__1__0_models.GetScheduleTaskResponse:
+        request: ali_geniessp__1__0_models.GetDeviceTagRequest,
+    ) -> ali_geniessp__1__0_models.GetDeviceTagResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetScheduleTaskHeaders()
-        return await self.get_schedule_task_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetDeviceTagHeaders()
+        return await self.get_device_tag_with_options_async(request, headers, runtime)
 
     def get_schedule_task_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetScheduleTaskRequest,
         headers: ali_geniessp__1__0_models.GetScheduleTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetScheduleTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetScheduleTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -2562,19 +3440,19 @@
         headers: ali_geniessp__1__0_models.GetScheduleTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetScheduleTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetScheduleTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -2601,41 +3479,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetScheduleTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_unread_message_count(
+    def get_schedule_task(
         self,
-        request: ali_geniessp__1__0_models.GetUnreadMessageCountRequest,
-    ) -> ali_geniessp__1__0_models.GetUnreadMessageCountResponse:
+        request: ali_geniessp__1__0_models.GetScheduleTaskRequest,
+    ) -> ali_geniessp__1__0_models.GetScheduleTaskResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetUnreadMessageCountHeaders()
-        return self.get_unread_message_count_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetScheduleTaskHeaders()
+        return self.get_schedule_task_with_options(request, headers, runtime)
 
-    async def get_unread_message_count_async(
+    async def get_schedule_task_async(
         self,
-        request: ali_geniessp__1__0_models.GetUnreadMessageCountRequest,
-    ) -> ali_geniessp__1__0_models.GetUnreadMessageCountResponse:
+        request: ali_geniessp__1__0_models.GetScheduleTaskRequest,
+    ) -> ali_geniessp__1__0_models.GetScheduleTaskResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetUnreadMessageCountHeaders()
-        return await self.get_unread_message_count_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetScheduleTaskHeaders()
+        return await self.get_schedule_task_with_options_async(request, headers, runtime)
 
     def get_unread_message_count_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetUnreadMessageCountRequest,
         headers: ali_geniessp__1__0_models.GetUnreadMessageCountHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetUnreadMessageCountResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetUnreadMessageCountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2668,15 +3546,15 @@
         headers: ali_geniessp__1__0_models.GetUnreadMessageCountHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetUnreadMessageCountResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetUnreadMessageCountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2699,41 +3577,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetUnreadMessageCountResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user_by_device_id(
+    def get_unread_message_count(
         self,
-        request: ali_geniessp__1__0_models.GetUserByDeviceIdRequest,
-    ) -> ali_geniessp__1__0_models.GetUserByDeviceIdResponse:
+        request: ali_geniessp__1__0_models.GetUnreadMessageCountRequest,
+    ) -> ali_geniessp__1__0_models.GetUnreadMessageCountResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetUserByDeviceIdHeaders()
-        return self.get_user_by_device_id_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetUnreadMessageCountHeaders()
+        return self.get_unread_message_count_with_options(request, headers, runtime)
 
-    async def get_user_by_device_id_async(
+    async def get_unread_message_count_async(
         self,
-        request: ali_geniessp__1__0_models.GetUserByDeviceIdRequest,
-    ) -> ali_geniessp__1__0_models.GetUserByDeviceIdResponse:
+        request: ali_geniessp__1__0_models.GetUnreadMessageCountRequest,
+    ) -> ali_geniessp__1__0_models.GetUnreadMessageCountResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetUserByDeviceIdHeaders()
-        return await self.get_user_by_device_id_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetUnreadMessageCountHeaders()
+        return await self.get_unread_message_count_with_options_async(request, headers, runtime)
 
     def get_user_by_device_id_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetUserByDeviceIdRequest,
         headers: ali_geniessp__1__0_models.GetUserByDeviceIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetUserByDeviceIdResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetUserByDeviceIdShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2766,15 +3644,15 @@
         headers: ali_geniessp__1__0_models.GetUserByDeviceIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetUserByDeviceIdResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetUserByDeviceIdShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -2797,45 +3675,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetUserByDeviceIdResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_weather(
+    def get_user_by_device_id(
         self,
-        request: ali_geniessp__1__0_models.GetWeatherRequest,
-    ) -> ali_geniessp__1__0_models.GetWeatherResponse:
+        request: ali_geniessp__1__0_models.GetUserByDeviceIdRequest,
+    ) -> ali_geniessp__1__0_models.GetUserByDeviceIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetWeatherHeaders()
-        return self.get_weather_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetUserByDeviceIdHeaders()
+        return self.get_user_by_device_id_with_options(request, headers, runtime)
 
-    async def get_weather_async(
+    async def get_user_by_device_id_async(
         self,
-        request: ali_geniessp__1__0_models.GetWeatherRequest,
-    ) -> ali_geniessp__1__0_models.GetWeatherResponse:
+        request: ali_geniessp__1__0_models.GetUserByDeviceIdRequest,
+    ) -> ali_geniessp__1__0_models.GetUserByDeviceIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.GetWeatherHeaders()
-        return await self.get_weather_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetUserByDeviceIdHeaders()
+        return await self.get_user_by_device_id_with_options_async(request, headers, runtime)
 
     def get_weather_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.GetWeatherRequest,
         headers: ali_geniessp__1__0_models.GetWeatherHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetWeatherResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetWeatherShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -2872,19 +3750,19 @@
         headers: ali_geniessp__1__0_models.GetWeatherHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.GetWeatherResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.GetWeatherShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -2911,45 +3789,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.GetWeatherResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def index_control_playing_list(
+    def get_weather(
         self,
-        request: ali_geniessp__1__0_models.IndexControlPlayingListRequest,
-    ) -> ali_geniessp__1__0_models.IndexControlPlayingListResponse:
+        request: ali_geniessp__1__0_models.GetWeatherRequest,
+    ) -> ali_geniessp__1__0_models.GetWeatherResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.IndexControlPlayingListHeaders()
-        return self.index_control_playing_list_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetWeatherHeaders()
+        return self.get_weather_with_options(request, headers, runtime)
 
-    async def index_control_playing_list_async(
+    async def get_weather_async(
         self,
-        request: ali_geniessp__1__0_models.IndexControlPlayingListRequest,
-    ) -> ali_geniessp__1__0_models.IndexControlPlayingListResponse:
+        request: ali_geniessp__1__0_models.GetWeatherRequest,
+    ) -> ali_geniessp__1__0_models.GetWeatherResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.IndexControlPlayingListHeaders()
-        return await self.index_control_playing_list_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.GetWeatherHeaders()
+        return await self.get_weather_with_options_async(request, headers, runtime)
 
     def index_control_playing_list_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.IndexControlPlayingListRequest,
         headers: ali_geniessp__1__0_models.IndexControlPlayingListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.IndexControlPlayingListResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.IndexControlPlayingListShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_index_control_request):
-            request.open_index_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_index_control_request), 'OpenIndexControlRequest', 'json')
+            request.open_index_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_index_control_request, 'OpenIndexControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_index_control_request_shrink):
@@ -2988,19 +3866,19 @@
         headers: ali_geniessp__1__0_models.IndexControlPlayingListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.IndexControlPlayingListResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.IndexControlPlayingListShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_index_control_request):
-            request.open_index_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_index_control_request), 'OpenIndexControlRequest', 'json')
+            request.open_index_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_index_control_request, 'OpenIndexControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_index_control_request_shrink):
@@ -3029,45 +3907,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.IndexControlPlayingListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_alarms(
+    def index_control_playing_list(
         self,
-        request: ali_geniessp__1__0_models.ListAlarmsRequest,
-    ) -> ali_geniessp__1__0_models.ListAlarmsResponse:
+        request: ali_geniessp__1__0_models.IndexControlPlayingListRequest,
+    ) -> ali_geniessp__1__0_models.IndexControlPlayingListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListAlarmsHeaders()
-        return self.list_alarms_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.IndexControlPlayingListHeaders()
+        return self.index_control_playing_list_with_options(request, headers, runtime)
 
-    async def list_alarms_async(
+    async def index_control_playing_list_async(
         self,
-        request: ali_geniessp__1__0_models.ListAlarmsRequest,
-    ) -> ali_geniessp__1__0_models.ListAlarmsResponse:
+        request: ali_geniessp__1__0_models.IndexControlPlayingListRequest,
+    ) -> ali_geniessp__1__0_models.IndexControlPlayingListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListAlarmsHeaders()
-        return await self.list_alarms_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.IndexControlPlayingListHeaders()
+        return await self.index_control_playing_list_with_options_async(request, headers, runtime)
 
     def list_alarms_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListAlarmsRequest,
         headers: ali_geniessp__1__0_models.ListAlarmsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListAlarmsResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListAlarmsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -3104,19 +3982,19 @@
         headers: ali_geniessp__1__0_models.ListAlarmsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListAlarmsResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListAlarmsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -3143,29 +4021,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListAlarmsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_album_detail(
+    def list_alarms(
         self,
-        request: ali_geniessp__1__0_models.ListAlbumDetailRequest,
-    ) -> ali_geniessp__1__0_models.ListAlbumDetailResponse:
+        request: ali_geniessp__1__0_models.ListAlarmsRequest,
+    ) -> ali_geniessp__1__0_models.ListAlarmsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListAlbumDetailHeaders()
-        return self.list_album_detail_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListAlarmsHeaders()
+        return self.list_alarms_with_options(request, headers, runtime)
 
-    async def list_album_detail_async(
+    async def list_alarms_async(
         self,
-        request: ali_geniessp__1__0_models.ListAlbumDetailRequest,
-    ) -> ali_geniessp__1__0_models.ListAlbumDetailResponse:
+        request: ali_geniessp__1__0_models.ListAlarmsRequest,
+    ) -> ali_geniessp__1__0_models.ListAlarmsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListAlbumDetailHeaders()
-        return await self.list_album_detail_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListAlarmsHeaders()
+        return await self.list_alarms_with_options_async(request, headers, runtime)
 
     def list_album_detail_with_options(
         self,
         request: ali_geniessp__1__0_models.ListAlbumDetailRequest,
         headers: ali_geniessp__1__0_models.ListAlbumDetailHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListAlbumDetailResponse:
@@ -3241,45 +4119,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListAlbumDetailResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_album_is_added(
+    def list_album_detail(
         self,
-        request: ali_geniessp__1__0_models.ListAlbumIsAddedRequest,
-    ) -> ali_geniessp__1__0_models.ListAlbumIsAddedResponse:
+        request: ali_geniessp__1__0_models.ListAlbumDetailRequest,
+    ) -> ali_geniessp__1__0_models.ListAlbumDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListAlbumIsAddedHeaders()
-        return self.list_album_is_added_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListAlbumDetailHeaders()
+        return self.list_album_detail_with_options(request, headers, runtime)
 
-    async def list_album_is_added_async(
+    async def list_album_detail_async(
         self,
-        request: ali_geniessp__1__0_models.ListAlbumIsAddedRequest,
-    ) -> ali_geniessp__1__0_models.ListAlbumIsAddedResponse:
+        request: ali_geniessp__1__0_models.ListAlbumDetailRequest,
+    ) -> ali_geniessp__1__0_models.ListAlbumDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListAlbumIsAddedHeaders()
-        return await self.list_album_is_added_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListAlbumDetailHeaders()
+        return await self.list_album_detail_with_options_async(request, headers, runtime)
 
     def list_album_is_added_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListAlbumIsAddedRequest,
         headers: ali_geniessp__1__0_models.ListAlbumIsAddedHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListAlbumIsAddedResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListAlbumIsAddedShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.album_id_list):
             request.album_id_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.album_id_list, 'AlbumIdList', 'json')
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.album_id_list_shrink):
             query['AlbumIdList'] = request.album_id_list_shrink
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -3318,17 +4196,17 @@
     ) -> ali_geniessp__1__0_models.ListAlbumIsAddedResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListAlbumIsAddedShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.album_id_list):
             request.album_id_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.album_id_list, 'AlbumIdList', 'json')
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.album_id_list_shrink):
             query['AlbumIdList'] = request.album_id_list_shrink
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -3355,45 +4233,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListAlbumIsAddedResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_cate_content(
+    def list_album_is_added(
         self,
-        request: ali_geniessp__1__0_models.ListCateContentRequest,
-    ) -> ali_geniessp__1__0_models.ListCateContentResponse:
+        request: ali_geniessp__1__0_models.ListAlbumIsAddedRequest,
+    ) -> ali_geniessp__1__0_models.ListAlbumIsAddedResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCateContentHeaders()
-        return self.list_cate_content_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListAlbumIsAddedHeaders()
+        return self.list_album_is_added_with_options(request, headers, runtime)
 
-    async def list_cate_content_async(
+    async def list_album_is_added_async(
         self,
-        request: ali_geniessp__1__0_models.ListCateContentRequest,
-    ) -> ali_geniessp__1__0_models.ListCateContentResponse:
+        request: ali_geniessp__1__0_models.ListAlbumIsAddedRequest,
+    ) -> ali_geniessp__1__0_models.ListAlbumIsAddedResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCateContentHeaders()
-        return await self.list_cate_content_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListAlbumIsAddedHeaders()
+        return await self.list_album_is_added_with_options_async(request, headers, runtime)
 
     def list_cate_content_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListCateContentRequest,
         headers: ali_geniessp__1__0_models.ListCateContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListCateContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListCateContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -3432,19 +4310,19 @@
         headers: ali_geniessp__1__0_models.ListCateContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListCateContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListCateContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -3473,29 +4351,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListCateContentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_cate_info(
+    def list_cate_content(
         self,
-        request: ali_geniessp__1__0_models.ListCateInfoRequest,
-    ) -> ali_geniessp__1__0_models.ListCateInfoResponse:
+        request: ali_geniessp__1__0_models.ListCateContentRequest,
+    ) -> ali_geniessp__1__0_models.ListCateContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCateInfoHeaders()
-        return self.list_cate_info_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCateContentHeaders()
+        return self.list_cate_content_with_options(request, headers, runtime)
 
-    async def list_cate_info_async(
+    async def list_cate_content_async(
         self,
-        request: ali_geniessp__1__0_models.ListCateInfoRequest,
-    ) -> ali_geniessp__1__0_models.ListCateInfoResponse:
+        request: ali_geniessp__1__0_models.ListCateContentRequest,
+    ) -> ali_geniessp__1__0_models.ListCateContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCateInfoHeaders()
-        return await self.list_cate_info_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCateContentHeaders()
+        return await self.list_cate_content_with_options_async(request, headers, runtime)
 
     def list_cate_info_with_options(
         self,
         request: ali_geniessp__1__0_models.ListCateInfoRequest,
         headers: ali_geniessp__1__0_models.ListCateInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListCateInfoResponse:
@@ -3563,29 +4441,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListCateInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_common_cate_first_floor(
+    def list_cate_info(
         self,
-        request: ali_geniessp__1__0_models.ListCommonCateFirstFloorRequest,
-    ) -> ali_geniessp__1__0_models.ListCommonCateFirstFloorResponse:
+        request: ali_geniessp__1__0_models.ListCateInfoRequest,
+    ) -> ali_geniessp__1__0_models.ListCateInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCommonCateFirstFloorHeaders()
-        return self.list_common_cate_first_floor_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCateInfoHeaders()
+        return self.list_cate_info_with_options(request, headers, runtime)
 
-    async def list_common_cate_first_floor_async(
+    async def list_cate_info_async(
         self,
-        request: ali_geniessp__1__0_models.ListCommonCateFirstFloorRequest,
-    ) -> ali_geniessp__1__0_models.ListCommonCateFirstFloorResponse:
+        request: ali_geniessp__1__0_models.ListCateInfoRequest,
+    ) -> ali_geniessp__1__0_models.ListCateInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCommonCateFirstFloorHeaders()
-        return await self.list_common_cate_first_floor_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCateInfoHeaders()
+        return await self.list_cate_info_with_options_async(request, headers, runtime)
 
     def list_common_cate_first_floor_with_options(
         self,
         request: ali_geniessp__1__0_models.ListCommonCateFirstFloorRequest,
         headers: ali_geniessp__1__0_models.ListCommonCateFirstFloorHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListCommonCateFirstFloorResponse:
@@ -3653,29 +4531,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListCommonCateFirstFloorResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_common_cate_second_floor(
+    def list_common_cate_first_floor(
         self,
-        request: ali_geniessp__1__0_models.ListCommonCateSecondFloorRequest,
-    ) -> ali_geniessp__1__0_models.ListCommonCateSecondFloorResponse:
+        request: ali_geniessp__1__0_models.ListCommonCateFirstFloorRequest,
+    ) -> ali_geniessp__1__0_models.ListCommonCateFirstFloorResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCommonCateSecondFloorHeaders()
-        return self.list_common_cate_second_floor_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCommonCateFirstFloorHeaders()
+        return self.list_common_cate_first_floor_with_options(request, headers, runtime)
 
-    async def list_common_cate_second_floor_async(
+    async def list_common_cate_first_floor_async(
         self,
-        request: ali_geniessp__1__0_models.ListCommonCateSecondFloorRequest,
-    ) -> ali_geniessp__1__0_models.ListCommonCateSecondFloorResponse:
+        request: ali_geniessp__1__0_models.ListCommonCateFirstFloorRequest,
+    ) -> ali_geniessp__1__0_models.ListCommonCateFirstFloorResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListCommonCateSecondFloorHeaders()
-        return await self.list_common_cate_second_floor_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCommonCateFirstFloorHeaders()
+        return await self.list_common_cate_first_floor_with_options_async(request, headers, runtime)
 
     def list_common_cate_second_floor_with_options(
         self,
         request: ali_geniessp__1__0_models.ListCommonCateSecondFloorRequest,
         headers: ali_geniessp__1__0_models.ListCommonCateSecondFloorHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListCommonCateSecondFloorResponse:
@@ -3743,41 +4621,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListCommonCateSecondFloorResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_device_basic_info(
+    def list_common_cate_second_floor(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceBasicInfoRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceBasicInfoResponse:
+        request: ali_geniessp__1__0_models.ListCommonCateSecondFloorRequest,
+    ) -> ali_geniessp__1__0_models.ListCommonCateSecondFloorResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceBasicInfoHeaders()
-        return self.list_device_basic_info_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCommonCateSecondFloorHeaders()
+        return self.list_common_cate_second_floor_with_options(request, headers, runtime)
 
-    async def list_device_basic_info_async(
+    async def list_common_cate_second_floor_async(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceBasicInfoRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceBasicInfoResponse:
+        request: ali_geniessp__1__0_models.ListCommonCateSecondFloorRequest,
+    ) -> ali_geniessp__1__0_models.ListCommonCateSecondFloorResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceBasicInfoHeaders()
-        return await self.list_device_basic_info_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListCommonCateSecondFloorHeaders()
+        return await self.list_common_cate_second_floor_with_options_async(request, headers, runtime)
 
     def list_device_basic_info_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListDeviceBasicInfoRequest,
         headers: ali_geniessp__1__0_models.ListDeviceBasicInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceBasicInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListDeviceBasicInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_infos):
-            request.device_infos_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_infos), 'DeviceInfos', 'json')
+            request.device_infos_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_infos, 'DeviceInfos', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_infos_shrink):
             query['DeviceInfos'] = request.device_infos_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -3810,15 +4688,15 @@
         headers: ali_geniessp__1__0_models.ListDeviceBasicInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceBasicInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListDeviceBasicInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_infos):
-            request.device_infos_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_infos), 'DeviceInfos', 'json')
+            request.device_infos_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_infos, 'DeviceInfos', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_infos_shrink):
             query['DeviceInfos'] = request.device_infos_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -3841,41 +4719,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListDeviceBasicInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_device_by_user_id(
+    def list_device_basic_info(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceByUserIdRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdResponse:
+        request: ali_geniessp__1__0_models.ListDeviceBasicInfoRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceBasicInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceByUserIdHeaders()
-        return self.list_device_by_user_id_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceBasicInfoHeaders()
+        return self.list_device_basic_info_with_options(request, headers, runtime)
 
-    async def list_device_by_user_id_async(
+    async def list_device_basic_info_async(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceByUserIdRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdResponse:
+        request: ali_geniessp__1__0_models.ListDeviceBasicInfoRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceBasicInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceByUserIdHeaders()
-        return await self.list_device_by_user_id_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceBasicInfoHeaders()
+        return await self.list_device_basic_info_with_options_async(request, headers, runtime)
 
     def list_device_by_user_id_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListDeviceByUserIdRequest,
         headers: ali_geniessp__1__0_models.ListDeviceByUserIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceByUserIdResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListDeviceByUserIdShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -3908,15 +4786,15 @@
         headers: ali_geniessp__1__0_models.ListDeviceByUserIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceByUserIdResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListDeviceByUserIdShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
@@ -3939,43 +4817,43 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListDeviceByUserIdResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_device_by_user_id_and_chanel(
+    def list_device_by_user_id(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse:
+        request: ali_geniessp__1__0_models.ListDeviceByUserIdRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelHeaders()
-        return self.list_device_by_user_id_and_chanel_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceByUserIdHeaders()
+        return self.list_device_by_user_id_with_options(request, headers, runtime)
 
-    async def list_device_by_user_id_and_chanel_async(
+    async def list_device_by_user_id_async(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse:
+        request: ali_geniessp__1__0_models.ListDeviceByUserIdRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelHeaders()
-        return await self.list_device_by_user_id_and_chanel_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceByUserIdHeaders()
+        return await self.list_device_by_user_id_with_options_async(request, headers, runtime)
 
     def list_device_by_user_id_and_chanel_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelRequest,
         headers: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.channel_info):
-            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel_info), 'ChannelInfo', 'json')
+            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.channel_info, 'ChannelInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.channel_info_shrink):
             query['ChannelInfo'] = request.channel_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -4010,17 +4888,17 @@
         headers: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.channel_info):
-            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel_info), 'ChannelInfo', 'json')
+            request.channel_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.channel_info, 'ChannelInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.channel_info_shrink):
             query['ChannelInfo'] = request.channel_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -4045,29 +4923,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_device_id_by_identities(
+    def list_device_by_user_id_and_chanel(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceIdByIdentitiesRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceIdByIdentitiesResponse:
+        request: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceIdByIdentitiesHeaders()
-        return self.list_device_id_by_identities_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelHeaders()
+        return self.list_device_by_user_id_and_chanel_with_options(request, headers, runtime)
 
-    async def list_device_id_by_identities_async(
+    async def list_device_by_user_id_and_chanel_async(
         self,
-        request: ali_geniessp__1__0_models.ListDeviceIdByIdentitiesRequest,
-    ) -> ali_geniessp__1__0_models.ListDeviceIdByIdentitiesResponse:
+        request: ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListDeviceIdByIdentitiesHeaders()
-        return await self.list_device_id_by_identities_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceByUserIdAndChanelHeaders()
+        return await self.list_device_by_user_id_and_chanel_with_options_async(request, headers, runtime)
 
     def list_device_id_by_identities_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListDeviceIdByIdentitiesRequest,
         headers: ali_geniessp__1__0_models.ListDeviceIdByIdentitiesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListDeviceIdByIdentitiesResponse:
@@ -4159,45 +5037,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListDeviceIdByIdentitiesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_music(
+    def list_device_id_by_identities(
         self,
-        request: ali_geniessp__1__0_models.ListMusicRequest,
-    ) -> ali_geniessp__1__0_models.ListMusicResponse:
+        request: ali_geniessp__1__0_models.ListDeviceIdByIdentitiesRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceIdByIdentitiesResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListMusicHeaders()
-        return self.list_music_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceIdByIdentitiesHeaders()
+        return self.list_device_id_by_identities_with_options(request, headers, runtime)
 
-    async def list_music_async(
+    async def list_device_id_by_identities_async(
         self,
-        request: ali_geniessp__1__0_models.ListMusicRequest,
-    ) -> ali_geniessp__1__0_models.ListMusicResponse:
+        request: ali_geniessp__1__0_models.ListDeviceIdByIdentitiesRequest,
+    ) -> ali_geniessp__1__0_models.ListDeviceIdByIdentitiesResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListMusicHeaders()
-        return await self.list_music_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListDeviceIdByIdentitiesHeaders()
+        return await self.list_device_id_by_identities_with_options_async(request, headers, runtime)
 
     def list_music_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListMusicRequest,
         headers: ali_geniessp__1__0_models.ListMusicHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListMusicResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListMusicShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -4234,19 +5112,19 @@
         headers: ali_geniessp__1__0_models.ListMusicHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListMusicResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListMusicShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -4273,45 +5151,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListMusicResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_play_history(
+    def list_music(
         self,
-        request: ali_geniessp__1__0_models.ListPlayHistoryRequest,
-    ) -> ali_geniessp__1__0_models.ListPlayHistoryResponse:
+        request: ali_geniessp__1__0_models.ListMusicRequest,
+    ) -> ali_geniessp__1__0_models.ListMusicResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListPlayHistoryHeaders()
-        return self.list_play_history_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListMusicHeaders()
+        return self.list_music_with_options(request, headers, runtime)
 
-    async def list_play_history_async(
+    async def list_music_async(
         self,
-        request: ali_geniessp__1__0_models.ListPlayHistoryRequest,
-    ) -> ali_geniessp__1__0_models.ListPlayHistoryResponse:
+        request: ali_geniessp__1__0_models.ListMusicRequest,
+    ) -> ali_geniessp__1__0_models.ListMusicResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListPlayHistoryHeaders()
-        return await self.list_play_history_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListMusicHeaders()
+        return await self.list_music_with_options_async(request, headers, runtime)
 
     def list_play_history_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListPlayHistoryRequest,
         headers: ali_geniessp__1__0_models.ListPlayHistoryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListPlayHistoryResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListPlayHistoryShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -4350,19 +5228,19 @@
         headers: ali_geniessp__1__0_models.ListPlayHistoryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListPlayHistoryResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListPlayHistoryShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -4391,45 +5269,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListPlayHistoryResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_recommend_content(
+    def list_play_history(
         self,
-        request: ali_geniessp__1__0_models.ListRecommendContentRequest,
-    ) -> ali_geniessp__1__0_models.ListRecommendContentResponse:
+        request: ali_geniessp__1__0_models.ListPlayHistoryRequest,
+    ) -> ali_geniessp__1__0_models.ListPlayHistoryResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListRecommendContentHeaders()
-        return self.list_recommend_content_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListPlayHistoryHeaders()
+        return self.list_play_history_with_options(request, headers, runtime)
 
-    async def list_recommend_content_async(
+    async def list_play_history_async(
         self,
-        request: ali_geniessp__1__0_models.ListRecommendContentRequest,
-    ) -> ali_geniessp__1__0_models.ListRecommendContentResponse:
+        request: ali_geniessp__1__0_models.ListPlayHistoryRequest,
+    ) -> ali_geniessp__1__0_models.ListPlayHistoryResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListRecommendContentHeaders()
-        return await self.list_recommend_content_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListPlayHistoryHeaders()
+        return await self.list_play_history_with_options_async(request, headers, runtime)
 
     def list_recommend_content_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListRecommendContentRequest,
         headers: ali_geniessp__1__0_models.ListRecommendContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListRecommendContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListRecommendContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -4468,19 +5346,19 @@
         headers: ali_geniessp__1__0_models.ListRecommendContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListRecommendContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListRecommendContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -4509,45 +5387,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListRecommendContentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_sub(
+    def list_recommend_content(
         self,
-        request: ali_geniessp__1__0_models.ListSubRequest,
-    ) -> ali_geniessp__1__0_models.ListSubResponse:
+        request: ali_geniessp__1__0_models.ListRecommendContentRequest,
+    ) -> ali_geniessp__1__0_models.ListRecommendContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListSubHeaders()
-        return self.list_sub_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListRecommendContentHeaders()
+        return self.list_recommend_content_with_options(request, headers, runtime)
 
-    async def list_sub_async(
+    async def list_recommend_content_async(
         self,
-        request: ali_geniessp__1__0_models.ListSubRequest,
-    ) -> ali_geniessp__1__0_models.ListSubResponse:
+        request: ali_geniessp__1__0_models.ListRecommendContentRequest,
+    ) -> ali_geniessp__1__0_models.ListRecommendContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListSubHeaders()
-        return await self.list_sub_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListRecommendContentHeaders()
+        return await self.list_recommend_content_with_options_async(request, headers, runtime)
 
     def list_sub_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListSubRequest,
         headers: ali_geniessp__1__0_models.ListSubHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListSubResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListSubShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.page):
-            request.page_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.page), 'Page', 'json')
+            request.page_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.page, 'Page', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.page_shrink):
             query['Page'] = request.page_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -4584,19 +5462,19 @@
         headers: ali_geniessp__1__0_models.ListSubHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListSubResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListSubShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.page):
-            request.page_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.page), 'Page', 'json')
+            request.page_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.page, 'Page', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.page_shrink):
             query['Page'] = request.page_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -4623,45 +5501,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListSubResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_sub_album(
+    def list_sub(
         self,
-        request: ali_geniessp__1__0_models.ListSubAlbumRequest,
-    ) -> ali_geniessp__1__0_models.ListSubAlbumResponse:
+        request: ali_geniessp__1__0_models.ListSubRequest,
+    ) -> ali_geniessp__1__0_models.ListSubResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListSubAlbumHeaders()
-        return self.list_sub_album_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListSubHeaders()
+        return self.list_sub_with_options(request, headers, runtime)
 
-    async def list_sub_album_async(
+    async def list_sub_async(
         self,
-        request: ali_geniessp__1__0_models.ListSubAlbumRequest,
-    ) -> ali_geniessp__1__0_models.ListSubAlbumResponse:
+        request: ali_geniessp__1__0_models.ListSubRequest,
+    ) -> ali_geniessp__1__0_models.ListSubResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListSubAlbumHeaders()
-        return await self.list_sub_album_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListSubHeaders()
+        return await self.list_sub_with_options_async(request, headers, runtime)
 
     def list_sub_album_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListSubAlbumRequest,
         headers: ali_geniessp__1__0_models.ListSubAlbumHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListSubAlbumResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListSubAlbumShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.query_subscription_album_request):
-            request.query_subscription_album_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.query_subscription_album_request), 'QuerySubscriptionAlbumRequest', 'json')
+            request.query_subscription_album_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.query_subscription_album_request, 'QuerySubscriptionAlbumRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.query_subscription_album_request_shrink):
             query['QuerySubscriptionAlbumRequest'] = request.query_subscription_album_request_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -4698,19 +5576,19 @@
         headers: ali_geniessp__1__0_models.ListSubAlbumHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListSubAlbumResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListSubAlbumShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.query_subscription_album_request):
-            request.query_subscription_album_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.query_subscription_album_request), 'QuerySubscriptionAlbumRequest', 'json')
+            request.query_subscription_album_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.query_subscription_album_request, 'QuerySubscriptionAlbumRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.query_subscription_album_request_shrink):
             query['QuerySubscriptionAlbumRequest'] = request.query_subscription_album_request_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
@@ -4737,29 +5615,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListSubAlbumResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_subscription_album_category(
+    def list_sub_album(
         self,
-        request: ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryRequest,
-    ) -> ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryResponse:
+        request: ali_geniessp__1__0_models.ListSubAlbumRequest,
+    ) -> ali_geniessp__1__0_models.ListSubAlbumResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryHeaders()
-        return self.list_subscription_album_category_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListSubAlbumHeaders()
+        return self.list_sub_album_with_options(request, headers, runtime)
 
-    async def list_subscription_album_category_async(
+    async def list_sub_album_async(
         self,
-        request: ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryRequest,
-    ) -> ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryResponse:
+        request: ali_geniessp__1__0_models.ListSubAlbumRequest,
+    ) -> ali_geniessp__1__0_models.ListSubAlbumResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryHeaders()
-        return await self.list_subscription_album_category_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListSubAlbumHeaders()
+        return await self.list_sub_album_with_options_async(request, headers, runtime)
 
     def list_subscription_album_category_with_options(
         self,
         request: ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryRequest,
         headers: ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryResponse:
@@ -4827,41 +5705,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_user_message(
+    def list_subscription_album_category(
         self,
-        request: ali_geniessp__1__0_models.ListUserMessageRequest,
-    ) -> ali_geniessp__1__0_models.ListUserMessageResponse:
+        request: ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryRequest,
+    ) -> ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListUserMessageHeaders()
-        return self.list_user_message_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryHeaders()
+        return self.list_subscription_album_category_with_options(request, headers, runtime)
 
-    async def list_user_message_async(
+    async def list_subscription_album_category_async(
         self,
-        request: ali_geniessp__1__0_models.ListUserMessageRequest,
-    ) -> ali_geniessp__1__0_models.ListUserMessageResponse:
+        request: ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryRequest,
+    ) -> ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ListUserMessageHeaders()
-        return await self.list_user_message_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListSubscriptionAlbumCategoryHeaders()
+        return await self.list_subscription_album_category_with_options_async(request, headers, runtime)
 
     def list_user_message_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ListUserMessageRequest,
         headers: ali_geniessp__1__0_models.ListUserMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListUserMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListUserMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.before_time):
             query['BeforeTime'] = request.before_time
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         if not UtilClient.is_unset(request.limit):
             query['limit'] = request.limit
@@ -4898,15 +5776,15 @@
         headers: ali_geniessp__1__0_models.ListUserMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ListUserMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ListUserMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.before_time):
             query['BeforeTime'] = request.before_time
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         if not UtilClient.is_unset(request.limit):
             query['limit'] = request.limit
@@ -4933,45 +5811,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ListUserMessageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def play_and_pause_control(
+    def list_user_message(
         self,
-        request: ali_geniessp__1__0_models.PlayAndPauseControlRequest,
-    ) -> ali_geniessp__1__0_models.PlayAndPauseControlResponse:
+        request: ali_geniessp__1__0_models.ListUserMessageRequest,
+    ) -> ali_geniessp__1__0_models.ListUserMessageResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.PlayAndPauseControlHeaders()
-        return self.play_and_pause_control_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListUserMessageHeaders()
+        return self.list_user_message_with_options(request, headers, runtime)
 
-    async def play_and_pause_control_async(
+    async def list_user_message_async(
         self,
-        request: ali_geniessp__1__0_models.PlayAndPauseControlRequest,
-    ) -> ali_geniessp__1__0_models.PlayAndPauseControlResponse:
+        request: ali_geniessp__1__0_models.ListUserMessageRequest,
+    ) -> ali_geniessp__1__0_models.ListUserMessageResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.PlayAndPauseControlHeaders()
-        return await self.play_and_pause_control_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ListUserMessageHeaders()
+        return await self.list_user_message_with_options_async(request, headers, runtime)
 
     def play_and_pause_control_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.PlayAndPauseControlRequest,
         headers: ali_geniessp__1__0_models.PlayAndPauseControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.PlayAndPauseControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.PlayAndPauseControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_play_and_pause_control_param):
-            request.open_play_and_pause_control_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_play_and_pause_control_param), 'OpenPlayAndPauseControlParam', 'json')
+            request.open_play_and_pause_control_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_play_and_pause_control_param, 'OpenPlayAndPauseControlParam', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_play_and_pause_control_param_shrink):
@@ -5010,19 +5888,19 @@
         headers: ali_geniessp__1__0_models.PlayAndPauseControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.PlayAndPauseControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.PlayAndPauseControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_play_and_pause_control_param):
-            request.open_play_and_pause_control_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_play_and_pause_control_param), 'OpenPlayAndPauseControlParam', 'json')
+            request.open_play_and_pause_control_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_play_and_pause_control_param, 'OpenPlayAndPauseControlParam', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_play_and_pause_control_param_shrink):
@@ -5051,45 +5929,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.PlayAndPauseControlResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def play_mode_control(
+    def play_and_pause_control(
         self,
-        request: ali_geniessp__1__0_models.PlayModeControlRequest,
-    ) -> ali_geniessp__1__0_models.PlayModeControlResponse:
+        request: ali_geniessp__1__0_models.PlayAndPauseControlRequest,
+    ) -> ali_geniessp__1__0_models.PlayAndPauseControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.PlayModeControlHeaders()
-        return self.play_mode_control_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.PlayAndPauseControlHeaders()
+        return self.play_and_pause_control_with_options(request, headers, runtime)
 
-    async def play_mode_control_async(
+    async def play_and_pause_control_async(
         self,
-        request: ali_geniessp__1__0_models.PlayModeControlRequest,
-    ) -> ali_geniessp__1__0_models.PlayModeControlResponse:
+        request: ali_geniessp__1__0_models.PlayAndPauseControlRequest,
+    ) -> ali_geniessp__1__0_models.PlayAndPauseControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.PlayModeControlHeaders()
-        return await self.play_mode_control_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.PlayAndPauseControlHeaders()
+        return await self.play_and_pause_control_with_options_async(request, headers, runtime)
 
     def play_mode_control_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.PlayModeControlRequest,
         headers: ali_geniessp__1__0_models.PlayModeControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.PlayModeControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.PlayModeControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_play_mode_control_request):
-            request.open_play_mode_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_play_mode_control_request), 'OpenPlayModeControlRequest', 'json')
+            request.open_play_mode_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_play_mode_control_request, 'OpenPlayModeControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_play_mode_control_request_shrink):
@@ -5128,19 +6006,19 @@
         headers: ali_geniessp__1__0_models.PlayModeControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.PlayModeControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.PlayModeControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_play_mode_control_request):
-            request.open_play_mode_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_play_mode_control_request), 'OpenPlayModeControlRequest', 'json')
+            request.open_play_mode_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_play_mode_control_request, 'OpenPlayModeControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_play_mode_control_request_shrink):
@@ -5169,45 +6047,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.PlayModeControlResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def previous_and_next_control(
+    def play_mode_control(
         self,
-        request: ali_geniessp__1__0_models.PreviousAndNextControlRequest,
-    ) -> ali_geniessp__1__0_models.PreviousAndNextControlResponse:
+        request: ali_geniessp__1__0_models.PlayModeControlRequest,
+    ) -> ali_geniessp__1__0_models.PlayModeControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.PreviousAndNextControlHeaders()
-        return self.previous_and_next_control_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.PlayModeControlHeaders()
+        return self.play_mode_control_with_options(request, headers, runtime)
 
-    async def previous_and_next_control_async(
+    async def play_mode_control_async(
         self,
-        request: ali_geniessp__1__0_models.PreviousAndNextControlRequest,
-    ) -> ali_geniessp__1__0_models.PreviousAndNextControlResponse:
+        request: ali_geniessp__1__0_models.PlayModeControlRequest,
+    ) -> ali_geniessp__1__0_models.PlayModeControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.PreviousAndNextControlHeaders()
-        return await self.previous_and_next_control_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.PlayModeControlHeaders()
+        return await self.play_mode_control_with_options_async(request, headers, runtime)
 
     def previous_and_next_control_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.PreviousAndNextControlRequest,
         headers: ali_geniessp__1__0_models.PreviousAndNextControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.PreviousAndNextControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.PreviousAndNextControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_control_playing_list_request):
-            request.open_control_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_control_playing_list_request), 'OpenControlPlayingListRequest', 'json')
+            request.open_control_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_control_playing_list_request, 'OpenControlPlayingListRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_control_playing_list_request_shrink):
@@ -5246,19 +6124,19 @@
         headers: ali_geniessp__1__0_models.PreviousAndNextControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.PreviousAndNextControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.PreviousAndNextControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_control_playing_list_request):
-            request.open_control_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_control_playing_list_request), 'OpenControlPlayingListRequest', 'json')
+            request.open_control_playing_list_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_control_playing_list_request, 'OpenControlPlayingListRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_control_playing_list_request_shrink):
@@ -5287,45 +6165,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.PreviousAndNextControlResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def progress_control(
+    def previous_and_next_control(
         self,
-        request: ali_geniessp__1__0_models.ProgressControlRequest,
-    ) -> ali_geniessp__1__0_models.ProgressControlResponse:
+        request: ali_geniessp__1__0_models.PreviousAndNextControlRequest,
+    ) -> ali_geniessp__1__0_models.PreviousAndNextControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ProgressControlHeaders()
-        return self.progress_control_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.PreviousAndNextControlHeaders()
+        return self.previous_and_next_control_with_options(request, headers, runtime)
 
-    async def progress_control_async(
+    async def previous_and_next_control_async(
         self,
-        request: ali_geniessp__1__0_models.ProgressControlRequest,
-    ) -> ali_geniessp__1__0_models.ProgressControlResponse:
+        request: ali_geniessp__1__0_models.PreviousAndNextControlRequest,
+    ) -> ali_geniessp__1__0_models.PreviousAndNextControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ProgressControlHeaders()
-        return await self.progress_control_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.PreviousAndNextControlHeaders()
+        return await self.previous_and_next_control_with_options_async(request, headers, runtime)
 
     def progress_control_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ProgressControlRequest,
         headers: ali_geniessp__1__0_models.ProgressControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ProgressControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ProgressControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_progress_control_request):
-            request.open_progress_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_progress_control_request), 'OpenProgressControlRequest', 'json')
+            request.open_progress_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_progress_control_request, 'OpenProgressControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_progress_control_request_shrink):
@@ -5364,19 +6242,19 @@
         headers: ali_geniessp__1__0_models.ProgressControlHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ProgressControlResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ProgressControlShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.open_progress_control_request):
-            request.open_progress_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_progress_control_request), 'OpenProgressControlRequest', 'json')
+            request.open_progress_control_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.open_progress_control_request, 'OpenProgressControlRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.open_progress_control_request_shrink):
@@ -5405,45 +6283,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ProgressControlResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def query_music_type(
+    def progress_control(
         self,
-        request: ali_geniessp__1__0_models.QueryMusicTypeRequest,
-    ) -> ali_geniessp__1__0_models.QueryMusicTypeResponse:
+        request: ali_geniessp__1__0_models.ProgressControlRequest,
+    ) -> ali_geniessp__1__0_models.ProgressControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.QueryMusicTypeHeaders()
-        return self.query_music_type_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ProgressControlHeaders()
+        return self.progress_control_with_options(request, headers, runtime)
 
-    async def query_music_type_async(
+    async def progress_control_async(
         self,
-        request: ali_geniessp__1__0_models.QueryMusicTypeRequest,
-    ) -> ali_geniessp__1__0_models.QueryMusicTypeResponse:
+        request: ali_geniessp__1__0_models.ProgressControlRequest,
+    ) -> ali_geniessp__1__0_models.ProgressControlResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.QueryMusicTypeHeaders()
-        return await self.query_music_type_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ProgressControlHeaders()
+        return await self.progress_control_with_options_async(request, headers, runtime)
 
     def query_music_type_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.QueryMusicTypeRequest,
         headers: ali_geniessp__1__0_models.QueryMusicTypeHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.QueryMusicTypeResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.QueryMusicTypeShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -5480,19 +6358,19 @@
         headers: ali_geniessp__1__0_models.QueryMusicTypeHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.QueryMusicTypeResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.QueryMusicTypeShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -5519,41 +6397,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.QueryMusicTypeResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def read_message(
+    def query_music_type(
         self,
-        request: ali_geniessp__1__0_models.ReadMessageRequest,
-    ) -> ali_geniessp__1__0_models.ReadMessageResponse:
+        request: ali_geniessp__1__0_models.QueryMusicTypeRequest,
+    ) -> ali_geniessp__1__0_models.QueryMusicTypeResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ReadMessageHeaders()
-        return self.read_message_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.QueryMusicTypeHeaders()
+        return self.query_music_type_with_options(request, headers, runtime)
 
-    async def read_message_async(
+    async def query_music_type_async(
         self,
-        request: ali_geniessp__1__0_models.ReadMessageRequest,
-    ) -> ali_geniessp__1__0_models.ReadMessageResponse:
+        request: ali_geniessp__1__0_models.QueryMusicTypeRequest,
+    ) -> ali_geniessp__1__0_models.QueryMusicTypeResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ReadMessageHeaders()
-        return await self.read_message_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.QueryMusicTypeHeaders()
+        return await self.query_music_type_with_options_async(request, headers, runtime)
 
     def read_message_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ReadMessageRequest,
         headers: ali_geniessp__1__0_models.ReadMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ReadMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ReadMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.message_id):
             query['MessageId'] = request.message_id
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -5588,15 +6466,15 @@
         headers: ali_geniessp__1__0_models.ReadMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ReadMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ReadMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.message_id):
             query['MessageId'] = request.message_id
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -5621,41 +6499,147 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ReadMessageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def scg_search(
+    def read_message(
         self,
-        request: ali_geniessp__1__0_models.ScgSearchRequest,
-    ) -> ali_geniessp__1__0_models.ScgSearchResponse:
+        request: ali_geniessp__1__0_models.ReadMessageRequest,
+    ) -> ali_geniessp__1__0_models.ReadMessageResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ScgSearchHeaders()
-        return self.scg_search_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ReadMessageHeaders()
+        return self.read_message_with_options(request, headers, runtime)
 
-    async def scg_search_async(
+    async def read_message_async(
         self,
-        request: ali_geniessp__1__0_models.ScgSearchRequest,
-    ) -> ali_geniessp__1__0_models.ScgSearchResponse:
+        request: ali_geniessp__1__0_models.ReadMessageRequest,
+    ) -> ali_geniessp__1__0_models.ReadMessageResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.ScgSearchHeaders()
-        return await self.scg_search_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ReadMessageHeaders()
+        return await self.read_message_with_options_async(request, headers, runtime)
+
+    def scan_code_bind_with_options(
+        self,
+        tmp_req: ali_geniessp__1__0_models.ScanCodeBindRequest,
+        headers: ali_geniessp__1__0_models.ScanCodeBindHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.ScanCodeBindResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ali_geniessp__1__0_models.ScanCodeBindShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.bind_req):
+            request.bind_req_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.bind_req, 'BindReq', 'json')
+        if not UtilClient.is_unset(tmp_req.user_info):
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.bind_req_shrink):
+            body['BindReq'] = request.bind_req_shrink
+        if not UtilClient.is_unset(request.user_info_shrink):
+            body['UserInfo'] = request.user_info_shrink
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ScanCodeBind',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/scanCode',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.ScanCodeBindResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def scan_code_bind_with_options_async(
+        self,
+        tmp_req: ali_geniessp__1__0_models.ScanCodeBindRequest,
+        headers: ali_geniessp__1__0_models.ScanCodeBindHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.ScanCodeBindResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ali_geniessp__1__0_models.ScanCodeBindShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.bind_req):
+            request.bind_req_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.bind_req, 'BindReq', 'json')
+        if not UtilClient.is_unset(tmp_req.user_info):
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.bind_req_shrink):
+            body['BindReq'] = request.bind_req_shrink
+        if not UtilClient.is_unset(request.user_info_shrink):
+            body['UserInfo'] = request.user_info_shrink
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ScanCodeBind',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/scanCode',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.ScanCodeBindResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def scan_code_bind(
+        self,
+        request: ali_geniessp__1__0_models.ScanCodeBindRequest,
+    ) -> ali_geniessp__1__0_models.ScanCodeBindResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.ScanCodeBindHeaders()
+        return self.scan_code_bind_with_options(request, headers, runtime)
+
+    async def scan_code_bind_async(
+        self,
+        request: ali_geniessp__1__0_models.ScanCodeBindRequest,
+    ) -> ali_geniessp__1__0_models.ScanCodeBindResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.ScanCodeBindHeaders()
+        return await self.scan_code_bind_with_options_async(request, headers, runtime)
 
     def scg_search_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.ScgSearchRequest,
         headers: ali_geniessp__1__0_models.ScgSearchHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ScgSearchResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ScgSearchShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.scg_filter):
-            request.scg_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.scg_filter), 'ScgFilter', 'json')
+            request.scg_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.scg_filter, 'ScgFilter', 'json')
         query = {}
         if not UtilClient.is_unset(request.scg_filter_shrink):
             query['ScgFilter'] = request.scg_filter_shrink
         if not UtilClient.is_unset(request.topic_id):
             query['TopicId'] = request.topic_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -5690,15 +6674,15 @@
         headers: ali_geniessp__1__0_models.ScgSearchHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.ScgSearchResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.ScgSearchShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.scg_filter):
-            request.scg_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.scg_filter), 'ScgFilter', 'json')
+            request.scg_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.scg_filter, 'ScgFilter', 'json')
         query = {}
         if not UtilClient.is_unset(request.scg_filter_shrink):
             query['ScgFilter'] = request.scg_filter_shrink
         if not UtilClient.is_unset(request.topic_id):
             query['TopicId'] = request.topic_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -5723,45 +6707,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.ScgSearchResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def search_content(
+    def scg_search(
         self,
-        request: ali_geniessp__1__0_models.SearchContentRequest,
-    ) -> ali_geniessp__1__0_models.SearchContentResponse:
+        request: ali_geniessp__1__0_models.ScgSearchRequest,
+    ) -> ali_geniessp__1__0_models.ScgSearchResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.SearchContentHeaders()
-        return self.search_content_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ScgSearchHeaders()
+        return self.scg_search_with_options(request, headers, runtime)
 
-    async def search_content_async(
+    async def scg_search_async(
         self,
-        request: ali_geniessp__1__0_models.SearchContentRequest,
-    ) -> ali_geniessp__1__0_models.SearchContentResponse:
+        request: ali_geniessp__1__0_models.ScgSearchRequest,
+    ) -> ali_geniessp__1__0_models.ScgSearchResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.SearchContentHeaders()
-        return await self.search_content_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.ScgSearchHeaders()
+        return await self.scg_search_with_options_async(request, headers, runtime)
 
     def search_content_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.SearchContentRequest,
         headers: ali_geniessp__1__0_models.SearchContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.SearchContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.SearchContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -5800,19 +6784,19 @@
         headers: ali_geniessp__1__0_models.SearchContentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.SearchContentResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.SearchContentShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.request):
-            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.request), 'Request', 'json')
+            request.request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.request, 'Request', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         body = {}
         if not UtilClient.is_unset(request.request_shrink):
@@ -5841,41 +6825,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.SearchContentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def send_message(
+    def search_content(
         self,
-        request: ali_geniessp__1__0_models.SendMessageRequest,
-    ) -> ali_geniessp__1__0_models.SendMessageResponse:
+        request: ali_geniessp__1__0_models.SearchContentRequest,
+    ) -> ali_geniessp__1__0_models.SearchContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.SendMessageHeaders()
-        return self.send_message_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.SearchContentHeaders()
+        return self.search_content_with_options(request, headers, runtime)
 
-    async def send_message_async(
+    async def search_content_async(
         self,
-        request: ali_geniessp__1__0_models.SendMessageRequest,
-    ) -> ali_geniessp__1__0_models.SendMessageResponse:
+        request: ali_geniessp__1__0_models.SearchContentRequest,
+    ) -> ali_geniessp__1__0_models.SearchContentResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.SendMessageHeaders()
-        return await self.send_message_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.SearchContentHeaders()
+        return await self.search_content_with_options_async(request, headers, runtime)
 
     def send_message_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.SendMessageRequest,
         headers: ali_geniessp__1__0_models.SendMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.SendMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.SendMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -5910,15 +6894,15 @@
         headers: ali_geniessp__1__0_models.SendMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.SendMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.SendMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
         if not UtilClient.is_unset(request.user_info_shrink):
             query['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -5943,41 +6927,41 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.SendMessageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def set_device_setting(
+    def send_message(
         self,
-        request: ali_geniessp__1__0_models.SetDeviceSettingRequest,
-    ) -> ali_geniessp__1__0_models.SetDeviceSettingResponse:
+        request: ali_geniessp__1__0_models.SendMessageRequest,
+    ) -> ali_geniessp__1__0_models.SendMessageResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.SetDeviceSettingHeaders()
-        return self.set_device_setting_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.SendMessageHeaders()
+        return self.send_message_with_options(request, headers, runtime)
 
-    async def set_device_setting_async(
+    async def send_message_async(
         self,
-        request: ali_geniessp__1__0_models.SetDeviceSettingRequest,
-    ) -> ali_geniessp__1__0_models.SetDeviceSettingResponse:
+        request: ali_geniessp__1__0_models.SendMessageRequest,
+    ) -> ali_geniessp__1__0_models.SendMessageResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.SetDeviceSettingHeaders()
-        return await self.set_device_setting_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.SendMessageHeaders()
+        return await self.send_message_with_options_async(request, headers, runtime)
 
     def set_device_setting_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.SetDeviceSettingRequest,
         headers: ali_geniessp__1__0_models.SetDeviceSettingHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.SetDeviceSettingResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.SetDeviceSettingShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         body = {}
         if not UtilClient.is_unset(request.key):
             body['Key'] = request.key
         if not UtilClient.is_unset(request.value):
@@ -6016,15 +7000,15 @@
         headers: ali_geniessp__1__0_models.SetDeviceSettingHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.SetDeviceSettingResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.SetDeviceSettingShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             query['DeviceInfo'] = request.device_info_shrink
         body = {}
         if not UtilClient.is_unset(request.key):
             body['Key'] = request.key
         if not UtilClient.is_unset(request.value):
@@ -6053,43 +7037,133 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.SetDeviceSettingResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def unbind_device(
+    def set_device_setting(
         self,
-        request: ali_geniessp__1__0_models.UnbindDeviceRequest,
-    ) -> ali_geniessp__1__0_models.UnbindDeviceResponse:
+        request: ali_geniessp__1__0_models.SetDeviceSettingRequest,
+    ) -> ali_geniessp__1__0_models.SetDeviceSettingResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.UnbindDeviceHeaders()
-        return self.unbind_device_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.SetDeviceSettingHeaders()
+        return self.set_device_setting_with_options(request, headers, runtime)
 
-    async def unbind_device_async(
+    async def set_device_setting_async(
         self,
-        request: ali_geniessp__1__0_models.UnbindDeviceRequest,
-    ) -> ali_geniessp__1__0_models.UnbindDeviceResponse:
+        request: ali_geniessp__1__0_models.SetDeviceSettingRequest,
+    ) -> ali_geniessp__1__0_models.SetDeviceSettingResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.UnbindDeviceHeaders()
-        return await self.unbind_device_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.SetDeviceSettingHeaders()
+        return await self.set_device_setting_with_options_async(request, headers, runtime)
+
+    def unbind_aligenie_user_with_options(
+        self,
+        request: ali_geniessp__1__0_models.UnbindAligenieUserRequest,
+        headers: ali_geniessp__1__0_models.UnbindAligenieUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.UnbindAligenieUserResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.login_state_access_token):
+            body['LoginStateAccessToken'] = request.login_state_access_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UnbindAligenieUser',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/unbindAligenieUser',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.UnbindAligenieUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def unbind_aligenie_user_with_options_async(
+        self,
+        request: ali_geniessp__1__0_models.UnbindAligenieUserRequest,
+        headers: ali_geniessp__1__0_models.UnbindAligenieUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_geniessp__1__0_models.UnbindAligenieUserResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.login_state_access_token):
+            body['LoginStateAccessToken'] = request.login_state_access_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UnbindAligenieUser',
+            version='ssp_1.0',
+            protocol='HTTPS',
+            pathname=f'/v1.0/ssp/unbindAligenieUser',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_geniessp__1__0_models.UnbindAligenieUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def unbind_aligenie_user(
+        self,
+        request: ali_geniessp__1__0_models.UnbindAligenieUserRequest,
+    ) -> ali_geniessp__1__0_models.UnbindAligenieUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.UnbindAligenieUserHeaders()
+        return self.unbind_aligenie_user_with_options(request, headers, runtime)
+
+    async def unbind_aligenie_user_async(
+        self,
+        request: ali_geniessp__1__0_models.UnbindAligenieUserRequest,
+    ) -> ali_geniessp__1__0_models.UnbindAligenieUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.UnbindAligenieUserHeaders()
+        return await self.unbind_aligenie_user_with_options_async(request, headers, runtime)
 
     def unbind_device_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.UnbindDeviceRequest,
         headers: ali_geniessp__1__0_models.UnbindDeviceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.UnbindDeviceResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.UnbindDeviceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -6124,17 +7198,17 @@
         headers: ali_geniessp__1__0_models.UnbindDeviceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.UnbindDeviceResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.UnbindDeviceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
@@ -6159,45 +7233,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.UnbindDeviceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_alarm(
+    def unbind_device(
         self,
-        request: ali_geniessp__1__0_models.UpdateAlarmRequest,
-    ) -> ali_geniessp__1__0_models.UpdateAlarmResponse:
+        request: ali_geniessp__1__0_models.UnbindDeviceRequest,
+    ) -> ali_geniessp__1__0_models.UnbindDeviceResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.UpdateAlarmHeaders()
-        return self.update_alarm_with_options(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.UnbindDeviceHeaders()
+        return self.unbind_device_with_options(request, headers, runtime)
 
-    async def update_alarm_async(
+    async def unbind_device_async(
         self,
-        request: ali_geniessp__1__0_models.UpdateAlarmRequest,
-    ) -> ali_geniessp__1__0_models.UpdateAlarmResponse:
+        request: ali_geniessp__1__0_models.UnbindDeviceRequest,
+    ) -> ali_geniessp__1__0_models.UnbindDeviceResponse:
         runtime = util_models.RuntimeOptions()
-        headers = ali_geniessp__1__0_models.UpdateAlarmHeaders()
-        return await self.update_alarm_with_options_async(request, headers, runtime)
+        headers = ali_geniessp__1__0_models.UnbindDeviceHeaders()
+        return await self.unbind_device_with_options_async(request, headers, runtime)
 
     def update_alarm_with_options(
         self,
         tmp_req: ali_geniessp__1__0_models.UpdateAlarmRequest,
         headers: ali_geniessp__1__0_models.UpdateAlarmHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.UpdateAlarmResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.UpdateAlarmShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -6234,19 +7308,19 @@
         headers: ali_geniessp__1__0_models.UpdateAlarmHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_geniessp__1__0_models.UpdateAlarmResponse:
         UtilClient.validate_model(tmp_req)
         request = ali_geniessp__1__0_models.UpdateAlarmShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
-            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.device_info), 'DeviceInfo', 'json')
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
-            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.payload), 'Payload', 'json')
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
-            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user_info), 'UserInfo', 'json')
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.device_info_shrink):
             body['DeviceInfo'] = request.device_info_shrink
         if not UtilClient.is_unset(request.payload_shrink):
             body['Payload'] = request.payload_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
@@ -6272,7 +7346,23 @@
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             ali_geniessp__1__0_models.UpdateAlarmResponse(),
             await self.call_api_async(params, req, runtime)
         )
+
+    def update_alarm(
+        self,
+        request: ali_geniessp__1__0_models.UpdateAlarmRequest,
+    ) -> ali_geniessp__1__0_models.UpdateAlarmResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.UpdateAlarmHeaders()
+        return self.update_alarm_with_options(request, headers, runtime)
+
+    async def update_alarm_async(
+        self,
+        request: ali_geniessp__1__0_models.UpdateAlarmRequest,
+    ) -> ali_geniessp__1__0_models.UpdateAlarmResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_geniessp__1__0_models.UpdateAlarmHeaders()
+        return await self.update_alarm_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0/models.py` & `alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,154 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, Any, List
+from typing import List, Dict, Any
+
+
+class LoginStateInfo(TeaModel):
+    def __init__(
+        self,
+        scene_code: str = None,
+        third_user_identifier: str = None,
+        third_user_type: str = None,
+        user_id: str = None,
+    ):
+        self.scene_code = scene_code
+        self.third_user_identifier = third_user_identifier
+        self.third_user_type = third_user_type
+        self.user_id = user_id
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
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.third_user_identifier is not None:
+            result['ThirdUserIdentifier'] = self.third_user_identifier
+        if self.third_user_type is not None:
+            result['ThirdUserType'] = self.third_user_type
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('ThirdUserIdentifier') is not None:
+            self.third_user_identifier = m.get('ThirdUserIdentifier')
+        if m.get('ThirdUserType') is not None:
+            self.third_user_type = m.get('ThirdUserType')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class ResultValueDeviceUnionIds(TeaModel):
+    def __init__(
+        self,
+        organization_id: str = None,
+        device_union_id: str = None,
+    ):
+        self.organization_id = organization_id
+        self.device_union_id = device_union_id
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
+        if self.organization_id is not None:
+            result['OrganizationId'] = self.organization_id
+        if self.device_union_id is not None:
+            result['DeviceUnionId'] = self.device_union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrganizationId') is not None:
+            self.organization_id = m.get('OrganizationId')
+        if m.get('DeviceUnionId') is not None:
+            self.device_union_id = m.get('DeviceUnionId')
+        return self
+
+
+class ResultValue(TeaModel):
+    def __init__(
+        self,
+        device_open_id: str = None,
+        device_union_ids: List[ResultValueDeviceUnionIds] = None,
+        name: str = None,
+        firmware_version: str = None,
+        mac: str = None,
+        sn: str = None,
+    ):
+        self.device_open_id = device_open_id
+        self.device_union_ids = device_union_ids
+        self.name = name
+        self.firmware_version = firmware_version
+        self.mac = mac
+        self.sn = sn
+
+    def validate(self):
+        if self.device_union_ids:
+            for k in self.device_union_ids:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_open_id is not None:
+            result['DeviceOpenId'] = self.device_open_id
+        result['DeviceUnionIds'] = []
+        if self.device_union_ids is not None:
+            for k in self.device_union_ids:
+                result['DeviceUnionIds'].append(k.to_map() if k else None)
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.firmware_version is not None:
+            result['FirmwareVersion'] = self.firmware_version
+        if self.mac is not None:
+            result['Mac'] = self.mac
+        if self.sn is not None:
+            result['Sn'] = self.sn
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DeviceOpenId') is not None:
+            self.device_open_id = m.get('DeviceOpenId')
+        self.device_union_ids = []
+        if m.get('DeviceUnionIds') is not None:
+            for k in m.get('DeviceUnionIds'):
+                temp_model = ResultValueDeviceUnionIds()
+                self.device_union_ids.append(temp_model.from_map(k))
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('FirmwareVersion') is not None:
+            self.firmware_version = m.get('FirmwareVersion')
+        if m.get('Mac') is not None:
+            self.mac = m.get('Mac')
+        if m.get('Sn') is not None:
+            self.sn = m.get('Sn')
+        return self
 
 
 class AddAndRemoveFavoriteContentHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
@@ -910,14 +1053,1447 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddSubResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AuthLoginWithAligenieUserInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoRequest(TeaModel):
+    def __init__(
+        self,
+        encrypted_aligenie_user_identifier: str = None,
+        session_id: str = None,
+    ):
+        self.encrypted_aligenie_user_identifier = encrypted_aligenie_user_identifier
+        self.session_id = session_id
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
+        if self.encrypted_aligenie_user_identifier is not None:
+            result['EncryptedAligenieUserIdentifier'] = self.encrypted_aligenie_user_identifier
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncryptedAligenieUserIdentifier') is not None:
+            self.encrypted_aligenie_user_identifier = m.get('EncryptedAligenieUserIdentifier')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        expired_time_long: int = None,
+        login_state_access_token: str = None,
+    ):
+        self.expired_time_long = expired_time_long
+        self.login_state_access_token = login_state_access_token
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
+        if self.expired_time_long is not None:
+            result['ExpiredTimeLong'] = self.expired_time_long
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpiredTimeLong') is not None:
+            self.expired_time_long = m.get('ExpiredTimeLong')
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: AuthLoginWithAligenieUserInfoResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = AuthLoginWithAligenieUserInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AuthLoginWithAligenieUserInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AuthLoginWithAligenieUserInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberRequest(TeaModel):
+    def __init__(
+        self,
+        session_id: str = None,
+    ):
+        self.session_id = session_id
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
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        expired_time_long: int = None,
+        login_state_access_token: str = None,
+    ):
+        self.expired_time_long = expired_time_long
+        self.login_state_access_token = login_state_access_token
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
+        if self.expired_time_long is not None:
+            result['ExpiredTimeLong'] = self.expired_time_long
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpiredTimeLong') is not None:
+            self.expired_time_long = m.get('ExpiredTimeLong')
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AuthLoginWithAligenieUserInfoGeneratedByPhoneNumberResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AuthLoginWithTaobaoUserInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class AuthLoginWithTaobaoUserInfoRequest(TeaModel):
+    def __init__(
+        self,
+        encrypted_taobao_user_identifier: str = None,
+        session_id: str = None,
+    ):
+        self.encrypted_taobao_user_identifier = encrypted_taobao_user_identifier
+        self.session_id = session_id
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
+        if self.encrypted_taobao_user_identifier is not None:
+            result['EncryptedTaobaoUserIdentifier'] = self.encrypted_taobao_user_identifier
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncryptedTaobaoUserIdentifier') is not None:
+            self.encrypted_taobao_user_identifier = m.get('EncryptedTaobaoUserIdentifier')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class AuthLoginWithTaobaoUserInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        expired_time_long: int = None,
+        login_state_access_token: str = None,
+    ):
+        self.expired_time_long = expired_time_long
+        self.login_state_access_token = login_state_access_token
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
+        if self.expired_time_long is not None:
+            result['ExpiredTimeLong'] = self.expired_time_long
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpiredTimeLong') is not None:
+            self.expired_time_long = m.get('ExpiredTimeLong')
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class AuthLoginWithTaobaoUserInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: AuthLoginWithTaobaoUserInfoResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = AuthLoginWithTaobaoUserInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AuthLoginWithTaobaoUserInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AuthLoginWithTaobaoUserInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AuthLoginWithTaobaoUserInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AuthLoginWithThirdUserInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class AuthLoginWithThirdUserInfoRequest(TeaModel):
+    def __init__(
+        self,
+        ext_info: Dict[str, Any] = None,
+        scene_code: str = None,
+        third_user_identifier: str = None,
+        third_user_type: str = None,
+    ):
+        self.ext_info = ext_info
+        self.scene_code = scene_code
+        self.third_user_identifier = third_user_identifier
+        self.third_user_type = third_user_type
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
+        if self.ext_info is not None:
+            result['ExtInfo'] = self.ext_info
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.third_user_identifier is not None:
+            result['ThirdUserIdentifier'] = self.third_user_identifier
+        if self.third_user_type is not None:
+            result['ThirdUserType'] = self.third_user_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExtInfo') is not None:
+            self.ext_info = m.get('ExtInfo')
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('ThirdUserIdentifier') is not None:
+            self.third_user_identifier = m.get('ThirdUserIdentifier')
+        if m.get('ThirdUserType') is not None:
+            self.third_user_type = m.get('ThirdUserType')
+        return self
+
+
+class AuthLoginWithThirdUserInfoShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        ext_info_shrink: str = None,
+        scene_code: str = None,
+        third_user_identifier: str = None,
+        third_user_type: str = None,
+    ):
+        self.ext_info_shrink = ext_info_shrink
+        self.scene_code = scene_code
+        self.third_user_identifier = third_user_identifier
+        self.third_user_type = third_user_type
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
+        if self.ext_info_shrink is not None:
+            result['ExtInfo'] = self.ext_info_shrink
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.third_user_identifier is not None:
+            result['ThirdUserIdentifier'] = self.third_user_identifier
+        if self.third_user_type is not None:
+            result['ThirdUserType'] = self.third_user_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExtInfo') is not None:
+            self.ext_info_shrink = m.get('ExtInfo')
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('ThirdUserIdentifier') is not None:
+            self.third_user_identifier = m.get('ThirdUserIdentifier')
+        if m.get('ThirdUserType') is not None:
+            self.third_user_type = m.get('ThirdUserType')
+        return self
+
+
+class AuthLoginWithThirdUserInfoResponseBodyDataObj(TeaModel):
+    def __init__(
+        self,
+        session_id: str = None,
+    ):
+        self.session_id = session_id
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
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class AuthLoginWithThirdUserInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        expired_time_long: int = None,
+        login_state_access_token: str = None,
+    ):
+        self.expired_time_long = expired_time_long
+        self.login_state_access_token = login_state_access_token
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
+        if self.expired_time_long is not None:
+            result['ExpiredTimeLong'] = self.expired_time_long
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpiredTimeLong') is not None:
+            self.expired_time_long = m.get('ExpiredTimeLong')
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class AuthLoginWithThirdUserInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data_obj: AuthLoginWithThirdUserInfoResponseBodyDataObj = None,
+        message: str = None,
+        request_id: str = None,
+        result: AuthLoginWithThirdUserInfoResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data_obj = data_obj
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.data_obj:
+            self.data_obj.validate()
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data_obj is not None:
+            result['DataObj'] = self.data_obj.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DataObj') is not None:
+            temp_model = AuthLoginWithThirdUserInfoResponseBodyDataObj()
+            self.data_obj = temp_model.from_map(m['DataObj'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = AuthLoginWithThirdUserInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AuthLoginWithThirdUserInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AuthLoginWithThirdUserInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AuthLoginWithThirdUserInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CheckAndDoVoipCallForHotelHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class CheckAndDoVoipCallForHotelRequestDeviceInfo(TeaModel):
+    def __init__(
+        self,
+        encode_key: str = None,
+        encode_type: str = None,
+        id: str = None,
+        id_type: str = None,
+        organization_id: str = None,
+    ):
+        self.encode_key = encode_key
+        self.encode_type = encode_type
+        self.id = id
+        self.id_type = id_type
+        self.organization_id = organization_id
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
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.id_type is not None:
+            result['IdType'] = self.id_type
+        if self.organization_id is not None:
+            result['OrganizationId'] = self.organization_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdType') is not None:
+            self.id_type = m.get('IdType')
+        if m.get('OrganizationId') is not None:
+            self.organization_id = m.get('OrganizationId')
+        return self
+
+
+class CheckAndDoVoipCallForHotelRequestUserInfo(TeaModel):
+    def __init__(
+        self,
+        encode_key: str = None,
+        encode_type: str = None,
+        id: str = None,
+        id_type: str = None,
+        organization_id: str = None,
+    ):
+        self.encode_key = encode_key
+        self.encode_type = encode_type
+        self.id = id
+        self.id_type = id_type
+        self.organization_id = organization_id
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
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.id_type is not None:
+            result['IdType'] = self.id_type
+        if self.organization_id is not None:
+            result['OrganizationId'] = self.organization_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdType') is not None:
+            self.id_type = m.get('IdType')
+        if m.get('OrganizationId') is not None:
+            self.organization_id = m.get('OrganizationId')
+        return self
+
+
+class CheckAndDoVoipCallForHotelRequest(TeaModel):
+    def __init__(
+        self,
+        biz_data: str = None,
+        callee_nick: str = None,
+        callee_phone_num: str = None,
+        device_info: CheckAndDoVoipCallForHotelRequestDeviceInfo = None,
+        user_info: CheckAndDoVoipCallForHotelRequestUserInfo = None,
+    ):
+        self.biz_data = biz_data
+        self.callee_nick = callee_nick
+        self.callee_phone_num = callee_phone_num
+        self.device_info = device_info
+        self.user_info = user_info
+
+    def validate(self):
+        if self.device_info:
+            self.device_info.validate()
+        if self.user_info:
+            self.user_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_data is not None:
+            result['BizData'] = self.biz_data
+        if self.callee_nick is not None:
+            result['CalleeNick'] = self.callee_nick
+        if self.callee_phone_num is not None:
+            result['CalleePhoneNum'] = self.callee_phone_num
+        if self.device_info is not None:
+            result['DeviceInfo'] = self.device_info.to_map()
+        if self.user_info is not None:
+            result['UserInfo'] = self.user_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizData') is not None:
+            self.biz_data = m.get('BizData')
+        if m.get('CalleeNick') is not None:
+            self.callee_nick = m.get('CalleeNick')
+        if m.get('CalleePhoneNum') is not None:
+            self.callee_phone_num = m.get('CalleePhoneNum')
+        if m.get('DeviceInfo') is not None:
+            temp_model = CheckAndDoVoipCallForHotelRequestDeviceInfo()
+            self.device_info = temp_model.from_map(m['DeviceInfo'])
+        if m.get('UserInfo') is not None:
+            temp_model = CheckAndDoVoipCallForHotelRequestUserInfo()
+            self.user_info = temp_model.from_map(m['UserInfo'])
+        return self
+
+
+class CheckAndDoVoipCallForHotelShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        biz_data: str = None,
+        callee_nick: str = None,
+        callee_phone_num: str = None,
+        device_info_shrink: str = None,
+        user_info_shrink: str = None,
+    ):
+        self.biz_data = biz_data
+        self.callee_nick = callee_nick
+        self.callee_phone_num = callee_phone_num
+        self.device_info_shrink = device_info_shrink
+        self.user_info_shrink = user_info_shrink
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
+        if self.biz_data is not None:
+            result['BizData'] = self.biz_data
+        if self.callee_nick is not None:
+            result['CalleeNick'] = self.callee_nick
+        if self.callee_phone_num is not None:
+            result['CalleePhoneNum'] = self.callee_phone_num
+        if self.device_info_shrink is not None:
+            result['DeviceInfo'] = self.device_info_shrink
+        if self.user_info_shrink is not None:
+            result['UserInfo'] = self.user_info_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizData') is not None:
+            self.biz_data = m.get('BizData')
+        if m.get('CalleeNick') is not None:
+            self.callee_nick = m.get('CalleeNick')
+        if m.get('CalleePhoneNum') is not None:
+            self.callee_phone_num = m.get('CalleePhoneNum')
+        if m.get('DeviceInfo') is not None:
+            self.device_info_shrink = m.get('DeviceInfo')
+        if m.get('UserInfo') is not None:
+            self.user_info_shrink = m.get('UserInfo')
+        return self
+
+
+class CheckAndDoVoipCallForHotelResponseBodyResultDeviceTargetsData(TeaModel):
+    def __init__(
+        self,
+        device_icon: str = None,
+        device_name: str = None,
+        device_type: str = None,
+        online: bool = None,
+        uuid: str = None,
+    ):
+        self.device_icon = device_icon
+        self.device_name = device_name
+        self.device_type = device_type
+        self.online = online
+        self.uuid = uuid
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
+        if self.device_icon is not None:
+            result['DeviceIcon'] = self.device_icon
+        if self.device_name is not None:
+            result['DeviceName'] = self.device_name
+        if self.device_type is not None:
+            result['DeviceType'] = self.device_type
+        if self.online is not None:
+            result['Online'] = self.online
+        if self.uuid is not None:
+            result['Uuid'] = self.uuid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DeviceIcon') is not None:
+            self.device_icon = m.get('DeviceIcon')
+        if m.get('DeviceName') is not None:
+            self.device_name = m.get('DeviceName')
+        if m.get('DeviceType') is not None:
+            self.device_type = m.get('DeviceType')
+        if m.get('Online') is not None:
+            self.online = m.get('Online')
+        if m.get('Uuid') is not None:
+            self.uuid = m.get('Uuid')
+        return self
+
+
+class CheckAndDoVoipCallForHotelResponseBodyResultDeviceTargets(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: List[CheckAndDoVoipCallForHotelResponseBodyResultDeviceTargetsData] = None,
+        msg: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.msg = msg
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.msg is not None:
+            result['Msg'] = self.msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = CheckAndDoVoipCallForHotelResponseBodyResultDeviceTargetsData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Msg') is not None:
+            self.msg = m.get('Msg')
+        return self
+
+
+class CheckAndDoVoipCallForHotelResponseBodyResultStartCallResult(TeaModel):
+    def __init__(
+        self,
+        message: str = None,
+        ret_code: int = None,
+        ret_value: str = None,
+        success: bool = None,
+        trace_id: str = None,
+    ):
+        self.message = message
+        self.ret_code = ret_code
+        self.ret_value = ret_value
+        self.success = success
+        self.trace_id = trace_id
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
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.ret_code is not None:
+            result['RetCode'] = self.ret_code
+        if self.ret_value is not None:
+            result['RetValue'] = self.ret_value
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.trace_id is not None:
+            result['TraceId'] = self.trace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RetCode') is not None:
+            self.ret_code = m.get('RetCode')
+        if m.get('RetValue') is not None:
+            self.ret_value = m.get('RetValue')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TraceId') is not None:
+            self.trace_id = m.get('TraceId')
+        return self
+
+
+class CheckAndDoVoipCallForHotelResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        device_targets: CheckAndDoVoipCallForHotelResponseBodyResultDeviceTargets = None,
+        is_start_call: bool = None,
+        passed: bool = None,
+        start_call_result: CheckAndDoVoipCallForHotelResponseBodyResultStartCallResult = None,
+    ):
+        self.device_targets = device_targets
+        self.is_start_call = is_start_call
+        self.passed = passed
+        self.start_call_result = start_call_result
+
+    def validate(self):
+        if self.device_targets:
+            self.device_targets.validate()
+        if self.start_call_result:
+            self.start_call_result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_targets is not None:
+            result['DeviceTargets'] = self.device_targets.to_map()
+        if self.is_start_call is not None:
+            result['IsStartCall'] = self.is_start_call
+        if self.passed is not None:
+            result['Passed'] = self.passed
+        if self.start_call_result is not None:
+            result['StartCallResult'] = self.start_call_result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DeviceTargets') is not None:
+            temp_model = CheckAndDoVoipCallForHotelResponseBodyResultDeviceTargets()
+            self.device_targets = temp_model.from_map(m['DeviceTargets'])
+        if m.get('IsStartCall') is not None:
+            self.is_start_call = m.get('IsStartCall')
+        if m.get('Passed') is not None:
+            self.passed = m.get('Passed')
+        if m.get('StartCallResult') is not None:
+            temp_model = CheckAndDoVoipCallForHotelResponseBodyResultStartCallResult()
+            self.start_call_result = temp_model.from_map(m['StartCallResult'])
+        return self
+
+
+class CheckAndDoVoipCallForHotelResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: CheckAndDoVoipCallForHotelResponseBodyResult = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = CheckAndDoVoipCallForHotelResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        return self
+
+
+class CheckAndDoVoipCallForHotelResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CheckAndDoVoipCallForHotelResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CheckAndDoVoipCallForHotelResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CheckAuthCodeBindForExtHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
         authorization: str = None,
     ):
@@ -1099,14 +2675,15 @@
 class CheckAuthCodeBindForExtResponseBodyResultDeviceOpenInfo(TeaModel):
     def __init__(
         self,
         id: str = None,
         id_type: str = None,
     ):
         self.id = id
+        # DEVICE_ID
         self.id_type = id_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1132,14 +2709,15 @@
 class CheckAuthCodeBindForExtResponseBodyResultUserOpenInfo(TeaModel):
     def __init__(
         self,
         id: str = None,
         id_type: str = None,
     ):
         self.id = id
+        # USER_ID
         self.id_type = id_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4195,14 +5773,757 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeviceControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class EcologyOpennessAuthenticateHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class EcologyOpennessAuthenticateRequest(TeaModel):
+    def __init__(
+        self,
+        encode_key: str = None,
+        encode_type: str = None,
+        login_state_access_token: str = None,
+    ):
+        self.encode_key = encode_key
+        self.encode_type = encode_type
+        self.login_state_access_token = login_state_access_token
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
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class EcologyOpennessAuthenticateResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        encode_key: str = None,
+        encode_type: str = None,
+        scene_code: str = None,
+        third_user_identifier: str = None,
+        third_user_type: str = None,
+        user_open_id: str = None,
+    ):
+        self.encode_key = encode_key
+        self.encode_type = encode_type
+        self.scene_code = scene_code
+        self.third_user_identifier = third_user_identifier
+        self.third_user_type = third_user_type
+        self.user_open_id = user_open_id
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
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.third_user_identifier is not None:
+            result['ThirdUserIdentifier'] = self.third_user_identifier
+        if self.third_user_type is not None:
+            result['ThirdUserType'] = self.third_user_type
+        if self.user_open_id is not None:
+            result['UserOpenId'] = self.user_open_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('ThirdUserIdentifier') is not None:
+            self.third_user_identifier = m.get('ThirdUserIdentifier')
+        if m.get('ThirdUserType') is not None:
+            self.third_user_type = m.get('ThirdUserType')
+        if m.get('UserOpenId') is not None:
+            self.user_open_id = m.get('UserOpenId')
+        return self
+
+
+class EcologyOpennessAuthenticateResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: EcologyOpennessAuthenticateResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = EcologyOpennessAuthenticateResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class EcologyOpennessAuthenticateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: EcologyOpennessAuthenticateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = EcologyOpennessAuthenticateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class EcologyOpennessSendVerificationCodeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class EcologyOpennessSendVerificationCodeRequest(TeaModel):
+    def __init__(
+        self,
+        phone_number: str = None,
+        region: str = None,
+        session_id: str = None,
+    ):
+        self.phone_number = phone_number
+        self.region = region
+        self.session_id = session_id
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
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class EcologyOpennessSendVerificationCodeResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        expire_in: int = None,
+        repeat_interval: int = None,
+    ):
+        self.expire_in = expire_in
+        self.repeat_interval = repeat_interval
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
+        if self.expire_in is not None:
+            result['ExpireIn'] = self.expire_in
+        if self.repeat_interval is not None:
+            result['RepeatInterval'] = self.repeat_interval
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpireIn') is not None:
+            self.expire_in = m.get('ExpireIn')
+        if m.get('RepeatInterval') is not None:
+            self.repeat_interval = m.get('RepeatInterval')
+        return self
+
+
+class EcologyOpennessSendVerificationCodeResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: EcologyOpennessSendVerificationCodeResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = EcologyOpennessSendVerificationCodeResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class EcologyOpennessSendVerificationCodeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: EcologyOpennessSendVerificationCodeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = EcologyOpennessSendVerificationCodeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberRequest(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        phone_number: str = None,
+        region: str = None,
+        session_id: str = None,
+    ):
+        self.code = code
+        self.phone_number = phone_number
+        self.region = region
+        self.session_id = session_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberResponseBodyDataObj(TeaModel):
+    def __init__(
+        self,
+        session_id: str = None,
+    ):
+        self.session_id = session_id
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
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberResponseBodyResultUserListToAuthLogin(TeaModel):
+    def __init__(
+        self,
+        avatar: str = None,
+        encrypted_user_identifier: str = None,
+        finding_type: str = None,
+        nickname: str = None,
+        user_type: str = None,
+    ):
+        self.avatar = avatar
+        self.encrypted_user_identifier = encrypted_user_identifier
+        self.finding_type = finding_type
+        self.nickname = nickname
+        self.user_type = user_type
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
+        if self.avatar is not None:
+            result['Avatar'] = self.avatar
+        if self.encrypted_user_identifier is not None:
+            result['EncryptedUserIdentifier'] = self.encrypted_user_identifier
+        if self.finding_type is not None:
+            result['FindingType'] = self.finding_type
+        if self.nickname is not None:
+            result['Nickname'] = self.nickname
+        if self.user_type is not None:
+            result['UserType'] = self.user_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Avatar') is not None:
+            self.avatar = m.get('Avatar')
+        if m.get('EncryptedUserIdentifier') is not None:
+            self.encrypted_user_identifier = m.get('EncryptedUserIdentifier')
+        if m.get('FindingType') is not None:
+            self.finding_type = m.get('FindingType')
+        if m.get('Nickname') is not None:
+            self.nickname = m.get('Nickname')
+        if m.get('UserType') is not None:
+            self.user_type = m.get('UserType')
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        user_list_to_auth_login: List[FindUserlistToAuthLoginWithPhoneNumberResponseBodyResultUserListToAuthLogin] = None,
+    ):
+        self.user_list_to_auth_login = user_list_to_auth_login
+
+    def validate(self):
+        if self.user_list_to_auth_login:
+            for k in self.user_list_to_auth_login:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['UserListToAuthLogin'] = []
+        if self.user_list_to_auth_login is not None:
+            for k in self.user_list_to_auth_login:
+                result['UserListToAuthLogin'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.user_list_to_auth_login = []
+        if m.get('UserListToAuthLogin') is not None:
+            for k in m.get('UserListToAuthLogin'):
+                temp_model = FindUserlistToAuthLoginWithPhoneNumberResponseBodyResultUserListToAuthLogin()
+                self.user_list_to_auth_login.append(temp_model.from_map(k))
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data_obj: FindUserlistToAuthLoginWithPhoneNumberResponseBodyDataObj = None,
+        message: str = None,
+        request_id: str = None,
+        result: FindUserlistToAuthLoginWithPhoneNumberResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data_obj = data_obj
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.data_obj:
+            self.data_obj.validate()
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data_obj is not None:
+            result['DataObj'] = self.data_obj.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DataObj') is not None:
+            temp_model = FindUserlistToAuthLoginWithPhoneNumberResponseBodyDataObj()
+            self.data_obj = temp_model.from_map(m['DataObj'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = FindUserlistToAuthLoginWithPhoneNumberResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class FindUserlistToAuthLoginWithPhoneNumberResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: FindUserlistToAuthLoginWithPhoneNumberResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = FindUserlistToAuthLoginWithPhoneNumberResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAlarmHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
         authorization: str = None,
     ):
@@ -4686,27 +7007,23 @@
         alarm_id: int = None,
         music_info: GetAlarmResponseBodyResultMusicInfo = None,
         schedule_info: GetAlarmResponseBodyResultScheduleInfo = None,
         schedule_type_desc: str = None,
         status: int = None,
         trigger_date_desc: str = None,
         trigger_time_desc: str = None,
-        user_id: int = None,
-        uuid: str = None,
         volume: int = None,
     ):
         self.alarm_id = alarm_id
         self.music_info = music_info
         self.schedule_info = schedule_info
         self.schedule_type_desc = schedule_type_desc
         self.status = status
         self.trigger_date_desc = trigger_date_desc
         self.trigger_time_desc = trigger_time_desc
-        self.user_id = user_id
-        self.uuid = uuid
         self.volume = volume
 
     def validate(self):
         if self.music_info:
             self.music_info.validate()
         if self.schedule_info:
             self.schedule_info.validate()
@@ -4727,18 +7044,14 @@
             result['ScheduleTypeDesc'] = self.schedule_type_desc
         if self.status is not None:
             result['Status'] = self.status
         if self.trigger_date_desc is not None:
             result['TriggerDateDesc'] = self.trigger_date_desc
         if self.trigger_time_desc is not None:
             result['TriggerTimeDesc'] = self.trigger_time_desc
-        if self.user_id is not None:
-            result['UserId'] = self.user_id
-        if self.uuid is not None:
-            result['Uuid'] = self.uuid
         if self.volume is not None:
             result['Volume'] = self.volume
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlarmId') is not None:
@@ -4753,18 +7066,14 @@
             self.schedule_type_desc = m.get('ScheduleTypeDesc')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TriggerDateDesc') is not None:
             self.trigger_date_desc = m.get('TriggerDateDesc')
         if m.get('TriggerTimeDesc') is not None:
             self.trigger_time_desc = m.get('TriggerTimeDesc')
-        if m.get('UserId') is not None:
-            self.user_id = m.get('UserId')
-        if m.get('Uuid') is not None:
-            self.uuid = m.get('Uuid')
         if m.get('Volume') is not None:
             self.volume = m.get('Volume')
         return self
 
 
 class GetAlarmResponseBody(TeaModel):
     def __init__(
@@ -5519,14 +7828,216 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetAlbumDetailByIdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetAligenieUserInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class GetAligenieUserInfoRequest(TeaModel):
+    def __init__(
+        self,
+        login_state_access_token: str = None,
+    ):
+        self.login_state_access_token = login_state_access_token
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
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class GetAligenieUserInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        aligenie_nickname: str = None,
+        avatar: str = None,
+        deletable: bool = None,
+    ):
+        self.aligenie_nickname = aligenie_nickname
+        self.avatar = avatar
+        self.deletable = deletable
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
+        if self.aligenie_nickname is not None:
+            result['AligenieNickname'] = self.aligenie_nickname
+        if self.avatar is not None:
+            result['Avatar'] = self.avatar
+        if self.deletable is not None:
+            result['Deletable'] = self.deletable
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AligenieNickname') is not None:
+            self.aligenie_nickname = m.get('AligenieNickname')
+        if m.get('Avatar') is not None:
+            self.avatar = m.get('Avatar')
+        if m.get('Deletable') is not None:
+            self.deletable = m.get('Deletable')
+        return self
+
+
+class GetAligenieUserInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: GetAligenieUserInfoResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = GetAligenieUserInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAligenieUserInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetAligenieUserInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetAligenieUserInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetCodeEnhanceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
         authorization: str = None,
     ):
@@ -5999,14 +8510,15 @@
         cover: GetContentResponseBodyResultCover = None,
         description: str = None,
         duration: int = None,
         hot_score: float = None,
         id: int = None,
         item_type: str = None,
         lyric: str = None,
+        raw_id: str = None,
         source: str = None,
         styles: List[str] = None,
         title: str = None,
         type: str = None,
         valid: str = None,
     ):
         self.album_id = album_id
@@ -6019,14 +8531,15 @@
         self.cover = cover
         self.description = description
         self.duration = duration
         self.hot_score = hot_score
         self.id = id
         self.item_type = item_type
         self.lyric = lyric
+        self.raw_id = raw_id
         self.source = source
         self.styles = styles
         self.title = title
         self.type = type
         self.valid = valid
 
     def validate(self):
@@ -6069,14 +8582,16 @@
             result['HotScore'] = self.hot_score
         if self.id is not None:
             result['Id'] = self.id
         if self.item_type is not None:
             result['ItemType'] = self.item_type
         if self.lyric is not None:
             result['Lyric'] = self.lyric
+        if self.raw_id is not None:
+            result['RawId'] = self.raw_id
         if self.source is not None:
             result['Source'] = self.source
         if self.styles is not None:
             result['Styles'] = self.styles
         if self.title is not None:
             result['Title'] = self.title
         if self.type is not None:
@@ -6115,14 +8630,16 @@
             self.hot_score = m.get('HotScore')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('ItemType') is not None:
             self.item_type = m.get('ItemType')
         if m.get('Lyric') is not None:
             self.lyric = m.get('Lyric')
+        if m.get('RawId') is not None:
+            self.raw_id = m.get('RawId')
         if m.get('Source') is not None:
             self.source = m.get('Source')
         if m.get('Styles') is not None:
             self.styles = m.get('Styles')
         if m.get('Title') is not None:
             self.title = m.get('Title')
         if m.get('Type') is not None:
@@ -10435,14 +12952,15 @@
     def __init__(
         self,
         code: int = None,
         message: str = None,
         request_id: str = None,
         result: GetWeatherResponseBodyResult = None,
     ):
+        # HttpCode
         self.code = code
         self.message = message
         self.request_id = request_id
         self.result = result
 
     def validate(self):
         if self.result:
@@ -11566,27 +14084,23 @@
         alarm_id: int = None,
         music_info: ListAlarmsResponseBodyResultModelMusicInfo = None,
         schedule_info: ListAlarmsResponseBodyResultModelScheduleInfo = None,
         schedule_type_desc: str = None,
         status: int = None,
         trigger_date_desc: str = None,
         trigger_time_desc: str = None,
-        user_id: int = None,
-        uuid: str = None,
         volume: int = None,
     ):
         self.alarm_id = alarm_id
         self.music_info = music_info
         self.schedule_info = schedule_info
         self.schedule_type_desc = schedule_type_desc
         self.status = status
         self.trigger_date_desc = trigger_date_desc
         self.trigger_time_desc = trigger_time_desc
-        self.user_id = user_id
-        self.uuid = uuid
         self.volume = volume
 
     def validate(self):
         if self.music_info:
             self.music_info.validate()
         if self.schedule_info:
             self.schedule_info.validate()
@@ -11607,18 +14121,14 @@
             result['ScheduleTypeDesc'] = self.schedule_type_desc
         if self.status is not None:
             result['Status'] = self.status
         if self.trigger_date_desc is not None:
             result['TriggerDateDesc'] = self.trigger_date_desc
         if self.trigger_time_desc is not None:
             result['TriggerTimeDesc'] = self.trigger_time_desc
-        if self.user_id is not None:
-            result['UserId'] = self.user_id
-        if self.uuid is not None:
-            result['Uuid'] = self.uuid
         if self.volume is not None:
             result['Volume'] = self.volume
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlarmId') is not None:
@@ -11633,18 +14143,14 @@
             self.schedule_type_desc = m.get('ScheduleTypeDesc')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TriggerDateDesc') is not None:
             self.trigger_date_desc = m.get('TriggerDateDesc')
         if m.get('TriggerTimeDesc') is not None:
             self.trigger_time_desc = m.get('TriggerTimeDesc')
-        if m.get('UserId') is not None:
-            self.user_id = m.get('UserId')
-        if m.get('Uuid') is not None:
-            self.uuid = m.get('Uuid')
         if m.get('Volume') is not None:
             self.volume = m.get('Volume')
         return self
 
 
 class ListAlarmsResponseBodyResult(TeaModel):
     def __init__(
@@ -12187,14 +14693,15 @@
         code: int = None,
         message: str = None,
         request_id: str = None,
         result: ListAlbumDetailResponseBodyResult = None,
     ):
         self.code = code
         self.message = message
+        # Id of the request
         self.request_id = request_id
         self.result = result
 
     def validate(self):
         if self.result:
             self.result.validate()
 
@@ -13288,14 +15795,15 @@
         code: int = None,
         message: str = None,
         request_id: str = None,
         result: ListCateContentResponseBodyResult = None,
     ):
         self.code = code
         self.message = message
+        # Id of the request
         self.request_id = request_id
         self.result = result
 
     def validate(self):
         if self.result:
             self.result.validate()
 
@@ -14121,112 +16629,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DeviceInfos') is not None:
             self.device_infos_shrink = m.get('DeviceInfos')
         return self
 
 
-class ResultValueDeviceUnionIds(TeaModel):
-    def __init__(
-        self,
-        organization_id: str = None,
-        device_union_id: str = None,
-    ):
-        self.organization_id = organization_id
-        self.device_union_id = device_union_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.organization_id is not None:
-            result['OrganizationId'] = self.organization_id
-        if self.device_union_id is not None:
-            result['DeviceUnionId'] = self.device_union_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('OrganizationId') is not None:
-            self.organization_id = m.get('OrganizationId')
-        if m.get('DeviceUnionId') is not None:
-            self.device_union_id = m.get('DeviceUnionId')
-        return self
-
-
-class ResultValue(TeaModel):
-    def __init__(
-        self,
-        device_open_id: str = None,
-        device_union_ids: List[ResultValueDeviceUnionIds] = None,
-        name: str = None,
-        firmware_version: str = None,
-        mac: str = None,
-        sn: str = None,
-    ):
-        self.device_open_id = device_open_id
-        self.device_union_ids = device_union_ids
-        self.name = name
-        self.firmware_version = firmware_version
-        self.mac = mac
-        self.sn = sn
-
-    def validate(self):
-        if self.device_union_ids:
-            for k in self.device_union_ids:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.device_open_id is not None:
-            result['DeviceOpenId'] = self.device_open_id
-        result['DeviceUnionIds'] = []
-        if self.device_union_ids is not None:
-            for k in self.device_union_ids:
-                result['DeviceUnionIds'].append(k.to_map() if k else None)
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.firmware_version is not None:
-            result['FirmwareVersion'] = self.firmware_version
-        if self.mac is not None:
-            result['Mac'] = self.mac
-        if self.sn is not None:
-            result['Sn'] = self.sn
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('DeviceOpenId') is not None:
-            self.device_open_id = m.get('DeviceOpenId')
-        self.device_union_ids = []
-        if m.get('DeviceUnionIds') is not None:
-            for k in m.get('DeviceUnionIds'):
-                temp_model = ResultValueDeviceUnionIds()
-                self.device_union_ids.append(temp_model.from_map(k))
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('FirmwareVersion') is not None:
-            self.firmware_version = m.get('FirmwareVersion')
-        if m.get('Mac') is not None:
-            self.mac = m.get('Mac')
-        if m.get('Sn') is not None:
-            self.sn = m.get('Sn')
-        return self
-
-
 class ListDeviceBasicInfoResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
         message: str = None,
         request_id: str = None,
         result: Dict[str, ResultValue] = None,
@@ -16305,14 +18715,15 @@
         message: str = None,
         result: List[ListPlayHistoryResponseBodyResult] = None,
         request_id: str = None,
     ):
         self.code = code
         self.message = message
         self.result = result
+        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
@@ -17810,14 +20221,15 @@
     def __init__(
         self,
         device_info: ListSubAlbumRequestDeviceInfo = None,
         query_subscription_album_request: ListSubAlbumRequestQuerySubscriptionAlbumRequest = None,
         user_info: ListSubAlbumRequestUserInfo = None,
     ):
         self.device_info = device_info
+        # request
         self.query_subscription_album_request = query_subscription_album_request
         self.user_info = user_info
 
     def validate(self):
         if self.device_info:
             self.device_info.validate()
         if self.query_subscription_album_request:
@@ -17857,14 +20269,15 @@
     def __init__(
         self,
         device_info_shrink: str = None,
         query_subscription_album_request_shrink: str = None,
         user_info_shrink: str = None,
     ):
         self.device_info_shrink = device_info_shrink
+        # request
         self.query_subscription_album_request_shrink = query_subscription_album_request_shrink
         self.user_info_shrink = user_info_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -20943,14 +23356,353 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ReadMessageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ScanCodeBindHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class ScanCodeBindRequestBindReq(TeaModel):
+    def __init__(
+        self,
+        client_id: str = None,
+        code: str = None,
+        ext_info: str = None,
+    ):
+        self.client_id = client_id
+        # authCode
+        self.code = code
+        self.ext_info = ext_info
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
+        if self.client_id is not None:
+            result['ClientId'] = self.client_id
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.ext_info is not None:
+            result['ExtInfo'] = self.ext_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientId') is not None:
+            self.client_id = m.get('ClientId')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('ExtInfo') is not None:
+            self.ext_info = m.get('ExtInfo')
+        return self
+
+
+class ScanCodeBindRequestUserInfo(TeaModel):
+    def __init__(
+        self,
+        encode_key: str = None,
+        encode_type: str = None,
+        id: str = None,
+        id_type: str = None,
+        organization_id: str = None,
+    ):
+        self.encode_key = encode_key
+        self.encode_type = encode_type
+        self.id = id
+        self.id_type = id_type
+        self.organization_id = organization_id
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
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.id_type is not None:
+            result['IdType'] = self.id_type
+        if self.organization_id is not None:
+            result['OrganizationId'] = self.organization_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdType') is not None:
+            self.id_type = m.get('IdType')
+        if m.get('OrganizationId') is not None:
+            self.organization_id = m.get('OrganizationId')
+        return self
+
+
+class ScanCodeBindRequest(TeaModel):
+    def __init__(
+        self,
+        bind_req: ScanCodeBindRequestBindReq = None,
+        user_info: ScanCodeBindRequestUserInfo = None,
+    ):
+        self.bind_req = bind_req
+        self.user_info = user_info
+
+    def validate(self):
+        if self.bind_req:
+            self.bind_req.validate()
+        if self.user_info:
+            self.user_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.bind_req is not None:
+            result['BindReq'] = self.bind_req.to_map()
+        if self.user_info is not None:
+            result['UserInfo'] = self.user_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BindReq') is not None:
+            temp_model = ScanCodeBindRequestBindReq()
+            self.bind_req = temp_model.from_map(m['BindReq'])
+        if m.get('UserInfo') is not None:
+            temp_model = ScanCodeBindRequestUserInfo()
+            self.user_info = temp_model.from_map(m['UserInfo'])
+        return self
+
+
+class ScanCodeBindShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        bind_req_shrink: str = None,
+        user_info_shrink: str = None,
+    ):
+        self.bind_req_shrink = bind_req_shrink
+        self.user_info_shrink = user_info_shrink
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
+        if self.bind_req_shrink is not None:
+            result['BindReq'] = self.bind_req_shrink
+        if self.user_info_shrink is not None:
+            result['UserInfo'] = self.user_info_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BindReq') is not None:
+            self.bind_req_shrink = m.get('BindReq')
+        if m.get('UserInfo') is not None:
+            self.user_info_shrink = m.get('UserInfo')
+        return self
+
+
+class ScanCodeBindResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        biz_group: str = None,
+        biz_type: str = None,
+        device_open_id: str = None,
+        user_open_id: str = None,
+    ):
+        self.biz_group = biz_group
+        self.biz_type = biz_type
+        # A963*0158
+        self.device_open_id = device_open_id
+        # DAFE****ce3ej=\
+        self.user_open_id = user_open_id
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
+        if self.biz_group is not None:
+            result['BizGroup'] = self.biz_group
+        if self.biz_type is not None:
+            result['BizType'] = self.biz_type
+        if self.device_open_id is not None:
+            result['DeviceOpenId'] = self.device_open_id
+        if self.user_open_id is not None:
+            result['UserOpenId'] = self.user_open_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizGroup') is not None:
+            self.biz_group = m.get('BizGroup')
+        if m.get('BizType') is not None:
+            self.biz_type = m.get('BizType')
+        if m.get('DeviceOpenId') is not None:
+            self.device_open_id = m.get('DeviceOpenId')
+        if m.get('UserOpenId') is not None:
+            self.user_open_id = m.get('UserOpenId')
+        return self
+
+
+class ScanCodeBindResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        result: ScanCodeBindResponseBodyResult = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = ScanCodeBindResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        return self
+
+
+class ScanCodeBindResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ScanCodeBindResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ScanCodeBindResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ScgSearchHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
         authorization: str = None,
     ):
@@ -21208,33 +23960,218 @@
         if m.get('ScgFilter') is not None:
             self.scg_filter_shrink = m.get('ScgFilter')
         if m.get('TopicId') is not None:
             self.topic_id = m.get('TopicId')
         return self
 
 
+class ScgSearchResponseBodyResultCover(TeaModel):
+    def __init__(
+        self,
+        img: str = None,
+        large: str = None,
+        medium: str = None,
+        small: str = None,
+        can_resize: bool = None,
+    ):
+        self.img = img
+        self.large = large
+        self.medium = medium
+        self.small = small
+        self.can_resize = can_resize
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
+        if self.img is not None:
+            result['Img'] = self.img
+        if self.large is not None:
+            result['Large'] = self.large
+        if self.medium is not None:
+            result['Medium'] = self.medium
+        if self.small is not None:
+            result['Small'] = self.small
+        if self.can_resize is not None:
+            result['canResize'] = self.can_resize
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Img') is not None:
+            self.img = m.get('Img')
+        if m.get('Large') is not None:
+            self.large = m.get('Large')
+        if m.get('Medium') is not None:
+            self.medium = m.get('Medium')
+        if m.get('Small') is not None:
+            self.small = m.get('Small')
+        if m.get('canResize') is not None:
+            self.can_resize = m.get('canResize')
+        return self
+
+
+class ScgSearchResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        album: bool = None,
+        album_raw_id: str = None,
+        album_type: int = None,
+        alias: List[str] = None,
+        author_ids: List[int] = None,
+        author_names: List[str] = None,
+        category: str = None,
+        content_type: str = None,
+        cover: ScgSearchResponseBodyResultCover = None,
+        is_audition: bool = None,
+        is_charge: str = None,
+        need_charge: bool = None,
+        raw_id: str = None,
+        singers: str = None,
+        source: str = None,
+        support_audition: bool = None,
+        title: str = None,
+        type: str = None,
+    ):
+        self.album = album
+        self.album_raw_id = album_raw_id
+        self.album_type = album_type
+        self.alias = alias
+        self.author_ids = author_ids
+        self.author_names = author_names
+        self.category = category
+        self.content_type = content_type
+        self.cover = cover
+        self.is_audition = is_audition
+        self.is_charge = is_charge
+        self.need_charge = need_charge
+        self.raw_id = raw_id
+        self.singers = singers
+        self.source = source
+        self.support_audition = support_audition
+        self.title = title
+        self.type = type
+
+    def validate(self):
+        if self.cover:
+            self.cover.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.album is not None:
+            result['Album'] = self.album
+        if self.album_raw_id is not None:
+            result['AlbumRawId'] = self.album_raw_id
+        if self.album_type is not None:
+            result['AlbumType'] = self.album_type
+        if self.alias is not None:
+            result['Alias'] = self.alias
+        if self.author_ids is not None:
+            result['AuthorIds'] = self.author_ids
+        if self.author_names is not None:
+            result['AuthorNames'] = self.author_names
+        if self.category is not None:
+            result['Category'] = self.category
+        if self.content_type is not None:
+            result['ContentType'] = self.content_type
+        if self.cover is not None:
+            result['Cover'] = self.cover.to_map()
+        if self.is_audition is not None:
+            result['IsAudition'] = self.is_audition
+        if self.is_charge is not None:
+            result['IsCharge'] = self.is_charge
+        if self.need_charge is not None:
+            result['NeedCharge'] = self.need_charge
+        if self.raw_id is not None:
+            result['RawId'] = self.raw_id
+        if self.singers is not None:
+            result['Singers'] = self.singers
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.support_audition is not None:
+            result['SupportAudition'] = self.support_audition
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Album') is not None:
+            self.album = m.get('Album')
+        if m.get('AlbumRawId') is not None:
+            self.album_raw_id = m.get('AlbumRawId')
+        if m.get('AlbumType') is not None:
+            self.album_type = m.get('AlbumType')
+        if m.get('Alias') is not None:
+            self.alias = m.get('Alias')
+        if m.get('AuthorIds') is not None:
+            self.author_ids = m.get('AuthorIds')
+        if m.get('AuthorNames') is not None:
+            self.author_names = m.get('AuthorNames')
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('ContentType') is not None:
+            self.content_type = m.get('ContentType')
+        if m.get('Cover') is not None:
+            temp_model = ScgSearchResponseBodyResultCover()
+            self.cover = temp_model.from_map(m['Cover'])
+        if m.get('IsAudition') is not None:
+            self.is_audition = m.get('IsAudition')
+        if m.get('IsCharge') is not None:
+            self.is_charge = m.get('IsCharge')
+        if m.get('NeedCharge') is not None:
+            self.need_charge = m.get('NeedCharge')
+        if m.get('RawId') is not None:
+            self.raw_id = m.get('RawId')
+        if m.get('Singers') is not None:
+            self.singers = m.get('Singers')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SupportAudition') is not None:
+            self.support_audition = m.get('SupportAudition')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
 class ScgSearchResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
         message: str = None,
         page_num: int = None,
         page_size: int = None,
         request_id: str = None,
-        result: str = None,
+        result: List[ScgSearchResponseBodyResult] = None,
     ):
         self.code = code
         self.message = message
         self.page_num = page_num
         self.page_size = page_size
         self.request_id = request_id
         self.result = result
 
     def validate(self):
-        pass
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -21244,32 +24181,37 @@
             result['Message'] = self.message
         if self.page_num is not None:
             result['PageNum'] = self.page_num
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        result['Result'] = []
         if self.result is not None:
-            result['Result'] = self.result
+            for k in self.result:
+                result['Result'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('PageNum') is not None:
             self.page_num = m.get('PageNum')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        self.result = []
         if m.get('Result') is not None:
-            self.result = m.get('Result')
+            for k in m.get('Result'):
+                temp_model = ScgSearchResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
         return self
 
 
 class ScgSearchResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -21940,14 +24882,15 @@
         code: int = None,
         message: str = None,
         request_id: str = None,
         result: List[SearchContentResponseBodyResult] = None,
     ):
         self.code = code
         self.message = message
+        # Id of the request
         self.request_id = request_id
         self.result = result
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
@@ -22527,14 +25470,169 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SetDeviceSettingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UnbindAligenieUserHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class UnbindAligenieUserRequest(TeaModel):
+    def __init__(
+        self,
+        login_state_access_token: str = None,
+    ):
+        self.login_state_access_token = login_state_access_token
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
+        if self.login_state_access_token is not None:
+            result['LoginStateAccessToken'] = self.login_state_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('LoginStateAccessToken') is not None:
+            self.login_state_access_token = m.get('LoginStateAccessToken')
+        return self
+
+
+class UnbindAligenieUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UnbindAligenieUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UnbindAligenieUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UnbindAligenieUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UnbindDeviceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
         authorization: str = None,
     ):
```

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO` & `alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligeniessp-1-0
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud AliGenie (ssp_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligeniessp_1_0-1.0.9/setup.py` & `alibabacloud_aligeniessp_1_0-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligeniessp_1_0.
 
-Created on 22/08/2022
+Created on 02/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligeniessp_1_0"
 NAME = "alibabacloud_aligeniessp_1_0" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (ssp_1_0) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

