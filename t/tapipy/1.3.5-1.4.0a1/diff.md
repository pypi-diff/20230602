# Comparing `tmp/tapipy-1.3.5.tar.gz` & `tmp/tapipy-1.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapipy-1.3.5.tar", max compression
+gzip compressed data, was "tapipy-1.4.0a1.tar", max compression
```

## Comparing `tapipy-1.3.5.tar` & `tapipy-1.4.0a1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.3.5/LICENSE.md
--rw-r--r--   0        0        0     8639 2023-05-31 22:55:27.557819 tapipy-1.3.5/README.md
--rw-r--r--   0        0        0      970 2023-06-02 16:27:40.254545 tapipy-1.3.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-02 16:32:05.527543 tapipy-1.3.5/tapipy/__init__.py
--rw-r--r--   0        0        0    13502 2023-05-31 22:55:11.637942 tapipy-1.3.5/tapipy/actors.py
--rw-r--r--   0        0        0     2071 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/errors.py
--rw-r--r--   0        0        0    38703 2023-06-02 16:26:38.119280 tapipy-1.3.5/tapipy/resources/openapi_v3-actors.yml
--rw-r--r--   0        0        0    65123 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/resources/openapi_v3-apps.yml
--rw-r--r--   0        0        0    23782 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/resources/openapi_v3-authenticator.yml
--rw-r--r--   0        0        0    74553 2023-06-02 16:30:47.592405 tapipy-1.3.5/tapipy/resources/openapi_v3-files.yml
--rw-r--r--   0        0        0    65915 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/resources/openapi_v3-jobs.yml
--rw-r--r--   0        0        0    28625 2023-05-31 20:34:22.484233 tapipy-1.3.5/tapipy/resources/openapi_v3-meta.yml
--rw-r--r--   0        0        0    52055 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/resources/openapi_v3-notifications.yml
--rw-r--r--   0        0        0    33814 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/resources/openapi_v3-pgrest.yml
--rw-r--r--   0        0        0    63213 2023-05-31 22:55:27.557819 tapipy-1.3.5/tapipy/resources/openapi_v3-pods.yml
--rw-r--r--   0        0        0   145319 2023-05-31 22:55:27.561818 tapipy-1.3.5/tapipy/resources/openapi_v3-sk.yml
--rw-r--r--   0        0        0   108752 2023-05-31 22:55:27.561818 tapipy-1.3.5/tapipy/resources/openapi_v3-streams.yml
--rw-r--r--   0        0        0    95703 2023-05-31 22:55:27.561818 tapipy-1.3.5/tapipy/resources/openapi_v3-systems.yml
--rw-r--r--   0        0        0    25448 2023-05-31 20:34:25.512199 tapipy-1.3.5/tapipy/resources/openapi_v3-tenants.yml
--rw-r--r--   0        0        0     8406 2023-05-31 22:55:27.561818 tapipy-1.3.5/tapipy/resources/openapi_v3-tokens.yml
--rw-r--r--   0        0        0    87200 2023-06-02 16:30:54.648327 tapipy-1.3.5/tapipy/resources/openapi_v3-workflows.yml
--rw-r--r--   0        0        0      907 2023-06-02 16:30:55.212320 tapipy-1.3.5/tapipy/resources/resource_etags.json
--rw-r--r--   0        0        0    49081 2023-06-02 16:30:58.068289 tapipy-1.3.5/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle
--rw-r--r--   0        0        0    30512 2023-06-02 16:30:55.740315 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
--rw-r--r--   0        0        0    49346 2023-06-02 16:30:58.700282 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
--rw-r--r--   0        0        0    19592 2023-06-02 16:30:55.844313 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
--rw-r--r--   0        0        0    56349 2023-06-02 16:30:56.248309 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
--rw-r--r--   0        0        0    49993 2023-06-02 16:30:58.380285 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
--rw-r--r--   0        0        0    21718 2023-06-02 16:30:55.960312 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
--rw-r--r--   0        0        0    40427 2023-06-02 16:30:58.888280 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
--rw-r--r--   0        0        0    27737 2023-06-02 16:30:57.796292 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
--rw-r--r--   0        0        0   117394 2023-06-02 16:30:56.700304 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
--rw-r--r--   0        0        0    81328 2023-06-02 16:30:57.124299 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
--rw-r--r--   0        0        0    73772 2023-06-02 16:30:57.488295 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
--rw-r--r--   0        0        0    20570 2023-06-02 16:30:57.604294 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
--rw-r--r--   0        0        0     7112 2023-06-02 16:30:57.656293 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
--rw-r--r--   0        0        0    64540 2023-06-02 16:31:00.360263 tapipy-1.3.5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
--rw-r--r--   0        0        0    70890 2023-06-02 16:26:47.819164 tapipy-1.3.5/tapipy/tapis.py
--rw-r--r--   0        0        0      695 2023-06-02 16:26:47.819164 tapipy-1.3.5/tapipy/util.py
--rw-r--r--   0        0        0    10018 1970-01-01 00:00:00.000000 tapipy-1.3.5/setup.py
--rw-r--r--   0        0        0    10051 1970-01-01 00:00:00.000000 tapipy-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.4.0a1/LICENSE.md
+-rw-r--r--   0        0        0     8639 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/README.md
+-rw-r--r--   0        0        0      972 2023-06-02 19:05:02.492889 tapipy-1.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/__init__.py
+-rw-r--r--   0        0        0    13502 2023-05-31 22:55:11.637942 tapipy-1.4.0a1/tapipy/actors.py
+-rw-r--r--   0        0        0     2071 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/errors.py
+-rw-r--r--   0        0        0    38703 2023-06-02 16:26:38.119280 tapipy-1.4.0a1/tapipy/resources/openapi_v3-actors.yml
+-rw-r--r--   0        0        0    65123 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/resources/openapi_v3-apps.yml
+-rw-r--r--   0        0        0    23782 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/resources/openapi_v3-authenticator.yml
+-rw-r--r--   0        0        0    73802 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/resources/openapi_v3-files.yml
+-rw-r--r--   0        0        0    65915 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/resources/openapi_v3-jobs.yml
+-rw-r--r--   0        0        0    28625 2023-05-31 20:34:22.484233 tapipy-1.4.0a1/tapipy/resources/openapi_v3-meta.yml
+-rw-r--r--   0        0        0    52055 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/resources/openapi_v3-notifications.yml
+-rw-r--r--   0        0        0    33814 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/resources/openapi_v3-pgrest.yml
+-rw-r--r--   0        0        0    63213 2023-05-31 22:55:27.557819 tapipy-1.4.0a1/tapipy/resources/openapi_v3-pods.yml
+-rw-r--r--   0        0        0   145319 2023-05-31 22:55:27.561818 tapipy-1.4.0a1/tapipy/resources/openapi_v3-sk.yml
+-rw-r--r--   0        0        0   108752 2023-05-31 22:55:27.561818 tapipy-1.4.0a1/tapipy/resources/openapi_v3-streams.yml
+-rw-r--r--   0        0        0    95703 2023-05-31 22:55:27.561818 tapipy-1.4.0a1/tapipy/resources/openapi_v3-systems.yml
+-rw-r--r--   0        0        0    25448 2023-05-31 20:34:25.512199 tapipy-1.4.0a1/tapipy/resources/openapi_v3-tenants.yml
+-rw-r--r--   0        0        0     8406 2023-05-31 22:55:27.561818 tapipy-1.4.0a1/tapipy/resources/openapi_v3-tokens.yml
+-rw-r--r--   0        0        0    87325 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/resources/openapi_v3-workflows.yml
+-rw-r--r--   0        0        0      785 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/resources/resource_etags.json
+-rw-r--r--   0        0        0    61852 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle
+-rw-r--r--   0        0        0    27037 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
+-rw-r--r--   0        0        0    69940 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
+-rw-r--r--   0        0        0    17736 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
+-rw-r--r--   0        0        0    54861 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
+-rw-r--r--   0        0        0    57550 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
+-rw-r--r--   0        0        0    14366 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
+-rw-r--r--   0        0        0    36903 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
+-rw-r--r--   0        0        0    23333 2023-06-02 19:03:59.121677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
+-rw-r--r--   0        0        0    99591 2023-06-02 19:03:59.125677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
+-rw-r--r--   0        0        0    75745 2023-06-02 19:03:59.125677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
+-rw-r--r--   0        0        0    77699 2023-06-02 19:03:59.125677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
+-rw-r--r--   0        0        0    20306 2023-06-02 19:03:59.125677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
+-rw-r--r--   0        0        0     5985 2023-06-02 19:03:59.125677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
+-rw-r--r--   0        0        0   156006 2023-06-02 19:03:59.125677 tapipy-1.4.0a1/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
+-rw-r--r--   0        0        0    71478 2023-06-02 19:03:59.129677 tapipy-1.4.0a1/tapipy/tapis.py
+-rw-r--r--   0        0        0     3297 2023-06-02 19:03:59.129677 tapipy-1.4.0a1/tapipy/util.py
+-rw-r--r--   0        0        0    10020 1970-01-01 00:00:00.000000 tapipy-1.4.0a1/setup.py
+-rw-r--r--   0        0        0    10003 1970-01-01 00:00:00.000000 tapipy-1.4.0a1/PKG-INFO
```

### Comparing `tapipy-1.3.5/LICENSE.md` & `tapipy-1.4.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/README.md` & `tapipy-1.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/actors.py` & `tapipy-1.4.0a1/tapipy/actors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/errors.py` & `tapipy-1.4.0a1/tapipy/errors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-actors.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-actors.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-apps.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-apps.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-authenticator.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-authenticator.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-files.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-files.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.3
 info:
   title: Tapis Files API
   description: The Tapis Files API provides for management of file resources on Tapis systems
-  version: '1.3.6'
+  version: '1.3.5'
   termsOfService: "https://tapis-project.org"
   contact:
     name: "Files API - CICSupport"
     url: "https://tapis-project.org"
     email: "cicsupport@tacc.utexas.edu"
   license:
     name: 3-Clause BSD License
@@ -23,24 +23,19 @@
     variables: {}
 security:
   - TapisJWT: []
 tags:
   - name: General
     description: General service health and readiness
   - name: File Operations
-    description: |
-      Manage file resources on Tapis systems. List, upload, copy, native operations, etc.
-      Note that not all operations are supported for all system types.
+    description: Manage file resources on Tapis systems. List, upload, copy, native operations, etc.
   - name: Content
-    description: Download a file or directory. Not supported for all system types.
+    description: Download a file or directory.
   - name: Transfers
-    description: |
-      Manage file transfers between two systems. Initiate, cancel and retrieve status.
-      Note that not all combinations of system types are supported. For example, transfers involving a GLOBUS
-      system must be GLOBUS to GLOBUS.
+    description: Manage file transfers. Initiate, cancel and retrieve status.
   - name: Permissions
     description: |
       The permissions model allows for fine grained access control of paths on a Tapis system. The system owner
       may grant READ and MODIFY permission to specific users. MODIFY implies READ.
   
       Please note that Tapis also supports a higher level approach to granting access known as *Sharing*.
 
@@ -198,16 +193,16 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/FileStringResponse'
     put:
       tags:
         - File Operations
       description: |
-        Move or copy a file, directory or object on {systemID} at path {path}.
-        Not all operations supported for all system types.
+        Move or copy a file, directory or object on {systemID} at path {path}. Not all operations supported for all
+        system types.
       operationId: moveCopy
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -388,21 +383,19 @@
                 $ref: '#/components/schemas/FileStringResponse'
   /v3/files/ops/{systemId}:
     post:
       tags:
         - File Operations
       description: |
         Create a directory on the system at the given path. Not supported for all system types. Currently supported
-        for LINUX, IRODS and GLOBUS type systems.
+        for LINUX and IRODS type systems.
 
         Certain services may use the query parameter *sharedCtx* to indicate that the request is in a shared
         context. *sharedCtx* must be set to the share grantor.
         Tapis will include the share grantor as part of authorization checks.
-
-        If the path already exists as a directory, no error will be returned.
       operationId: mkdir
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -586,15 +579,15 @@
                 $ref: '#/components/schemas/FileStringResponse'
 
   /v3/files/utils/linux/facl/{systemId}/{path}:
     get:
       tags:
         - File Operations
       description: |
-        Get file ACLs for files or directories for a system of type LINUX.
+        Get file ACLs for files or directories.
       operationId: getFacl
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -638,15 +631,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/FileStringResponse'
     post:
       tags:
         - File Operations
       description: |
-        Set file ACLs for files or directories for a system of type LINUX.
+        Set file ACLs for files or directories.
 
         This can be used for a single file or directory, or can be recursive.  If recursion is
         used, it can be made to follow symlinks, or not follow symlinks.
 
         The operations support adding or removing Acl Entries as well as removing all acls or all
         default acls
       operationId: setFacl
@@ -819,16 +812,14 @@
               schema:
                 $ref: '#/components/schemas/TransferTaskListResponse'
     post:
       tags:
         - Transfers
       description: |
         Create a background task which will transfer files between systems.
-        Note that not all combinations of system types are supported. For example, transfers involving a GLOBUS
-        system must be GLOBUS to GLOBUS.
       operationId: createTransferTask
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ReqTransfer'
         required: true
@@ -1680,15 +1671,15 @@
     # --- FileInfo -----------------------------------------------------------------
     FileInfo:
       type: object
       properties:
         mimeType:
           type: string
         type:
-          $ref: '#/components/schemas/FileTypeEnum'
+          type: string
         owner:
           type: string
         group:
           type: string
         nativePermissions:
           type: string
         url:
@@ -2461,16 +2452,8 @@
         - MODIFY
     ListTypeEnum:
       type: string
       default: OWNED
       enum:
         - OWNED
         - ALL
-    FileTypeEnum:
-      type: string
-      enum:
-        - file
-        - dir
-        - symbolic_link
-        - other
-        - unknown
```

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-jobs.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-jobs.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-meta.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-meta.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-notifications.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-notifications.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-pgrest.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-pgrest.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-pods.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-pods.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-sk.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-sk.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-streams.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-streams.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-systems.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-systems.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-tenants.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-tenants.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-tokens.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-tokens.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.5/tapipy/resources/openapi_v3-workflows.yml` & `tapipy-1.4.0a1/tapipy/resources/openapi_v3-workflows.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2187,36 +2187,41 @@
           type: string
 
     Event:
       type: object
       properties:
         branch:
           type: string
+          nullable: true
           default: null
         commit:
+          nullable: true
           type: string
           default: null
         commit_sha:
           type: string
+          nullable: true
           default: null
         context_url:
           type: string
+          nullable: true
           default: null
         directives:
           type: string
         message:
           type: string
         pipeline:
           type: string
         source:
           type: string
         username:
           $ref: '#/components/schemas/Username'
         identity:
           type: string
+          nullable: true
           default: null
         uuid:
           type: string
           format: uuid
 
     # --- String types with constraints ------------------------------------
     ID:
```

### Comparing `tapipy-1.3.5/tapipy/resources/resource_etags.json` & `tapipy-1.4.0a1/tapipy/resources/resource_etags.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8666666666666667%*

 * *Differences: {'delete': "['files', 'workflows']"}*

```diff
@@ -1,17 +1,15 @@
 {
     "actors": "W/\"790d47ac8c8c65e702080db8e564c154ee3ba420\"",
     "apps": "W/\"0a4a20d1bc8b11ff2733248cfc30821ddd4324f7\"",
     "authenticator": "W/\"16fca2e73ad502ffcc2da2c755df8d3abf680a6e\"",
-    "files": "W/\"ee9feff01143ad76c0cc8cfd66c4c2706e0226a8\"",
     "jobs": "W/\"eceba29d169471ccee3d1a1d0db8bff8374fffe2\"",
     "meta": "W/\"e49bc20f1b1e3296278db40fdd6b33d92c44beea\"",
     "notifications": "W/\"897fb360129add26d02c77562f7ee168ce8f7625\"",
     "pgrest": "W/\"6494d146379036fdd95de0ed7da22d1bec1335cd\"",
     "pods": "W/\"3a0278fd3115296c03324d28cd449ce8aa4d8793\"",
     "sk": "W/\"1d60d95dc6576e129817e90c107bd4daf0200e4c\"",
     "streams": "W/\"d48bb1cdc3a01f8b4b42ecacc9f41585c29a660b\"",
     "systems": "W/\"c0f9059da975bd80b9911958945521765ec020b8\"",
     "tenants": "W/\"19937e762737fba432a63c8f32e824c182d2e973\"",
-    "tokens": "W/\"8de22c7d82f2ba9906e937cb1da1610007319e45\"",
-    "workflows": "W/\"fc3153b26218559770d10ed10e7b8743b9c430a8\""
+    "tokens": "W/\"8de22c7d82f2ba9906e937cb1da1610007319e45\""
 }
```

### Comparing `tapipy-1.3.5/tapipy/tapis.py` & `tapipy-1.4.0a1/tapipy/tapis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 from collections.abc import Sequence
 import datetime
 import importlib
 import json
 import jwt
 import os
 import requests
-from openapi_core import create_spec
-from openapi_core.schema.parameters.enums import ParameterLocation
+from openapi_core import Spec
+from jsonschema_spec.handlers.file import BaseFilePathHandler
 import yaml
-from . import errors
 import pickle
 import shutil
+import time
 import concurrent.futures
 import copy
 from typing import Dict, NewType, Mapping, Optional
 from atomicwrites import atomic_write
-import openapi_core
 
+from tapipy.util import dereference_spec
 import tapipy.errors
+from . import errors
+
+start_time = time.time()
 
 # Type declarations
 ResourceName = NewType('ResourceName', str)
 ResourceUrl = NewType('ResourceUrl', str)
 SpecPath = NewType('SpecPath', str)
-OpenApiSpec = NewType('OpenApiSpec', openapi_core.schema.specs.models.Spec)
+OpenApiSpec = NewType('OpenApiSpec', Spec)
 Resources = Dict[ResourceName, ResourceUrl]
 Specs = Dict[ResourceName, OpenApiSpec]
 ResourceInfo = Mapping[ResourceName, SpecPath]
 
 
 def _seq_but_not_str(obj: object) -> bool:
     """
@@ -66,15 +69,15 @@
         'files': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-files.yml',
         'sk': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-sk.yml',
         'streams': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-streams.yml',
         'systems': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-systems.yml',
         'tenants': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-tenants.yml',
         'tokens': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-tokens.yml',
         'pgrest': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-pgrest.yml',
-        'pods': 'https://raw.githubusercontent.com/tapis-project/pods_service/prod/docs/openapi_v3-pods.yml',
+        'pods': 'https://raw.githubusercontent.com/tapis-project/tapipy/main/tapipy/resources/openapi_v3-pods.yml',
         'jobs': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-jobs.yml',
         'apps': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-apps.yml',
         'workflows': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-workflows.yml',
         'notifications': 'https://raw.githubusercontent.com/tapis-project/tapipy/prod/tapipy/resources/openapi_v3-notifications.yml'
     },
     'prod': {
         'actors': 'https://raw.githubusercontent.com/TACC/abaco/prod-v3/docs/specs/openapi_v3.yml',               
@@ -173,41 +176,51 @@
     # Set off some parallel processes cause it's quick.
     #POOL_SIZE = os.environ.get('POOL_SIZE', 16)
     #pool = multiprocessing.Pool(processes=POOL_SIZE)
     #pool.map(_thread_download_spec_dict, urls_to_download)
     #pool.close()
     #pool.join()
 
+from urllib.parse import urlparse
+def new_call(self, uri):
+    if hasattr(uri, 'read'):
+        return super(BaseFilePathHandler, self).__call__(uri)
+    
+    parsed_url = urlparse(uri)
+    if parsed_url.scheme not in self.allowed_schemes:
+        raise ValueError("Not allowed scheme")
+
+    return self._open(uri)
+
+BaseFilePathHandler.__call__ = new_call
+
 
 def _thread_download_spec_dict(resource_info: ResourceInfo) -> None:
     """
     Function that multiprocessing pool calls to download and store pickled
     spec dicts. Gets spec dict, if it's valid, stores it at 'spec_path',
     else it does nothing.
     """
     resource_name, resource_url, spec_path = resource_info
     # Attempt to get spec from url
     response = requests.get(resource_url)
     if response.status_code == 200:
         try:
-            # Loads yaml into Python dictionary
-            spec_dict = yaml.load(response.content, Loader=yaml.FullLoader)
+            # Directly creates spec from response. This validates spec as valid.
+            spec = Spec.from_file(response.content)
         except Exception as e:
-            print(f'Got exception when attempting to load yaml for '
-                  f'"{resource_name}" resource; exception: {e}')
+            print(f'Got exception when test creating spec for "{resource_name}" '
+                  f'resource; Spec probably not verifying; exception: {e}')
             return
         try:
-            # Attempts to create spec from dict to ensure the spec is valid
-            # We do a deepcopy as create_spec for some reason adds fields
-            # to the dictionary that's given
-            test_spec_dict = copy.deepcopy(spec_dict)
-            create_spec(test_spec_dict)
+            # Dereference spec so we have a dict we can pickle.
+            spec_dict = dereference_spec(spec)
         except Exception as e:
-            print(f'Got exception when test creating spec for "{resource_name}" '
-                  f'resource; Spec probably not verifying; exception: {e}')
+            print(f'Got exception when derefrencing spec for "{resource_name}" '
+                  f'resource; exception: {e}')
             return
         try:
             # Pickles and saves the spec dict to the spec_path atomically
             with atomic_write(f'{spec_path}', overwrite=True, mode='wb') as spec_file:
                 pickle.dump(spec_dict, spec_file, protocol=4)
         except Exception as e:
             print(f'Got exception when attempting to pickle spec_dict for '
@@ -226,45 +239,45 @@
     specs = {}
     dicts = {}
     # Get resource path to point the unpickling at.
     for resource_name, url in resources.items():
         if "local:" in url:
             try:
                 spec_path = url.replace('local:', '').strip()
-                with open(spec_path, 'rb') as spec_file:
-                    spec_dict = yaml.load(spec_file, Loader=yaml.FullLoader)
-                specs.update({resource_name: create_spec(spec_dict)})
+                spec = Spec.from_file_path(spec_path)
+                spec_dict = dereference_spec(spec)
+                specs.update({resource_name: spec_dict})
                 dicts.update({resource_name: spec_dict})
             except Exception as e:
                 print(f'Error reading local "{resource_name}" resource. '
-                      f'Ensure path is absolute. e:{e}')
+                      f'Ensure path is absolute {spec_path}. e:{e}')
             continue
         _, _, spec_path = get_file_info_from_url(url, spec_dir)
         try:
             # Unpickle and create_spec
             with open(spec_path, 'rb') as spec_file:
                 spec_dict = pickle.load(spec_file)
-            specs.update({resource_name: create_spec(spec_dict)})
+            specs.update({resource_name: spec_dict})
             dicts.update({resource_name: spec_dict})
         except Exception as e:
-            print(f'Got exception trying to unpickle and create spec for '
+            print(f'Got exception trying to unpickle spec for '
                   f'spec_path: "{resource_name}"; exception: {e}')
             # Using resource name to look if the resource exists in the
             # tapipy prod resources. If it is found, we fall back and use that!
             # If it isn't we just skip it.
             print(f'Falling back to prod spec for "{resource_name}" resource')
             if resource_name in RESOURCES['tapipy']:
                 url = RESOURCES['tapipy'][resource_name]
                 _, _, spec_path = get_file_info_from_url(url, spec_dir)
                 try:
                     # Unpickle and create_spec
                     with open(spec_path, 'rb') as spec_file:
-                        spec_dict = pickle.load(spec_file)
-                    specs.update({resource_name: create_spec(spec_dict)})
-                    dicts.update({resource_name: spec_dict})
+                        spec = pickle.load(spec_file)
+                    specs.update({resource_name: spec})
+                    dicts.update({resource_name: spec})
                 except Exception as e:
                     print('Error opening tapipy prod spec. This is bad.')
             else:
                 print(f'No "{resource_name}" spec was found to fallback on')
     return specs, dicts
 
 
@@ -315,15 +328,19 @@
                                       f"to your specifed spec_dir at '{spec_dir}.'")
     else:
         # Fallback on the spec folder from the Tapipy package directory
         spec_dir = os.path.join(os.path.dirname(__file__), 'specs')
     return spec_dir
     
 
+print(f"TIMING: Before _get_specs for tapipy resources: Took: {time.time() - start_time} seconds")
+before_time = time.time()
 RESOURCE_SPECS, RESOURCE_DICTS = _get_specs(RESOURCES['tapipy'])
+print(f"TIMING: After _get_specs for tapipy resources: Took: {time.time() - before_time} seconds for get_specs")
+print(f"TIMING: After _get_specs for tapipy resources: Took: {time.time() - start_time} seconds from start")
 
 
 def get_basic_auth_header(username: str, password: str) -> str:
     """
     Convenience function with will return a properly formatted Authorization
     header from a username and password.
     """
@@ -479,15 +496,15 @@
             resource_specs, self.resource_dicts = _get_specs(RESOURCES[resource_set], spec_dir=self.spec_dir, download_latest_specs=self.download_latest_specs)
         else:
             resource_specs, self.resource_dicts = RESOURCE_SPECS, RESOURCE_DICTS
 
         # create resources for each API defined above. In the future we could make this more dynamic in multiple ways.
         for resource_name, spec in resource_specs.items():
             # each API is a top-level attribute on the DynaTapy object, a Resource object constructed as follows:
-            setattr(self, resource_name, Resource(resource_name, spec.paths, self))
+            setattr(self, resource_name, Resource(resource_name, spec['paths'], self))
 
         # deal with plugins
         self.plugins = plugins
         # callables plugins can set that get executed within self.<resource>.<operation>.__call__() BEFORE the 
         # prepared request is sent to the Tapis API server.
         # method signature should be def fn(op: Opertaion, request: PreparedRequest, **kwargs)
         self.plugin_on_call_pre_request_callables = []
@@ -920,54 +937,55 @@
 
         # resource_spec is the associated definition from the spec file.
         self.resource_spec = resource_spec
 
         # tapis_client stores configuration data (api_server, token, etc..)
         self.tapis_client = tapis_client
 
-        # Here we create an attr on the object for each operation_id in the spec. The attr is itself an
+        # Here we create an attr on the object for each operationId in the spec. The attr is itself an
         # Operation object, defined below, with a special __call__ method.
-        # Examples operation_id's inclue "list_files", "upload_file", etc...
+        # Examples operationId's include "list_files", "upload_file", etc...
         for path_name, path_desc in self.resource_spec.items():
             # Each path_desc is an openapi_core.schema.paths.models.Path object
             # it has an operations object, which is a dictionary of operations associated with the path:
-            for op, op_desc in path_desc.operations.items():
+            for op, op_desc in path_desc.items():
                 # each op_desc is an openapi_core.schema.operations.models.Operation object.
-                # the op_desc has a number of associated attributes, including operation_id, parameters, path_name, etc.
+                # the op_desc has a number of associated attributes, including operationId, parameters, etc.
                 # we create an Operation object for each one of these:
-                if not op_desc.operation_id:
-                    print(f"invalid op_dec for {resource_name}; missing operation_id. op_dec: {op_desc}")
+                if not op_desc["operationId"]:
+                    print(f"invalid op_dec for {resource_name}; missing operationId. op_desc: {op_desc}")
                     continue
-                setattr(self, op_desc.operation_id, Operation(self.resource_name, op_desc, self.tapis_client))
+                setattr(self, op_desc["operationId"], Operation(self.resource_name, op_desc, path_name, op, self.tapis_client))
 
 
 class Operation(object):
     """
     Represents a single operation on an API resource defined by an OpenAPI spec file.
-    Operation objects are in one-to-one correspondence with operation_id's defined in the spec file.
+    Operation objects are in one-to-one correspondence with operationId's defined in the spec file.
     """
 
-    def __init__(self, resource_name, op_desc, tapis_client):
+    def __init__(self, resource_name, op_desc, path_name, http_method, tapis_client):
         """
         Instantiate an operation. The op_desc should an openapi_core Operation object associated with the operation.
         :param resource_name: (str) The resource associated with this operation.
         :param op_desc: (openapi_core.schema.operations.models.Operation) OpenAPI description of the operation.
         :param tapis_client: Pointer to the Tapis object to which this resource will be attached.
         :return:
         """
         self.resource_name = resource_name
         self.op_desc = op_desc
+        self.path_name = path_name
+        self.http_method = http_method
         self.tapis_client = tapis_client
 
         # derived attributes - for convenience
-        self.operation_id = op_desc.operation_id
-        self.http_method = op_desc.http_method
-        self.path_parameters = [p for _, p in op_desc.parameters.items() if p.location == ParameterLocation.PATH]
-        self.query_parameters = [p for _, p in op_desc.parameters.items() if p.location == ParameterLocation.QUERY]
-        self.request_body = op_desc.request_body
+        self.operation_id = op_desc["operationId"]
+        self.path_parameters = [p for p in op_desc.get('parameters', []) if p['in'] == 'path']
+        self.query_parameters = [p for p in op_desc.get('parameters', []) if p['in'] == 'query']
+        self.request_body = op_desc.get('requestBody', {})
 
     def __call__(self, **kwargs):
         """
         Turns the operation object into a callable. Arguments must be passed as kwargs, where the name of each kwarg
         corresponds to a "parameter" in the OpenApi definition. Here, parameter could be a path parameter, body
         parameter, or query parameter.
 
@@ -980,54 +998,55 @@
 
         # use the base_url set on the client --
         base_url = self.tapis_client.base_url
 
         # construct the http path -
         # some API definitions, such as SK, chose to not include the "/v3/" at the beginning of their paths,
         # so we add it in:
-        if not self.op_desc.path_name.startswith('/v3/'):
-            self.url = f'{base_url}/v3{self.op_desc.path_name}'  # base url
+        if not self.path_name.startswith('/v3/'):
+            self.url = f'{base_url}/v3{self.path_name}'  # base url
         else:
-            self.url = f'{base_url}{self.op_desc.path_name}'  # base url
+            self.url = f'{base_url}{self.path_name}'  # base url
+
         url = self.url
         for param in self.path_parameters:
             # look for the name in the kwargs
-            if param.required:
-                if param.name not in kwargs:
-                    raise errors.InvalidInputError(msg=f"{param.name} is a required argument.")
-            p_val = kwargs.pop(param.name)
+            if param.get("required"):
+                if param["name"] not in kwargs:
+                    raise errors.InvalidInputError(msg=f"{param['name']} is a required argument.")
+            p_val = kwargs.pop(param["name"])
             if isinstance(p_val, int):
                 p_val = str(p_val)
             if isinstance(p_val, float):
                 p_val = str(p_val)
-            if param.required and not p_val:
-                raise errors.InvalidInputError(msg=f"{param.name} is a required argument and cannot be None.")
+            if param.get("required") and not p_val:
+                raise errors.InvalidInputError(msg=f"{param['name']} is a required argument and cannot be None.")
             # replace the parameter in the path template with the parameter value
-            s = '{' + f'{param.name}' + '}'
+            s = '{' + f'{param["name"]}' + '}'
             url = url.replace(s, p_val)
 
         # check for the _tapis_debug flag for generating debug data
         debug = False
         if '_tapis_debug' in kwargs:
             debug = kwargs.get('_tapis_debug', False)
             # ignore non-boolean values for the debug flag and set it to False.
             if not type(debug) == bool:
                 debug = False
 
         # construct the http query parameters -
         params = {}
         for param in self.query_parameters:
             # look for the name in the kwargs
-            if param.required:
-                if param.name not in kwargs:
-                    raise errors.InvalidInputError(msg=f"{param.name} is a required argument.")
+            if param.get("required"):
+                if param["name"] not in kwargs:
+                    raise errors.InvalidInputError(msg=f"{param['name']} is a required argument.")
             # only set the parameter if it was actually sent in the function -
-            if param.name in kwargs:
-                p_val = kwargs.pop(param.name, None)
-                params[param.name] = p_val
+            if param["name"] in kwargs:
+                p_val = kwargs.pop(param["name"], None)
+                params[param["name"]] = p_val
         
         # allow arbitrary query parameters to b passed in via the special "_tapis_query_parameters" kwarg --
         if '_tapis_query_parameters' in kwargs:
             try:
                 params.update(kwargs.pop('_tapis_query_parameters'))
             except ValueError:
                 raise errors.InvalidInputError(
@@ -1087,75 +1106,77 @@
                 raise errors.InvalidInputError(
                     msg="The headers argument, if passed, must be a dictionary-like object.")
 
         # construct the data -
         data = None
         files = None
         # these are the list of allowable request body content types; ex., 'application/json'.
-        if hasattr(self.op_desc.request_body, 'content') and hasattr(self.op_desc.request_body.content, 'keys'):
+        if 'content' in self.request_body and hasattr(self.request_body['content'], 'keys'):
             # Find possible headers, user specified
             # headers override spec's possibilities.
             if 'Content-Type' in headers:
-                requestContentTypes = headers['Content-Type']
+                request_content_types = headers['Content-Type']
             else:
-                requestContentTypes = self.op_desc.request_body.content.keys()
+                request_content_types = self.request_body['content'].keys()
 
             # Note: If multiple content types, we use first content type we have code for
-            if 'application/json' in requestContentTypes:
+            if 'application/json' in request_content_types:
                 headers['Content-Type'] = 'application/json'
-                required_fields = self.op_desc.request_body.content['application/json'].schema.required
+                required_fields = self.request_body['content']['application/json']['schema'].get('required', {})
+
                 data = {}
                 # if the request body has no defined properties, look for a single "request_body" parameter.
-                if self.op_desc.request_body.content['application/json'].schema.properties == {}:
+                if self.request_body['content']['application/json']['schema']['properties'] == {}:
                     # choice of "request_body" is arbitrary, as the property name is not provided by the
                     # openapi spec in this case
                     data = kwargs['request_body']
                 else:
                     # otherwise, the request body has defined properties, so look for each one in the function kwargs
-                    for p_name, p_desc in self.op_desc.request_body.content['application/json'].schema.properties.items():
+                    for p_name, p_desc in self.request_body['content']['application/json']['schema']['properties'].items():
                         if p_name in kwargs:
                             data[p_name] = kwargs[p_name]
                         elif p_name in required_fields:
                             raise errors.InvalidInputError(msg=f'{p_name} is a required argument.')
                     # serialize data before passing it to the request
                 data = json.dumps(data)
-            elif 'application/octet-stream' in requestContentTypes:
+            elif 'application/octet-stream' in request_content_types:
                 headers['Content-Type'] = 'application/octet-stream'
                 data = kwargs['message']
             # x-www-form-urlencoded
-            elif 'application/x-www-form-urlencoded' in requestContentTypes:
+            elif 'application/x-www-form-urlencoded' in request_content_types:
                 headers['Content-Type'] = 'application/x-www-form-urlencoded'
                 data = f"message={kwargs['message']}"
-            elif 'multipart/form-data' in requestContentTypes:
+            elif 'multipart/form-data' in request_content_types:
                 # We DO NOT set multipart/form-data headers. The requests library will do header creation for us.
                 # multipart/form-data should use request.Request(files={"formpart1": "formdata1", "formpart2": "formdata2}, ...)
                 # With the files arg, requests will set the Content-Type, boundary and Content-Length headers for us.
                 # It doesn't seem to work if we set Content-Type ourselves.
                 # headers['Content-Type'] = 'multipart/form-data'
 
-                required_fields = self.op_desc.request_body.content['multipart/form-data'].schema.required
+                required_fields = self.request_body['content']['multipart/form-data']['schema']['required']
                 data = {}
                 # if the request body has no defined properties, look for a single "request_body" parameter.
-                if self.op_desc.request_body.content['multipart/form-data'].schema.properties == {}:
+                if self.request_body['content']['multipart/form-data']['schema']['properties'] == {}:
                     # choice of "request_body" is arbitrary, as the property name is not provided by the
                     # openapi spec in this case
                     data['request_body'] = kwargs['request_body']
                 else:
                     # otherwise, the request body has defined properties, so look for each one in the function kwargs
-                    for p_name, p_desc in self.op_desc.request_body.content['multipart/form-data'].schema.properties.items():
+                    for p_name, p_desc in self.request_body['content']['multipart/form-data']['schema']['properties'].items():
                         if p_name in kwargs:
                             data[p_name] = kwargs[p_name]
                         elif p_name in required_fields:
                             raise errors.InvalidInputError(msg=f'{p_name} is a required argument.')
                 files = data
             else:
                 # We could default to providing message field
                 # Error seems better
                 # data = kwargs['message']
-                raise NotImplementedError(f'Content type/s specified have not been implemented. Types: {requestContentTypes}')
+                raise NotImplementedError(f'Content type/s specified have not been implemented. Types: {request_content_types}')
+
 
         # create a prepared request -
         # cf., https://requests.kennethreitz.org/en/master/user/advanced/#request-and-response-objects
         # Either multipart/form-data (files) or every other type of header.
         if files:
             r = requests.Request(http_method,
                                  url,
@@ -1164,19 +1185,19 @@
                                  headers=headers).prepare()
         else:
             r = requests.Request(http_method,
                                  url,
                                  params=params,
                                  data=data,
                                  headers=headers).prepare()
-            
+
         # call the plugins' pre-request callables:
         for f in self.tapis_client.plugin_on_call_pre_request_callables:
             f(self, r, **kwargs)
-        
+
         # the create_token operation requires HTTP basic auth, though some services, such as the authenticator, need to
         # use create_token to generate tokens on behalf of other users; in these cases, it is important to not set the
         # BasicAuth header, so we look for a special kwarg in this case
         if self.resource_name == 'tokens' and self.operation_id == 'create_token':
             # if a service token was included, we don't need to set the basic auth header
             if 'X-Tapis-Token' not in r.headers.keys():
                 # look for kwarg, use_basic_auth, to turn off use of BasicAuth; we default this to true so that BasicAuth
@@ -1307,15 +1328,14 @@
             arg = args[0]
             # the arg is a list and not a string, there are two cases: 1) at least one object in the list is a
             # primitive type, in which case we just return a list of the objects
             if _seq_but_not_str(arg):
                 setattr(self, 'result', [x for x in arg])
             else:
                 setattr(self, 'result', arg)
-
         for k, v in kwargs.items():
             # primitive types
             if type(v) in TapisResult.PRIMITIVE_TYPES:
                 # just set the attribute to the value
                 setattr(self, k, v)
             # lists
             elif _seq_but_not_str(v):
@@ -1353,7 +1373,9 @@
     """
     Debug data for an API request.
     """
 
     def __init__(self, request, response):
         self.request = request
         self.response = response
+
+print(f"TIMING: After entire tapis.py file. Took: {time.time() - start_time} seconds")
```

### Comparing `tapipy-1.3.5/setup.py` & `tapipy-1.4.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 install_requires = \
 ['PyJWT>=1.7.1',
  'atomicwrites>=1.4.0,<2.0.0',
  'certifi>=2020.11.8',
  'cloudpickle>=1.6.0',
  'cryptography>=3.3.2',
  'jsonschema>=3.2.0',
- 'openapi_core>=0.12,<0.13',
- 'openapi_spec_validator>=0.4.0,<0.5.0',
+ 'openapi_core>=0.17,<0.18',
+ 'openapi_spec_validator>=0.5.0,<0.6.0',
  'python_dateutil>=2.5.3,<3.0.0',
  'pyyaml>=5.4',
  'requests>=2.20.0,<3.0.0',
  'setuptools>=21.0.0',
  'six>=1.10,<2.0',
  'urllib3>=1.26.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'tapipy',
-    'version': '1.3.5',
+    'version': '1.4.0a1',
     'description': 'Python lib for interacting with an instance of the Tapis API Framework',
     'long_description': '# tapipy - Tapis V3 Python SDK\n\nPython library for interacting with an instance of the Tapis API Framework.\n\nThe library is automatically generated by referencing the OpenAPI spec files which  a `Tapis` object built from the OpenAPI spec files from TACC\'s Tapis services. With this functionality a user is able to authorize itself with the `Tapis` object and have a \'live\' library in order to interact with Tapis services.\n\n## Development\n\nThis project is under active development, exploring different approaches to SDK generation.\n\n## Installation\nTapipy is packaged on [pypi](https://pypi.org/project/tapipy/) and can be installed with pip.\n\n```\npip install tapipy\n```\n\n\n## Usage\nTapipy\'s Tapis object first must be initialized in order to be used.\nA basic example of logging in with a user account is below.\n\n```\n# Import the Tapis object\nfrom tapipy.tapis import Tapis\n\n# Log into you the Tapis service by providing user/pass and the base url of your tenant. For example, to interact with the tacc tenant --\nt = Tapis(base_url=\'https://tacc.tapis.io\',\n          username=\'myuser\',\n          password=\'mypass\')\n\t  \n# Get tokens that will be used for authentication function calls\nt.get_tokens()\n```\n\nNow you have a Tapis object that is authenticated and able to call Tapis service endpoints. It\'s useful to know that the Tapis object will automatically refresh it\'s token if it is deemed appropriate, so the object should stay in the good graces of Tapis indefinitely.\n\nNow in order to use the Tapis object you can reference the [Tapis Framework](https://tapis-project.github.io/live-docs/) to browse all functions. For example, if I wanted to use the SK service in order to check if a user has a specific role I would find the function on the site (which is just a better way to look at the json specs).\n\nWith the site I can see that I need to use my Tapis object, initialized as `t`, access `sk`, and then use the `hasRole` function with the required inputs as follows.\n```\nt.sk.hasRole(tenant=\'dev\', user=\'_testuser\', roleName=\'Do you have this role?\')\n```\n\n### Special Query Parameters and Headers\nFor the most part, arguments that can or should be passed to a Tapis endpoint are described in the OpenAPI \ndefinition files and recognized automatically by `tapipy`. However, due to limitations in what can be expressed\nin OpenAPI, there are some paramaters that are not defined in the definition files; for example, the search\nparameters for various endpoints.\n\nTo accommodate these cases, `tapipy` recognizes two special keyword arguments to all of its methods that\ncorrespond to Tapis API calls (i.e., all of its "operations"). They are:\n\n  * `_tapis_headers` -- dictionary-like object of header names (keys) and vales.\n  * `_tapis_query_parameters` -- dictionary-like object of query parameter names (keys) and values.\n\nUse the above two special arguments for passing headers (respectively, query parameters) that are not specified\nin the OpenAPI definition of an endpoint.\n\nFor example, I can issue a search using the following syntax:\n\n```\nt.jobs.getJobSearchList(limit=5, orderBy=\'lastUpdated(desc),name(asc)\', _tapis_query_parameters={\'key\': \'value\'})\n```\n\n# Development Docs\n## Running the tests\n\nTests resources are contained within the `test` directory. `Dockerfile-tests` is at root.\n1. Build the test docker image: `docker build -t tapis/tapipy-tests -f Dockerfile-tests .`\n2. Run these tests using the built docker image: `docker run -it --rm -e username=<dev_user> -e password=<dev_pass> tapis/tapipy-tests`\n\n\n## Important Parameters to Know\n\nThe `tapipy` package allows for spec file customization in Tapis object initialization:\n* resource_set: str \n\t* Determines which set of resource to use, master or dev, defaults to master.\n\t* Important to note that if a custom_spec_dictionary is used, it is appended to this resource_set.\n\t\t* For example, you would set master and then specify a custom specs that will be added on.\n* custom_spec_dict: {resource_name: str, resource_url: str}\n\t* Allows users to modify the base resource set urls.\n\t\t* e.g. I can specify actor as a resource name and change the url.\n\t* Also allows users to add new resources to the set.\n\t\t* e.g. I can add a new resource named "test" with a  custom url.\n\t\t* Important that know that any new specs will be downloaded and added to the cache\n\t\t\t* No need to specify download_latest_specs or update spec files.\n\t* ALLOWS LOCAL RESOURCES!\n\t\t* Specify an absolute path in the dict with `local:` prefixing it and tapipy will load in a local OpenAPI v3 yml spec file.\n\t\t* `custom_spec_dict={\'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'}`\n* download_latest_specs: bool\n\t* Allows users to re-download all specs regardless on if they already exist in the cache. Defaulted to False\n\t* This will happen every time the Tapis object is initialized, it\'s a tad slower, and can cause live updates to specs.\n\t\t* As such, be warned. There are functions to update spec files below.\n* spec_dir: str\n\t* Allows users to specify folder to save specs to. Defaults to none which uses Tapipy\'s package folder.\n\t* If you are updating specs it\'s wise to use a different folder in order to not modify the base specs.\n\nThe following is an example of some custom parameter setting. As you can see, the abaco resource will now use the spec at `URL#1`, overwriting the resource definition in the master resource set, it\'ll download it if it doesn\'t exist. The same for the longhorn resource. This means that the Tapis object will now have access to all specs in master like normal, but with a modified abaco and with a new longhorn resource. All of these are stored at the new spec_dir because I don\'t want to accidentally overwrite any base specs if I call `update_spec_cache()` later (talked about in the next section).\n```\nfrom tapipy.tapis import Tapis\n\nt = Tapis(base_url=\'https://admin.develop.tapis.io\',\n          tenant_id=\'admin\',\n          username=\'username\',\n          account_type=\'user\',\n          password=\'password\',\n          resource_set=\'admin\',\n          custom_spec_dict={\'abaco\': \'URL#1\',\n                            \'longhorn\': \'URL#2\'},\n                            \'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'},\n          spec_dir=\'/home/username/tapipy_specs\')\nt.get_tokens()\n```\n\n## Update Specs Files\n\nThe Tapipy package now uses a cache to organize spec dictionaries as pickled files and has the ability to accept custom spec files. By default Tapipy keeps a set of base spec files in the `%tapipy%/specs` folder. These specs are pre-pickled at package creation time.\n\nIn order to update all default spec files a user can use the `update_spec_cache()` function. Said function\'s definition is below. If no resources are provided the function will download all default spec urls in the RESOURCES object in `%tapipy%/tapipy/tapis.py` file.\n```\nResources = Dict[ResourceName, ResourceUrl]\nupdate_spec_cache(resources: Resources = None, spec_dir: str = None)\n```\nUsers are able to specify custom resources to download by providing their own resource dictionary. For example, providing `{\'actors\': \'URLToMyActorDictionary\'}` would update that spec.\n\nUsers can also specify here where to update the spec with the `spec_dir` variable.\n\nThe Tapis object itself also has a `update_spec_cache()` function that takes the Tapis parameters given at startup and updates the spec cache. Meaning that if the Tapis object was given a custom dictionary, the `update_spec_cache()` function would update it without the need for setting parameters.\n```\nt.update_spec_cache()\n```\n\n## Build instructions\n\nBuilding is done with poetry as follows:\n```\npip install poetry\npoetry install\n```\nThis installs `tapipy` to a virtual environment. Run a shell in this environment with:\n```\npoetry shell\n```\n\nTo install locally (not in a virtual environment):\n```\npip install poetry\npoetry build\ncd dists\npip install *.whl\n```\n\n## PyPi Push Instructions\n\n```\npoetry build\npoetry publish\n```\n\n## Archive Usage\nTODO - provide working examples, e.g., \n```\nimport tapipy\nt = tapipy.Tapis(base_url=\'http://localhost:5001\')\nreq = t.tokens.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\nt.tokens.create_token(req)\n\nimport openapi_client\nconfiguration = openapi_client.Configuration()\nconfiguration.host = \'http://localhost:5001\'\napi_instance = openapi_client.TokensApi(openapi_client.ApiClient(configuration))\n\nnew_token = openapi_client.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\n\nresp = api_instance.create_token(new_token)\njwt = resp.get(\'result\').get(\'access_token\').get(\'access_token\')\n```\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tapipy-1.3.5/PKG-INFO` & `tapipy-1.4.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: tapipy
-Version: 1.3.5
+Version: 1.4.0a1
 Summary: Python lib for interacting with an instance of the Tapis API Framework
 Home-page: https://github.com/tapis-project/tapipy
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=1.7.1)
 Requires-Dist: atomicwrites (>=1.4.0,<2.0.0)
 Requires-Dist: certifi (>=2020.11.8)
 Requires-Dist: cloudpickle (>=1.6.0)
 Requires-Dist: cryptography (>=3.3.2)
 Requires-Dist: jsonschema (>=3.2.0)
-Requires-Dist: openapi_core (>=0.12,<0.13)
-Requires-Dist: openapi_spec_validator (>=0.4.0,<0.5.0)
+Requires-Dist: openapi_core (>=0.17,<0.18)
+Requires-Dist: openapi_spec_validator (>=0.5.0,<0.6.0)
 Requires-Dist: python_dateutil (>=2.5.3,<3.0.0)
 Requires-Dist: pyyaml (>=5.4)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: six (>=1.10,<2.0)
 Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
 Project-URL: Repository, https://github.com/tapis-project/tapipy
```

