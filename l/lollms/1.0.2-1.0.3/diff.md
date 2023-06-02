# Comparing `tmp/lollms-1.0.2.tar.gz` & `tmp/lollms-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-1.0.2.tar", last modified: Fri Jun  2 14:31:24 2023, max compression
+gzip compressed data, was "lollms-1.0.3.tar", last modified: Fri Jun  2 14:53:07 2023, max compression
```

## Comparing `lollms-1.0.2.tar` & `lollms-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 14:31:24.449156 lollms-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-06-02 10:47:30.000000 lollms-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3922 2023-06-02 14:31:24.447158 lollms-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3406 2023-06-02 14:30:56.000000 lollms-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 14:31:24.422154 lollms-1.0.2/lollms/
--rw-rw-rw-   0        0        0    32012 2023-06-02 14:30:56.000000 lollms-1.0.2/lollms/__init__.py
--rw-rw-rw-   0        0        0     6608 2023-06-01 08:52:43.000000 lollms-1.0.2/lollms/binding.py
--rw-rw-rw-   0        0        0     9348 2023-06-02 14:30:56.000000 lollms-1.0.2/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7558 2023-06-02 11:00:49.000000 lollms-1.0.2/lollms/lllm_server.py
-drwxrwxrwx   0        0        0        0 2023-06-02 14:31:24.443158 lollms-1.0.2/lollms.egg-info/
--rw-rw-rw-   0        0        0     3922 2023-06-02 14:31:24.000000 lollms-1.0.2/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-02 14:31:24.000000 lollms-1.0.2/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 14:31:24.000000 lollms-1.0.2/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-02 14:31:24.000000 lollms-1.0.2/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      143 2023-06-02 14:31:24.000000 lollms-1.0.2/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 14:31:24.000000 lollms-1.0.2/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 14:31:24.450159 lollms-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-02 14:30:56.000000 lollms-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:07.797795 lollms-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-02 10:47:30.000000 lollms-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6748 2023-06-02 14:53:07.796796 lollms-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6232 2023-06-02 14:52:39.000000 lollms-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:07.778795 lollms-1.0.3/lollms/
+-rw-rw-rw-   0        0        0    32012 2023-06-02 14:30:56.000000 lollms-1.0.3/lollms/__init__.py
+-rw-rw-rw-   0        0        0     6608 2023-06-01 08:52:43.000000 lollms-1.0.3/lollms/binding.py
+-rw-rw-rw-   0        0        0     9348 2023-06-02 14:30:56.000000 lollms-1.0.3/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7558 2023-06-02 11:00:49.000000 lollms-1.0.3/lollms/server.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:07.793797 lollms-1.0.3/lollms.egg-info/
+-rw-rw-rw-   0        0        0     6748 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 14:53:07.798797 lollms-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2023-06-02 14:39:07.000000 lollms-1.0.3/setup.py
```

### Comparing `lollms-1.0.2/LICENSE` & `lollms-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-1.0.2/lollms/__init__.py` & `lollms-1.0.3/lollms/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-1.0.2/lollms/binding.py` & `lollms-1.0.3/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-1.0.2/lollms/langchain_integration.py` & `lollms-1.0.3/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-1.0.2/lollms/lllm_server.py` & `lollms-1.0.3/lollms/server.py`

 * *Files identical despite different names*

### Comparing `lollms-1.0.2/setup.py` & `lollms-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="lollms",
-    version="1.0.2",
+    version="1.0.3",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'lollms-server = lollms.lollms_server:main',
+            'lollms-server = lollms.server:main',
         ],
     },
     extras_require={"dev": requirements_dev},
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

