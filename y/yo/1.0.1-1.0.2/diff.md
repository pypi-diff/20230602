# Comparing `tmp/yo-1.0.1.tar.gz` & `tmp/yo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yo-1.0.1.tar", last modified: Tue May  9 18:33:19 2023, max compression
+gzip compressed data, was "yo-1.0.2.tar", last modified: Fri Jun  2 18:55:31 2023, max compression
```

## Comparing `yo-1.0.1.tar` & `yo-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.289710 yo-1.0.1/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.1/LICENSE.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-05-09 18:33:19.289710 yo-1.0.1/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.1/README.md
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.1/THIRD_PARTY_LICENSES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-05-09 18:33:19.289710 yo-1.0.1/setup.cfg
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-05-09 18:31:11.000000 yo-1.0.1/setup.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/tests/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.1/tests/test_api.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.1/tests/test_cmds.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/yo/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.1/yo/__init__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.1/yo/__main__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67592 2023-03-23 20:42:24.000000 yo-1.0.1/yo/api.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/yo/data/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.1/yo/data/sample.yo.ini
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.289710 yo-1.0.1/yo/data/yo-tasks/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/drgn
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/ocid
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/test-deps
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.1/yo/data/yo-tasks/test-existing-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/test-run-many
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/test-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.1/yo/data/yo_tasklib.sh
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   107744 2023-05-09 18:31:11.000000 yo-1.0.1/yo/main.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.1/yo/oci.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.1/yo/util.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/yo.egg-info/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/SOURCES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/dependency_links.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/entry_points.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/requires.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/top_level.txt
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.2/LICENSE.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 18:55:31.402872 yo-1.0.2/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.2/README.md
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.2/THIRD_PARTY_LICENSES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-06-02 18:55:31.402872 yo-1.0.2/setup.cfg
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-06-02 18:54:59.000000 yo-1.0.2/setup.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/tests/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.2/tests/test_api.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.2/tests/test_cmds.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.2/yo/__init__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.2/yo/__main__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67881 2023-06-02 18:54:59.000000 yo-1.0.2/yo/api.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo/data/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.2/yo/data/sample.yo.ini
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo/data/yo-tasks/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/drgn
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/ocid
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/test-deps
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.2/yo/data/yo-tasks/test-existing-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/test-run-many
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/test-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.2/yo/data/yo_tasklib.sh
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   108412 2023-06-02 18:54:59.000000 yo-1.0.2/yo/main.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.2/yo/oci.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.2/yo/util.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo.egg-info/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/entry_points.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/requires.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/top_level.txt
```

### Comparing `yo-1.0.1/LICENSE.txt` & `yo-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/PKG-INFO` & `yo-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.1
+Version: 1.0.2
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yo-1.0.1/README.md` & `yo-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/THIRD_PARTY_LICENSES.txt` & `yo-1.0.2/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/setup.py` & `yo-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md").read()
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 
 setup(
     name="yo",
     version=VERSION,
     description="A fast and simple CLI client for managing OCI instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `yo-1.0.1/tests/test_api.py` & `yo-1.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/tests/test_cmds.py` & `yo-1.0.2/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/__main__.py` & `yo-1.0.2/yo/__main__.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/api.py` & `yo-1.0.2/yo/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1205,19 +1205,24 @@
             vnic_gen = self.oci.list_call_get_all_results_generator(
                 self.compute.list_vnic_attachments,
                 "record",
                 cid,
                 instance_id=inst.id,
             )
             vnic_attachments = list(vnic_gen)
-            vnic_attachment = one(
-                vnic_attachments,
-                "There are no attached vnics for this instance (expected one)",
-                "There are multiple attached vnics for this instance (expected one)",
-            )
+            if not vnic_attachments:
+                raise YoExc("There are no attached VNICs for this instance")
+            elif len(vnic_attachments) > 1:
+                self.con.print(
+                    "[red]warning:[/red] your instance has multiple attached "
+                    "VNICs, which may have multiple IPs. Yo is choosing to use "
+                    "first one. If you encounter issues, please mention this "
+                    "when reporting it."
+                )
+            vnic_attachment = vnic_attachments[0]
             vnic = self.vnet.get_vnic(vnic_attachment.vnic_id).data
             yovnic = YoVnic.from_oci(vnic, vnic_attachment)
             self._vnics.insert(yovnic)
             self.save_cache()
         ip = yovnic.public_ip or yovnic.private_ip
         if not quiet:
             self.con.print(f"Found instance ip [blue]{ip}")
```

### Comparing `yo-1.0.1/yo/data/sample.yo.ini` & `yo-1.0.2/yo/data/sample.yo.ini`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/data/yo-tasks/drgn` & `yo-1.0.2/yo/data/yo-tasks/drgn`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/data/yo-tasks/ocid` & `yo-1.0.2/yo/data/yo-tasks/ocid`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/data/yo-tasks/test-deps` & `yo-1.0.2/yo/data/yo-tasks/test-deps`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/data/yo-tasks/test-run-many` & `yo-1.0.2/yo/data/yo-tasks/test-run-many`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/data/yo-tasks/test-task` & `yo-1.0.2/yo/data/yo-tasks/test-task`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/data/yo_tasklib.sh` & `yo-1.0.2/yo/data/yo_tasklib.sh`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/main.py` & `yo-1.0.2/yo/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,27 @@
     # The following two options are mostly useful for long-running serial
     # console connections. But they certainly don't harm things when you're
     # keeping SSH open for a while.
     "-oServerAliveInterval=60",
     "-oTCPKeepAlive=yes",
 ]
 SSH_CONSOLE_OPTIONS = [
-    "-oHostKeyAlgorithms +ssh-rsa",
-    "-oPubkeyAcceptedAlgorithms +ssh-rsa",
+    "-oHostKeyAlgorithms=+ssh-rsa",
+    # From the OpenSSH 8.5 Changelog:
+    #
+    #   ssh(1), sshd(8): rename the PubkeyAcceptedKeyTypes keyword to
+    #   PubkeyAcceptedAlgorithms. The previous name incorrectly suggested
+    #   that it control allowed key algorithms, when this option actually
+    #   specifies the signature algorithms that are accepted. The previous
+    #   name remains available as an alias. bz#3253
+    #
+    # Thankfully, the alias seems to be available for a while. Unfortunately,
+    # it means we're using an "undocumented" option in order to retain maximal
+    # compatibility with OpenSSH versions.
+    "-oPubkeyAcceptedKeyTypes=+ssh-rsa",
 ]
 SSH_MINIMUM_TIME = 4
 
 # TODO: update with an external link
 REPOSITORY_URL = "https://github.com/oracle/yo"
 DOCUMENTATION_URL = "https://oracle.github.io/yo/"
 INITIAL_CONFIG_LINK = REPOSITORY_URL
@@ -1297,14 +1308,17 @@
         subprocess.run(rsync_args + replaced)
 
 
 class ConsoleCmd(SingleInstanceCommand):
     name = "console"
     description = "ssh into an instance serial console"
 
+    states_allowlist = ()
+    states_denylist = ("STOPPED", "TERMINATED")
+
     def add_args(self, parser: argparse.ArgumentParser) -> None:
         super().add_args(parser)
         parser.add_argument(
             "--refresh",
             action="store_true",
             help="refresh the local cache of serial consoles for this instance",
         )
```

### Comparing `yo-1.0.1/yo/oci.py` & `yo-1.0.2/yo/oci.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo/util.py` & `yo-1.0.2/yo/util.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.1/yo.egg-info/PKG-INFO` & `yo-1.0.2/yo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.1
+Version: 1.0.2
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yo-1.0.1/yo.egg-info/SOURCES.txt` & `yo-1.0.2/yo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

