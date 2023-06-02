# Comparing `tmp/msal_streamlit_authentication-1.0.8.tar.gz` & `tmp/msal_streamlit_authentication-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_streamlit_authentication-1.0.8.tar", max compression
+gzip compressed data, was "msal_streamlit_authentication-1.0.9.tar", max compression
```

## Comparing `msal_streamlit_authentication-1.0.8.tar` & `msal_streamlit_authentication-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3826 2023-04-28 22:59:42.840537 msal_streamlit_authentication-1.0.8/README.md
--rw-r--r--   0        0        0     1190 2023-04-28 22:59:42.844537 msal_streamlit_authentication-1.0.8/msal_streamlit_authentication/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-28 22:59:52.744474 msal_streamlit_authentication-1.0.8/msal_streamlit_authentication/frontend/dist/assets/index-4081600b.css
--rw-r--r--   0        0        0   732010 2023-04-28 22:59:52.744474 msal_streamlit_authentication-1.0.8/msal_streamlit_authentication/frontend/dist/assets/index-99fcc6ac.js
--rw-r--r--   0        0        0      399 2023-04-28 22:59:52.744474 msal_streamlit_authentication-1.0.8/msal_streamlit_authentication/frontend/dist/index.html
--rw-r--r--   0        0        0     1078 2023-04-28 22:59:42.844537 msal_streamlit_authentication-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 msal_streamlit_authentication-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3830 2023-06-02 09:13:47.785942 msal_streamlit_authentication-1.0.9/README.md
+-rw-r--r--   0        0        0     1190 2023-06-02 09:13:47.785942 msal_streamlit_authentication-1.0.9/msal_streamlit_authentication/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-02 09:13:58.602090 msal_streamlit_authentication-1.0.9/msal_streamlit_authentication/frontend/dist/assets/index-297265e4.css
+-rw-r--r--   0        0        0   732004 2023-06-02 09:13:58.602090 msal_streamlit_authentication-1.0.9/msal_streamlit_authentication/frontend/dist/assets/index-2ec6ec11.js
+-rw-r--r--   0        0        0      399 2023-06-02 09:13:58.602090 msal_streamlit_authentication-1.0.9/msal_streamlit_authentication/frontend/dist/index.html
+-rw-r--r--   0        0        0     1078 2023-06-02 09:13:47.789942 msal_streamlit_authentication-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 msal_streamlit_authentication-1.0.9/PKG-INFO
```

### Comparing `msal_streamlit_authentication-1.0.8/README.md` & `msal_streamlit_authentication-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This Streamlit component enables client-side authentication using [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) work and school accounts (AAD), Microsoft personal accounts (MSA) and social identity providers like Facebook, Google, LinkedIn, Microsoft accounts, etc. through [Azure AD B2C](https://docs.microsoft.com/azure/active-directory-b2c/active-directory-b2c-overview#identity-providers) service.
 The component is achieving this by applying the [Microsoft MSAL JS Library](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) inside of a React project. Since the component is based on MSAL, it can be configured to support any provider that supports the OpenID Connect Authorization Code Flow (PKCE).
 For more information on MSAL, consult the [Github project](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) and its [offical documentation](https://learn.microsoft.com/en-us/azure/active-directory/develop/msal-overview).
 
 ## Usage
 
-Below is a sample Python snippet displaying how to apply component. Visually, the component gives rise to a single button
+Below is a sample Python snippet displaying how to apply the component. Visually, the component gives rise to a single button
 in the Streamlit Dashboard with a text that depends on whether an active login session exists. The `auth` and `cache`
 parameters are entirely equivalent to the properties mentioned in the [Github documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/initialization.md).
 The `login_request` and `logout_request` parameters are covered [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/login-user.md).
 ```python
 import streamlit as st
 from msal_streamlit_authentication import msal_authentication
```

### Comparing `msal_streamlit_authentication-1.0.8/msal_streamlit_authentication/__init__.py` & `msal_streamlit_authentication-1.0.9/msal_streamlit_authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `msal_streamlit_authentication-1.0.8/msal_streamlit_authentication/frontend/dist/assets/index-99fcc6ac.js` & `msal_streamlit_authentication-1.0.9/msal_streamlit_authentication/frontend/dist/assets/index-2ec6ec11.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26097,41 +26097,41 @@
                         })]
                 }
             })
         })
     }, e
 }(hk);
 const pk = function(t, e) {
-    return new fk({
-        auth: t,
-        cache: e,
-        system: {
-            loggerOptions: {
-                loggerCallback: (r, n, i) => {
-                    if (!i) switch (r) {
-                        case ze.Error:
-                            console.error(n);
-                            return;
-                        case ze.Info:
-                            return;
-                        case ze.Verbose:
-                            console.debug(n);
-                            return;
-                        case ze.Warning:
-                            console.warn(n);
-                            return;
-                        default:
-                            return
+        return new fk({
+            auth: t,
+            cache: e,
+            system: {
+                loggerOptions: {
+                    loggerCallback: (r, n, i) => {
+                        if (!i) switch (r) {
+                            case ze.Error:
+                                console.error(n);
+                                return;
+                            case ze.Info:
+                                return;
+                            case ze.Verbose:
+                                console.debug(n);
+                                return;
+                            case ze.Warning:
+                                console.warn(n);
+                                return;
+                            default:
+                                return
+                        }
                     }
                 }
             }
-        }
-    })
-};
-const gk = ({
+        })
+    },
+    gk = ({
         args: t
     }) => {
         const e = pk(t.auth, t.cache),
             r = t.login_request ?? void 0,
             n = t.logout_request ?? void 0,
             i = t.login_button_text ?? "",
             s = t.logout_button_text ?? "",
```

### Comparing `msal_streamlit_authentication-1.0.8/pyproject.toml` & `msal_streamlit_authentication-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msal_streamlit_authentication"
-version = "1.0.8"
+version = "1.0.9"
 description = "Streamlit Authentication library based on MSAL.JS"
 readme = "README.md"
 repository = "https://github.com/mstaal/msal_streamlit_authentication"
 authors = ["Michael Staal-Olsen"]
 packages=[
     { include="msal_streamlit_authentication" }
 ]
```

### Comparing `msal_streamlit_authentication-1.0.8/PKG-INFO` & `msal_streamlit_authentication-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal-streamlit-authentication
-Version: 1.0.8
+Version: 1.0.9
 Summary: Streamlit Authentication library based on MSAL.JS
 Home-page: https://github.com/mstaal/msal_streamlit_authentication
 Author: Michael Staal-Olsen
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 
 This Streamlit component enables client-side authentication using [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) work and school accounts (AAD), Microsoft personal accounts (MSA) and social identity providers like Facebook, Google, LinkedIn, Microsoft accounts, etc. through [Azure AD B2C](https://docs.microsoft.com/azure/active-directory-b2c/active-directory-b2c-overview#identity-providers) service.
 The component is achieving this by applying the [Microsoft MSAL JS Library](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) inside of a React project. Since the component is based on MSAL, it can be configured to support any provider that supports the OpenID Connect Authorization Code Flow (PKCE).
 For more information on MSAL, consult the [Github project](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) and its [offical documentation](https://learn.microsoft.com/en-us/azure/active-directory/develop/msal-overview).
 
 ## Usage
 
-Below is a sample Python snippet displaying how to apply component. Visually, the component gives rise to a single button
+Below is a sample Python snippet displaying how to apply the component. Visually, the component gives rise to a single button
 in the Streamlit Dashboard with a text that depends on whether an active login session exists. The `auth` and `cache`
 parameters are entirely equivalent to the properties mentioned in the [Github documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/initialization.md).
 The `login_request` and `logout_request` parameters are covered [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/login-user.md).
 ```python
 import streamlit as st
 from msal_streamlit_authentication import msal_authentication
```

