# Comparing `tmp/pulumi_pulumiservice-0.7.2.tar.gz` & `tmp/pulumi_pulumiservice-0.7.3a1685724591.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_pulumiservice-0.7.2.tar", last modified: Thu May 25 17:14:18 2023, max compression
+gzip compressed data, was "dist/pulumi_pulumiservice-0.7.3a1685724591.tar", last modified: Fri Jun  2 16:53:38 2023, max compression
```

## Comparing `pulumi_pulumiservice-0.7.2.tar` & `pulumi_pulumiservice-0.7.3a1685724591.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.640098 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/deployment_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/org_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/stack_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_stack_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.640098 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/deployment_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/org_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/stack_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/team_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/team_stack_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-02 16:53:38.000000 pulumi_pulumiservice-0.7.3a1685724591/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pulumi_pulumiservice-0.7.2/PKG-INFO` & `pulumi_pulumiservice-0.7.3a1685724591/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_pulumiservice
-Version: 0.7.2
-Summary: A native Pulumi package for creating and managing Pulumi Service constructs
-Home-page: https://pulumi.com
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
-Keywords: pulumi kind/native category/infrastructure
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Pulumi Service Provider
 
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
 [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
 [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
@@ -102,9 +91,7 @@
     ],
 });
 
 export const members = team.members;
 ```
 
 Check out the [examples/](examples/) directory for more examples.
-
-
```

### Comparing `pulumi_pulumiservice-0.7.2/README.md` & `pulumi_pulumiservice-0.7.3a1685724591/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,108 @@
-# Pulumi Service Provider
-
-[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-[![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
-[![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
-[![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
-[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
-
-A Pulumi Resource Provider for The Pulumi Service.
-
-The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
-
-#### Supported Resources
-
-- [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
-- [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
-  - You can grant a team access to stacks via the `TeamStackPermission` resource
-- [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
-- [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
-
-For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
-
-## Installing
-
-This package is available in many languages in the standard packaging formats.
-
-### Node.js (Java/TypeScript)
-
-To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-
-    $ npm install @pulumi/pulumiservice
-
-or `yarn`:
-
-    $ yarn add @pulumi/pulumiservice
-
-### Python
-
-To use from Python, install using `pip`:
-
-    $ pip install pulumi_pulumiservice
-
-### Go
-
-To use from Go, use `go get` to grab the latest version of the library
-
-    $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
-
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-    $ dotnet add package Pulumi.PulumiService
-
-## Setup
-
-Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
-
-### Configuration Options
-
-Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
-
-| Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
-| ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
-| `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
-
-## Examples
-
-```typescript
-import * as aws from "@pulumi/awsx"
-import * as pulumi from "@pulumi/pulumi";
-import * as service from "@pulumi/pulumiservice";
-
-const team = new service.Team("team", {
-    name: "pulumi-service-team",
-    displayName: "Pulumi Service",
-    description: "The Pulumi Service Team",
-    organizationName: "pulumi",
-    teamType: "pulumi",
-    members: [
-        "piers",
-        "bryce",
-        "casey"
-        "evan",
-        "devon",
-        "meagan"
-        "myles",
-        "steve"
-    ],
-});
-
-export const members = team.members;
-```
-
-Check out the [examples/](examples/) directory for more examples.
+Metadata-Version: 2.1
+Name: pulumi_pulumiservice
+Version: 0.7.3a1685724591
+Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
+Home-page: https://pulumi.com
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
+Description: # Pulumi Service Provider
+        
+        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
+        [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
+        [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
+        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
+        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
+        
+        A Pulumi Resource Provider for The Pulumi Service.
+        
+        The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
+        
+        #### Supported Resources
+        
+        - [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
+        - [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
+          - You can grant a team access to stacks via the `TeamStackPermission` resource
+        - [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
+        - [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
+        
+        For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
+        
+        ## Installing
+        
+        This package is available in many languages in the standard packaging formats.
+        
+        ### Node.js (Java/TypeScript)
+        
+        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+        
+            $ npm install @pulumi/pulumiservice
+        
+        or `yarn`:
+        
+            $ yarn add @pulumi/pulumiservice
+        
+        ### Python
+        
+        To use from Python, install using `pip`:
+        
+            $ pip install pulumi_pulumiservice
+        
+        ### Go
+        
+        To use from Go, use `go get` to grab the latest version of the library
+        
+            $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
+        
+        ### .NET
+        
+        To use from .NET, install using `dotnet add package`:
+        
+            $ dotnet add package Pulumi.PulumiService
+        
+        ## Setup
+        
+        Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
+        
+        ### Configuration Options
+        
+        Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
+        
+        | Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
+        | ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+        | `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
+        | `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
+        
+        ## Examples
+        
+        ```typescript
+        import * as aws from "@pulumi/awsx"
+        import * as pulumi from "@pulumi/pulumi";
+        import * as service from "@pulumi/pulumiservice";
+        
+        const team = new service.Team("team", {
+            name: "pulumi-service-team",
+            displayName: "Pulumi Service",
+            description: "The Pulumi Service Team",
+            organizationName: "pulumi",
+            teamType: "pulumi",
+            members: [
+                "piers",
+                "bryce",
+                "casey"
+                "evan",
+                "devon",
+                "meagan"
+                "myles",
+                "steve"
+            ],
+        });
+        
+        export const members = team.members;
+        ```
+        
+        Check out the [examples/](examples/) directory for more examples.
+        
+Keywords: pulumi kind/native category/infrastructure
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/__init__.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_enums.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_inputs.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_utilities.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/access_token.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/access_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,28 +38,28 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Access tokens allow a user to authenticate against the Pulumi Service
+        Access tokens allow a user to authenticate against the Pulumi Cloud
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the access token.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AccessTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Access tokens allow a user to authenticate against the Pulumi Service
+        Access tokens allow a user to authenticate against the Pulumi Cloud
 
         :param str resource_name: The name of the resource.
         :param AccessTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/vars.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/deployment_settings.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/deployment_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/org_access_token.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/org_access_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,30 +71,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The Pulumi Service allows users to create access tokens scoped to orgs. Org access tokens is a resource to create them and assign them to an org
+        The Pulumi Cloud allows users to create access tokens scoped to orgs. Org access tokens is a resource to create them and assign them to an org
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Optional. Team description.
         :param pulumi.Input[str] name: The name for the token.
         :param pulumi.Input[str] organization_name: The organization's name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: OrgAccessTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Pulumi Service allows users to create access tokens scoped to orgs. Org access tokens is a resource to create them and assign them to an org
+        The Pulumi Cloud allows users to create access tokens scoped to orgs. Org access tokens is a resource to create them and assign them to an org
 
         :param str resource_name: The name of the resource.
         :param OrgAccessTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/provider.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  access_token: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] access_token: Access Token to authenticate with Pulumi Service.
+        :param pulumi.Input[str] access_token: Access Token to authenticate with Pulumi Cloud.
         """
         if access_token is None:
             access_token = (_utilities.get_env('PULUMI_ACCESS_TOKEN') or '')
         if access_token is not None:
             pulumi.set(__self__, "access_token", access_token)
 
     @property
     @pulumi.getter(name="accessToken")
     def access_token(self) -> Optional[pulumi.Input[str]]:
         """
-        Access Token to authenticate with Pulumi Service.
+        Access Token to authenticate with Pulumi Cloud.
         """
         return pulumi.get(self, "access_token")
 
     @access_token.setter
     def access_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_token", value)
 
@@ -44,15 +44,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Pulumiservice resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] access_token: Access Token to authenticate with Pulumi Service.
+        :param pulumi.Input[str] access_token: Access Token to authenticate with Pulumi Cloud.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/stack_tag.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/stack_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                  display_name: Optional[pulumi.Input[str]] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  team_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The Pulumi Service offers role-based access control (RBAC) using teams. Teams allow organization admins to assign a set of stack permissions to a group of users.
+        The Pulumi Cloud offers role-based access control (RBAC) using teams. Teams allow organization admins to assign a set of stack permissions to a group of users.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Optional. Team description.
         :param pulumi.Input[str] display_name: Optional. Team display name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of team members.
         :param pulumi.Input[str] name: The team name.
@@ -139,15 +139,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TeamArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Pulumi Service offers role-based access control (RBAC) using teams. Teams allow organization admins to assign a set of stack permissions to a group of users.
+        The Pulumi Cloud offers role-based access control (RBAC) using teams. Teams allow organization admins to assign a set of stack permissions to a group of users.
 
         :param str resource_name: The name of the resource.
         :param TeamArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_access_token.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/team_access_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  team_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The Pulumi Service allows users to create access tokens scoped to team. Team access tokens is a resource to create them and assign them to a team
+        The Pulumi Cloud allows users to create access tokens scoped to team. Team access tokens is a resource to create them and assign them to a team
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Optional. Team description.
         :param pulumi.Input[str] name: The name for the token. This must be unique amongst all machine tokens within your organization.
         :param pulumi.Input[str] organization_name: The organization's name.
         :param pulumi.Input[str] team_name: The team name.
@@ -103,15 +103,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TeamAccessTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Pulumi Service allows users to create access tokens scoped to team. Team access tokens is a resource to create them and assign them to a team
+        The Pulumi Cloud allows users to create access tokens scoped to team. Team access tokens is a resource to create them and assign them to a team
 
         :param str resource_name: The name of the resource.
         :param TeamAccessTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_stack_permission.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/team_stack_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/webhook.py` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice/webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                  format: Optional[pulumi.Input['WebhookFormat']] = None,
                  project_name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  stack_name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Webhook resource.
         :param pulumi.Input[bool] active: Indicates whether this webhook is enabled or not.
-        :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Service.
+        :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Cloud.
         :param pulumi.Input[str] organization_name: Name of the organization.
         :param pulumi.Input[str] payload_url: URL to send request to.
         :param pulumi.Input[Sequence[pulumi.Input['WebhookFilters']]] filters: Optional set of filters to apply to the webhook. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#filters) for more information.
         :param pulumi.Input['WebhookFormat'] format: Format of the webhook payload. Can be either `raw` or `slack`. Defaults to `raw`.
         :param pulumi.Input[str] project_name: Name of the project. Only needed if this is a stack webhook.
         :param pulumi.Input[str] secret: Optional. secret used as the HMAC key. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#headers) for more information.
         :param pulumi.Input[str] stack_name: Name of the stack. Only needed if this is a stack webhook.
@@ -65,15 +65,15 @@
     def active(self, value: pulumi.Input[bool]):
         pulumi.set(self, "active", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> pulumi.Input[str]:
         """
-        The friendly name displayed in the Pulumi Service.
+        The friendly name displayed in the Pulumi Cloud.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "display_name", value)
 
@@ -187,15 +187,15 @@
         ```sh
          $ pulumi import pulumiservice:index:Webhook my_webhook my-org/my-project/my-stack/4b0d0671
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Indicates whether this webhook is enabled or not.
-        :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Service.
+        :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Cloud.
         :param pulumi.Input[Sequence[pulumi.Input['WebhookFilters']]] filters: Optional set of filters to apply to the webhook. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#filters) for more information.
         :param pulumi.Input['WebhookFormat'] format: Format of the webhook payload. Can be either `raw` or `slack`. Defaults to `raw`.
         :param pulumi.Input[str] organization_name: Name of the organization.
         :param pulumi.Input[str] payload_url: URL to send request to.
         :param pulumi.Input[str] project_name: Name of the project. Only needed if this is a stack webhook.
         :param pulumi.Input[str] secret: Optional. secret used as the HMAC key. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#headers) for more information.
         :param pulumi.Input[str] stack_name: Name of the stack. Only needed if this is a stack webhook.
@@ -314,15 +314,15 @@
         """
         return pulumi.get(self, "active")
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> pulumi.Output[Optional[str]]:
         """
-        The friendly name displayed in the Pulumi Service.
+        The friendly name displayed in the Pulumi Cloud.
         """
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter
     def filters(self) -> pulumi.Output[Optional[Sequence['WebhookFilters']]]:
         """
@@ -338,15 +338,15 @@
         """
         return pulumi.get(self, "format")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         """
-        Webhook identifier generated by pulumi service.
+        Webhook identifier generated by Pulumi Cloud.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="organizationName")
     def organization_name(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/PKG-INFO` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,108 @@
 Metadata-Version: 2.1
 Name: pulumi-pulumiservice
-Version: 0.7.2
-Summary: A native Pulumi package for creating and managing Pulumi Service constructs
+Version: 0.7.3a1685724591
+Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
+Description: # Pulumi Service Provider
+        
+        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
+        [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
+        [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
+        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
+        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
+        
+        A Pulumi Resource Provider for The Pulumi Service.
+        
+        The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
+        
+        #### Supported Resources
+        
+        - [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
+        - [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
+          - You can grant a team access to stacks via the `TeamStackPermission` resource
+        - [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
+        - [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
+        
+        For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
+        
+        ## Installing
+        
+        This package is available in many languages in the standard packaging formats.
+        
+        ### Node.js (Java/TypeScript)
+        
+        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+        
+            $ npm install @pulumi/pulumiservice
+        
+        or `yarn`:
+        
+            $ yarn add @pulumi/pulumiservice
+        
+        ### Python
+        
+        To use from Python, install using `pip`:
+        
+            $ pip install pulumi_pulumiservice
+        
+        ### Go
+        
+        To use from Go, use `go get` to grab the latest version of the library
+        
+            $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
+        
+        ### .NET
+        
+        To use from .NET, install using `dotnet add package`:
+        
+            $ dotnet add package Pulumi.PulumiService
+        
+        ## Setup
+        
+        Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
+        
+        ### Configuration Options
+        
+        Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
+        
+        | Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
+        | ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+        | `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
+        | `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
+        
+        ## Examples
+        
+        ```typescript
+        import * as aws from "@pulumi/awsx"
+        import * as pulumi from "@pulumi/pulumi";
+        import * as service from "@pulumi/pulumiservice";
+        
+        const team = new service.Team("team", {
+            name: "pulumi-service-team",
+            displayName: "Pulumi Service",
+            description: "The Pulumi Service Team",
+            organizationName: "pulumi",
+            teamType: "pulumi",
+            members: [
+                "piers",
+                "bryce",
+                "casey"
+                "evan",
+                "devon",
+                "meagan"
+                "myles",
+                "steve"
+            ],
+        });
+        
+        export const members = team.members;
+        ```
+        
+        Check out the [examples/](examples/) directory for more examples.
+        
 Keywords: pulumi kind/native category/infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-
-# Pulumi Service Provider
-
-[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-[![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
-[![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
-[![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
-[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
-
-A Pulumi Resource Provider for The Pulumi Service.
-
-The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
-
-#### Supported Resources
-
-- [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
-- [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
-  - You can grant a team access to stacks via the `TeamStackPermission` resource
-- [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
-- [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
-
-For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
-
-## Installing
-
-This package is available in many languages in the standard packaging formats.
-
-### Node.js (Java/TypeScript)
-
-To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-
-    $ npm install @pulumi/pulumiservice
-
-or `yarn`:
-
-    $ yarn add @pulumi/pulumiservice
-
-### Python
-
-To use from Python, install using `pip`:
-
-    $ pip install pulumi_pulumiservice
-
-### Go
-
-To use from Go, use `go get` to grab the latest version of the library
-
-    $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
-
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-    $ dotnet add package Pulumi.PulumiService
-
-## Setup
-
-Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
-
-### Configuration Options
-
-Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
-
-| Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
-| ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
-| `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
-
-## Examples
-
-```typescript
-import * as aws from "@pulumi/awsx"
-import * as pulumi from "@pulumi/pulumi";
-import * as service from "@pulumi/pulumiservice";
-
-const team = new service.Team("team", {
-    name: "pulumi-service-team",
-    displayName: "Pulumi Service",
-    description: "The Pulumi Service Team",
-    organizationName: "pulumi",
-    teamType: "pulumi",
-    members: [
-        "piers",
-        "bryce",
-        "casey"
-        "evan",
-        "devon",
-        "meagan"
-        "myles",
-        "steve"
-    ],
-});
-
-export const members = team.members;
-```
-
-Check out the [examples/](examples/) directory for more examples.
-
-
```

### Comparing `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/SOURCES.txt` & `pulumi_pulumiservice-0.7.3a1685724591/pulumi_pulumiservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.2/setup.py` & `pulumi_pulumiservice-0.7.3a1685724591/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.2"
-PLUGIN_VERSION = "0.7.2"
+VERSION = "0.7.3a1685724591"
+PLUGIN_VERSION = "0.7.3-alpha.1685724591+9cc47b02"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pulumiservice', PLUGIN_VERSION])
         except OSError as error:
@@ -35,15 +35,15 @@
             return f.read()
     except FileNotFoundError:
         return "pulumiservice Pulumi Package - Development Version"
 
 
 setup(name='pulumi_pulumiservice',
       version=VERSION,
-      description="A native Pulumi package for creating and managing Pulumi Service constructs",
+      description="A native Pulumi package for creating and managing Pulumi Cloud constructs",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi kind/native category/infrastructure',
       url='https://pulumi.com',
```

