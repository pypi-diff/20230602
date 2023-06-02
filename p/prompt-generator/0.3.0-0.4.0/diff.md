# Comparing `tmp/prompt-generator-0.3.0.tar.gz` & `tmp/prompt-generator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-generator-0.3.0.tar", last modified: Tue May 23 18:22:37 2023, max compression
+gzip compressed data, was "prompt-generator-0.4.0.tar", last modified: Fri Jun  2 16:10:46 2023, max compression
```

## Comparing `prompt-generator-0.3.0.tar` & `prompt-generator-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.468586 prompt-generator-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.468586 prompt-generator-0.3.0/src/directory_structure/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/directory_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/directory_structure/get_directory_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.468586 prompt-generator-0.3.0/src/docs_generator/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/docs_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/docs_generator/generate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/get_code_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/get_dir_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/load_gitignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/read_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/input_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/input_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/input_utils/input_color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/markdown_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/markdown_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/markdown_parser/parse_md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/print_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/print_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/print_utils/print_color.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/print_utils/print_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/prompt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.482992 prompt-generator-0.4.0/prompt_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/prompt_generator/docs_prompt_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/docs_prompt_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/docs_prompt_generator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/prompt_generator/get_dir_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/get_dir_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/get_dir_structure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/prompt_generator/markdown_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/markdown_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/markdown_parser/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/prompt_generator/tasks_prompt_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/tasks_prompt_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/tasks_prompt_generator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/prompt_generator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/prompt_generator/utils/print_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/prompt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-02 16:10:46.000000 prompt-generator-0.4.0/prompt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-02 16:10:46.000000 prompt-generator-0.4.0/prompt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:10:46.000000 prompt-generator-0.4.0/prompt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 16:10:46.000000 prompt-generator-0.4.0/prompt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 16:10:46.000000 prompt-generator-0.4.0/prompt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:10:46.000000 prompt-generator-0.4.0/prompt_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-02 16:10:36.000000 prompt-generator-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:10:46.486992 prompt-generator-0.4.0/setup.cfg
```

### Comparing `prompt-generator-0.3.0/LICENSE` & `prompt-generator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-generator-0.3.0/PKG-INFO` & `prompt-generator-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-generator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code.
 Author: Vincenzo Cascone
 License: MIT License
         
         Copyright (c) 2023 Vince
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,42 +44,107 @@
 
 ```bash
 pip install prompt-generator
 ```
 
 ## Features
 
-- ### Generate Docs
+- ### Generate Project Documentation
 
-  This script generates a prompt that can be used to make the AI write documentation
-  for the project. When executed, it will first ask for some info about the project, such as the name, description, root
-  path. Optionally you can provide the path to config files such as pyproject.toml for a python project or
-  package.json for a node project. The same can be done with particularly relevant files. This will allow the AI to have
-  a better understanding of the project and generate more accurate documentation.
+  This script generates a prompt that can be used to make the AI write documentation for the project.
 
-  To utilize it, use the following command in your terminal:
+  When executed without arguments it will ask for some info about the project, such as the name, description, root
+  directory, paths to config files, main files, and docs specs.
+
+  Instead of writing the info manually you can also provide the path to a JSON file that contains the prompt
+  configuration.
+  The JSON should have the following structure:
+
+  ```
+  {
+    "name": "<string> (required)",
+    "description": "<string> (required)",
+    "target_audience": "<string> (optional)",
+    "root_dir": "<string> (required)",
+    "config_files": [
+        {
+            "path": "<string> (required)",
+            "label": "<string> (optional)"
+        },
+        ...
+    ] (optional),
+    "main_files": [
+        {
+            "path": "<string> (required)",
+            "label": "<string> (optional)"
+        },
+        ...
+    ] (optional),
+    "docs_specs": "<string> (optional)"
+  }
+  ```
+
+  To utilize this script, use the following command in your terminal:
+
+  ```bash
+  pg docs_prompt [--config <path to config file>]
+  ```
+
+  Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
+  immediate use or future reference.
+
+- ### Complete Tasks
+
+  This script generates a prompt that can be used to help AI complete tasks for the project.
 
-    ```bash
-    generate_docs
-    ```
+  It will ask for the project name, description or the path to README/docs, root directory, and optionally the paths and
+  labels to the files related to the tasks. Finally, it will ask for the single task or task list.
+
+  Instead of writing the info manually you can also provide the path to a JSON file that contains the prompt
+  configuration.
+  The JSON should have the following structure:
+
+  ```
+  {
+    "project_overview": "<string> (optional)",
+    "docs_path": "<string> (optional)",
+    "relevant_files": [
+      {
+        "path": "<string> (required)",
+        "label": "<string> (optional)"
+      },
+      ...
+    ] (optional),
+    "tasks": [
+      "<string> (required)",
+      ...
+    ] (required)
+  }
+  ```
+
+  To utilize this script, use the following command in your terminal:
+
+  ```bash
+  pg tasks_prompt [--config <path to config file>]
+  ```
 
   Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
   immediate use or future reference.
 
 - ### Markdown Parser
 
   The Markdown Parser is a robust utility specifically designed to parse markdown files. It works by replacing all
   hyperlinks within a Markdown document with the actual content of the linked files. This function proves extremely
   useful if you maintain a collection of prompt files written in Markdown format, and these files contain references to
   other project documents.
 
   To utilize it, use the following command in your terminal:
 
   ```bash
-  parse_md <path to the markdown file>
+  pg parse_md <path to the markdown file>
   ```
 
   Upon successful execution, the resultant parsed content will be displayed in your terminal and copied to your
   clipboard for immediate use or future reference.
 
 - ### Directory Structure
 
@@ -88,12 +153,12 @@
   .gitignore file. This makes it an essential tool for giving the AI a better understanding of the context of your
   project. The returned JSON is minified in order to be more token efficient.
 
   To utilize it, use the following command in your terminal. You can optionally provide the .gitignore file path using
   the -gitignore flag, if not provided, the script will search for a .gitignore file in the root directory:
 
   ```bash
-  get_directory_structure <path to the directory> [-gitignore]
+  pg get_dir_structure <path to the directory> [--gitignore <path to the .gitignore file>]
   ```
 
   Upon successful execution, the resultant json will be displayed in your terminal and copied to your
   clipboard for immediate use or future reference.
```

### Comparing `prompt-generator-0.3.0/pyproject.toml` & `prompt-generator-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "prompt-generator"
-version = "0.3.0"
+version = "0.4.0"
 description = "Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Vincenzo Cascone" },
 ]
 license = { file = "LICENSE" }
@@ -19,14 +19,12 @@
 
 dependencies = [
     "pyperclip",
     "pathspec",
 ]
 
 [project.scripts]
-parse_md = "markdown_parser:main"
-get_directory_structure = "directory_structure:main"
-generate_docs = "docs_generator:main"
+pg = "prompt_generator.run:main"
 
 [project.urls]
 repository = "https://github.com/vincenzocascone/prompt-generator"
```

### Comparing `prompt-generator-0.3.0/src/directory_structure/get_directory_structure.py` & `prompt-generator-0.4.0/prompt_generator/get_dir_structure/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import argparse
+import os
 
-from file_utils import get_dir_json, load_gitignore
-from print_utils import print_result
+from prompt_generator.utils import FileUtils, PrintUtils
 
 
 def get_args():
-    """Parse command line arguments."""
-    parser = argparse.ArgumentParser(description="Directory Structure")
-    parser.add_argument(
-        "root_dir_path", help="path to the root directory", type=str)
-    parser.add_argument(
-        "-gitignore", help="path to the .gitignore file", type=str, default=None)
+    """Parses command line arguments."""
+    parser = argparse.ArgumentParser(description="Get directory structure of a project.")
+    parser.add_argument("root_dir", type=str, help="Root directory of the project.")
+    parser.add_argument("--gitignore", type=str, help="Path to the .gitignore file.", default=None)
     return parser.parse_args()
 
 
-def main():
-    """Main function to get the directory structure."""
-    args = get_args()
-    gitignore = load_gitignore(args.root_dir_path, args.gitignore)
-    result = get_dir_json(args.root_dir_path, gitignore)
-    if result:
-        print_result(result, "Directory Structure:")
+def main(args):
+    """Main function to get the directory structure as json."""
+    root_dir = args.root_dir
+    gitignore_path = args.gitignore
+
+    if not os.path.isdir(root_dir):
+        PrintUtils.print_error("The specified root directory does not exist.")
+        return
+
+    gitignore = FileUtils.load_gitignore(root_dir, gitignore_path)
+    dir_structure = FileUtils.get_dir_json(root_dir, gitignore)
+    PrintUtils.print_result(dir_structure, "Directory Structure:")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `prompt-generator-0.3.0/src/prompt_generator.egg-info/PKG-INFO` & `prompt-generator-0.4.0/prompt_generator.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-generator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code.
 Author: Vincenzo Cascone
 License: MIT License
         
         Copyright (c) 2023 Vince
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,42 +44,107 @@
 
 ```bash
 pip install prompt-generator
 ```
 
 ## Features
 
-- ### Generate Docs
+- ### Generate Project Documentation
 
-  This script generates a prompt that can be used to make the AI write documentation
-  for the project. When executed, it will first ask for some info about the project, such as the name, description, root
-  path. Optionally you can provide the path to config files such as pyproject.toml for a python project or
-  package.json for a node project. The same can be done with particularly relevant files. This will allow the AI to have
-  a better understanding of the project and generate more accurate documentation.
+  This script generates a prompt that can be used to make the AI write documentation for the project.
 
-  To utilize it, use the following command in your terminal:
+  When executed without arguments it will ask for some info about the project, such as the name, description, root
+  directory, paths to config files, main files, and docs specs.
+
+  Instead of writing the info manually you can also provide the path to a JSON file that contains the prompt
+  configuration.
+  The JSON should have the following structure:
+
+  ```
+  {
+    "name": "<string> (required)",
+    "description": "<string> (required)",
+    "target_audience": "<string> (optional)",
+    "root_dir": "<string> (required)",
+    "config_files": [
+        {
+            "path": "<string> (required)",
+            "label": "<string> (optional)"
+        },
+        ...
+    ] (optional),
+    "main_files": [
+        {
+            "path": "<string> (required)",
+            "label": "<string> (optional)"
+        },
+        ...
+    ] (optional),
+    "docs_specs": "<string> (optional)"
+  }
+  ```
+
+  To utilize this script, use the following command in your terminal:
+
+  ```bash
+  pg docs_prompt [--config <path to config file>]
+  ```
+
+  Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
+  immediate use or future reference.
+
+- ### Complete Tasks
+
+  This script generates a prompt that can be used to help AI complete tasks for the project.
 
-    ```bash
-    generate_docs
-    ```
+  It will ask for the project name, description or the path to README/docs, root directory, and optionally the paths and
+  labels to the files related to the tasks. Finally, it will ask for the single task or task list.
+
+  Instead of writing the info manually you can also provide the path to a JSON file that contains the prompt
+  configuration.
+  The JSON should have the following structure:
+
+  ```
+  {
+    "project_overview": "<string> (optional)",
+    "docs_path": "<string> (optional)",
+    "relevant_files": [
+      {
+        "path": "<string> (required)",
+        "label": "<string> (optional)"
+      },
+      ...
+    ] (optional),
+    "tasks": [
+      "<string> (required)",
+      ...
+    ] (required)
+  }
+  ```
+
+  To utilize this script, use the following command in your terminal:
+
+  ```bash
+  pg tasks_prompt [--config <path to config file>]
+  ```
 
   Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
   immediate use or future reference.
 
 - ### Markdown Parser
 
   The Markdown Parser is a robust utility specifically designed to parse markdown files. It works by replacing all
   hyperlinks within a Markdown document with the actual content of the linked files. This function proves extremely
   useful if you maintain a collection of prompt files written in Markdown format, and these files contain references to
   other project documents.
 
   To utilize it, use the following command in your terminal:
 
   ```bash
-  parse_md <path to the markdown file>
+  pg parse_md <path to the markdown file>
   ```
 
   Upon successful execution, the resultant parsed content will be displayed in your terminal and copied to your
   clipboard for immediate use or future reference.
 
 - ### Directory Structure
 
@@ -88,12 +153,12 @@
   .gitignore file. This makes it an essential tool for giving the AI a better understanding of the context of your
   project. The returned JSON is minified in order to be more token efficient.
 
   To utilize it, use the following command in your terminal. You can optionally provide the .gitignore file path using
   the -gitignore flag, if not provided, the script will search for a .gitignore file in the root directory:
 
   ```bash
-  get_directory_structure <path to the directory> [-gitignore]
+  pg get_dir_structure <path to the directory> [--gitignore <path to the .gitignore file>]
   ```
 
   Upon successful execution, the resultant json will be displayed in your terminal and copied to your
   clipboard for immediate use or future reference.
```

