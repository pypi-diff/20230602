# Comparing `tmp/agconnect-1.2.0.300.tar.gz` & `tmp/agconnect-1.3.0.300.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agconnect-1.2.0.300.tar", last modified: Wed Jan  4 10:38:40 2023, max compression
+gzip compressed data, was "dist\agconnect-1.3.0.300.tar", last modified: Fri Jun  2 05:42:54 2023, max compression
```

## Comparing `agconnect-1.2.0.300.tar` & `agconnect-1.3.0.300.tar`

### file list

```diff
@@ -1,179 +1,215 @@
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.786399 agconnect-1.2.0.300/
--rw-r--r--   0 slave1     (544) slave1     (344)      176 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/.gitignore
--rw-r--r--   0 slave1     (544) slave1     (344)      403 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/MANIFEST.in
--rw-r--r--   0 slave1     (544) slave1     (344)     4458 2023-01-04 10:38:40.786399 agconnect-1.2.0.300/PKG-INFO
--rw-r--r--   0 slave1     (544) slave1     (344)     4084 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/README.md
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.773398 agconnect-1.2.0.300/agconnect/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/__init__.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.774398 agconnect-1.2.0.300/agconnect/auth_server/
--rw-r--r--   0 slave1     (544) slave1     (344)      850 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      200 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/agconnect_auth.json
--rw-r--r--   0 slave1     (544) slave1     (344)       49 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/pytest.ini
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.774398 agconnect-1.2.0.300/agconnect/auth_server/src/
--rw-r--r--   0 slave1     (544) slave1     (344)       86 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/__init__.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.774398 agconnect-1.2.0.300/agconnect/auth_server/src/backend/
--rw-r--r--   0 slave1     (544) slave1     (344)       73 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/backend/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     6241 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/backend/auth_backend.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.775398 agconnect-1.2.0.300/agconnect/auth_server/src/entity/
--rw-r--r--   0 slave1     (544) slave1     (344)      483 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/entity/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     3474 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/entity/auth_access_token.py
--rw-r--r--   0 slave1     (544) slave1     (344)      540 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/entity/provider.py
--rw-r--r--   0 slave1     (544) slave1     (344)      626 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/entity/token_provider_info.py
--rw-r--r--   0 slave1     (544) slave1     (344)      500 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/entity/user_import_export_result.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.775398 agconnect-1.2.0.300/agconnect/auth_server/src/error/
--rw-r--r--   0 slave1     (544) slave1     (344)      210 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/error/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     3992 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/error/agc_auth_error_message.py
--rw-r--r--   0 slave1     (544) slave1     (344)      456 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/error/agc_auth_exception.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.776398 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/
--rw-r--r--   0 slave1     (544) slave1     (344)      246 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1851 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_jwt.py
--rw-r--r--   0 slave1     (544) slave1     (344)      500 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_jwttoken.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1504 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_public_key_manager.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1981 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_rsa_verifier.py
--rw-r--r--   0 slave1     (544) slave1     (344)      453 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/jwt/rsa_key_pair.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.777398 agconnect-1.2.0.300/agconnect/auth_server/src/request/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1058 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/export_user_list_req.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1026 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/export_user_req.py
--rw-r--r--   0 slave1     (544) slave1     (344)     6405 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/import_export_user_info.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1388 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/import_user_req.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1995 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/provider_info.py
--rw-r--r--   0 slave1     (544) slave1     (344)      455 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/public_key_req.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1030 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/revoke_token_req.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1087 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/request/verify_token_req.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.777398 agconnect-1.2.0.300/agconnect/auth_server/src/response/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      220 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/auth_operate_rsp.py
--rw-r--r--   0 slave1     (544) slave1     (344)      857 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/export_user_list_rsp.py
--rw-r--r--   0 slave1     (544) slave1     (344)     2359 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/export_user_rsp.py
--rw-r--r--   0 slave1     (544) slave1     (344)      430 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/import_success_user.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1047 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/import_user_rsp.py
--rw-r--r--   0 slave1     (544) slave1     (344)      354 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/publickey_rsp.py
--rw-r--r--   0 slave1     (544) slave1     (344)      462 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/token_info.py
--rw-r--r--   0 slave1     (544) slave1     (344)      976 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/response/verify_token.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.778398 agconnect-1.2.0.300/agconnect/auth_server/src/service/
--rw-r--r--   0 slave1     (544) slave1     (344)      160 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/service/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      911 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/service/agc_auth.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.778398 agconnect-1.2.0.300/agconnect/auth_server/src/service/impl/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/service/impl/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1584 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/service/impl/agc_auth_service.py
--rw-r--r--   0 slave1     (544) slave1     (344)    18431 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/service/impl/agc_auth_service_impl.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.778398 agconnect-1.2.0.300/agconnect/auth_server/src/utils/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/utils/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     2760 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/utils/auth_service_api_util.py
--rw-r--r--   0 slave1     (544) slave1     (344)     2938 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/auth_server/src/utils/key_header_util.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.778398 agconnect-1.2.0.300/agconnect/cloud_function/
--rw-r--r--   0 slave1     (544) slave1     (344)      186 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/__init__.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.778398 agconnect-1.2.0.300/agconnect/cloud_function/src/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/__init__.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.779398 agconnect-1.2.0.300/agconnect/cloud_function/src/exception/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/exception/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      440 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/exception/agc_function_error_code.py
--rw-r--r--   0 slave1     (544) slave1     (344)      447 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/exception/agc_function_exception.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.779398 agconnect-1.2.0.300/agconnect/cloud_function/src/function_types/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/function_types/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1649 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/function_types/base.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.780398 agconnect-1.2.0.300/agconnect/cloud_function/src/impl/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/impl/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1046 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/impl/agconnect_function_impl.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1577 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/impl/function_callable.py
--rw-r--r--   0 slave1     (544) slave1     (344)      529 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/impl/function_result_impl.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.780398 agconnect-1.2.0.300/agconnect/cloud_function/src/server/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/server/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     3668 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/server/function_backend.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.780398 agconnect-1.2.0.300/agconnect/cloud_function/src/server/request/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/server/request/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     2047 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/server/request/function_request.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.780398 agconnect-1.2.0.300/agconnect/cloud_function/src/util/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/util/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      844 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/cloud_function/src/util/hash_util.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.780398 agconnect-1.2.0.300/agconnect/common_server/
--rw-r--r--   0 slave1     (544) slave1     (344)     2225 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      912 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/agconnect_common.json
--rw-r--r--   0 slave1     (544) slave1     (344)      260 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/logging_config.json
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.772398 agconnect-1.2.0.300/agconnect/common_server/src/
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.781398 agconnect-1.2.0.300/agconnect/common_server/src/agc_client/
--rw-r--r--   0 slave1     (544) slave1     (344)      171 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/agc_client/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     3770 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/agc_client/agc_client.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.781398 agconnect-1.2.0.300/agconnect/common_server/src/config/
--rw-r--r--   0 slave1     (544) slave1     (344)      280 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/config/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1332 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/config/cloud_gw_url_utils.py
--rw-r--r--   0 slave1     (544) slave1     (344)     4315 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/config/config_service.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.781398 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/
--rw-r--r--   0 slave1     (544) slave1     (344)       73 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      586 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/access_token.py
--rw-r--r--   0 slave1     (544) slave1     (344)     4250 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/client_id_credential.py
--rw-r--r--   0 slave1     (544) slave1     (344)     3835 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/credential_parser.py
--rw-r--r--   0 slave1     (544) slave1     (344)      585 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/credential_service.py
--rw-r--r--   0 slave1     (544) slave1     (344)      208 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/credential_service/credential_type.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.782398 agconnect-1.2.0.300/agconnect/common_server/src/error/
--rw-r--r--   0 slave1     (544) slave1     (344)      304 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/error/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1345 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/error/error.py
--rw-r--r--   0 slave1     (544) slave1     (344)     2565 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/error/error_message.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.782398 agconnect-1.2.0.300/agconnect/common_server/src/http_client/
--rw-r--r--   0 slave1     (544) slave1     (344)      679 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      609 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/base_response.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1563 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/common_headers.py
--rw-r--r--   0 slave1     (544) slave1     (344)      400 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/connect_ret.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1002 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/http_client.py
--rw-r--r--   0 slave1     (544) slave1     (344)     6720 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/http_client_api.py
--rw-r--r--   0 slave1     (544) slave1     (344)      369 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/http_client/request_constructor.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.783398 agconnect-1.2.0.300/agconnect/common_server/src/log_config/
--rw-r--r--   0 slave1     (544) slave1     (344)      270 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/log_config/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      307 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/log_config/common_log.py
--rw-r--r--   0 slave1     (544) slave1     (344)     6315 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/log_config/logging_config.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.783398 agconnect-1.2.0.300/agconnect/common_server/src/service/
--rw-r--r--   0 slave1     (544) slave1     (344)      268 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/service/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      368 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/service/agc_service.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1649 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/service/service_factory.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.783398 agconnect-1.2.0.300/agconnect/common_server/src/utils/
--rw-r--r--   0 slave1     (544) slave1     (344)      169 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/utils/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1768 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/common_server/src/utils/utils.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.783398 agconnect-1.2.0.300/agconnect/database_server/
--rw-r--r--   0 slave1     (544) slave1     (344)     1370 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)       67 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/agconnect-database.json
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.783398 agconnect-1.2.0.300/agconnect/database_server/src/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/__init__.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.784398 agconnect-1.2.0.300/agconnect/database_server/src/communicator/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/communicator/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     6119 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/communicator/https_communicator.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1282 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/communicator/request_header.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.784398 agconnect-1.2.0.300/agconnect/database_server/src/exception/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/exception/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      526 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/exception/agconnect_cloud_db_exception.py
--rw-r--r--   0 slave1     (544) slave1     (344)     9124 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/exception/cloud_db_error_code.py
--rw-r--r--   0 slave1     (544) slave1     (344)    22904 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/exception/error_code_message.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.785398 agconnect-1.2.0.300/agconnect/database_server/src/query/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/query/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1382 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_config.py
--rw-r--r--   0 slave1     (544) slave1     (344)     2878 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator.py
--rw-r--r--   0 slave1     (544) slave1     (344)     4346 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator_constraint.py
--rw-r--r--   0 slave1     (544) slave1     (344)    16953 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_query.py
--rw-r--r--   0 slave1     (544) slave1     (344)      434 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_snapshot.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.785398 agconnect-1.2.0.300/agconnect/database_server/src/services/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/services/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)     5113 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/services/agconnect_cloud_db.py
--rw-r--r--   0 slave1     (544) slave1     (344)     5428 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/services/cloud_db_service.py
--rw-r--r--   0 slave1     (544) slave1     (344)    43773 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/services/cloud_db_zone.py
--rw-r--r--   0 slave1     (544) slave1     (344)    10388 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/services/transaction.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.786399 agconnect-1.2.0.300/agconnect/database_server/src/utils/
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/__init__.py
--rw-r--r--   0 slave1     (544) slave1     (344)      222 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/aggregare_type.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1109 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/cloud_db_sdk_utils.py
--rw-r--r--   0 slave1     (544) slave1     (344)      707 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/condition_type.py
--rw-r--r--   0 slave1     (544) slave1     (344)    15052 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/condition_validate.py
--rw-r--r--   0 slave1     (544) slave1     (344)    12439 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/data_model_helper.py
--rw-r--r--   0 slave1     (544) slave1     (344)      456 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/field_type.py
--rw-r--r--   0 slave1     (544) slave1     (344)     7716 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/object_creator.py
--rw-r--r--   0 slave1     (544) slave1     (344)     1479 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/scheme_utils.py
--rw-r--r--   0 slave1     (544) slave1     (344)    17522 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/agconnect/database_server/src/utils/utils.py
-drwxr-xr-x   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:40.774398 agconnect-1.2.0.300/agconnect.egg-info/
--rw-r--r--   0 slave1     (544) slave1     (344)     4458 2023-01-04 10:38:40.000000 agconnect-1.2.0.300/agconnect.egg-info/PKG-INFO
--rw-r--r--   0 slave1     (544) slave1     (344)     6991 2023-01-04 10:38:40.000000 agconnect-1.2.0.300/agconnect.egg-info/SOURCES.txt
--rw-r--r--   0 slave1     (544) slave1     (344)        1 2023-01-04 10:38:40.000000 agconnect-1.2.0.300/agconnect.egg-info/dependency_links.txt
--rw-r--r--   0 slave1     (544) slave1     (344)      106 2023-01-04 10:38:40.000000 agconnect-1.2.0.300/agconnect.egg-info/requires.txt
--rw-r--r--   0 slave1     (544) slave1     (344)       10 2023-01-04 10:38:40.000000 agconnect-1.2.0.300/agconnect.egg-info/top_level.txt
--rw-r--r--   0 slave1     (544) slave1     (344)        0 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/requirements.in
--rw-r--r--   0 slave1     (544) slave1     (344)      221 2023-01-04 10:38:17.000000 agconnect-1.2.0.300/requirements.txt
--rw-r--r--   0 slave1     (544) slave1     (344)      558 2023-01-04 10:38:40.787398 agconnect-1.2.0.300/setup.cfg
--rw-r--r--   0 slave1     (544) slave1     (344)      564 2023-01-04 10:38:39.000000 agconnect-1.2.0.300/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.208510 agconnect-1.3.0.300/
+-rw-rw-rw-   0        0        0      241 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/.gitignore
+-rw-rw-rw-   0        0        0      438 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/MANIFEST.in
+-rw-rw-rw-   0        0        0     6554 2023-06-02 05:42:54.208510 agconnect-1.3.0.300/PKG-INFO
+-rw-rw-rw-   0        0        0     5005 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.947637 agconnect-1.3.0.300/agconnect/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.958637 agconnect-1.3.0.300/agconnect/auth_server/
+-rw-rw-rw-   0        0        0      850 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/agconnect_auth.json
+-rw-rw-rw-   0        0        0       49 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/pytest.ini
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.960637 agconnect-1.3.0.300/agconnect/auth_server/src/
+-rw-rw-rw-   0        0        0       86 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.963638 agconnect-1.3.0.300/agconnect/auth_server/src/backend/
+-rw-rw-rw-   0        0        0       73 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/backend/__init__.py
+-rw-rw-rw-   0        0        0     6241 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/backend/auth_backend.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.973202 agconnect-1.3.0.300/agconnect/auth_server/src/entity/
+-rw-rw-rw-   0        0        0      483 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/entity/__init__.py
+-rw-rw-rw-   0        0        0     3474 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/entity/auth_access_token.py
+-rw-rw-rw-   0        0        0      540 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/entity/provider.py
+-rw-rw-rw-   0        0        0      626 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/entity/token_provider_info.py
+-rw-rw-rw-   0        0        0      500 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/entity/user_import_export_result.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.978215 agconnect-1.3.0.300/agconnect/auth_server/src/error/
+-rw-rw-rw-   0        0        0      210 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/error/__init__.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/error/agc_auth_error_message.py
+-rw-rw-rw-   0        0        0      456 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/error/agc_auth_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.990213 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/
+-rw-rw-rw-   0        0        0      246 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/__init__.py
+-rw-rw-rw-   0        0        0     1851 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_jwt.py
+-rw-rw-rw-   0        0        0      500 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_jwttoken.py
+-rw-rw-rw-   0        0        0     1504 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_public_key_manager.py
+-rw-rw-rw-   0        0        0     1981 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_rsa_verifier.py
+-rw-rw-rw-   0        0        0      453 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/jwt/rsa_key_pair.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.004216 agconnect-1.3.0.300/agconnect/auth_server/src/request/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/export_user_list_req.py
+-rw-rw-rw-   0        0        0     1026 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/export_user_req.py
+-rw-rw-rw-   0        0        0     6405 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/import_export_user_info.py
+-rw-rw-rw-   0        0        0     1388 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/import_user_req.py
+-rw-rw-rw-   0        0        0     1995 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/provider_info.py
+-rw-rw-rw-   0        0        0      455 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/public_key_req.py
+-rw-rw-rw-   0        0        0     1030 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/revoke_token_req.py
+-rw-rw-rw-   0        0        0     1087 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/request/verify_token_req.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.018211 agconnect-1.3.0.300/agconnect/auth_server/src/response/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/__init__.py
+-rw-rw-rw-   0        0        0      220 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/auth_operate_rsp.py
+-rw-rw-rw-   0        0        0      857 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/export_user_list_rsp.py
+-rw-rw-rw-   0        0        0     2359 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/export_user_rsp.py
+-rw-rw-rw-   0        0        0      430 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/import_success_user.py
+-rw-rw-rw-   0        0        0     1047 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/import_user_rsp.py
+-rw-rw-rw-   0        0        0      354 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/publickey_rsp.py
+-rw-rw-rw-   0        0        0      462 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/token_info.py
+-rw-rw-rw-   0        0        0      976 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/response/verify_token.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.021218 agconnect-1.3.0.300/agconnect/auth_server/src/service/
+-rw-rw-rw-   0        0        0      160 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/service/__init__.py
+-rw-rw-rw-   0        0        0      911 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/service/agc_auth.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.026213 agconnect-1.3.0.300/agconnect/auth_server/src/service/impl/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/service/impl/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/service/impl/agc_auth_service.py
+-rw-rw-rw-   0        0        0    18431 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/service/impl/agc_auth_service_impl.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.030214 agconnect-1.3.0.300/agconnect/auth_server/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     2760 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/utils/auth_service_api_util.py
+-rw-rw-rw-   0        0        0     2938 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/auth_server/src/utils/key_header_util.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.031244 agconnect-1.3.0.300/agconnect/cloud_function/
+-rw-rw-rw-   0        0        0      186 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.033213 agconnect-1.3.0.300/agconnect/cloud_function/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.037212 agconnect-1.3.0.300/agconnect/cloud_function/src/exception/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/exception/__init__.py
+-rw-rw-rw-   0        0        0      440 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/exception/agc_function_error_code.py
+-rw-rw-rw-   0        0        0      447 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/exception/agc_function_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.040232 agconnect-1.3.0.300/agconnect/cloud_function/src/function_types/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/function_types/__init__.py
+-rw-rw-rw-   0        0        0     1649 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/function_types/base.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.046214 agconnect-1.3.0.300/agconnect/cloud_function/src/impl/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/impl/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/impl/agconnect_function_impl.py
+-rw-rw-rw-   0        0        0     1577 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/impl/function_callable.py
+-rw-rw-rw-   0        0        0      529 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/impl/function_result_impl.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.050210 agconnect-1.3.0.300/agconnect/cloud_function/src/server/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/server/__init__.py
+-rw-rw-rw-   0        0        0     3668 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/server/function_backend.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.053249 agconnect-1.3.0.300/agconnect/cloud_function/src/server/request/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/server/request/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/server/request/function_request.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.056214 agconnect-1.3.0.300/agconnect/cloud_function/src/util/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/util/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_function/src/util/hash_util.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.059251 agconnect-1.3.0.300/agconnect/cloud_storage/
+-rw-rw-rw-   0        0        0     1832 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/agconnect_cloud_storage.json
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.060233 agconnect-1.3.0.300/agconnect/cloud_storage/src/
+-rw-rw-rw-   0        0        0       73 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.062251 agconnect-1.3.0.300/agconnect/cloud_storage/src/config/
+-rw-rw-rw-   0        0        0     4570 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/config/config.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.066213 agconnect-1.3.0.300/agconnect/cloud_storage/src/exception/
+-rw-rw-rw-   0        0        0      948 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/exception/agconnect_cloud_storage_error_code.py
+-rw-rw-rw-   0        0        0     8335 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/exception/agconnect_cloud_storage_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.075213 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/
+-rw-rw-rw-   0        0        0       73 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/agc_cloud_storage.py
+-rw-rw-rw-   0        0        0    14111 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/bucket.py
+-rw-rw-rw-   0        0        0      350 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/constant.py
+-rw-rw-rw-   0        0        0     8802 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/file.py
+-rw-rw-rw-   0        0        0     4865 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/impl/storage_management.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.081217 agconnect-1.3.0.300/agconnect/cloud_storage/src/model/
+-rw-rw-rw-   0        0        0     1135 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/model/callback.py
+-rw-rw-rw-   0        0        0      458 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/model/models.py
+-rw-rw-rw-   0        0        0      842 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/model/options.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.085247 agconnect-1.3.0.300/agconnect/cloud_storage/src/request/
+-rw-rw-rw-   0        0        0     7253 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/request/request.py
+-rw-rw-rw-   0        0        0     2340 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/request/upload_request.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.089212 agconnect-1.3.0.300/agconnect/cloud_storage/src/shared/
+-rw-rw-rw-   0        0        0     4145 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/shared/request_with_storage_shared.py
+-rw-rw-rw-   0        0        0      660 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/shared/shared_dataclass_stream_file.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.094213 agconnect-1.3.0.300/agconnect/cloud_storage/src/upload/
+-rw-rw-rw-   0        0        0     1459 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/upload/fetch.py
+-rw-rw-rw-   0        0        0     1170 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/upload/file_stream.py
+-rw-rw-rw-   0        0        0     4335 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/upload/resumable_upload.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.099214 agconnect-1.3.0.300/agconnect/cloud_storage/src/utils/
+-rw-rw-rw-   0        0        0      723 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/utils/common.py
+-rw-rw-rw-   0        0        0       73 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/utils/common_log.py
+-rw-rw-rw-   0        0        0     3563 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/cloud_storage/src/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.104216 agconnect-1.3.0.300/agconnect/common_server/
+-rw-rw-rw-   0        0        0     2225 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/agconnect_common.json
+-rw-rw-rw-   0        0        0      382 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/logging_config.json
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.928636 agconnect-1.3.0.300/agconnect/common_server/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.107215 agconnect-1.3.0.300/agconnect/common_server/src/agc_client/
+-rw-rw-rw-   0        0        0      171 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/agc_client/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/agc_client/agc_client.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.111259 agconnect-1.3.0.300/agconnect/common_server/src/config/
+-rw-rw-rw-   0        0        0      280 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/config/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/config/cloud_gw_url_utils.py
+-rw-rw-rw-   0        0        0     4315 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/config/config_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.124221 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/
+-rw-rw-rw-   0        0        0       73 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/__init__.py
+-rw-rw-rw-   0        0        0      586 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/access_token.py
+-rw-rw-rw-   0        0        0     4250 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/client_id_credential.py
+-rw-rw-rw-   0        0        0     3835 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/credential_parser.py
+-rw-rw-rw-   0        0        0      585 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/credential_service.py
+-rw-rw-rw-   0        0        0      208 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/credential_service/credential_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.129215 agconnect-1.3.0.300/agconnect/common_server/src/error/
+-rw-rw-rw-   0        0        0      304 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/error/__init__.py
+-rw-rw-rw-   0        0        0     1345 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/error/error.py
+-rw-rw-rw-   0        0        0     2565 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/error/error_message.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.140246 agconnect-1.3.0.300/agconnect/common_server/src/http_client/
+-rw-rw-rw-   0        0        0      679 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/base_response.py
+-rw-rw-rw-   0        0        0     1563 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/common_headers.py
+-rw-rw-rw-   0        0        0      400 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/connect_ret.py
+-rw-rw-rw-   0        0        0     1002 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/http_client.py
+-rw-rw-rw-   0        0        0     6720 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/http_client_api.py
+-rw-rw-rw-   0        0        0      369 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/http_client/request_constructor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.146215 agconnect-1.3.0.300/agconnect/common_server/src/log_config/
+-rw-rw-rw-   0        0        0      270 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/log_config/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/log_config/common_log.py
+-rw-rw-rw-   0        0        0     5849 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/log_config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.150554 agconnect-1.3.0.300/agconnect/common_server/src/service/
+-rw-rw-rw-   0        0        0      268 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/service/__init__.py
+-rw-rw-rw-   0        0        0      368 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/service/agc_service.py
+-rw-rw-rw-   0        0        0     1649 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/service/service_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.154512 agconnect-1.3.0.300/agconnect/common_server/src/utils/
+-rw-rw-rw-   0        0        0      169 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/common_server/src/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.157539 agconnect-1.3.0.300/agconnect/database_server/
+-rw-rw-rw-   0        0        0     1370 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/agconnect-database.json
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.159510 agconnect-1.3.0.300/agconnect/database_server/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.164514 agconnect-1.3.0.300/agconnect/database_server/src/communicator/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/communicator/__init__.py
+-rw-rw-rw-   0        0        0     6119 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/communicator/https_communicator.py
+-rw-rw-rw-   0        0        0     1282 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/communicator/request_header.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.171514 agconnect-1.3.0.300/agconnect/database_server/src/exception/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/exception/__init__.py
+-rw-rw-rw-   0        0        0      526 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/exception/agconnect_cloud_db_exception.py
+-rw-rw-rw-   0        0        0     9124 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/exception/cloud_db_error_code.py
+-rw-rw-rw-   0        0        0    22904 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/exception/error_code_message.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.181510 agconnect-1.3.0.300/agconnect/database_server/src/query/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/query/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_config.py
+-rw-rw-rw-   0        0        0     2878 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator.py
+-rw-rw-rw-   0        0        0     4346 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator_constraint.py
+-rw-rw-rw-   0        0        0    16953 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_query.py
+-rw-rw-rw-   0        0        0      434 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_snapshot.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.188512 agconnect-1.3.0.300/agconnect/database_server/src/services/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/services/__init__.py
+-rw-rw-rw-   0        0        0     5113 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/services/agconnect_cloud_db.py
+-rw-rw-rw-   0        0        0     5428 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/services/cloud_db_service.py
+-rw-rw-rw-   0        0        0    43773 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/services/cloud_db_zone.py
+-rw-rw-rw-   0        0        0    10388 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/services/transaction.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:54.206515 agconnect-1.3.0.300/agconnect/database_server/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/aggregare_type.py
+-rw-rw-rw-   0        0        0     1109 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/cloud_db_sdk_utils.py
+-rw-rw-rw-   0        0        0      707 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/condition_type.py
+-rw-rw-rw-   0        0        0    15052 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/condition_validate.py
+-rw-rw-rw-   0        0        0    12461 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/data_model_helper.py
+-rw-rw-rw-   0        0        0      456 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/field_type.py
+-rw-rw-rw-   0        0        0     7716 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/object_creator.py
+-rw-rw-rw-   0        0        0     1479 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/scheme_utils.py
+-rw-rw-rw-   0        0        0    17522 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/agconnect/database_server/src/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:42:53.954649 agconnect-1.3.0.300/agconnect.egg-info/
+-rw-rw-rw-   0        0        0     6554 2023-06-02 05:42:53.000000 agconnect-1.3.0.300/agconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8277 2023-06-02 05:42:53.000000 agconnect-1.3.0.300/agconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 05:42:53.000000 agconnect-1.3.0.300/agconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-06-02 05:42:53.000000 agconnect-1.3.0.300/agconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 05:42:53.000000 agconnect-1.3.0.300/agconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/requirements.in
+-rw-rw-rw-   0        0        0      266 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/requirements.txt
+-rw-rw-rw-   0        0        0      316 2023-04-18 08:01:24.000000 agconnect-1.3.0.300/requirements_dev.txt
+-rw-rw-rw-   0        0        0      638 2023-06-02 05:42:54.209511 agconnect-1.3.0.300/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-04-18 08:02:01.000000 agconnect-1.3.0.300/setup.py
```

### Comparing `agconnect-1.2.0.300/PKG-INFO` & `agconnect-1.3.0.300/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: agconnect
-Version: 1.2.0.300
-Summary: AppGallery Connect Server-SDK for Python development
-Home-page: https://developer.huawei.com/consumer/en/service/josp/agc/index.html,,AppGalleryConnect#/
-Author: AppGallery Connect
-License: ISC
-Keywords: agconnect,server SDK,Python,authentication
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Huawei AppGallery Connect Python Server SDK
 
 ## Overview
 
 AppGallery Connect is dedicated to providing one-stop services for app creation, development,
 distribution, operations, and engagement, and building a smart app ecosystem for all scenarios.
 By opening up a wide range of services and capabilities, which are built upon Huawei's profound
@@ -21,14 +10,15 @@
 scope of users and generate higher revenue.You can access the services listed below.
 
 This module contains Server SDKs for following AGC Services:
 
 1.Auth Service
 2.Cloud Function
 3.Cloud DB
+4.Cloud Storage
 
 For more information, visit
 the [AppGallery Connect Introduction](https://developer.huawei.com/consumer/en/doc/development/AppGallery-connect-Guides/agc-introduction-0000001057492641)
 
 ## Auth Service Overview
 
 Auth Service provides an SDK and backend services, supports multiple authentication modes,
@@ -56,27 +46,39 @@
 data models, and various data management APIs. In addition to ensuring data availability, reliability,
 consistency, and security, CloudDB enables seamless data synchronization between the device and cloud,
 and supports offline application operations, helping developers quickly develop device-cloud and multi-device
 synergy applications. As a part of the AppGallery Connect solution, Cloud DB builds the Mobile Backend as a Service
 (MBaaS) capability for the AppGallery Connect platform. In this way, application developers can focus on
 application services, greatly improving the production efficiency.
 
-- [Cloud DB Introduction](https://developer.huawei.com/consumer/en/doc/development/AppGallery-connect-Guides/agc-clouddb-introduction-0000001054212760)
+## Cloud Storage Overview
+
+AppGallery Connect Cloud Storage allows you to store high volumes of data such as images, audio, videos, and other 
+user-generated content securely and economically. This scalable and maintenance-free service can free you 
+from development, deployment, O&M, and capacity expansion of storage servers, so you can focus on 
+service capability building and operations with better user experience. The Cloud Storage SDK provided 
+for various clients has the following advantages in file uploads and downloads.Strong security: 
+Data is transmitted using HTTPS, and files are encrypted and stored on the cloud using secure 
+encryption protocols. Resumable transfer, You can resume uploads or downloads from the breakpoint 
+if there is a network failure or misoperation while the upload or download is underway.
+
+- [Cloud Storage Introduction](https://developer.huawei.com/consumer/en/doc/development/AppGallery-connect-Guides/agc-cloudstorage-introduction-0000001054847259)
 
 ## Agconnect Installation
 
 You can install the agconnect via PyPi
 
     pip install agconnect
 
 After the installation takes place, you can import the SDKs as shown below:
 
     from agconnect.auth_server import AGCAuth
     from agconnect.cloud_function import AGConnectFunction
     from agconnect.database_server import AGConnectCloudDB
+    from agconnect.cloud_storage import AGConnectCloudStorage
 
 # Supported Environments
 
 This project supports Python version 3.7 or higher
 
 Also note that the Huawei AppGallery Connect Python Server SDK should only be used in server-side/back-end environments
 controlled by the application developer.This includes most server and serverless platforms. Do not use the Python Server
@@ -91,9 +93,7 @@
 [agconnect](https://pypi.org/search/?q=agconnect&o=)
 
 [python](https://pypi.org/search/?q=python&o=)
 
 [server sdk](https://pypi.org/search/?q=server+sdk&o=)
 
 [authentication](https://pypi.org/search/?q=authentication&o=)
-
-
```

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/__init__.py` & `agconnect-1.3.0.300/agconnect/auth_server/__init__.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/backend/auth_backend.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/backend/auth_backend.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/entity/auth_access_token.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/entity/auth_access_token.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/entity/provider.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/entity/provider.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/entity/token_provider_info.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/entity/token_provider_info.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/error/agc_auth_error_message.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/error/agc_auth_error_message.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_jwt.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_jwt.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_public_key_manager.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_public_key_manager.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/jwt/agc_auth_rsa_verifier.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/jwt/agc_auth_rsa_verifier.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/export_user_list_req.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/export_user_list_req.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/export_user_req.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/export_user_req.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/import_export_user_info.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/import_export_user_info.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/import_user_req.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/import_user_req.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/provider_info.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/provider_info.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/revoke_token_req.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/revoke_token_req.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/request/verify_token_req.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/request/verify_token_req.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/response/export_user_list_rsp.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/response/export_user_list_rsp.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/response/export_user_rsp.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/response/export_user_rsp.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/response/import_user_rsp.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/response/import_user_rsp.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/response/verify_token.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/response/verify_token.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/service/agc_auth.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/service/agc_auth.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/service/impl/agc_auth_service.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/service/impl/agc_auth_service.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/service/impl/agc_auth_service_impl.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/service/impl/agc_auth_service_impl.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/utils/auth_service_api_util.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/utils/auth_service_api_util.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/auth_server/src/utils/key_header_util.py` & `agconnect-1.3.0.300/agconnect/auth_server/src/utils/key_header_util.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/function_types/base.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/function_types/base.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/impl/agconnect_function_impl.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/impl/agconnect_function_impl.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/impl/function_callable.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/impl/function_callable.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/impl/function_result_impl.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/impl/function_result_impl.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/server/function_backend.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/server/function_backend.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/server/request/function_request.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/server/request/function_request.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/cloud_function/src/util/hash_util.py` & `agconnect-1.3.0.300/agconnect/cloud_function/src/util/hash_util.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/__init__.py` & `agconnect-1.3.0.300/agconnect/common_server/__init__.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/agconnect_common.json` & `agconnect-1.3.0.300/agconnect/common_server/agconnect_common.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sdk_version'": "'1.3.0'"}*

```diff
@@ -19,11 +19,11 @@
         {
             "backupUrl": "https://connect-api-dre.cloud.huawei.com.cn/",
             "region": "DE",
             "url": "https://connect-api-dre.cloud.huawei.com/"
         }
     ],
     "sdk_name": "common",
-    "sdk_version": "1.2.0",
+    "sdk_version": "1.3.0",
     "team_cloudgw_url": "https://agc-api.cloud.huawei.com/",
     "team_cloudgw_url_backup": "https://agc-api.cloud.huawei.com/"
 }
```

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/agc_client/agc_client.py` & `agconnect-1.3.0.300/agconnect/common_server/src/agc_client/agc_client.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/config/cloud_gw_url_utils.py` & `agconnect-1.3.0.300/agconnect/common_server/src/config/cloud_gw_url_utils.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/config/config_service.py` & `agconnect-1.3.0.300/agconnect/common_server/src/config/config_service.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/credential_service/access_token.py` & `agconnect-1.3.0.300/agconnect/common_server/src/credential_service/access_token.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/credential_service/client_id_credential.py` & `agconnect-1.3.0.300/agconnect/common_server/src/credential_service/client_id_credential.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/credential_service/credential_parser.py` & `agconnect-1.3.0.300/agconnect/common_server/src/credential_service/credential_parser.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/credential_service/credential_service.py` & `agconnect-1.3.0.300/agconnect/common_server/src/credential_service/credential_service.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/error/error.py` & `agconnect-1.3.0.300/agconnect/common_server/src/error/error.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/error/error_message.py` & `agconnect-1.3.0.300/agconnect/common_server/src/error/error_message.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/http_client/__init__.py` & `agconnect-1.3.0.300/agconnect/common_server/src/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/http_client/base_response.py` & `agconnect-1.3.0.300/agconnect/common_server/src/http_client/base_response.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/http_client/common_headers.py` & `agconnect-1.3.0.300/agconnect/common_server/src/http_client/common_headers.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/http_client/http_client.py` & `agconnect-1.3.0.300/agconnect/common_server/src/http_client/http_client.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/http_client/http_client_api.py` & `agconnect-1.3.0.300/agconnect/common_server/src/http_client/http_client_api.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/log_config/logging_config.py` & `agconnect-1.3.0.300/agconnect/common_server/src/log_config/logging_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) Huawei Technologies Co., Ltd. 2022. All rights reserved.
 
 import json
-import logging
 import os
 import time
+import logging
+
 from datetime import datetime
+from loguru import logger as loguru_logger
 from logging.handlers import RotatingFileHandler
 
 from agconnect.common_server.src.error.error import AGCException
 from agconnect.common_server.src.error.error_message import ErrorCodeConstant
 
 DEFAULT_LOG_DIR = '../logs'
 
@@ -22,37 +24,31 @@
 
 DEFAULT_META_INFO = 'common_server'
 
 DEFAULT_FILE_SWITCH = 'off'
 
 DEFAULT_CONSOLE_SWITCH = 'on'
 
+DEFAULT_LEVEL_COLORS = {
+    "TRACE": "cyan",
+    "DEBUG": "blue",
+    "INFO": "",
+    "SUCCESS": "green",
+    "WARNING": "yellow",
+    "ERROR": "red",
+    "CRITICAL": "RED"
+}
+
 DEFAULT_DIRECTORY = os.path.normpath(os.path.join(os.path.dirname(__file__), '../../logging_config.json'))
 
 local_time = time.localtime()
 now = datetime(local_time[0], local_time[1], local_time[2], local_time[3], local_time[4], local_time[5])
 DT_STRING = now.strftime("-%m-%d-%Y-%H")
 
 
-def update_config(logger_level=None, file_switch=None, console_switch=None, log_file_path=None):
-    with open(DEFAULT_DIRECTORY, 'r') as file:
-        data = json.load(file)
-    if logger_level:
-        data['logger_level'] = logger_level
-    if file_switch:
-        data['file_switch'] = file_switch
-    if console_switch:
-        data['console_switch'] = console_switch
-    if log_file_path:
-        data['path'] = log_file_path
-    fd = os.open(DEFAULT_DIRECTORY, os.O_CREAT | os.O_WRONLY, 0o644)
-    with os.fdopen(fd, 'w') as file:
-        json.dump(data, file, indent=4)
-
-
 def log_configuration(config_path: str) -> logging.Logger:
     logging_config = read_config_file(config_path)
     config_info = get_config_info(logging_config)
     log_directory = os.path.normpath(os.path.join(os.path.dirname(
         config_path), config_info[2]))
     try:
         os.mkdir(log_directory)
@@ -131,22 +127,22 @@
         meta_info = config_meta_info
 
     console_switch = DEFAULT_CONSOLE_SWITCH
     config_console_switch = logging_config['console_switch']
     if config_console_switch:
         console_switch = config_console_switch
 
-    logger_level = DEFAULT_LOG_LEVEL
-    config_logger_level = logging_config['logger_level']
-    if config_logger_level:
-        logger_level = config_logger_level
+    level_colors = DEFAULT_LEVEL_COLORS
+    config_level_colors = logging_config['level_colors']
+    if config_level_colors:
+        level_colors = config_level_colors
 
     return_list = (file_switch, prefix, log_dir, file_log_level,
                    log_max_size, log_max_files, console_log_level,
-                   meta_info, console_switch, logger_level)
+                   meta_info, console_switch, level_colors)
     return return_list
 
 
 def log_transports_config(config_info, error_file: str, log_file: str):
     file = None
     rotate_file = None
 
@@ -167,28 +163,22 @@
 
 formatter = logging.Formatter(
     fmt='[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
     datefmt='%m-%d %H:%M:%S')
 
 
 def create_instance(config_info, transports_config):
-    logger = logging.getLogger(__name__)
-    logger.setLevel(config_info[9])
+    loguru_logger.remove()
     if config_info[0] == 'on' and isinstance(config_info[0], str):
         file_handler = transports_config['file']
-        file_handler.setLevel('ERROR')
-        file_handler.setFormatter(formatter)
-
+        loguru_logger.add(file_handler, level='ERROR')
         rotate_file_handler = transports_config['rotate_file']
-        rotate_file_handler.setLevel(config_info[3])
-        rotate_file_handler.setFormatter(formatter)
-
-        logger.addHandler(file_handler)
-        logger.addHandler(rotate_file_handler)
+        loguru_logger.add(rotate_file_handler, level=config_info[3])
 
     if config_info[8] == 'on' and isinstance(config_info[8], str):
         console_handler = transports_config['console_config']
-        console_handler.setLevel(config_info[6])
-        console_handler.setFormatter(formatter)
+        for level, color in config_info[9].items():
+            if color:
+                loguru_logger.level(level, color=f"<{color}><bold>")
+        loguru_logger.add(console_handler, colorize=True, level=config_info[6])
 
-        logger.addHandler(console_handler)
-    return logger
+        return loguru_logger
```

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/service/service_factory.py` & `agconnect-1.3.0.300/agconnect/common_server/src/service/service_factory.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/common_server/src/utils/utils.py` & `agconnect-1.3.0.300/agconnect/common_server/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/__init__.py` & `agconnect-1.3.0.300/agconnect/database_server/__init__.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/communicator/https_communicator.py` & `agconnect-1.3.0.300/agconnect/database_server/src/communicator/https_communicator.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/communicator/request_header.py` & `agconnect-1.3.0.300/agconnect/database_server/src/communicator/request_header.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/exception/agconnect_cloud_db_exception.py` & `agconnect-1.3.0.300/agconnect/database_server/src/exception/agconnect_cloud_db_exception.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/exception/cloud_db_error_code.py` & `agconnect-1.3.0.300/agconnect/database_server/src/exception/cloud_db_error_code.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/exception/error_code_message.py` & `agconnect-1.3.0.300/agconnect/database_server/src/exception/error_code_message.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_config.py` & `agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_config.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator.py` & `agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator_constraint.py` & `agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_object_operator_constraint.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/query/cloud_db_zone_query.py` & `agconnect-1.3.0.300/agconnect/database_server/src/query/cloud_db_zone_query.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/services/agconnect_cloud_db.py` & `agconnect-1.3.0.300/agconnect/database_server/src/services/agconnect_cloud_db.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/services/cloud_db_service.py` & `agconnect-1.3.0.300/agconnect/database_server/src/services/cloud_db_service.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/services/cloud_db_zone.py` & `agconnect-1.3.0.300/agconnect/database_server/src/services/cloud_db_zone.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/services/transaction.py` & `agconnect-1.3.0.300/agconnect/database_server/src/services/transaction.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/cloud_db_sdk_utils.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/cloud_db_sdk_utils.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/condition_type.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/condition_type.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/condition_validate.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/condition_validate.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/data_model_helper.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/data_model_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     if value is not None and type(
         value) is float and FLOAT_MIN_VALUE <= value <= FLOAT_MAX_VALUE and is_number(value) else False)
 
 add_validator(
     FieldType.Double,
     lambda value: True
     if value is not None and type(
-        value) is float and DOUBLE_MIN_VALUE <= value <= DOUBLE_MAX_VALUE
+        value) is float or type(value) is int and DOUBLE_MIN_VALUE <= value <= DOUBLE_MAX_VALUE
     else False
 )
 add_validator(
     FieldType.String,
     lambda value: True
     if isinstance(value, str) and len(value) <= MAX_STRING_LENGTH
     else False,
```

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/object_creator.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/object_creator.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/scheme_utils.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/scheme_utils.py`

 * *Files identical despite different names*

### Comparing `agconnect-1.2.0.300/agconnect/database_server/src/utils/utils.py` & `agconnect-1.3.0.300/agconnect/database_server/src/utils/utils.py`

 * *Files identical despite different names*

