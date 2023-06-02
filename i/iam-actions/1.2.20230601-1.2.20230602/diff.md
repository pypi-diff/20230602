# Comparing `tmp/iam_actions-1.2.20230601.tar.gz` & `tmp/iam_actions-1.2.20230602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230601.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230602.tar", max compression
```

## Comparing `iam_actions-1.2.20230601.tar` & `iam_actions-1.2.20230602.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/README.md
--rw-r--r--   0        0        0      228 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/__init__.py
--rw-r--r--   0        0        0  4277029 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/services.py
--rw-r--r--   0        0        0   550024 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/policies.json
--rw-r--r--   0        0        0   195249 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   533536 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-01 03:07:24.029086 iam_actions-1.2.20230601/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230601/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230601/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/README.md
+-rw-r--r--   0        0        0      228 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4282803 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   551055 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/policies.json
+-rw-r--r--   0        0        0   195514 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   534521 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-02 02:45:19.547908 iam_actions-1.2.20230602/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230602/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230602/PKG-INFO
```

### Comparing `iam_actions-1.2.20230601/LICENSE` & `iam_actions-1.2.20230602/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/README.md` & `iam_actions-1.2.20230602/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/actions.json` & `iam_actions-1.2.20230602/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989367191118268%*

 * *Differences: {"'appflow'": "{'CancelFlowExecutions': {'access_level': 'Write', 'description': 'Grants "*

 * *              "permission to cancel in-progress executions of an Amazon AppFlow flow', "*

 * *              "'resources': ['flow']}}",*

 * * "'aws-marketplace-management'": "{'PutBankAccountVerificationDetails': "*

 * *                                 "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                                 "'PutBankAccountVerificationDetails'), ('condition_keys', []), "*

 * *                          […]*

```diff
@@ -4134,20 +4134,22 @@
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appflow": {
         "CancelFlowExecutions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelFlowExecutions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to cancel in-progress executions of an Amazon AppFlow flow",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "flow"
+            ]
         },
         "CreateConnectorProfile": {
             "access_level": "Write",
             "action": "CreateConnectorProfile",
             "condition_keys": [],
             "description": "Grants permission to create a login profile to be used with Amazon AppFlow flows",
             "orphan": false,
@@ -10600,14 +10602,78 @@
             "condition_keys": [],
             "description": "Grants permission to users to see their account's subscriptions",
             "orphan": false,
             "resources": []
         }
     },
     "aws-marketplace-management": {
+        "GetAdditionalSellerNotificationRecipients": {
+            "access_level": "Undocumented",
+            "action": "GetAdditionalSellerNotificationRecipients",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetBankAccountVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "GetBankAccountVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSecondaryUserVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "GetSecondaryUserVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSellerVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "GetSellerVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutAdditionalSellerNotificationRecipients": {
+            "access_level": "Undocumented",
+            "action": "PutAdditionalSellerNotificationRecipients",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutBankAccountVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "PutBankAccountVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutSecondaryUserVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "PutSecondaryUserVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutSellerVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "PutSellerVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "uploadFiles": {
             "access_level": "Write",
             "action": "uploadFiles",
             "condition_keys": [],
             "description": "Allows access to the File Upload page inside the AWS Marketplace Management Portal.",
             "orphan": false,
             "resources": []
@@ -38695,14 +38761,22 @@
             "condition_keys": [],
             "description": "Grants permission to cancel a single premigration assessment run",
             "orphan": false,
             "resources": [
                 "ReplicationTaskAssessmentRun"
             ]
         },
+        "CreateDataMigration": {
+            "access_level": "Undocumented",
+            "action": "CreateDataMigration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateDataProvider": {
             "access_level": "Write",
             "action": "CreateDataProvider",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "dms:req-tag/${TagKey}"
@@ -38766,14 +38840,22 @@
             "description": "Grants permission to create an migration project using the provided settings",
             "orphan": false,
             "resources": [
                 "DataProvider",
                 "InstanceProfile"
             ]
         },
+        "CreateReplicationConfig": {
+            "access_level": "Undocumented",
+            "action": "CreateReplicationConfig",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateReplicationInstance": {
             "access_level": "Write",
             "action": "CreateReplicationInstance",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "dms:req-tag/${TagKey}"
@@ -38826,14 +38908,22 @@
             "description": "Grants permission to delete the specified connection between a replication instance and an endpoint",
             "orphan": false,
             "resources": [
                 "Endpoint",
                 "ReplicationInstance"
             ]
         },
+        "DeleteDataMigration": {
+            "access_level": "Undocumented",
+            "action": "DeleteDataMigration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteDataProvider": {
             "access_level": "Write",
             "action": "DeleteDataProvider",
             "condition_keys": [],
             "description": "Grants permission to delete the specified data provider",
             "orphan": false,
             "resources": [
@@ -38892,14 +38982,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete the specified migration project",
             "orphan": false,
             "resources": [
                 "MigrationProject"
             ]
         },
+        "DeleteReplicationConfig": {
+            "access_level": "Undocumented",
+            "action": "DeleteReplicationConfig",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteReplicationInstance": {
             "access_level": "Write",
             "action": "DeleteReplicationInstance",
             "condition_keys": [],
             "description": "Grants permission to delete the specified replication instance",
             "orphan": false,
             "resources": [
@@ -38967,14 +39065,22 @@
             "access_level": "Read",
             "action": "DescribeConnections",
             "condition_keys": [],
             "description": "Grants permission to describe the status of the connections that have been made between the replication instance and an endpoint",
             "orphan": false,
             "resources": []
         },
+        "DescribeDataMigrations": {
+            "access_level": "Undocumented",
+            "action": "DescribeDataMigrations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeEndpointSettings": {
             "access_level": "Read",
             "action": "DescribeEndpointSettings",
             "condition_keys": [],
             "description": "Grants permission to return the possible endpoint settings available when you create an endpoint for a specific database engine",
             "orphan": false,
             "resources": []
@@ -39097,14 +39203,22 @@
             "condition_keys": [],
             "description": "Grants permission to returns the status of the RefreshSchemas operation",
             "orphan": false,
             "resources": [
                 "Endpoint"
             ]
         },
+        "DescribeReplicationConfigs": {
+            "access_level": "Undocumented",
+            "action": "DescribeReplicationConfigs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeReplicationInstanceTaskLogs": {
             "access_level": "Read",
             "action": "DescribeReplicationInstanceTaskLogs",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -39126,14 +39240,22 @@
             "access_level": "Read",
             "action": "DescribeReplicationSubnetGroups",
             "condition_keys": [],
             "description": "Grants permission to return information about the replication subnet groups",
             "orphan": false,
             "resources": []
         },
+        "DescribeReplicationTableStatistics": {
+            "access_level": "Undocumented",
+            "action": "DescribeReplicationTableStatistics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeReplicationTaskAssessmentResults": {
             "access_level": "Read",
             "action": "DescribeReplicationTaskAssessmentResults",
             "condition_keys": [],
             "description": "Grants permission to return the latest task assessment results from Amazon S3",
             "orphan": false,
             "resources": [
@@ -39167,14 +39289,22 @@
             "access_level": "Read",
             "action": "DescribeReplicationTasks",
             "condition_keys": [],
             "description": "Grants permission to return information about replication tasks for your account in the current region",
             "orphan": false,
             "resources": []
         },
+        "DescribeReplications": {
+            "access_level": "Undocumented",
+            "action": "DescribeReplications",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeSchemas": {
             "access_level": "Read",
             "action": "DescribeSchemas",
             "condition_keys": [],
             "description": "Grants permission to return information about the schema for the specified endpoint",
             "orphan": false,
             "resources": [
@@ -39325,14 +39455,22 @@
                 "Endpoint",
                 "EventSubscription",
                 "ReplicationInstance",
                 "ReplicationSubnetGroup",
                 "ReplicationTask"
             ]
         },
+        "ModifyDataMigration": {
+            "access_level": "Undocumented",
+            "action": "ModifyDataMigration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ModifyEndpoint": {
             "access_level": "Write",
             "action": "ModifyEndpoint",
             "condition_keys": [],
             "description": "Grants permission to modify the specified endpoint",
             "orphan": false,
             "resources": [
@@ -39360,14 +39498,22 @@
             "access_level": "Write",
             "action": "ModifyFleetAdvisorCollectorStatuses",
             "condition_keys": [],
             "description": "Grants permission to modify the status of the specified Fleet Advisor collector",
             "orphan": false,
             "resources": []
         },
+        "ModifyReplicationConfig": {
+            "access_level": "Undocumented",
+            "action": "ModifyReplicationConfig",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ModifyReplicationInstance": {
             "access_level": "Write",
             "action": "ModifyReplicationInstance",
             "condition_keys": [],
             "description": "Grants permission to modify the replication instance to apply new settings",
             "orphan": false,
             "resources": [
@@ -39420,14 +39566,22 @@
             "description": "Grants permission to populate the schema for the specified endpoint",
             "orphan": false,
             "resources": [
                 "Endpoint",
                 "ReplicationInstance"
             ]
         },
+        "ReloadReplicationTables": {
+            "access_level": "Undocumented",
+            "action": "ReloadReplicationTables",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ReloadTables": {
             "access_level": "Write",
             "action": "ReloadTables",
             "condition_keys": [],
             "description": "Grants permission to reload the target database table with the source data",
             "orphan": false,
             "resources": [
@@ -39458,14 +39612,22 @@
             "access_level": "Write",
             "action": "RunFleetAdvisorLsaAnalysis",
             "condition_keys": [],
             "description": "Grants permission to run a large-scale assessment (LSA) analysis on every Fleet Advisor collector in your account",
             "orphan": false,
             "resources": []
         },
+        "StartDataMigration": {
+            "access_level": "Undocumented",
+            "action": "StartDataMigration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartMetadataModelAssessment": {
             "access_level": "Write",
             "action": "StartMetadataModelAssessment",
             "condition_keys": [],
             "description": "Grants permission to start a new assessment of metadata model",
             "orphan": false,
             "resources": [
@@ -39516,14 +39678,22 @@
             "access_level": "Write",
             "action": "StartRecommendations",
             "condition_keys": [],
             "description": "Grants permission to start the analysis of your source database to provide recommendations of target engines",
             "orphan": false,
             "resources": []
         },
+        "StartReplication": {
+            "access_level": "Undocumented",
+            "action": "StartReplication",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartReplicationTask": {
             "access_level": "Write",
             "action": "StartReplicationTask",
             "condition_keys": [],
             "description": "Grants permission to start the replication task",
             "orphan": false,
             "resources": [
@@ -39546,14 +39716,30 @@
             "condition_keys": [],
             "description": "Grants permission to start a new premigration assessment run for one or more individual assessments of a migration task",
             "orphan": false,
             "resources": [
                 "ReplicationTask"
             ]
         },
+        "StopDataMigration": {
+            "access_level": "Undocumented",
+            "action": "StopDataMigration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopReplication": {
+            "access_level": "Undocumented",
+            "action": "StopReplication",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StopReplicationTask": {
             "access_level": "Write",
             "action": "StopReplicationTask",
             "condition_keys": [],
             "description": "Grants permission to stop the replication task",
             "orphan": false,
             "resources": [
@@ -152423,20 +152609,23 @@
             "orphan": false,
             "resources": [
                 "browserSettings",
                 "portal"
             ]
         },
         "AssociateIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateIpAccessSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to associate ip access settings with web portals",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipAccessSettings",
+                "portal"
+            ]
         },
         "AssociateNetworkSettings": {
             "access_level": "Write",
             "action": "AssociateNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to associate network settings to web portals",
             "orphan": false,
@@ -152492,22 +152681,26 @@
         "CreateIdentityProvider": {
             "access_level": "Write",
             "action": "CreateIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to create identity providers",
             "orphan": false,
             "resources": [
+                "identityProvider",
                 "portal"
             ]
         },
         "CreateIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateIpAccessSettings",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create ip access settings",
             "orphan": false,
             "resources": []
         },
         "CreateNetworkSettings": {
             "access_level": "Write",
             "action": "CreateNetworkSettings",
             "condition_keys": [
@@ -152574,23 +152767,28 @@
         },
         "DeleteIdentityProvider": {
             "access_level": "Write",
             "action": "DeleteIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to delete identity providers",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "identityProvider",
+                "portal"
+            ]
         },
         "DeleteIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteIpAccessSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete ip access settings",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipAccessSettings"
+            ]
         },
         "DeleteNetworkSettings": {
             "access_level": "Write",
             "action": "DeleteNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to delete network settings",
             "orphan": false,
@@ -152645,20 +152843,22 @@
             "description": "Grants permission to disassociate browser settings from web portals",
             "orphan": false,
             "resources": [
                 "portal"
             ]
         },
         "DisassociateIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateIpAccessSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to disassociate ip access logging from web portals",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "portal"
+            ]
         },
         "DisassociateNetworkSettings": {
             "access_level": "Write",
             "action": "DisassociateNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to disassociate network settings from web portals",
             "orphan": false,
@@ -152708,23 +152908,27 @@
         },
         "GetIdentityProvider": {
             "access_level": "Read",
             "action": "GetIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to get details on identity providers",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "identityProvider"
+            ]
         },
         "GetIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetIpAccessSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get details on ip access settings",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipAccessSettings"
+            ]
         },
         "GetNetworkSettings": {
             "access_level": "Read",
             "action": "GetNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to get details on network settings",
             "orphan": false,
@@ -152802,21 +153006,23 @@
         },
         "ListIdentityProviders": {
             "access_level": "Read",
             "action": "ListIdentityProviders",
             "condition_keys": [],
             "description": "Grants permission to list identity providers",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "identityProvider"
+            ]
         },
         "ListIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListIpAccessSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list ip access settings",
             "orphan": false,
             "resources": []
         },
         "ListNetworkSettings": {
             "access_level": "Read",
             "action": "ListNetworkSettings",
             "condition_keys": [],
@@ -152879,14 +153085,15 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to add one or more tags to a resource",
             "orphan": false,
             "resources": [
                 "browserSettings",
+                "ipAccessSettings",
                 "networkSettings",
                 "portal",
                 "trustStore",
                 "userAccessLoggingSettings",
                 "userSettings"
             ]
         },
@@ -152897,14 +153104,15 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove one or more tags from a resource",
             "orphan": false,
             "resources": [
                 "browserSettings",
+                "ipAccessSettings",
                 "networkSettings",
                 "portal",
                 "trustStore",
                 "userAccessLoggingSettings",
                 "userSettings"
             ]
         },
@@ -152920,23 +153128,28 @@
         },
         "UpdateIdentityProvider": {
             "access_level": "Write",
             "action": "UpdateIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to update identity provider",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "identityProvider",
+                "portal"
+            ]
         },
         "UpdateIpAccessSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateIpAccessSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update ip access settings",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipAccessSettings"
+            ]
         },
         "UpdateNetworkSettings": {
             "access_level": "Write",
             "action": "UpdateNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to update network settings",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230601/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230602/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230602/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/generate/generate.py` & `iam_actions-1.2.20230602/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230602/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230602/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/generate/services.py` & `iam_actions-1.2.20230602/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230601/iam_actions/policies.json` & `iam_actions-1.2.20230602/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999932458984183%*

 * *Differences: {"'serviceMap'": "{'AWS Marketplace Management Portal': {'Actions': {insert: [(0, "*

 * *                 "'GetAdditionalSellerNotificationRecipients'), (1, "*

 * *                 "'GetBankAccountVerificationDetails'), (2, "*

 * *                 "'GetSecondaryUserVerificationDetails'), (3, 'GetSellerVerificationDetails'), (4, "*

 * *                 "'PutAdditionalSellerNotificationRecipients'), (5, "*

 * *                 "'PutBankAccountVerificationDetails'), (6, "*

 * *                 "'PutSecondaryUserVerificationDetails'), (7, ' […]*

```diff
@@ -2636,40 +2636,45 @@
                 "ApplyPendingMaintenanceAction",
                 "AssociateExtensionPack",
                 "BatchStartRecommendations",
                 "CancelMetadataModelAssessment",
                 "CancelMetadataModelConversion",
                 "CancelMetadataModelExport",
                 "CancelReplicationTaskAssessmentRun",
+                "CreateDataMigration",
                 "CreateDataProvider",
                 "CreateEndpoint",
                 "CreateEventSubscription",
                 "CreateFleetAdvisorCollector",
                 "CreateInstanceProfile",
                 "CreateMigrationProject",
+                "CreateReplicationConfig",
                 "CreateReplicationInstance",
                 "CreateReplicationSubnetGroup",
                 "CreateReplicationTask",
                 "DeleteCertificate",
                 "DeleteConnection",
+                "DeleteDataMigration",
                 "DeleteDataProvider",
                 "DeleteEndpoint",
                 "DeleteEventSubscription",
                 "DeleteFleetAdvisorCollector",
                 "DeleteFleetAdvisorDatabases",
                 "DeleteInstanceProfile",
                 "DeleteMigrationProject",
+                "DeleteReplicationConfig",
                 "DeleteReplicationInstance",
                 "DeleteReplicationSubnetGroup",
                 "DeleteReplicationTask",
                 "DeleteReplicationTaskAssessmentRun",
                 "DescribeAccountAttributes",
                 "DescribeApplicableIndividualAssessments",
                 "DescribeCertificates",
                 "DescribeConnections",
+                "DescribeDataMigrations",
                 "DescribeEndpointSettings",
                 "DescribeEndpointTypes",
                 "DescribeEndpoints",
                 "DescribeEventCategories",
                 "DescribeEventSubscriptions",
                 "DescribeEvents",
                 "DescribeFleetAdvisorCollectors",
@@ -2678,21 +2683,24 @@
                 "DescribeFleetAdvisorSchemaObjectSummary",
                 "DescribeFleetAdvisorSchemas",
                 "DescribeOrderableReplicationInstances",
                 "DescribePendingMaintenanceActions",
                 "DescribeRecommendationLimitations",
                 "DescribeRecommendations",
                 "DescribeRefreshSchemasStatus",
+                "DescribeReplicationConfigs",
                 "DescribeReplicationInstanceTaskLogs",
                 "DescribeReplicationInstances",
                 "DescribeReplicationSubnetGroups",
+                "DescribeReplicationTableStatistics",
                 "DescribeReplicationTaskAssessmentResults",
                 "DescribeReplicationTaskAssessmentRuns",
                 "DescribeReplicationTaskIndividualAssessments",
                 "DescribeReplicationTasks",
+                "DescribeReplications",
                 "DescribeSchemas",
                 "DescribeTableStatistics",
                 "DisassociateExtensionPack",
                 "ExportMetadataModelAssessment",
                 "GetMetadataModel",
                 "ImportCertificate",
                 "ListDataProviders",
@@ -2700,36 +2708,43 @@
                 "ListInstanceProfiles",
                 "ListMetadataModelAssessmentActionItems",
                 "ListMetadataModelAssessments",
                 "ListMetadataModelConversions",
                 "ListMetadataModelExports",
                 "ListMigrationProjects",
                 "ListTagsForResource",
+                "ModifyDataMigration",
                 "ModifyEndpoint",
                 "ModifyEventSubscription",
                 "ModifyFleetAdvisorCollector",
                 "ModifyFleetAdvisorCollectorStatuses",
+                "ModifyReplicationConfig",
                 "ModifyReplicationInstance",
                 "ModifyReplicationSubnetGroup",
                 "ModifyReplicationTask",
                 "MoveReplicationTask",
                 "RebootReplicationInstance",
                 "RefreshSchemas",
+                "ReloadReplicationTables",
                 "ReloadTables",
                 "RemoveTagsFromResource",
                 "RunFleetAdvisorLsaAnalysis",
+                "StartDataMigration",
                 "StartMetadataModelAssessment",
                 "StartMetadataModelConversion",
                 "StartMetadataModelExportAsScripts",
                 "StartMetadataModelExportToTarget",
                 "StartMetadataModelImport",
                 "StartRecommendations",
+                "StartReplication",
                 "StartReplicationTask",
                 "StartReplicationTaskAssessment",
                 "StartReplicationTaskAssessmentRun",
+                "StopDataMigration",
+                "StopReplication",
                 "StopReplicationTask",
                 "TestConnection",
                 "UpdateConversionConfiguration",
                 "UpdateDataProvider",
                 "UpdateInstanceProfile",
                 "UpdateMigrationProject",
                 "UpdateSubscriptionsToEventBridge",
@@ -2738,20 +2753,22 @@
             "HasResource": true,
             "StringPrefix": "dms",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "dms:cert-tag/${TagKey}",
-                "dms:dp-tag/${TagKey}",
+                "dms:data-migration-tag/${TagKey}",
+                "dms:data-provider-tag/${TagKey}",
                 "dms:endpoint-tag/${TagKey}",
                 "dms:es-tag/${TagKey}",
-                "dms:ip-tag/${TagKey}",
-                "dms:mp-tag/${TagKey}",
+                "dms:instance-profile-tag/${TagKey}",
+                "dms:migration-project-tag/${TagKey}",
                 "dms:rep-tag/${TagKey}",
+                "dms:replication-config-tag/${TagKey}",
                 "dms:req-tag/${TagKey}",
                 "dms:subgrp-tag/${TagKey}",
                 "dms:task-tag/${TagKey}"
             ]
         },
         "AWS DeepComposer": {
             "ARNFormat": "arn:aws:deepcomposer:${Region}:${Account}:${ResourceType}/${ResourceName}",
@@ -6406,15 +6423,25 @@
                 "ListBuilds",
                 "StartBuild"
             ],
             "HasResource": false,
             "StringPrefix": "aws-marketplace"
         },
         "AWS Marketplace Management Portal": {
+            "ARNFormat": "arn:${Partition}:Marketplace:${Region}:${Account}:${Resource}",
+            "ARNRegex": "^arn:${Partition}:Marketplace:.+",
             "Actions": [
+                "GetAdditionalSellerNotificationRecipients",
+                "GetBankAccountVerificationDetails",
+                "GetSecondaryUserVerificationDetails",
+                "GetSellerVerificationDetails",
+                "PutAdditionalSellerNotificationRecipients",
+                "PutBankAccountVerificationDetails",
+                "PutSecondaryUserVerificationDetails",
+                "PutSellerVerificationDetails",
                 "uploadFiles",
                 "viewMarketing",
                 "viewReports",
                 "viewSettings",
                 "viewSupport"
             ],
             "HasResource": false,
```

### Comparing `iam_actions-1.2.20230601/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230602/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'workspaces-web'": "{'identityProvider': OrderedDict([('arn_pattern', "*

 * *                     "'arn:*:workspaces-web:*:*:identityProvider/*/*'), ('condition_keys', "*

 * *                     "None)]), 'ipAccessSettings': OrderedDict([('arn_pattern', "*

 * *                     "'arn:*:workspaces-web:*:*:ipAccessSettings/*'), ('condition_keys', "*

 * *                     "'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -6607,14 +6607,22 @@
         }
     },
     "workspaces-web": {
         "browserSettings": {
             "arn_pattern": "arn:*:workspaces-web:*:*:browserSettings/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "identityProvider": {
+            "arn_pattern": "arn:*:workspaces-web:*:*:identityProvider/*/*",
+            "condition_keys": null
+        },
+        "ipAccessSettings": {
+            "arn_pattern": "arn:*:workspaces-web:*:*:ipAccessSettings/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "networkSettings": {
             "arn_pattern": "arn:*:workspaces-web:*:*:networkSettings/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "portal": {
             "arn_pattern": "arn:*:workspaces-web:*:*:portal/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230601/iam_actions/services.json` & `iam_actions-1.2.20230602/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996310145615701%*

 * *Differences: {"'aws-marketplace-management'": "{'Actions': {insert: [(0, "*

 * *                                 "'GetAdditionalSellerNotificationRecipients'), (1, "*

 * *                                 "'GetBankAccountVerificationDetails'), (2, "*

 * *                                 "'GetSecondaryUserVerificationDetails'), (3, "*

 * *                                 "'GetSellerVerificationDetails'), (4, "*

 * *                                 "'PutAdditionalSellerNotificationRecipients'), (5, "*

 * *                                 "'PutBankAccou […]*

```diff
@@ -1672,17 +1672,29 @@
             "AWS Marketplace Metering Service",
             "AWS Marketplace Private Marketplace",
             "AWS Marketplace Procurement Systems Integration",
             "AWS Marketplace Seller Reporting"
         ]
     },
     "aws-marketplace-management": {
-        "ARNFormats": [],
-        "ARNRegexes": [],
+        "ARNFormats": [
+            "arn:${Partition}:Marketplace:${Region}:${Account}:${Resource}"
+        ],
+        "ARNRegexes": [
+            "^arn:${Partition}:Marketplace:.+"
+        ],
         "Actions": [
+            "GetAdditionalSellerNotificationRecipients",
+            "GetBankAccountVerificationDetails",
+            "GetSecondaryUserVerificationDetails",
+            "GetSellerVerificationDetails",
+            "PutAdditionalSellerNotificationRecipients",
+            "PutBankAccountVerificationDetails",
+            "PutSecondaryUserVerificationDetails",
+            "PutSellerVerificationDetails",
             "uploadFiles",
             "viewMarketing",
             "viewReports",
             "viewSettings",
             "viewSupport"
         ],
         "ConditionKeys": [],
@@ -5797,40 +5809,45 @@
             "ApplyPendingMaintenanceAction",
             "AssociateExtensionPack",
             "BatchStartRecommendations",
             "CancelMetadataModelAssessment",
             "CancelMetadataModelConversion",
             "CancelMetadataModelExport",
             "CancelReplicationTaskAssessmentRun",
+            "CreateDataMigration",
             "CreateDataProvider",
             "CreateEndpoint",
             "CreateEventSubscription",
             "CreateFleetAdvisorCollector",
             "CreateInstanceProfile",
             "CreateMigrationProject",
+            "CreateReplicationConfig",
             "CreateReplicationInstance",
             "CreateReplicationSubnetGroup",
             "CreateReplicationTask",
             "DeleteCertificate",
             "DeleteConnection",
+            "DeleteDataMigration",
             "DeleteDataProvider",
             "DeleteEndpoint",
             "DeleteEventSubscription",
             "DeleteFleetAdvisorCollector",
             "DeleteFleetAdvisorDatabases",
             "DeleteInstanceProfile",
             "DeleteMigrationProject",
+            "DeleteReplicationConfig",
             "DeleteReplicationInstance",
             "DeleteReplicationSubnetGroup",
             "DeleteReplicationTask",
             "DeleteReplicationTaskAssessmentRun",
             "DescribeAccountAttributes",
             "DescribeApplicableIndividualAssessments",
             "DescribeCertificates",
             "DescribeConnections",
+            "DescribeDataMigrations",
             "DescribeEndpointSettings",
             "DescribeEndpointTypes",
             "DescribeEndpoints",
             "DescribeEventCategories",
             "DescribeEventSubscriptions",
             "DescribeEvents",
             "DescribeFleetAdvisorCollectors",
@@ -5839,21 +5856,24 @@
             "DescribeFleetAdvisorSchemaObjectSummary",
             "DescribeFleetAdvisorSchemas",
             "DescribeOrderableReplicationInstances",
             "DescribePendingMaintenanceActions",
             "DescribeRecommendationLimitations",
             "DescribeRecommendations",
             "DescribeRefreshSchemasStatus",
+            "DescribeReplicationConfigs",
             "DescribeReplicationInstanceTaskLogs",
             "DescribeReplicationInstances",
             "DescribeReplicationSubnetGroups",
+            "DescribeReplicationTableStatistics",
             "DescribeReplicationTaskAssessmentResults",
             "DescribeReplicationTaskAssessmentRuns",
             "DescribeReplicationTaskIndividualAssessments",
             "DescribeReplicationTasks",
+            "DescribeReplications",
             "DescribeSchemas",
             "DescribeTableStatistics",
             "DisassociateExtensionPack",
             "ExportMetadataModelAssessment",
             "GetMetadataModel",
             "ImportCertificate",
             "ListDataProviders",
@@ -5861,56 +5881,65 @@
             "ListInstanceProfiles",
             "ListMetadataModelAssessmentActionItems",
             "ListMetadataModelAssessments",
             "ListMetadataModelConversions",
             "ListMetadataModelExports",
             "ListMigrationProjects",
             "ListTagsForResource",
+            "ModifyDataMigration",
             "ModifyEndpoint",
             "ModifyEventSubscription",
             "ModifyFleetAdvisorCollector",
             "ModifyFleetAdvisorCollectorStatuses",
+            "ModifyReplicationConfig",
             "ModifyReplicationInstance",
             "ModifyReplicationSubnetGroup",
             "ModifyReplicationTask",
             "MoveReplicationTask",
             "RebootReplicationInstance",
             "RefreshSchemas",
+            "ReloadReplicationTables",
             "ReloadTables",
             "RemoveTagsFromResource",
             "RunFleetAdvisorLsaAnalysis",
+            "StartDataMigration",
             "StartMetadataModelAssessment",
             "StartMetadataModelConversion",
             "StartMetadataModelExportAsScripts",
             "StartMetadataModelExportToTarget",
             "StartMetadataModelImport",
             "StartRecommendations",
+            "StartReplication",
             "StartReplicationTask",
             "StartReplicationTaskAssessment",
             "StartReplicationTaskAssessmentRun",
+            "StopDataMigration",
+            "StopReplication",
             "StopReplicationTask",
             "TestConnection",
             "UpdateConversionConfiguration",
             "UpdateDataProvider",
             "UpdateInstanceProfile",
             "UpdateMigrationProject",
             "UpdateSubscriptionsToEventBridge",
             "UploadFileMetadataList"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "dms:cert-tag/${TagKey}",
-            "dms:dp-tag/${TagKey}",
+            "dms:data-migration-tag/${TagKey}",
+            "dms:data-provider-tag/${TagKey}",
             "dms:endpoint-tag/${TagKey}",
             "dms:es-tag/${TagKey}",
-            "dms:ip-tag/${TagKey}",
-            "dms:mp-tag/${TagKey}",
+            "dms:instance-profile-tag/${TagKey}",
+            "dms:migration-project-tag/${TagKey}",
             "dms:rep-tag/${TagKey}",
+            "dms:replication-config-tag/${TagKey}",
             "dms:req-tag/${TagKey}",
             "dms:subgrp-tag/${TagKey}",
             "dms:task-tag/${TagKey}"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Database Migration Service"
```

### Comparing `iam_actions-1.2.20230601/pyproject.toml` & `iam_actions-1.2.20230602/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230601"
+version = "1.2.20230602"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230601/setup.py` & `iam_actions-1.2.20230602/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230601',
+    'version': '1.2.20230602',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230601/PKG-INFO` & `iam_actions-1.2.20230602/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230601
+Version: 1.2.20230602
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

