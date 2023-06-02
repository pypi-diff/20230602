# Comparing `tmp/pyrc-python-utils-0.0.2.tar.gz` & `tmp/pyrc-python-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-python-utils-0.0.2.tar", last modified: Mon May 22 19:35:44 2023, max compression
+gzip compressed data, was "pyrc-python-utils-0.0.4.tar", last modified: Fri Jun  2 18:27:12 2023, max compression
```

## Comparing `pyrc-python-utils-0.0.2.tar` & `pyrc-python-utils-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.669543 pyrc-python-utils-0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       57 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      460 2023-05-22 19:35:44.668543 pyrc-python-utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-06 11:45:56.000000 pyrc-python-utils-0.0.2/README.md
--rw-rw-rw-   0        0        0      630 2023-05-22 19:34:17.000000 pyrc-python-utils-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 19:35:44.669543 pyrc-python-utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      394 2023-05-22 19:30:49.000000 pyrc-python-utils-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.633543 pyrc-python-utils-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.655543 pyrc-python-utils-0.0.2/src/pyrc_python_utils/
--rw-rw-rw-   0        0        0        0 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/__init__.py
--rw-rw-rw-   0        0        0     1153 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_datetime.py
--rw-rw-rw-   0        0        0     5730 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_exchange.py
--rw-rw-rw-   0        0        0      229 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_file.py
--rw-rw-rw-   0        0        0     1352 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_ms_teams.py
--rw-rw-rw-   0        0        0    28193 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sftp.py
--rw-rw-rw-   0        0        0     6416 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sharepoint.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.666543 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/
--rw-rw-rw-   0        0        0      460 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:12.118957 pyrc-python-utils-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-30 19:52:10.000000 pyrc-python-utils-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-30 19:52:10.000000 pyrc-python-utils-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-06-02 18:27:12.117957 pyrc-python-utils-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-30 19:52:10.000000 pyrc-python-utils-0.0.4/README.md
+-rw-rw-rw-   0        0        0      654 2023-06-02 18:26:57.000000 pyrc-python-utils-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 18:27:12.118957 pyrc-python-utils-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:12.087960 pyrc-python-utils-0.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-01 11:37:45.000000 pyrc-python-utils-0.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:12.104957 pyrc-python-utils-0.0.4/src/pyrc_python_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-30 19:52:10.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/__init__.py
+-rw-rw-rw-   0        0        0     1199 2023-06-01 11:13:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_datetime.py
+-rw-rw-rw-   0        0        0     5776 2023-06-01 11:13:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_exchange.py
+-rw-rw-rw-   0        0        0     3438 2023-06-02 11:30:13.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_file.py
+-rw-rw-rw-   0        0        0     1382 2023-06-01 11:13:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_ms_teams.py
+-rw-rw-rw-   0        0        0    19013 2023-06-02 18:24:49.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_s3.py
+-rw-rw-rw-   0        0        0    30466 2023-06-01 11:13:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_sftp.py
+-rw-rw-rw-   0        0        0     6440 2023-06-01 11:13:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_sharepoint.py
+-rw-rw-rw-   0        0        0       77 2023-06-01 11:13:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_string.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:12.113957 pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-06-02 18:27:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-06-02 18:27:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 18:27:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-02 18:27:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-02 18:27:12.000000 pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:12.115957 pyrc-python-utils-0.0.4/tests/
+-rw-rw-rw-   0        0        0    12451 2023-06-02 12:37:28.000000 pyrc-python-utils-0.0.4/tests/test_util_s3.py
```

### Comparing `pyrc-python-utils-0.0.2/LICENSE` & `pyrc-python-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-0.0.2/pyproject.toml` & `pyrc-python-utils-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrc-python-utils"
-version = "0.0.2"
+version = "0.0.4"
 description = "Generic set of helper functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "O365>=2.0.26",
     "paramiko>=3.1.0",
-    "pymsteams>=0.2.2"
+    "pymsteams>=0.2.2",
+    "boto3>=1.26.141"
 ]
 
 [project.urls]
 # "Homepage" = "https://github.com/pypa/sampleproject"
 # "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_datetime.py` & `pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_datetime.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# TODO: Add Unit Tests
+# TODO: Add comments
 from datetime import datetime, timedelta
 
 
 def get_utc_now(offset_minutes: int) -> str:
     """
     Returns the current UTC time adjusted by a specified offset.
```

### Comparing `pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_exchange.py` & `pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# TODO: Add Unit Tests
+# TODO: Add comments
 # An Exchange convenience wrapper around python-o365 library - https://github.com/O365/python-o365
 # Source reference
 # - https://github.com/O365/python-o365/blob/master/O365/mailbox.py
 # - https://github.com/O365/python-o365/blob/master/O365/message.py
 # Message properties
 # - https://learn.microsoft.com/en-us/graph/api/resources/message?view=graph-rest-1.0
 # - https://learn.microsoft.com/en-us/graph/filter-query-parameter?tabs=http
```

### Comparing `pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_ms_teams.py` & `pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_ms_teams.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,35 @@
+# TODO: Add Unit Tests
 import pymsteams
 
-def post_to_teams(webhook:str,message:str) -> str:
+
+def post_to_teams(webhook: str, message: str) -> str:
     """
     Posts a simple message to a Teams Channel via webhook.
     Pass the webhook and message to the function and the message will be posted to the channel.
 
     :param webhook: a unique link generated by Microsoft Teams that allows posts to a channel via api.
     :type host: str
-
     :param message: The message that will be posted to said Teams channel.
     :type host: str
-
     :return: On success nothing is returned.
     :rtype: None
-    
     :return: Upon an exception, the exception message is returned. 
     :rtype: str
 
     To generate a webhook:
     * Navigate to the channel where you want to add the webhook
         * select (•••) Connectors from the top navigation bar.
         * Search for Incoming Webhook, and add it.
         * Click Configure and provide a name for your webhook.
         * Copy the URL which appears and click "OK".
     """
     try:
-        
+
         # Define connector to MS Teams - using provided webhook
-        myTeamsMessage = pymsteams.connectorcard(webhook)
+        connector_card = pymsteams.connectorcard(webhook)
         # Define the message to post
-        myTeamsMessage.text(message)
+        connector_card.text(message)
         # Method to post message to channel
-        myTeamsMessage.send()
-    except Exception as E:
-        # Return any caught exceptions
-        return E
-    
+        connector_card.send()
+    except Exception as e:
+        raise Exception(f"Failed to create card for webhook {webhook}.") from e
```

### Comparing `pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sftp.py` & `pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_sftp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# TODO: Add remove_files, remove_files_from_list
+# TODO: Clean up comments
+# TODO: Update examples with newest functions
+# TODO: Add Unit Tests
 # A SFTP convenience wrapper around python-o365 library - https://github.com/paramiko/paramiko
 # Source reference - https://github.com/paramiko/paramiko/tree/main/paramiko
 # See examples/sftp folder for usage scenarios
 import os
 import re
 import stat
 from io import BytesIO
@@ -45,46 +49,46 @@
     """
     try:
         client.close()
     except Exception as e:
         raise IOError("Failed to close the connection with the SFTP server.") from e
 
 
-def create_directory(client: paramiko.SFTPClient, remote_path: str):
+def create_directory(client: paramiko.SFTPClient, remote_directory: str):
     """
     Creates a directory at the specified path on the remote server if it does not already exist.
 
     :param client: The SFTP client used to interact with the remote server.
     :type client: paramiko.SFTPClient
-    :param remote_path: The path where the directory will be created on the remote server.
-    :type remote_path: str
+    :param remote_directory: The path where the directory will be created on the remote server.
+    :type remote_directory: str
     :raises IOError: If the directory creation fails due to any exception.
     """
     try:
-        if not directory_exists(client, remote_path):
-            client.mkdir(remote_path)
+        if not directory_exists(client, remote_directory):
+            client.mkdir(remote_directory)
     except Exception as e:
-        raise IOError(f"Failed to create directory at {remote_path}.") from e
+        raise IOError(f"Failed to create directory at {remote_directory}.") from e
 
 
-def remove_directory(client: paramiko.SFTPClient, remote_path: str):
+def remove_directory(client: paramiko.SFTPClient, remote_diretory: str):
     """
     Removes a directory from the remote SFTP server.
 
     :param client: The SFTP client used to interact with the remote server.
     :type client: paramiko.SFTPClient
-    :param remote_path: The full path to the existing directory (e.g. new-dir-name, dir-name/new-dir-name)
-    :type remote_path: str
+    :param remote_diretory: The full path to the existing directory (e.g. new-dir-name, dir-name/new-dir-name)
+    :type remote_diretory: str
     :raises IOError: If an error occurs while trying to remove the directory.
     """
     try:
-        if directory_exists(client, remote_path):
-            client.rmdir(remote_path)
+        if directory_exists(client, remote_diretory):
+            client.rmdir(remote_diretory)
     except Exception as e:
-        raise IOError(f"Failed to remove directory {remote_path} from the SFTP server.") from e
+        raise IOError(f"Failed to remove directory {remote_diretory} from the SFTP server.") from e
 
 
 def remove_file(client: paramiko.SFTPClient, remote_file: str):
     """
     Removes a file from the remote SFTP server.
 
     :param client: The SFTP client used to interact with the remote server.
@@ -95,460 +99,481 @@
     """
     if file_exists(client, remote_file):
         try:
             client.remove(remote_file)
         except Exception as e:
             raise IOError(f'Error while attempting to remove file: {remote_file}') from e
     else:
-        raise IOError(f'remote_file does not exist: {remote_file}')
+        raise FileNotFoundError(f'remote_file does not exist: {remote_file}')
 
 
-def rebuild_directory(client: paramiko.SFTPClient, remote_path: str):
+def rebuild_directory(client: paramiko.SFTPClient, remote_directory: str):
     """
     Removes and re-creates a directory on the remote SFTP server.
 
     :param client: The SFTP client used to interact with the remote server.
     :type client: paramiko.SFTPClient
-    :param remote_path: The full path to the directory to be removed and recreated (e.g. dir-name, dir-name/sub-dir-name)
-    :type remote_path: str
+    :param remote_directory: The full path to the directory to be removed and recreated (e.g. dir-name, dir-name/sub-dir-name)
+    :type remote_directory: str
     :raises Exception: If there's an error while removing or creating the directory.
     """
     try:
         # Delete the directory if it exists
-        remove_directory(client, remote_path)
+        remove_directory(client, remote_directory)
 
         # Recreate the directory
-        create_directory(client, remote_path)
+        create_directory(client, remote_directory)
     except Exception as e:
-        raise Exception(f'Error while attempting to rebuild directory: {remote_path}') from e
+        raise Exception(f'Error while attempting to rebuild directory: {remote_directory}') from e
 
 
-def copy_file(client: paramiko.SFTPClient, source_remote_file: str, target_remote_path: str,
-              target_remote_file: Optional[str] = None, buffer_size=8192, overwrite_target_file: bool = True):
+def copy_file(client: paramiko.SFTPClient, source_remote_file: str, target_remote_directory: str,
+              target_remote_file: Optional[str] = None, overwrite_target_file: Optional[bool] = True):
     """
     Copies a file from a source path to a target path on a remote system using SFTP.
 
     The function reads the source file in chunks, writes to the destination file,
     and avoids loading the entire file into memory at once. If the target file already
     exists and `overwrite_target_file` is `False`, it will use a different name for the
     copied file to avoid overwriting.
 
     :param client: The SFTP client used for file transfer.
     :type client: paramiko.SFTPClient
     :param source_remote_file: The path to the source file on the remote system.
     :type source_remote_file: str
-    :param target_remote_path: The directory path where the file will be copied to on the remote system.
-    :type target_remote_path: str
+    :param target_remote_directory: The directory path where the file will be copied to on the remote system.
+    :type target_remote_directory: str
     :param target_remote_file: The name of the copied file. If `None`, the source file name is used. Defaults to `None`.
     :type target_remote_file: Optional[str]
-    :param buffer_size: The size of chunks in which the file is read. Defaults to 8192.
-    :type buffer_size: int
     :param overwrite_target_file: Whether to overwrite the target file if it already exists. Defaults to `True`.
     :type overwrite_target_file: bool
     :raises IOError: If the source file does not exist or is not a file, or if the target directory does not exist
     :return: None
     """
     # Check if the source file exists and is a file
     if not file_exists(client, source_remote_file):
         raise IOError(f"The source file does not exist or is not a file: {source_remote_file}")
 
     # Check if the target directory exists
-    if not directory_exists(client, target_remote_path):
-        raise IOError(f"The target directory does not exist: {target_remote_path}")
+    if not directory_exists(client, target_remote_directory):
+        raise IOError(f"The target directory does not exist: {target_remote_directory}")
 
     # If target_remote_file is not provided, us
     target_remote_file = target_remote_file or os.path.basename(source_remote_file)
-    full_path = f"{target_remote_path}/{target_remote_file}"
+    full_path = f"{target_remote_directory}/{target_remote_file}"
 
     if not overwrite_target_file:
         full_path = get_next_available_filename(full_path)
 
     with client.open(source_remote_file, 'rb') as source_file, client.open(full_path, 'wb') as destination_file:
-        for data in iter(lambda: source_file.read(buffer_size), b''):
+        for data in iter(lambda: source_file.read(8192), b''):
             destination_file.write(data)
 
 
-def copy_files(client: paramiko.SFTPClient, source_remote_path: str, target_remote_path: str,
-               match_exp: Optional[str] = None,
-               buffer_size: int = 8192):
+def copy_files(client: paramiko.SFTPClient, source_remote_directory: str, target_remote_directory: str,
+               match_regex: Optional[str] = None, overwrite_target_file: Optional[bool] = True):
     """
     Copies all files (or those matching a given regex pattern) from one remote directory to another.
 
     :param client: The SFTP client used to interact with the remote server.
     :type client: paramiko.SFTPClient
-    :param source_remote_path: The full path to the source directory on the remote server.
-    :type source_remote_path: str
-    :param target_remote_path: The full path to the target directory on the remote server.
-    :type target_remote_path: str
-    :param match_exp: The regex pattern to match the files to be copied. If None, all files are copied. Defaults to None.
-    :type match_exp: str, optional
-    :param buffer_size: The buffer size to use during the file transfer. Defaults to 8192.
-    :type buffer_size: int, optional
+    :param source_remote_directory: The full path to the source directory on the remote server.
+    :type source_remote_directory: str
+    :param target_remote_directory: The full path to the target directory on the remote server.
+    :type target_remote_directory: str
+    :param match_regex: The regex pattern to match the files to be copied. If None, all files are copied. Defaults to None.
+    :type match_regex: str, optional
+    :param overwrite_target_file: Whether to overwrite the target file if it already exists. Defaults to `True`.
+    :type overwrite_target_file: bool
     :raises Exception: If there's an error while copying files.
     """
     try:
-        for remote_file in client.listdir(source_remote_path):
-            full_path = f"{source_remote_path}/{remote_file}"
-            if file_exists(client, full_path) and (match_exp is None or re.match(match_exp, remote_file)):
-                copy_file(client, full_path, target_remote_path, buffer_size=buffer_size)
+        for remote_file in client.listdir(source_remote_directory):
+            full_path = f"{source_remote_directory}/{remote_file}"
+            if file_exists(client, full_path) and (match_regex is None or re.match(match_regex, remote_file)):
+                copy_file(client, full_path, target_remote_directory, overwrite_target_file=overwrite_target_file)
     except Exception as e:
         raise Exception(
-            f'Error while attempting to copy files from {source_remote_path} to {target_remote_path}') from e
+            f'Error while attempting to copy files from {source_remote_directory} to {target_remote_directory}') from e
 
 
-def copy_files_from_list(client: paramiko.SFTPClient, remote_file_list: List[str], target_remote_path: str,
-                         buffer_size: int = 8192) -> None:
+def copy_files_from_list(client: paramiko.SFTPClient, remote_file_list: List[str], target_remote_directory: str,
+                         overwrite_target_file: Optional[bool] = True) -> None:
     """
     Copy a list of files to a specified remote directory using an SFTP client.
 
     :param client: A connected SFTPClient object.
     :type client: paramiko.SFTPClient
     :param remote_file_list: A list of full path strings to the remote files to be copied.
     :type remote_file_list: List[str]
-    :param target_remote_path: The target directory on the remote system where the files should be copied to.
-    :type target_remote_path: str
-    :param buffer_size: The buffer size to use while copying files, defaults to 8192.
-    :type buffer_size: int, optional
+    :param target_remote_directory: The target directory on the remote system where the files should be copied to.
+    :type target_remote_directory: str
+    :param overwrite_target_file: Whether to overwrite the target file if it already exists. Defaults to `True`.
+    :type overwrite_target_file: bool
     """
     for remote_file in remote_file_list:
-        copy_file(client, remote_file, target_remote_path, buffer_size=buffer_size)
+        copy_file(client, remote_file, target_remote_directory, overwrite_target_file=overwrite_target_file)
 
 
-def move_file(client: paramiko.SFTPClient, source_remote_file: str, target_remote_path: str,
-              target_remote_file: Optional[str] = None, buffer_size=8192, overwrite_target_file: bool = True):
+def move_file(client: paramiko.SFTPClient, source_remote_file: str, target_remote_directory: str,
+              target_remote_file: Optional[str] = None, overwrite_target_file: Optional[bool] = True):
     """
     Moves a file from a source path to a target path on a remote system using SFTP.
 
     As SFTP does not support moving files directly, this function first copies the file to the target path,
     and then deletes the source file. If the target file already exists and `overwrite_target_file` is `False`,
     it will use a different name for the moved file to avoid overwriting.
 
     :param client: The SFTP client used for file transfer.
     :type client: paramiko.SFTPClient
     :param source_remote_file: The path to the source file on the remote system.
     :type source_remote_file: str
-    :param target_remote_path: The directory path where the file will be moved to on the remote system.
-    :type target_remote_path: str
+    :param target_remote_directory: The directory path where the file will be moved to on the remote system.
+    :type target_remote_directory: str
     :param target_remote_file: The name of the moved file. If `None`, the source file name is used. Defaults to `None`.
     :type target_remote_file: Optional[str]
-    :param buffer_size: The size of chunks in which the file is read and written. Defaults to 8192.
-    :type buffer_size: int
     :param overwrite_target_file: Whether to overwrite the target file if it already exists. Defaults to `True`.
     :type overwrite_target_file: bool
     :raises IOError: If the source file does not exist or is not a file.
     :return: None
     """
-    copy_file(client, source_remote_file, target_remote_path, target_remote_file, buffer_size, overwrite_target_file)
+    copy_file(client, source_remote_file, target_remote_directory, target_remote_file, overwrite_target_file)
     remove_file(client, source_remote_file)
 
 
-def move_files(client: paramiko.SFTPClient, source_remote_path: str, target_remote_path: str,
-               match_exp: Optional[str] = None,
-               buffer_size=8192):
+def move_files(client: paramiko.SFTPClient, source_remote_directory: str, target_remote_directory: str,
+               match_exp: Optional[str] = None, overwrite_target_file: Optional[bool] = True):
     """
     Moves files from a source directory to a target directory on a remote system using SFTP.
 
     This function moves all files or those matching the provided regular expression from the source directory
     to the target directory. As SFTP does not support moving files directly, this function first copies the file
     to the target path, and then deletes the source file.
 
     :param client: The SFTP client used for file transfer.
     :type client: paramiko.SFTPClient
-    :param source_remote_path: The directory path of the source files on the remote system.
-    :type source_remote_path: str
-    :param target_remote_path: The directory path where the files will be moved to on the remote system.
-    :type target_remote_path: str
+    :param source_remote_directory: The directory path of the source files on the remote system.
+    :type source_remote_directory: str
+    :param target_remote_directory: The directory path where the files will be moved to on the remote system.
+    :type target_remote_directory: str
     :param match_exp: A regular expression to filter the files to be moved. If `None`, all files are moved. Defaults to `None`.
     :type match_exp: Optional[str]
-    :param buffer_size: The size of chunks in which the file is read and written. Defaults to 8192.
-    :type buffer_size: int
+    :param overwrite_target_file: Whether to overwrite the target file if it already exists. Defaults to `True`.
+    :type overwrite_target_file: bool
     :raises IOError: If a source file does not exist, is not a file, or an error occurs during the move operation.
     :return: None
     """
-    for remote_file in client.listdir(source_remote_path):
-        full_path = f"{source_remote_path}/{remote_file}"
+    for remote_file in client.listdir(source_remote_directory):
+        full_path = f"{source_remote_directory}/{remote_file}"
         if is_file(client, full_path) and (match_exp is None or re.match(match_exp, remote_file)):
-            move_file(client, full_path, target_remote_path, buffer_size=buffer_size)
+            move_file(client, full_path, target_remote_directory, overwrite_target_file=overwrite_target_file)
 
 
-def move_files_from_list(client: paramiko.SFTPClient, remote_file_list: list[str], target_remote_path: str,
-                         buffer_size=8192):
+def move_files_from_list(client: paramiko.SFTPClient, remote_file_list: list[str], target_remote_directory: str,
+                         overwrite_target_file: Optional[bool] = True):
     """
     Moves a list of files from their source paths to a target directory on a remote system using SFTP.
 
     This function moves all files in the provided list to the target directory. As SFTP does not support moving
     files directly, this function first copies the file to the target path, and then deletes the source file.
 
     :param client: The SFTP client used for file transfer.
     :type client: paramiko.SFTPClient
     :param remote_file_list: A list of the full paths to the source files on the remote system.
     :type remote_file_list: List[str]
-    :param target_remote_path: The directory path where the files will be moved to on the remote system.
-    :type target_remote_path: str
-    :param buffer_size: The size of chunks in which the file is read and written. Defaults to 8192.
-    :type buffer_size: int
+    :param target_remote_directory: The directory path where the files will be moved to on the remote system.
+    :type target_remote_directory: str
+    :param overwrite_target_file: Whether to overwrite the target file if it already exists. Defaults to `True`.
+    :type overwrite_target_file: bool
     :raises IOError: If a source file does not exist, is not a file.
     :return: None
     """
     for remote_file in remote_file_list:
-        move_file(client, remote_file, target_remote_path, buffer_size=buffer_size)
+        move_file(client, remote_file, target_remote_directory, overwrite_target_file=overwrite_target_file)
 
 
-def put_file(client: paramiko.SFTPClient, local_file: Union[str, bytes], remote_path: str,
+def put_file(client: paramiko.SFTPClient, local_file: Union[str, bytes], remote_directory: Optional[str] = '.',
              remote_file: Optional[str] = None,
-             overwrite_remote_file: bool = True):
+             overwrite_remote_file: Optional[bool] = True):
     """
     Uploads a local file to a remote server.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
     :param local_file: Union[str, bytes]: The local file to upload, either as a path or as bytes.
-    :param remote_path: str: The directory on the remote server to which to upload the file.
+    :param remote_directory: str: The directory on the remote server to which to upload the file.
     :param remote_file: Optional[str]: The name to use for the remote file. If not provided, the name of the local file
            will be used.
     :param overwrite_remote_file: bool: Whether to overwrite the remote file if it exists. If False, a counter will be
            appended to the base name of the file to create a unique filename. Default is True.
-    :raises IOError: If local_file is a path and it does not exist, is not a file, or cannot be read, or if the remote
+    :raises IOError: If local_file is a path, and it does not exist, is not a file, or cannot be read, or if the remote
             directory does not exist or is not writable.
     """
     # Create the remote directory if it does not exist
-    create_directory(client, remote_path)
+    create_directory(client, remote_directory)
 
     # If remote_file is not provided, use the name of the local file
     if not remote_file:
         remote_file = os.path.basename(local_file)
 
     # If overwrite_remote_file is False, get a unique filename
     if not overwrite_remote_file:
-        remote_file = get_next_available_filename(client, remote_path, remote_file)
+        remote_file = get_next_available_filename(client, remote_directory, remote_file)
 
     # Upload the file
     # If local_file is a path, use the put method
     # If local_file is bytes, use the putfo method
-    full_path = f"{remote_path}/{remote_file}"
+    full_path = f"{remote_directory}/{remote_file}"
     if type(local_file) is str:
         client.put(local_file, full_path)
     else:
         with BytesIO(local_file) as local_file_obj:
             client.putfo(local_file_obj, full_path)
 
 
-def put_files(client: paramiko.SFTPClient, local_path: str, remote_path: str):
+def put_files(client: paramiko.SFTPClient, local_directory: str, remote_directory: str,
+              match_regex: Optional[str] = None, overwrite_remote_file: Optional[bool] = True):
     """
     Uploads all files from a local directory to a remote server.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
-    :param local_path: str: The local directory containing the files to upload.
-    :param remote_path: str: The directory on the remote server to which to upload the files.
+    :param local_directory: str: The local directory containing the files to upload.
+    :param remote_directory: str: The directory on the remote server to which to upload the files.
+    :param match_regex: Optional[str]: A regular expression to match against file names.
+        Only files with names that match this expression will be retrieved.
+        Default is None, which means all files will be retrieved.
+    :param overwrite_remote_file: bool: Whether to overwrite the remote file if it exists. If False, a counter will be
+        appended to the base name of the file to create a unique filename. Default is True.
     :raises IOError: If the local directory does not exist or is not a directory, or if a local file cannot be read,
-            or if the remote directory does not exist or is not writable.
+        or if the remote directory does not exist or is not writable.
     """
     # Check if the local directory exists and is a directory
-    if not os.path.isdir(local_path):
-        raise IOError(f"The local directory {local_path} does not exist or is not a directory.")
+    if not os.path.isdir(local_directory):
+        raise IOError(f"The local directory {local_directory} does not exist or is not a directory.")
 
     # Iterate over the files in the local directory
-    for root, dirs, files in os.walk(local_path):
+    for root, dirs, files in os.walk(local_directory):
         for file in files:
-            # Get the full path of the file
-            local_file = os.path.join(root, file)
-            # Check if the file can be read
-            if not os.access(local_file, os.R_OK):
-                raise IOError(f"The local file {local_file} cannot be read.")
-
-            # Upload the file
-            put_file(client, local_file, remote_path, file)
+            if match_regex is None or re.match(match_regex, file):
+                # Get the full path of the file
+                local_file = os.path.join(root, file)
+                # Check if the file can be read
+                if not os.access(local_file, os.R_OK):
+                    raise IOError(f"The local file {local_file} cannot be read.")
 
+                # Upload the file
+                put_file(client, local_file, remote_directory, file, overwrite_remote_file)
 
-def get_file(client: paramiko.SFTPClient, remote_file: str, local_path: Optional[str] = None,
-             local_file: Optional[str] = None,
-             as_bytes: bool = False, overwrite_local_file: bool = True) -> bytes:
+
+def put_files_from_list(client: paramiko.SFTPClient, local_file_list: list[str], remote_directory: str,
+                        overwrite_remote_file: Optional[bool] = True):
+    """
+    Retrieves each file from a list of remote files and saves them to a local directory.
+
+    :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
+    :param local_file_list: List[str]: A list of the full paths to the local files.
+    :param remote_directory: str: The remote directory to which to save the files.
+    :param overwrite_remote_file: bool: Whether to overwrite the remote file if it exists. If False, a counter will be
+        appended to the base name of the file to create a unique filename. Default is True.
+    """
+    # Iterate over the remote files
+    for local_file in local_file_list:
+        # Construct the full local path for the file
+        full_path = os.path.join(remote_directory, os.path.basename(local_file))
+
+        # Retrieve the file
+        put_file(client, local_file, full_path, overwrite_remote_file=overwrite_remote_file)
+
+
+def get_file_as_bytes(client: paramiko.SFTPClient, remote_file: str) -> bytes:
+    # Check if the remote file exists and is a file
+    if not file_exists(client, remote_file):
+        raise IOError(f"The remote file does not exist or is not a file: {remote_file}")
+
+    with BytesIO() as remote_file_obj:
+        client.getfo(remote_file, remote_file_obj)
+        remote_file_obj.seek(0)
+
+    return remote_file_obj.read()
+
+
+def get_file(client: paramiko.SFTPClient, remote_file: str, local_directory: str,
+             local_file: Optional[str] = None, overwrite_local_file: Optional[bool] = True):
     """
     Retrieves a file from a remote server. The file can be returned as bytes or saved to a local directory.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
     :param remote_file: str: The full path to the remote file.
-    :param local_path: Optional[str]: The local directory to which to save the file. Required if as_bytes is False.
+    :param local_directory: The local directory to which to save the file.
     :param local_file: Optional[str]: The name to use for the local file. If not provided, the name of the remote file
            will be used.
-    :param as_bytes: bool: Whether to return the file as bytes. If True, the function will return the file as bytes.
-           If False, the function will save the file to the local_path and return None. Default is False.
-    :param overwrite_local_file: bool: Whether to overwrite the local file if it exists. If False, a counter will be
+    :param overwrite_local_file: Optional[bool]: Whether to overwrite the local file if it exists. If False, a counter will be
            appended to the base name of the file to create a unique filename. Default is True.
-    :return: Optional[bytes]: If as_bytes is True, the file contents as bytes. Otherwise, None.
     :raises IOError: If the remote file does not exist, or if as_bytes is False and local_path is not provided or is
             not a writable directory.
     """
 
-    # Check if the remote file exists and is a file
-    if not file_exists(client, remote_file):
-        raise IOError(f"The remote file does not exist or is not a file: {remote_file}")
-
-    # If as_bytes is True, get the file as bytes and return it
-    if as_bytes:
-        with BytesIO() as remote_file_obj:
-            client.getfo(remote_file, remote_file_obj)
-            remote_file_obj.seek(0)
-            return remote_file_obj.read()
-
-    # If as_bytes is False, local_path must be provided, and it must be a writable directory
-    if not local_path or not os.path.isdir(local_path) or not os.access(local_path, os.W_OK):
-        raise IOError("If as_bytes is False, local_path must be provided and it must be a writable directory.")
+    if not util_file.file_path_is_valid(local_directory):
+        raise IOError("local_path must be provided and it must be a writable directory.")
 
     # If local_file is provided, use it as the name for the local file
     # Otherwise, use the name of the remote file
-    full_path = os.path.join(local_path, local_file if local_file else os.path.basename(remote_file))
+    full_path = os.path.join(local_directory, local_file if local_file else os.path.basename(remote_file))
 
-    # If we're asked NOT to overwrite, get next available file name
+    # If we're asked NOT to overwrite, get the next available file name
     if not overwrite_local_file:
         full_path = util_file.get_next_available_filename(full_path)
 
     client.get(remote_file, full_path)
 
 
-def get_files(client: paramiko.SFTPClient, remote_path: str, local_path: str, match_exp: Optional[str] = None):
+def get_files(client: paramiko.SFTPClient, remote_directory: str, local_directory: str,
+              match_regex: Optional[str] = None, overwrite_local_file: Optional[bool] = True):
     """
     Retrieves files from a remote directory to a local directory. If a match_exp is provided, only files
     whose names match the regular expression will be retrieved.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
-    :param remote_path: str: The directory from which to retrieve the files.
-    :param local_path: str: The directory to which to save the retrieved files.
-    :param match_exp: Optional[str]: A regular expression to match against file names.
+    :param remote_directory: str: The directory from which to retrieve the files.
+    :param local_directory: str: The directory to which to save the retrieved files.
+    :param match_regex: Optional[str]: A regular expression to match against file names.
                       Only files with names that match this expression will be retrieved.
                       Default is None, which means all files will be retrieved.
     """
     # Check if the remote directory exists and is readable
     try:
-        if not directory_exists(client, remote_path):
-            raise IOError(f"The remote directory {remote_path} does not exist or is not readable.")
+        if not directory_exists(client, remote_directory):
+            raise IOError(f"The remote directory {remote_directory} does not exist or is not readable.")
 
         # Iterate over the files in the remote directory
-        for remote_file in client.listdir(remote_path):
-            full_path = f"{remote_path}/{remote_file}"
-            if is_file(client, full_path) and (match_exp is None or re.match(match_exp, remote_file)):
-                get_file(client, full_path, local_path)
+        for remote_file in client.listdir(remote_directory):
+            full_remote_file = f"{remote_directory}/{remote_file}"
+            if is_file(client, full_remote_file) and (match_regex is None or re.match(match_regex, remote_file)):
+                get_file(client, full_remote_file, local_directory, overwrite_local_file=overwrite_local_file)
 
     except Exception as e:
         print(f"An error occurred while retrieving files: {str(e)}")
 
 
-def get_files_from_list(client: paramiko.SFTPClient, remote_file_list: list[str], local_path: str):
+def get_files_from_list(client: paramiko.SFTPClient, remote_file_list: list[str], local_directory: str,
+                        overwrite_local_file: Optional[bool] = True):
     """
     Retrieves each file from a list of remote files and saves them to a local directory.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
     :param remote_file_list: List[str]: A list of the full paths to the remote files.
-    :param local_path: str: The local directory to which to save the files.
-    :raises IOError: If a remote file does not exist, is not a file, or cannot be read, or if the local directory does not exist or is not writable.
+    :param local_directory: str: The local directory to which to save the files.
+    :param overwrite_local_file: Optional[bool]: Whether to overwrite the local file if it exists. If False, a counter will be
+        appended to the base name of the file to create a unique filename. Default is True.
     """
     # Iterate over the remote files
     for remote_file in remote_file_list:
         # Construct the full local path for the file
-        full_path = os.path.join(local_path, os.path.basename(remote_file))
+        full_path = os.path.join(local_directory, os.path.basename(remote_file))
 
         # Retrieve the file
-        get_file(client, remote_file, full_path)
+        get_file(client, remote_file, full_path, overwrite_local_file=overwrite_local_file)
 
 
-def get_file_list(client: paramiko.SFTPClient, remote_path: str, file_match_exp: Optional[str] = None,
-                  dir_match_exp: Optional[str] = None,
+def get_file_list(client: paramiko.SFTPClient, remote_directory: str, file_match_regex: Optional[str] = None,
+                  directory_match_regex: Optional[str] = None,
                   recursive: bool = False,
-                  max_depth: Optional[int] = None) -> list:
+                  recursion_depth: Optional[int] = None) -> list:
     """
     Returns a list of file paths based on a remote directory. Supports recursive search, regex filtering,
     and max_depth traversal.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
-    :param remote_path: str: The directory in which to start the search.
-    :param file_match_exp: Optional[str]: A regular expression to match against file names. Only files with names that
+    :param remote_directory: str: The directory in which to start the search.
+    :param file_match_regex: Optional[str]: A regular expression to match against file names. Only files with names that
            match this expression will be included in the result. Default is None, which means all files will be
            included.
-    :param dir_match_exp: Optional[str]: A regular expression to match against directory names. Only directories with
+    :param directory_match_regex: Optional[str]: A regular expression to match against directory names. Only directories with
            names that match this expression will be traversed. Default is None, which means all directories will be
            traversed.
     :param recursive: bool: Whether to search directories recursively. Default is False.
-    :param max_depth: Optional[int]: The maximum depth to traverse. Default is None, which means there is no limit to
+    :param recursion_depth: Optional[int]: The maximum depth to traverse. Default is None, which means there is no limit to
            the depth.
     :return: list: A list of the full paths of all files that match the specified criteria.
     """
     result = []
 
-    def _traverse_directory(current_path, current_depth):
+    def _traverse_directory(current_directory, current_depth):
         nonlocal result
-        if max_depth is not None and current_depth > max_depth:
+        if recursion_depth is not None and current_depth > recursion_depth:
             return
 
-        for item in client.listdir(current_path):
-            full_path = f"{current_path}/{item}"
+        for item in client.listdir(current_directory):
+            full_path = f"{current_directory}/{item}"
 
             # if this is a file, and it matches the regex (if supplied_), add to the list
-            if is_file(client, full_path) and (file_match_exp is None or re.match(file_match_exp, item)):
+            if is_file(client, full_path) and (file_match_regex is None or re.match(file_match_regex, item)):
                 result.append(full_path)
             elif is_directory(client, full_path) and recursive and (
-                    dir_match_exp is None or re.match(dir_match_exp, item)):
+                    directory_match_regex is None or re.match(directory_match_regex, item)):
                 _traverse_directory(full_path, current_depth + 1)
 
-    _traverse_directory(remote_path, 0)
+    _traverse_directory(remote_directory, 0)
     return result
 
 
-def get_next_available_filename(client: paramiko.SFTPClient, remote_path: str, remote_file: str) -> str:
+def get_next_available_filename(client: paramiko.SFTPClient, remote_directory: str, remote_file: str) -> str:
     """
     Generates a unique filename in the specified directory by appending a counter to the base name of the file.
 
     :param client: paramiko.SFTPClient: The SFTP client used to interact with the remote server.
-    :param remote_path: str: The directory in which to check for file existence.
+    :param remote_directory: str: The directory in which to check for file existence.
     :param remote_file: str: The original filename.
     :return: str: A filename which does not exist in the specified directory. If the original filename does not exist,
                   it is returned as is. If it does exist, a counter is appended to the base name of the file.
      """
     base, ext = os.path.splitext(remote_file)
 
     counter = 1
     while True:
         file = f"{base}_{counter}{ext}" if counter > 1 else remote_file
-        full_path = os.path.join(remote_path, file)
+        # full_path = os.path.join(remote_path, file)
+        full_path = f'{remote_directory}/{file}'
         if not file_exists(client, full_path):
             break
         counter += 1
 
     return file
 
 
-def is_directory(client: paramiko.SFTPClient, remote_path: str) -> bool:
+def is_directory(client: paramiko.SFTPClient, remote_directory: str) -> bool:
     """
     Checks if the specified remote path corresponds to a directory.
 
     :param client: The SFTP client used to interact with the remote server.
     :type client: paramiko.SFTPClient
-    :param remote_path: The full path to the remote directory.
-    :type remote_path: str
+    :param remote_directory: The full path to the remote directory.
+    :type remote_directory: str
     :return: True if the remote path corresponds to a directory, False otherwise.
     :rtype: bool
     """
     try:
-        item = client.lstat(remote_path)
+        item = client.lstat(remote_directory)
         return stat.S_ISDIR(item.st_mode)
     except IOError:
         return False
 
 
-def directory_exists(client: paramiko.SFTPClient, remote_path: str) -> bool:
+def directory_exists(client: paramiko.SFTPClient, remote_directory: str) -> bool:
     """
     Checks if the specified remote directory exists.
 
     :param client: The SFTP client used to interact with the remote server.
     :type client: paramiko.SFTPClient
-    :param remote_path: The full path to the remote directory.
-    :type remote_path: str
+    :param remote_directory: The full path to the remote directory.
+    :type remote_directory: str
     :return: True if the remote directory exists, False otherwise.
     :rtype: bool
     """
     try:
-        return is_directory(client, remote_path)
+        return is_directory(client, remote_directory)
     except IOError:
         return False
 
 
 def file_exists(client: paramiko.SFTPClient, remote_file: str) -> bool:
     """
     Checks if the specified remote file exists.
```

### Comparing `pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sharepoint.py` & `pyrc-python-utils-0.0.4/src/pyrc_python_utils/util_sharepoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# TODO: Add Unit Tests
 # A SharePoint convenience wrapper around python-o365 library - https://github.com/O365/python-o365
 # Source reference
 #   https://github.com/O365/python-o365/blob/master/O365/sharepoint.py
 # See examples/sharepoint folder for usage scenarios
 
 import os
 from multiprocessing import AuthenticationError
```

### Comparing `pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/SOURCES.txt` & `pyrc-python-utils-0.0.4/src/pyrc_python_utils.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
+src/__init__.py
 src/pyrc_python_utils/__init__.py
 src/pyrc_python_utils/util_datetime.py
 src/pyrc_python_utils/util_exchange.py
 src/pyrc_python_utils/util_file.py
 src/pyrc_python_utils/util_ms_teams.py
+src/pyrc_python_utils/util_s3.py
 src/pyrc_python_utils/util_sftp.py
 src/pyrc_python_utils/util_sharepoint.py
+src/pyrc_python_utils/util_string.py
 src/pyrc_python_utils.egg-info/PKG-INFO
 src/pyrc_python_utils.egg-info/SOURCES.txt
 src/pyrc_python_utils.egg-info/dependency_links.txt
 src/pyrc_python_utils.egg-info/requires.txt
-src/pyrc_python_utils.egg-info/top_level.txt
+src/pyrc_python_utils.egg-info/top_level.txt
+tests/test_util_s3.py
```

