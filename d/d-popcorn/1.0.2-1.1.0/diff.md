# Comparing `tmp/d-popcorn-1.0.2.tar.gz` & `tmp/d-popcorn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d-popcorn-1.0.2.tar", last modified: Wed Apr 19 15:07:26 2023, max compression
+gzip compressed data, was "d-popcorn-1.1.0.tar", last modified: Fri Jun  2 08:35:40 2023, max compression
```

## Comparing `d-popcorn-1.0.2.tar` & `d-popcorn-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 15:07:26.769088 d-popcorn-1.0.2/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-12 09:35:52.000000 d-popcorn-1.0.2/LICENSE
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-04-19 15:07:26.769088 d-popcorn-1.0.2/PKG-INFO
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     2256 2023-04-19 14:17:01.000000 d-popcorn-1.0.2/README.md
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 15:07:26.769088 d-popcorn-1.0.2/d_popcorn.egg-info/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-04-19 15:07:26.000000 d-popcorn-1.0.2/d_popcorn.egg-info/PKG-INFO
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      290 2023-04-19 15:07:26.000000 d-popcorn-1.0.2/d_popcorn.egg-info/SOURCES.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        1 2023-04-19 15:07:26.000000 d-popcorn-1.0.2/d_popcorn.egg-info/dependency_links.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       53 2023-04-19 15:07:26.000000 d-popcorn-1.0.2/d_popcorn.egg-info/entry_points.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        6 2023-04-19 15:07:26.000000 d-popcorn-1.0.2/d_popcorn.egg-info/requires.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        8 2023-04-19 15:07:26.000000 d-popcorn-1.0.2/d_popcorn.egg-info/top_level.txt
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 15:07:26.769088 d-popcorn-1.0.2/popcorn/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       55 2023-04-19 15:07:13.000000 d-popcorn-1.0.2/popcorn/__init__.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)    11464 2023-04-18 14:23:23.000000 d-popcorn-1.0.2/popcorn/popcornS3.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     3296 2023-04-19 15:05:27.000000 d-popcorn-1.0.2/popcorn/popcorn_cli.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       38 2023-04-19 15:07:26.769088 d-popcorn-1.0.2/setup.cfg
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1072 2023-04-19 15:06:54.000000 d-popcorn-1.0.2/setup.py
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-12 09:35:52.000000 d-popcorn-1.1.0/LICENSE
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/PKG-INFO
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     3060 2023-06-02 08:27:50.000000 d-popcorn-1.1.0/README.md
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/d_popcorn.egg-info/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/PKG-INFO
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      306 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/SOURCES.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        1 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/dependency_links.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       53 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/entry_points.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        6 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/requires.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        8 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/top_level.txt
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/popcorn/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       22 2023-06-02 08:34:11.000000 d-popcorn-1.1.0/popcorn/__init__.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     6627 2023-06-02 08:29:15.000000 d-popcorn-1.1.0/popcorn/dump.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)    15287 2023-06-02 08:29:16.000000 d-popcorn-1.1.0/popcorn/popcornS3.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     4595 2023-06-02 08:29:16.000000 d-popcorn-1.1.0/popcorn/popcorn_cli.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       38 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/setup.cfg
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1060 2023-06-02 08:29:16.000000 d-popcorn-1.1.0/setup.py
```

### Comparing `d-popcorn-1.0.2/LICENSE` & `d-popcorn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.0.2/README.md` & `d-popcorn-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,60 @@
 # Popcorn
 Popcorn is a command-line tool for managing `.nc` files in the Polarplot dedicated S3 bucket. The script supports uploading and downloading files, listing files, and subscribing to notifications.
 ## Requirements
 - Python 3
 - boto3 library
 
 ## Features
-- Upload and download .nc files to/from the Polarplot dedicated S3 bucket
-- List available files in the bucket
-- Subscribe to bucket notifications
+- Create a new project with its metadata.
+- Upload and download .nc files to/from the Polarplot dedicated S3 bucket.
+- List available files in the bucket.
+- Download .nc files from the bucket.
+- Delete .nc files from the bucket and its corresponding metadata.
+- Subscribe to bucket notifications.
 ## Installation
 You can either install the tool from pip using ``` pip install d-popcorn``` or by following the steps below : 
 
-- Clone the repository: git clone https://github.com/YOUR_USERNAME/puploader.git
+- Clone the repository: git clone git@d-ice.gitlab.host:common/popcorn.git
 - Change into the directory: cd popcorn
-- Install the required libraries: pip install -r requirements.txt
+- Install popcorn locally: `pip install -e i
 - Add your AWS credentials to your environment variables or to your ~/.aws/credentials file. For example:
 
 
 ``` shell
 aws_access_key_id = YOUR_ACCESS_KEY_ID
 aws_secret_access_key = YOUR_SECRET_ACCESS_KEY
 ```
 
 ## Usage
+
+### Create a project
+To create a project, use the following command:
+
+
+```shell
+popcorn create_project PROJECT_CODE --client CLIENT_NAME --project-description "One sentence project description"
+```
+
+PROJECT_CODE should respect the prefixes used internally : ["SCE", "RDX", "RDI", "RDS", "OCX", "SQD", "RBK", "SHY", "THX", "FG"]
+
+
 ### Upload a file
 To upload a file, use the following command:
 
+If the project doesn't exist in the metadata file 
+```shell
+popcorn upload /path/to/file.nc  --project PROJECT_CODE --file-description "Description of the file" --client CLIENT_NAME --project-description "One sentence project description"
+```
 
+If the project already exists in the metadata file you only need to point to this project and give a file description 
 ```shell
-popcorn /path/to/file.nc upload --project PROJECT_CODE --file-description "Description of the file" --client CLIENT_NAME --project-description "One sentence project description" file_to_upload.nc 
+popcorn upload /path/to/file.nc upload --project PROJECT_CODE --file-description "Description of the file"
 ```
+
 Replace PROJECT_CODE, CLIENT_NAME, and /path/to/file.nc with the appropriate values for your file.
 
 PROJECT_CODE should respect the prefixes used internally : ["SCE", "RDX", "RDI", "RDS", "OCX", "SQD", "RBK", "SHY", "THX", "FG"]
 
 
 ### List uploaded files
 To list all uploaded files and their metadata, use the following command:
@@ -51,14 +72,19 @@
 ```
 
 ### Download a file
 ```shell
 popcorn download HASH_VALUE --output /path/to/output/directory
 ```
 
+### Delete a file and it's metadata
+```shell
+popcorn delete HASH_VALUE 
+```
+
 ### Subscribe to bucket notifications  
 
 ```shell
 popcorn subscribe --email your-email@example.com
 ```
 
 ### Remove a subscription
```

### Comparing `d-popcorn-1.0.2/popcorn/popcornS3.py` & `d-popcorn-1.1.0/popcorn/popcornS3.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 import hashlib
 import json
 import os
 import re
 import boto3
 
 
-MANDATORY_REGION = 'us-east-1'
-AWS_ARN_PATTERN = R"^arn:(?P<Partition>[^:\n]*):" \
-                  R"(?P<Service>[^:\n]*):" \
-                  R"(?P<Region>[^:\n]*):" \
-                  R"(?P<AccountID>[^:\n]*):" \
-                  R"(?P<Ignore>(?P<ResourceType>[^:\/\n]*)[:\/])?(?P<Resource>.*)$"
-__dice_projects_prefixes__ = ["SCE", "RDX", "RDI", "RDS", "OCX", "SQD", "RBK", "SHY", "THX", "FG"]
+MANDATORY_REGION = "us-east-1"
+AWS_ARN_PATTERN = (
+    R"^arn:(?P<Partition>[^:\n]*):"
+    R"(?P<Service>[^:\n]*):"
+    R"(?P<Region>[^:\n]*):"
+    R"(?P<AccountID>[^:\n]*):"
+    R"(?P<Ignore>(?P<ResourceType>[^:\/\n]*)[:\/])?(?P<Resource>.*)$"
+)
+__dice_projects_prefixes__ = [
+    "SCE",
+    "RDX",
+    "RDI",
+    "RDS",
+    "OCX",
+    "SQD",
+    "RBK",
+    "SHY",
+    "THX",
+    "FG",
+]
 
 
 class Popcorn:
     def __init__(self):
         self._bucket_name = "polarplot-data"
         self.meta_file = "popcorn_meta.json"
         self._session = boto3.session.Session(region_name=MANDATORY_REGION)
-        self.s3 = boto3.resource('s3')
+        self.s3 = boto3.resource("s3")
         self._bucket = self.s3.Bucket(self._bucket_name)
 
-
-
     def _get_normalized_sns_topic_name(self):
         return f"{self._bucket_name}-sns-topic"
 
     def get_bucket_topic(self):
-        sns = self._session.resource('sns')
+        sns = self._session.resource("sns")
         topic_name = self._get_normalized_sns_topic_name()
 
         bucket_topic = None
         for topic in sns.topics.all():
             if re.match(AWS_ARN_PATTERN, topic.arn)["Resource"] == topic_name:
                 bucket_topic = topic
                 break
@@ -52,89 +63,93 @@
                 "Statement": [
                     {
                         "Effect": "Allow",
                         "Principal": "*",
                         "Action": "sns:Publish",
                         "Resource": bucket_topic.arn,
                         "Condition": {
-                            "ArnLike": {"AWS:SourceArn": f"arn:aws:s3:*:*:{self._bucket_name}"},
+                            "ArnLike": {
+                                "AWS:SourceArn": f"arn:aws:s3:*:*:{self._bucket_name}"
+                            },
                         },
                     },
                 ],
             }
 
             bucket_topic.set_attributes(
-                AttributeName='Policy',
-                AttributeValue=json.dumps(sns_topic_policy)
+                AttributeName="Policy", AttributeValue=json.dumps(sns_topic_policy)
             )
 
             # Set notification config
             notification = self._bucket.Notification()
 
-            notification.put(NotificationConfiguration={
-                'TopicConfigurations': [
-                    {
-                        'TopicArn': bucket_topic.arn,
-                        'Events': [  # s3 Events we want to trig notification
-                            's3:ObjectCreated:*',
-                            's3:ObjectRemoved:*',
-                            's3:ObjectRestore:*',
-                        ]
-                    }
-                ]
-            }
+            notification.put(
+                NotificationConfiguration={
+                    "TopicConfigurations": [
+                        {
+                            "TopicArn": bucket_topic.arn,
+                            "Events": [  # s3 Events we want to trig notification
+                                "s3:ObjectCreated:*",
+                                "s3:ObjectRemoved:*",
+                                "s3:ObjectRestore:*",
+                            ],
+                        }
+                    ]
+                }
             )
 
         return bucket_topic
 
     def subscribe_to_bucket_notifications(self, email: str):
         # 1- on veut recuperer le topic associe a ce bucket
         bucket_topic = self.get_bucket_topic()
 
         # Getting subscriptions
         for subscription in bucket_topic.subscriptions.all():
-            if subscription.arn == 'PendingConfirmation':
+            if subscription.arn == "PendingConfirmation":
                 continue
 
-            if subscription.attributes['Endpoint'] == email:
+            if subscription.attributes["Endpoint"] == email:
                 return None
 
-        subscription = bucket_topic.subscribe(Protocol='email', Endpoint=email)
+        subscription = bucket_topic.subscribe(Protocol="email", Endpoint=email)
 
         return subscription
 
     def list_subscriptions(self):
         bucket_topic = self.get_bucket_topic()
 
         subscriptions = []
         for subscription in bucket_topic.subscriptions.all():
-            if subscription.arn == 'PendingConfirmation':
-                subscriptions.append('Pending Subscription')
+            if subscription.arn == "PendingConfirmation":
+                subscriptions.append("Pending Subscription")
 
             else:
-                subscriptions.append(subscription.attributes['Endpoint'])
+                subscriptions.append(subscription.attributes["Endpoint"])
 
         return subscriptions
 
     def remove_subscription(self, email: str):
         bucket_topic = self.get_bucket_topic()
 
         subscription_to_delete = None
         for subscription in bucket_topic.subscriptions.all():
-            if subscription.arn == 'PendingConfirmation':
+            if subscription.arn == "PendingConfirmation":
                 continue
 
-            if subscription.attributes['Endpoint'] == email:
+            if subscription.attributes["Endpoint"] == email:
                 subscription_to_delete = subscription
 
         if subscription_to_delete is not None:
             subscription_to_delete.delete()
-            print(f'This subscription is deleted')
+            print(f"This subscription is deleted")
         else:
-            print(f'\t> Email address {email} was not subscribing to the bucket notifications')
+            print(
+                f"\t> Email address {email} was not subscribing to the bucket notifications"
+            )
 
     def subscribe(self, args):
         if args.list:
             print("\nList of subscriptions:")
             for subscription_email in self.list_subscriptions():
                 print(f"\t* {subscription_email}")
 
@@ -152,128 +167,225 @@
                 print(f"\t> {args.email} was already subscribing")
 
         if args.remove:
             print(f"\nRemoving email address {args.remove} from the subscriptions")
             self.remove_subscription(args.remove)
 
     def list_files(self, args):
-        with self._bucket.Object(self.meta_file).get()['Body'] as f:
-            file_content = f.read().decode('utf-8')
+        with self._bucket.Object(self.meta_file).get()["Body"] as f:
+            file_content = f.read().decode("utf-8")
             meta_data = json.loads(file_content)
         if args.project:
-            # Is the project existing?
-            new_metadata = {}
-
-            for hash_key, metadata_dict in meta_data.items():
-                project_name = metadata_dict['project']
-                if project_name not in new_metadata:
-                    new_metadata[project_name] = {}
-                new_metadata[project_name][hash_key] = {
-                    'client': metadata_dict['client'],
-                    'file-description': metadata_dict['file-description'],
-                }
-                new_metadata[project_name]["project-description"] = metadata_dict['project-description']
-
-            for project_key, metadata_dict in new_metadata.items():
-                print("Project : {}".format(project_key))
-                print(f"Project Description:               {metadata_dict['project-description']}")
-                for hash_key, file_data in metadata_dict.items():
-                    if hash_key != "project-description":
-                        print(f"\n\t File: {hash_key}")
-                        print(f"\t\t Client:                          {file_data['client']}")
-                        print(f"\t\t File Description:                {file_data['file-description']}")
+            if args.project not in meta_data["projects"]:
+                print(f"No such project: {args.project}")
+                return
+            project_metadata = meta_data["projects"][args.project]
+            print(f"Project : {args.project}")
+            print(f"Client : {project_metadata['client']}")
+            print(f"Project Description: {project_metadata['project-description']}")
+
+            file_metadata = {
+                k: v
+                for k, v in meta_data["files"].items()
+                if v["project"] == args.project
+            }
+            for hash_key, file_data in file_metadata.items():
+                print(f"\n\t File: {hash_key}")
+                print(f"\t\t File Description: {file_data['file-description']}")
+
+            # for hash_key, metadata_dict in meta_data.items():
+            #     project_name = metadata_dict['project']
+            #     if project_name not in new_metadata:
+            #         new_metadata[project_name] = {}
+            #     new_metadata[project_name][hash_key] = {
+            #         'client': metadata_dict['client'],
+            #         'file-description': metadata_dict['file-description'],
+            #     }
+            #     new_metadata[project_name]["project-description"] = metadata_dict['project-description']
+            #
+            # for project_key, metadata_dict in new_metadata.items():
+            #     print("Project : {}".format(project_key))
+            #     print(f"Project Description:               {metadata_dict['project-description']}")
+            #     for hash_key, file_data in metadata_dict.items():
+            #         if hash_key != "project-description":
+            #             print(f"\n\t File: {hash_key}")
+            #             print(f"\t\t Client:                          {file_data['client']}")
+            #             print(f"\t\t File Description:                {file_data['file-description']}")
         else:
-            for hash_key, metadata_dict in meta_data.items():
+            for hash_key, file_data in meta_data["files"].items():
                 print("File : {}".format(hash_key))
-                print(f"\t Project:                         {metadata_dict['project']}")
-                print(f"\t Client:                          {metadata_dict['client']}")
-                print(f"\t Project Description:             {metadata_dict['project-description']}")
-                print(f"\t File Description:                {metadata_dict['file-description']}")
+                print(f"\t Project:                         {file_data['project']}")
+                project_data = meta_data["projects"][file_data["project"]]
+                print(f"\t Client:                          {project_data['client']}")
+                print(
+                    f"\t Project Description:             {project_data['project-description']}"
+                )
+                print(
+                    f"\t File Description:                {file_data['file-description']}"
+                )
             return
 
     def get_file_hashes(self):
         hashes = []
 
         # get all objects with .nc extension in bucket
         objects = self._bucket.objects.all()
-        files = [obj.key for obj in objects if obj.key.endswith('.nc')]
+        files = [obj.key for obj in objects if obj.key.endswith(".nc")]
 
         # calculate hash for each file and add to hashes list
         for file in files:
             response = self._bucket.Object(file).get()
             hasher = hashlib.sha256()
-            hasher.update(response['Body'].read())
+            hasher.update(response["Body"].read())
             hashes.append(hasher.hexdigest())
         return hashes
 
     def _get_metadata(self):
         try:
-            with self._bucket.Object(self.meta_file).get() as f:
-                metadata = json.loads(f.read().decode('utf-8'))
-                return metadata
-        except Exception:
-            return {}
+            # with self._bucket.Object(self.meta_file).get() as f:
+            #     metadata = json.loads(f.read().decode('utf-8'))
+            #     print(metadata)
+            #     return metadata
+            response = self._bucket.Object(self.meta_file).get()
+            existing_metadata = json.loads(response["Body"].read().decode("utf-8"))
+            print(existing_metadata)
+            return existing_metadata
+        except Exception as e:
+            print("here", e)
+            return {"files": {}, "projects": {}}
 
     def _generate_hash(self, file):
         hasher = hashlib.sha256()
-        with open(file, 'rb') as f:
+        with open(file, "rb") as f:
             buf = f.read()
             hasher.update(buf)
         return hasher.hexdigest()
 
     def upload(self, args):
+        #####################
+        #  HANDLE METADATA  #
+        #####################
+        # Get existing metadata
+        metadata = self._get_metadata()
         # generate unique hash for file
         file_hash = self._generate_hash(args.file)
-        # set polaplot link
+        # set polarplot link
         link = "http://polarplot.d-ice.net/polarplot/" + file_hash
         # get file name from path
         file_name = os.path.basename(args.file)
+        # Build metadata tags dictionary for the file
+        file_metadata_tags = {
+            "project": args.project,
+            "file-description": args.file_description,
+        }
+        # test if project prefix is valid (RDX, SCE etc...)
+        pattern = "^(" + "|".join(__dice_projects_prefixes__) + ")[0-9]{3}$"
+        if not bool(re.match(pattern, args.project)):
+            raise RuntimeError(
+                f"Projects names must have the following form: <prefix><number> where "
+                f"prefix is in {__dice_projects_prefixes__} and "
+                f"number is a 3-digit number referencing the project number."
+                f"\nExample: SCE072"
+            )
+
+        if args.project not in metadata["projects"]:
+            print("Adding project metadata to json")
+            project_metadata_tags = {
+                "client": args.client,
+                "project-description": args.project_description,
+            }
+            metadata["projects"][args.project] = project_metadata_tags
 
+        if file_hash not in metadata["files"]:
+            print("Adding file metadata to json")
+            metadata["files"][file_hash] = file_metadata_tags
+
+        self._bucket.put_object(Body=json.dumps(metadata), Key=self.meta_file)
+        print(f"Metadata for {file_name} added successfully.")
+        #####################
+        #    HANDLE FILE    #
+        #####################
         # check if file with same hash already exists
         for f in self.get_file_hashes():
             if f == file_hash:
-                print(f"The file {file_name} already exists with the same hash {file_hash}.")
+                print(
+                    f"The file {file_name} already exists with the same hash {file_hash}."
+                )
                 print(f"You can visualize the uploaded data using this link: {link}")
                 return
 
-        # TODO: tester si project est valide (RDX, SCE etc...)
-        pattern = "^(" + "|".join(__dice_projects_prefixes__) + ")[0-9]{3}$"
-        if not bool(re.match(pattern, args.project)):
-            raise RuntimeError(f"Projects names must have the following form: <prefix><number> where "
-                               f"prefix is in {__dice_projects_prefixes__} and "
-                               f"number is a 3-digit number referencing the project number."
-                               f"\nExample: SCE072")
-
         # upload file to bucket with client and project metadata
-        metadata_tags = {'client': args.client,
-                         'project': args.project,
-                         'project-description': args.project_description,
-                         'file-description': args.file_description}
-        with open(args.file, 'rb') as f:
-            self._bucket.put_object(Body=f, Key=file_hash + '.nc', Metadata=metadata_tags)
-
-        # add file metadata to metadata file with hash as key
-        metadata = self._get_metadata()
-        metadata[file_hash] = metadata_tags
+        with open(args.file, "rb") as f:
+            self._bucket.put_object(
+                Body=f, Key=file_hash + ".nc", Metadata=file_metadata_tags
+            )
 
-        # write updated metadata file
-        self._bucket.put_object(Body=json.dumps(metadata), Key=self.meta_file)
         print(f"{file_name} uploaded successfully. File hash {file_hash} ")
         print(f"You can visualize the uploaded data using this link: {link}")
 
     def download(self, args):
         # retrieve metadata for file with hash
         metadata = self._get_metadata()
-        nc_file = args.hash + '.nc'
+        nc_file = args.hash + ".nc"
         if not any(obj.key == nc_file for obj in self._bucket.objects.all()):
             # print(f"The file {key} does not exist in the bucket {bucket_name}.")
             print(f"No file with hash {args.hash} found.")
             print(self.list_files(args))
             return
         # Get the S3 object
         s3_object = self.s3.Object(self._bucket_name, nc_file)
         # Download the file from S3 to a local file
-        local_file_path = str(os.path.join(args.output, os.path.basename(s3_object.key)))
+        local_file_path = str(
+            os.path.join(args.output, os.path.basename(s3_object.key))
+        )
         print(f"Downloading file to: {local_file_path}")
         s3_object.download_file(local_file_path)
         print("Download succeeded")
         return
+
+    def create_project(self, args):
+        pattern = "^(" + "|".join(__dice_projects_prefixes__) + ")[0-9]{3}$"
+        if not bool(re.match(pattern, args.project)):
+            raise RuntimeError(
+                f"Projects names must have the following form: <prefix><number> where "
+                f"prefix is in {__dice_projects_prefixes__} and "
+                f"number is a 3-digit number referencing the project number."
+                f"\nExample: SCE072"
+            )
+
+        project_metadata_tags = {
+            "client": args.client,
+            "project-description": args.project_description,
+        }
+
+        metadata = self._get_metadata()
+
+        if args.project in metadata["projects"]:
+            print(f"The project {args.project} already exists.")
+            return
+
+        metadata["projects"][args.project] = project_metadata_tags
+
+        self._bucket.put_object(Body=json.dumps(metadata), Key=self.meta_file)
+        print(f"Project {args.project} created successfully.")
+
+    def delete_file(self, args):
+        metadata = self._get_metadata()
+
+        # Check if file hash exists in the metadata
+        if args.file_hash not in self.get_file_hashes():
+            print(f"No file found with the hash {args.file_hash}.")
+            return
+
+        try:
+            self._bucket.Object(args.file_hash + ".nc").delete()
+            print(f"File {args.file_hash} deleted successfully from the bucket.")
+        except Exception as e:
+            print(
+                f"An error occurred while deleting the file from the bucket: {str(e)}"
+            )
+            return
+
+        if args.file_hash in metadata["files"]:
+            del metadata["files"][args.file_hash]
+            self._bucket.put_object(Body=json.dumps(metadata), Key=self.meta_file)
+            print("Metadata updated successfully.")
```

### Comparing `d-popcorn-1.0.2/setup.py` & `d-popcorn-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,30 @@
 
 __version__ = "Undefined"
 for line in open(os.path.join("popcorn", "__init__.py")):
     if line.startswith("__version__"):
         exec(line.strip())
 
 setup(
-    name='d-popcorn',
+    name="d-popcorn",
     version=__version__,
     description="A command line tool to push data to "
-                "the Polarplot dedicated AWS S3 bucket for D-ICE Engineering needs.",
-
+    "the Polarplot dedicated AWS S3 bucket for D-ICE Engineering needs.",
     author="Omar El Bakouchi",
     author_email="omar.elbakouchi@dice-engineering.com",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Natural Language :: English",
     ],
     packages=find_packages(),
     install_requires=[
-        'boto3',
+        "boto3",
     ],
     entry_points={
-        'console_scripts': [
-            'popcorn=popcorn.popcorn_cli:main',
+        "console_scripts": [
+            "popcorn=popcorn.popcorn_cli:main",
         ],
     },
-)
+)
```

