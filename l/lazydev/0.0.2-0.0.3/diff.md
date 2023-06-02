# Comparing `tmp/lazydev-0.0.2.tar.gz` & `tmp/lazydev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.2.tar", last modified: Fri Jun  2 18:24:34 2023, max compression
+gzip compressed data, was "lazydev-0.0.3.tar", last modified: Fri Jun  2 18:31:22 2023, max compression
```

## Comparing `lazydev-0.0.2.tar` & `lazydev-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:24:34.944016 lazydev-0.0.2/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.2/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4231 2023-06-02 18:24:34.943874 lazydev-0.0.2/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3561 2023-06-02 13:22:20.000000 lazydev-0.0.2/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:24:34.941717 lazydev-0.0.2/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.2/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.2/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:24:34.943566 lazydev-0.0.2/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.2/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     5556 2023-06-02 12:54:47.000000 lazydev-0.0.2/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     4428 2023-06-02 16:54:25.000000 lazydev-0.0.2/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.2/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:24:34.942670 lazydev-0.0.2/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4231 2023-06-02 18:24:34.000000 lazydev-0.0.2/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 18:24:34.000000 lazydev-0.0.2/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 18:24:34.000000 lazydev-0.0.2/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 18:24:34.000000 lazydev-0.0.2/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 18:24:34.000000 lazydev-0.0.2/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 18:24:34.000000 lazydev-0.0.2/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 18:24:34.944051 lazydev-0.0.2/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 18:20:13.000000 lazydev-0.0.2/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:22.002395 lazydev-0.0.3/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.3/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 18:31:22.002204 lazydev-0.0.3/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3464 2023-06-02 18:29:53.000000 lazydev-0.0.3/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:21.999833 lazydev-0.0.3/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.3/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.3/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:22.001863 lazydev-0.0.3/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.3/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     5556 2023-06-02 12:54:47.000000 lazydev-0.0.3/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4428 2023-06-02 16:54:25.000000 lazydev-0.0.3/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.3/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:22.000930 lazydev-0.0.3/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 18:31:22.002444 lazydev-0.0.3/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 18:30:32.000000 lazydev-0.0.3/setup.py
```

### Comparing `lazydev-0.0.2/LICENSE` & `lazydev-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.2/PKG-INFO` & `lazydev-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.2
+Version: 0.0.3
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,39 +29,37 @@
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
 ```
-git clone https://github.com/thecodacus/lazy-dev.git
-cd lazy-dev
-pip install -r requirements.txt
+pip install lazydev
 ```
 
 LazyDev requires Python 3.6 or above.
 
 ## Usage
 
 Using LazyDev is as simple as running a single command. Once installed, you can initiate the project generation process by executing the following command:
 
 ```
-python -m lazydev.develop -r <what you want to do>
+lazydev develop -r <what you want to do>
 ```
 
 Replace `<what you want to do>` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
 
 After answering the questions, LazyDev will proceed to plan the project structure, create the appropriate file tree, generate the required code files, and even run tests to verify the functionality.
 
 ## Example
 
 Let's say you want to create a Python web application for managing a book library. You can use LazyDev to automate the project setup. Here's an example command:
 
 ```
-python -m lazydev.develop -r "Book Library Web App"
+lazydev develop -r "Book Library Web App"
 ```
 
 LazyDev will ask you questions like:
 
 - What database system would you like to use?
 - What features would you like to include in your web app?
 - Are there any specific libraries or frameworks you want to use?
```

### Comparing `lazydev-0.0.2/README.md` & `lazydev-0.0.3/lazydev.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: lazydev
+Version: 0.0.3
+Summary: AI developer for lazy programmer
+Home-page: https://github.com/thecodacus/lazy-dev
+Author: Anirban Kat
+Author-email: thecodacus@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LazyDev: Automated Coding Project
 
 `Lazyness is the mother of invention`
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
@@ -11,39 +29,37 @@
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
 ```
-git clone https://github.com/thecodacus/lazy-dev.git
-cd lazy-dev
-pip install -r requirements.txt
+pip install lazydev
 ```
 
 LazyDev requires Python 3.6 or above.
 
 ## Usage
 
 Using LazyDev is as simple as running a single command. Once installed, you can initiate the project generation process by executing the following command:
 
 ```
-python -m lazydev.develop -r <what you want to do>
+lazydev develop -r <what you want to do>
 ```
 
 Replace `<what you want to do>` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
 
 After answering the questions, LazyDev will proceed to plan the project structure, create the appropriate file tree, generate the required code files, and even run tests to verify the functionality.
 
 ## Example
 
 Let's say you want to create a Python web application for managing a book library. You can use LazyDev to automate the project setup. Here's an example command:
 
 ```
-python -m lazydev.develop -r "Book Library Web App"
+lazydev develop -r "Book Library Web App"
 ```
 
 LazyDev will ask you questions like:
 
 - What database system would you like to use?
 - What features would you like to include in your web app?
 - Are there any specific libraries or frameworks you want to use?
```

### Comparing `lazydev-0.0.2/lazydev/develop.py` & `lazydev-0.0.3/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.2/lazydev/modules/developer.py` & `lazydev-0.0.3/lazydev/modules/developer.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.2/lazydev/modules/prompts.py` & `lazydev-0.0.3/lazydev/modules/prompts.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.2/lazydev/modules/utils.py` & `lazydev-0.0.3/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.2/setup.py` & `lazydev-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
```

