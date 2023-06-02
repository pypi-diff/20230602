# Comparing `tmp/SecuriPy-1.0.8.tar.gz` & `tmp/SecuriPy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.0.8.tar", last modified: Thu Jun  1 16:37:35 2023, max compression
+gzip compressed data, was "SecuriPy-1.1.0.tar", last modified: Fri Jun  2 16:43:24 2023, max compression
```

## Comparing `SecuriPy-1.0.8.tar` & `SecuriPy-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 16:37:35.182075 SecuriPy-1.0.8/
--rw-rw-rw-   0        0        0     3594 2023-06-01 16:37:35.179055 SecuriPy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 16:37:35.176100 SecuriPy-1.0.8/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3594 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5163 2023-06-01 16:36:46.000000 SecuriPy-1.0.8/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 16:37:35.182075 SecuriPy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-06-01 16:37:09.000000 SecuriPy-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 16:43:24.351083 SecuriPy-1.1.0/
+-rw-rw-rw-   0        0        0     3594 2023-06-02 16:43:24.346246 SecuriPy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 16:43:24.340091 SecuriPy-1.1.0/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7336 2023-06-02 16:02:30.000000 SecuriPy-1.1.0/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 16:43:24.351506 SecuriPy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-06-02 16:42:57.000000 SecuriPy-1.1.0/setup.py
```

### Comparing `SecuriPy-1.0.8/PKG-INFO` & `SecuriPy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.8
+Version: 1.1.0
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.8/README.md` & `SecuriPy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.0.8/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.1.0/SecuriPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.8
+Version: 1.1.0
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.8/SecuriPy.py` & `SecuriPy-1.1.0/SecuriPy.py`

 * *Files 21% similar despite different names*

```diff
@@ -81,16 +81,14 @@
                 img.save(buffer, format=((image_path.split("."))[1].upper()))
                 img_data = buffer.getvalue()
             with open("key.txt","rb") as k:
                 key = k.read()
             encrypted_data = encrypt_data(img_data, key)
             with open(output_path, 'wb') as f:
                 f.write(encrypted_data)
-            with open("key.txt","wb") as k:
-                k.write(key)
 
         # Replace 'path/to/your/image.jpg' with the actual path to your image file
 
         # Convert the image to an encrypted image
         # Replace 'path/to/your/new_image.jpg' with the desired path for the new image
         new_image_path = image_path
         encryption_key = image_to_encrypted_image(image_path, new_image_path)
@@ -137,7 +135,76 @@
             images = os.listdir()
 
             for image in images:
                 try:
                     Image.Decrypt(image)
                 except:
                     pass
+
+class File:
+    @staticmethod
+    def Key():
+        from cryptography.fernet import Fernet
+        
+        with open("key.txt","wb") as k:
+            k.write(Fernet.generate_key())
+            
+    @staticmethod
+    def Encrypt(file_path):
+        from cryptography.fernet import Fernet
+        from io import BytesIO
+
+        def encrypt_data(data, key):
+            fernet = Fernet(key)
+            encrypted_data = fernet.encrypt(data)
+            return encrypted_data
+
+        def file_to_encrypted_file(file_path,output_path):        
+            with open(file_path, "rb") as file:
+                file_data = file.read()
+            with open("key.txt","rb") as k:
+                    key = k.read()
+            encrypted_data = encrypt_data(file_data, key)
+            with open(output_path, 'wb') as f:
+                f.write(encrypted_data)
+                
+        new_file_path = file_path
+        encryption_key = file_to_encrypted_file(file_path, new_file_path)
+
+    @staticmethod
+    def Decrypt(encrypted_file_path):
+        from cryptography.fernet import Fernet
+
+        def decrypt_data(encrypted_data, key):
+            fernet = Fernet(key)
+            decrypted_data = fernet.decrypt(encrypted_data)
+            return decrypted_data
+
+        # Decrypt the encrypted image
+        with open("key.txt","rb") as k:
+            encryption_key = k.read()
+        with open(encrypted_file_path, 'rb') as f:
+            encrypted_data = f.read()
+        decrypted_data = decrypt_data(encrypted_data, encryption_key)
+
+        # Save the decrypted image as a new image
+        # Replace 'path/to/your/decrypted_image.jpg' with the desired path for the decrypted image
+        decrypted_file_path = encrypted_file_path
+        with open(decrypted_file_path, 'wb') as f:
+            f.write(decrypted_data)
+
+    @staticmethod
+    def EncryptAll(path):
+        import os
+        files = os.listdir(path)
+
+        for file in files:
+                File.Encrypt(file)
+            
+    @staticmethod
+    def DecryptAll():
+            import os
+            files = os.listdir(path)
+
+            for file in files:
+                    File.Decrypt(file)
+
```

### Comparing `SecuriPy-1.0.8/setup.py` & `SecuriPy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.8",
+    version="1.1.0",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

