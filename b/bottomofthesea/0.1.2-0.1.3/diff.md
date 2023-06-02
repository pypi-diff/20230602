# Comparing `tmp/bottomofthesea-0.1.2.tar.gz` & `tmp/bottomofthesea-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bottomofthesea-0.1.2.tar", max compression
+gzip compressed data, was "bottomofthesea-0.1.3.tar", max compression
```

## Comparing `bottomofthesea-0.1.2.tar` & `bottomofthesea-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476356 bottomofthesea-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476293 bottomofthesea-0.1.2/bottomofthesea/__init__.py
--rw-r--r--   0        0        0     7891 2023-06-01 17:32:14.480642 bottomofthesea-0.1.2/bottomofthesea/bottomofthesea.py
--rw-r--r--   0        0        0     1825 2023-05-31 23:29:45.720330 bottomofthesea-0.1.2/bottomofthesea/preprocess.py
--rw-r--r--   0        0        0      608 2023-06-01 17:32:25.829987 bottomofthesea-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 bottomofthesea-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476356 bottomofthesea-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476293 bottomofthesea-0.1.3/bottomofthesea/__init__.py
+-rw-r--r--   0        0        0     8354 2023-06-02 13:55:50.784561 bottomofthesea-0.1.3/bottomofthesea/bottomofthesea.py
+-rw-r--r--   0        0        0     1825 2023-05-31 23:29:45.720330 bottomofthesea-0.1.3/bottomofthesea/preprocess.py
+-rw-r--r--   0        0        0      608 2023-06-02 13:56:17.820359 bottomofthesea-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 bottomofthesea-0.1.3/PKG-INFO
```

### Comparing `bottomofthesea-0.1.2/bottomofthesea/bottomofthesea.py` & `bottomofthesea-0.1.3/bottomofthesea/bottomofthesea.py`

 * *Files 15% similar despite different names*

```diff
@@ -142,20 +142,26 @@
         if sys.platform == "win32":
             os.startfile(filepath)
         else:
             opener = "open" if sys.platform == "darwin" else "xdg-open"
             subprocess.call([opener, filepath])
 
     def get_input():
-        video = input("which video do you want to decode?(e.g. 02ss.mov): ")
+        video = input("\nwhich video do you want to decode?(e.g. 02ss.mov): ")
         seconds = input(
-            "Choose a second in the video to see different contents (e.g. 11 seconds into the video = 11; 1 minute 30 seconds = 90):"
+            "Choose a second in the video to see different contents \n(e.g. 11 seconds into the video = 11; 1 minute 30 seconds = 90): "
         ) 
         
         return (video, seconds)
+    
+    def get_seconds():
+        seconds = input(
+            "\nChoose another second in the video to see different contents \n (e.g. 11 seconds into the video = 11; 1 minute 30 seconds = 90): "
+        )
+        return seconds 
 
     def found_video(filename):
         # Try this folder
         file_path = os.path.join(os.getcwd(), filename)
         if os.path.exists(file_path):
             return True, file_path
         else:
@@ -167,15 +173,23 @@
             else:
                 # Try the '/Downloads' folder
                 downloads_folder = os.path.join(os.path.expanduser("~"), "Downloads")
                 file_path = os.path.join(downloads_folder, filename)
                 if os.path.exists(file_path):
                     return True, file_path
                 else:
-                    return False, "no_path"
+                    return False
+                
+    def _decode(path, seconds):
+        images = bottomofthesea.preprocess.prepareFrames(path, seconds)
+        Steganography.RESOLUTION = bottomofthesea.preprocess.get_video_size(path)
+        for i in images:
+            img = Image.fromarray(i)
+            # img.show()
+            Steganography().decode(img).show()
 
     def decode(self, image):
         """decode an image.
 
         :param image: The input image.
         :return: The unmerged/extracted image.
         """
@@ -198,35 +212,32 @@
                     )
 
         return Image.fromarray(cv2.cvtColor(np.array(new_image), cv2.COLOR_BGR2RGB))
 
 
 def main():
     print(
-        "Welcome to the land at the bottom of the sea. \nI want to show you something.\n\n"
+        "\nWelcome to the land at the bottom of the sea. \nI want to show you something.\n\n"
     )
-    parser = argparse.ArgumentParser(description="Steganography")
-    subparser = parser.add_subparsers(dest="command")
-
-    video, seconds = Steganography.get_input()
-    print(f"got {video}")
-    args = parser.parse_args()
 
-    # check video path
-    while not Steganography.found_video(video)[0]:
+    while True:
         video, seconds = Steganography.get_input()
-        print(
-            f"The file {video} was not found in the expected location. Suggestions: Check typo. Move the video to the same directory with this folder.\n "
-        )
-    if Steganography.found_video(video)[0]:
+
+        # check video path
+        while not Steganography.found_video(video)[0]:
+            video, seconds = Steganography.get_input()
+            print(
+                f"The file {video} was not found in the expected location. Suggestions: Check typo. Move the video to the same directory with this folder.\n "
+            )
+    
         path = Steganography.found_video(video)[1]
-        images = bottomofthesea.preprocess.prepareFrames(path, seconds)
-        Steganography.RESOLUTION = bottomofthesea.preprocess.get_video_size(path)
-        for i in images:
-            img = Image.fromarray(i)
-            # img.show()
-            Steganography().decode(img).show()
+        Steganography._decode(path,seconds)
         
+        choice = input("\nDo you want to decode another second in the video? (y/n): ")
+        while choice.lower() == 'y':
+            seconds = Steganography.get_seconds()
+            Steganography._decode(path,seconds)
+            choice = input("\nDo you want to decode another second in the video? (y/n): ")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bottomofthesea-0.1.2/bottomofthesea/preprocess.py` & `bottomofthesea-0.1.3/bottomofthesea/preprocess.py`

 * *Files identical despite different names*

### Comparing `bottomofthesea-0.1.2/pyproject.toml` & `bottomofthesea-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bottomofthesea"
-version = "0.1.2"
+version = "0.1.3"
 description = "Decodes hidden materials in the video from the Land At The Bottom Of The Sea project"
 authors = ["doublescoop <backslash.share@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["decode", "decoding", "steganography", "steg", "thelandatthebottomofthesea"]
```

### Comparing `bottomofthesea-0.1.2/PKG-INFO` & `bottomofthesea-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bottomofthesea
-Version: 0.1.2
+Version: 0.1.3
 Summary: Decodes hidden materials in the video from the Land At The Bottom Of The Sea project
 License: MIT
 Keywords: decode,decoding,steganography,steg,thelandatthebottomofthesea
 Author: doublescoop
 Author-email: backslash.share@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

