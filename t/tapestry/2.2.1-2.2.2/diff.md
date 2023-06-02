# Comparing `tmp/tapestry-2.2.1-py3-none-any.whl.zip` & `tmp/tapestry-2.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 45013 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       71 b- defN 21-Feb-06 00:31 tapestry/__init__.py
--rw-rw-r--  2.0 unx      423 b- defN 21-Feb-06 00:31 tapestry/__main__.py
--rw-rw-r--  2.0 unx    21182 b- defN 21-Feb-06 00:31 tapestry/classes.py
--rw-rw-r--  2.0 unx    72787 b- defN 22-Nov-11 11:17 tapestry/functions.py
--rw-rw-r--  2.0 unx    35141 b- defN 22-Nov-11 17:00 tapestry-2.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    13564 b- defN 22-Nov-11 17:00 tapestry-2.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Nov-11 17:00 tapestry-2.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Nov-11 17:00 tapestry-2.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      699 b- defN 22-Nov-11 17:00 tapestry-2.2.1.dist-info/RECORD
-9 files, 143968 bytes uncompressed, 43819 bytes compressed:  69.6%
+Zip file size: 45443 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       76 b- defN 23-Jun-02 17:50 tapestry/__init__.py
+-rw-rw-r--  2.0 unx      423 b- defN 23-Jun-02 17:50 tapestry/__main__.py
+-rw-rw-r--  2.0 unx    21241 b- defN 23-Jun-02 17:50 tapestry/classes.py
+-rw-rw-r--  2.0 unx    74637 b- defN 23-Jun-02 17:50 tapestry/functions.py
+-rw-rw-r--  2.0 unx    35141 b- defN 23-Jun-02 18:02 tapestry-2.2.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    13612 b- defN 23-Jun-02 18:02 tapestry-2.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 18:02 tapestry-2.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-02 18:02 tapestry-2.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      699 b- defN 23-Jun-02 18:02 tapestry-2.2.2.dist-info/RECORD
+9 files, 145930 bytes uncompressed, 44249 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tapestry/classes.py
 Comment: 
 
 Filename: tapestry/functions.py
 Comment: 
 
-Filename: tapestry-2.2.1.dist-info/LICENSE
+Filename: tapestry-2.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: tapestry-2.2.1.dist-info/METADATA
+Filename: tapestry-2.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tapestry-2.2.1.dist-info/WHEEL
+Filename: tapestry-2.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tapestry-2.2.1.dist-info/top_level.txt
+Filename: tapestry-2.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tapestry-2.2.1.dist-info/RECORD
+Filename: tapestry-2.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tapestry/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "2.1.1"
+__version__ = "2.2.2_dev1"
 
 from .classes import *
 from .functions import *
```

## tapestry/classes.py

```diff
@@ -384,15 +384,15 @@
         """Accepts an arbitrary file index identifier and the corresponding
         dictionary of metadata, as from a recovery index object"""
         if file_index_object['fsize'] <= self.remaining:  # the new file will fit
             self.file_index.update({file_identifier: file_index_object})
             self.size += file_index_object['fsize']
             self.files += 1
             self.remaining = self.max_size - self.size
-            if self.remaining <= self.smallest:
+            if self.remaining < self.smallest:  # This must not include equivalence or we'll loop forever.
                 self.full = True
             return True
         else:  # This file won't fit and has to be placed somewhere else.
             return False
 
     def meta(self, sum_blocks, sum_size, sum_files, datestamp, comment_string, full_index, drop_dir):
         """Provided these arguments, populate the runMetadata portion of a RIFF,
```

## tapestry/functions.py

```diff
@@ -25,15 +25,15 @@
 from random import shuffle
 import shutil
 import sys
 import tarfile
 import textwrap
 import uuid
 
-__version__ = "2.1.1"
+__version__ = "2.2.2-dev1"
 
 # Class Definitions
 
 
 class Namespace(object):  # this just creates an object with arbitrary attributes.
     pass
 
@@ -91,15 +91,15 @@
         for category in ns.categories_inclusive:
             run_list.append(category)
     for category in run_list:
         for dir_path, sub_dirs, files in os.walk(ns.category_paths[category]):
             for file in files:
                 absolute_path = os.path.join(dir_path, file)
                 sub_path = os.path.relpath(absolute_path, ns.category_paths[category])
-                access_test_results = access_test(absolute_path)
+                access_test_results = access_test(absolute_path, test_W=False)  # Forcing false here fixes issue #34
                 if False not in access_test_results:
                     size = os.path.getsize(absolute_path)
                     try:
                         if size <= ns.block_size_raw:  # We'll be handling this file.
                             hasher = hashlib.new('sha256')
                             with open(absolute_path, "rb") as contents:
                                 chunk = contents.read(io.DEFAULT_BUFFER_SIZE)
@@ -685,21 +685,32 @@
     counter = 1  # Remember to increment this later
     smallest = ops_list[sizes[-1]]['fsize']
     working_block = tapestry.Block(
         (block_name_base+"-"+str(counter)), ns.block_size_raw, counter, smallest
     )
     packing = True
     while packing:
+        placed_items = []
         for item in sizes:
             placed = working_block.put(item, ops_list[item])
             if placed:
-                sizes.remove(item)
+                placed_items.append(item)
+        for placed_item in placed_items:  # We need to do this rather than popping them immediately
+            sizes.remove(placed_item)     # Because that would break the indexing, and you still get recursion.
+        if smallest == 0:  # Special edge case, causes infinite loops if true after the first run through the list.
+            new_smallest = ops_list[sizes[-1]]['fsize']
+            if new_smallest == 0:  # This in theory should be unreachable code but we need to account for this case.
+                print("Fatal Error: Infinite Recursion in block build algorithm.")
+                exit(7)
+            else:
+                working_block.full = True  # at this point this must necessarily be true
         if working_block.full:  # We need a new block, unpacked items.
             collection_blocks.append(working_block)
             counter += 1
+            smallest = ops_list[sizes[-1]]['fsize']  # There is a new smallest file, and we need to start over.
             working_block = tapestry.Block(
                 (block_name_base+"-"+str(counter)), ns.block_size_raw, counter, smallest
             )
         elif len(sizes) == 0:
             collection_blocks.append(working_block)
             packing = False  # The list is empty and we're therefore done.
     tarf_queue = mp.JoinableQueue()
@@ -747,15 +758,15 @@
             status_print(rounds_complete, sum_jobs, "Packing", message)
             if rounds_complete == sum_jobs:
                 done.put(None)  # Use none as a poison pill to kill the queue.
             done.task_done()
     tarf_queue.join()
     for w in workers:
         tarf_queue.put(None)
-
+    print("\n")
     return block_final_paths
 
 
 def parse_args(namespace):
     """Parse arguments and return the modified namespace object"""
     ns = namespace
     parser = argparse.ArgumentParser(description="""
@@ -821,18 +832,28 @@
         (block_name_base + "-" + str(counter)), ns.block_size_raw, counter, smallest
     )
     if not os.path.exists(ns.workDir):
         os.mkdir(ns.workDir)
 
     packing = True
     while packing:
+        placed_items = []
         for item in sizes:
             placed = working_block.put(item, ops_list[item])
             if placed:
-                sizes.remove(item)
+                placed_items.append(item)
+        for placed_item in placed_items:  # We need to do this rather than popping them immediately
+            sizes.remove(placed_item)     # Because that would break the indexing, and you still get recursion.
+        if smallest == 0:  # Special edge case, causes infinite loops if true after the first run through the list.
+            new_smallest = ops_list[sizes[-1]]['fsize']
+            if new_smallest == 0:  # This in theory should be unreachable code but we need to account for this case.
+                print("Fatal Error: Infinite Recursion in block build algorithm.")
+                exit(7)
+            else:
+                working_block.full = True  # at this point this must necessarily be true
         if working_block.full:  # We need a new block, unpacked items.
             collection_blocks.append(working_block)
             counter += 1
             working_block = tapestry.Block(
                 (block_name_base + "-" + str(counter)), ns.block_size_raw, counter, smallest
             )
         elif len(sizes) == 0:
@@ -853,15 +874,15 @@
             with tarfile.open(tarf, "a:") as tf:
                 tf.add(path, arcname=fid, recursive=False)
             status_print(current_counter, sum_files, "Packing", None)
         this_riff = block.meta(len(collection_blocks), sum_sizes, sum_files,
                                str(datetime.date.today()), ns.comment_string, ops_list, ns.drop)
         with tarfile.open(tarf, "a:") as tf:
             tf.add(this_riff, arcname="recovery-riff", recursive=False)
-
+    print("/n")
     return block_final_paths
 
 
 def parse_config(namespace):
     """mounts the configparser instance, grabs the config file, and passes its
     values into the namespace.
     """
@@ -1087,15 +1108,15 @@
     """Prints a basic status message. If not interrupted, prints it on one line"""
     length_bar = 15.0
     done_bar = int(round((done / total) * length_bar))
     done_bar_print = str("#" * int(done_bar) + "-" * int(round((length_bar - done_bar))))
     percent = int(round((done / total) * 100))
     if percent == 100:  # More Pretty Printing!
         if message == "Working...":
-            message = "Done!    \n"
+            message = "Done!     "
     text = ("\r {0}: [{1}] {2}% - {3}".format(job, done_bar_print, percent, message))
     sys.stdout.write(text)
     sys.stdout.flush()
 
 
 def unpack_blocks(namespace):
     """Provided a namespace object, this function will crawl the defined
@@ -1159,14 +1180,15 @@
             status_print(rounds_complete, sum_jobs, "Unpacking", message)
             if rounds_complete >= sum_jobs:
                 done.put(None)  # Use none as a poison pill to kill the queue.
             done.task_done()
     tasks.join()
     for w in workers:
         tasks.put(None)
+    print("/n")
     tasks.join()
 
 
 def update_secrets():
     print("You have selected --secrets, and we will now go through the possible secret values to encode them.")
     print("Secrets stored in this way are stored in your system keyring and not the tapestry system files.")
     print("Python will have access to these fields! If a secret value is not desired to be stored, press enter to skip")
@@ -1572,17 +1594,19 @@
     return list_to_fetch
 
 
 def prevalidate_blocks(namespace, list_blocks, index):
     if namespace.do_validation:
         ns = namespace
         ns.logs.log("Lines beneath this point are failed hash validation checks.")
+        print("Starting post-packaging validation of block data.")
         jobs = mp.JoinableQueue()
         for file in list_blocks:
             with tarfile.open(file, mode="r:*") as tf:
+                print("Scanning block %s for files to validate." % file)
                 list_members = tf.getnames()
                 for member in list_members:
                     if member != "recovery-riff":  # Obviously we can't validate this noise.
                         task = tapestry.TaskCheckIntegrity(file, member, index[member]['sha256'])
                         jobs.put(task)
         workers = []
         sum_jobs = int(jobs.qsize())
```

## Comparing `tapestry-2.2.1.dist-info/LICENSE` & `tapestry-2.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tapestry-2.2.1.dist-info/METADATA` & `tapestry-2.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: tapestry
-Version: 2.2.1
+Version: 2.2.2
 Summary: Tapestry Bespoke Backup Utility
 Home-page: https://www.github.com/zadammac/Tapestry
 Author: Zac Adam-MacEwen
 Author-email: zadammac@arcanalabs.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: keyring
 Requires-Dist: paramiko
 Requires-Dist: pysftp
 Requires-Dist: python-gnupg
 
 # Tapestry (Specialized Backup Tool)
 
 ## Introduction
@@ -20,21 +22,21 @@
 
 Full documentation is available as part of DOCUMENTATION.md
 
 ## Requirements
 	-Python 3.6.7 or later
 	-Python-gnupg 0.4.2
 	-GnuPG 2 or later, installed as default
-
+	
 ## Contribution and Acknowledgement
 
 Building Tapestry has been a large and time-consuming project, but it would have been even more so without the work of the developers of our dependencies - GnuPG, the Python-GnuPG module, and obvious python itself.
 
 If you would like to contribute to the development of Tapestry, feel free to submit a pull request, or perhaps buy me a coffee at [ko-fi.com/KenshoSec](https://ko-fi.com/KenshoSec), or consider backing [@ZAdamMac on Github Sponsors](https://github.com/users/ZAdamMac/sponsorship.)
-
+	
 ## Security Considerations
 Tapestry relies on Gnu Privacy Guard (GPG), a well-known FOSS implementation of the PGP protocol, in order to securely store the archives it generates, and also to provide a mechanism for verifying the individual who generated the backup. It does this using two separate keys - the Encryption Key (sometimes called the "Disaster Recovery" key, after the comment included on keys Tapestry generates) and an optional, though strongly recommended, signing key specified by the user.
 
 ### Care and Feeding of the Disaster Recovery Key
 When you run Tapestry with the `--genKey` flag the program will export a new Disaster Recovery key from GPG as two separate files: `DR.key` and `DR-pub.key`. The former contains both the private and public keys of the RSA key-pair - the latter contains only the public portion.
 
 The private key and its associated file should be kept in a secure location - preferably either on removable media accessible only by trusted administrators or possibly on the keyring of a single-user/single-machine system, protected by a pass-phrase. **The use of DR keys without pass-phrases is considered harmful and should not be implemented.** It is even recommendable that you change the pass-phrase of the DR key regularly. If you are using the DR key across several systems, it is recommended that you also generate a revocation certificate (see GPG's docs) so that it can be revoked in the event of compromise.
@@ -60,15 +62,15 @@
 Tapestry cannot see the passphrase you use to unlock your signing key. Instead, we trust the local GPG installation's existing pinentry configuration to launch the appropriate pin-entry binary to collect the passphrase and unlock the key.
 
 
 ### How to Store Keys
 I can't speak for everyone's use case and I'm also not an expert on the matter. I personally store the public key of the disaster recovery key on every device I intend to use it on. The private key lives on a USB drive along with a few tools I use for cleaning up computers, and can be imported if necessary. I also keep a paper copy of the private key.
 
 As for my signing key, I am currently using my main signing key, which lives on an OpenPGP smart key. In point of fact, Tapestry is perfectly oblivious to how you choose to store your keys - if it can't find them in your keyring it assumes they don't exist.
-
+	
 ## Installation and First Time Setup
 ### Dependencies
 If you are lacking any of the above requirements, please install them first. GPG is available on most Linux distros by default.
 
 In any event, it is likely you are missing python-gnupg. That's okay, we can get python modules using `pip` at the command line.
 
 Under Linux:
```

