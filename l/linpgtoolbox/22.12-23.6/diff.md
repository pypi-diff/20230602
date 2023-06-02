# Comparing `tmp/linpgtoolbox-22.12.tar.gz` & `tmp/linpgtoolbox-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linpgtoolbox-22.12.tar", last modified: Sat Dec 17 21:35:26 2022, max compression
+gzip compressed data, was "linpgtoolbox-23.6.tar", last modified: Fri Jun  2 20:44:16 2023, max compression
```

## Comparing `linpgtoolbox-22.12.tar` & `linpgtoolbox-23.6.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-12-17 21:35:26.342486 linpgtoolbox-22.12/
--rw-rw-rw-   0        0        0    35803 2022-12-01 20:38:01.000000 linpgtoolbox-22.12/LICENSE
--rw-rw-rw-   0        0        0       36 2022-12-01 20:38:01.000000 linpgtoolbox-22.12/MANIFEST.in
--rw-rw-rw-   0        0        0     2207 2022-12-17 21:35:26.343487 linpgtoolbox-22.12/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2022-12-01 20:38:01.000000 linpgtoolbox-22.12/README.md
--rw-rw-rw-   0        0        0      363 2022-12-01 20:38:01.000000 linpgtoolbox-22.12/pyproject.toml
--rw-rw-rw-   0        0        0      755 2022-12-17 21:35:26.344486 linpgtoolbox-22.12/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-17 21:35:26.246971 linpgtoolbox-22.12/src/
-drwxrwxrwx   0        0        0        0 2022-12-17 21:35:26.318486 linpgtoolbox-22.12/src/linpgtoolbox/
--rw-rw-rw-   0        0        0     5349 2022-12-17 21:35:08.000000 linpgtoolbox-22.12/src/linpgtoolbox/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0    35803 2022-12-17 21:35:08.000000 linpgtoolbox-22.12/src/linpgtoolbox/LICENSE
--rw-rw-rw-   0        0        0     1669 2022-12-17 21:35:08.000000 linpgtoolbox-22.12/src/linpgtoolbox/README.md
--rw-rw-rw-   0        0        0    18944 2022-12-17 21:35:06.000000 linpgtoolbox-22.12/src/linpgtoolbox/__init__.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0        0 2022-12-17 21:35:07.000000 linpgtoolbox-22.12/src/linpgtoolbox/__init__.pyi
-drwxrwxrwx   0        0        0        0 2022-12-17 21:35:26.342486 linpgtoolbox-22.12/src/linpgtoolbox/__pyinstaller/
--rw-rw-rw-   0        0        0       90 2022-12-01 20:38:01.000000 linpgtoolbox-22.12/src/linpgtoolbox/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      850 2022-12-01 20:38:01.000000 linpgtoolbox-22.12/src/linpgtoolbox/__pyinstaller/hook.py
--rw-rw-rw-   0        0        0   126976 2022-12-17 21:35:07.000000 linpgtoolbox-22.12/src/linpgtoolbox/builder.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0      899 2022-12-17 21:35:08.000000 linpgtoolbox-22.12/src/linpgtoolbox/builder.pyi
--rw-rw-rw-   0        0        0     4643 2022-12-01 20:55:43.000000 linpgtoolbox-22.12/src/linpgtoolbox/compiler.py
--rw-rw-rw-   0        0        0    49152 2022-12-17 21:35:06.000000 linpgtoolbox-22.12/src/linpgtoolbox/organizer.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0       96 2022-12-17 21:35:07.000000 linpgtoolbox-22.12/src/linpgtoolbox/organizer.pyi
--rw-rw-rw-   0        0        0    56320 2022-12-17 21:35:06.000000 linpgtoolbox-22.12/src/linpgtoolbox/pyinstaller.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0      126 2022-12-17 21:35:08.000000 linpgtoolbox-22.12/src/linpgtoolbox/pyinstaller.pyi
--rw-rw-rw-   0        0        0    63488 2022-12-17 21:35:06.000000 linpgtoolbox-22.12/src/linpgtoolbox/zipper.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0       68 2022-12-17 21:35:07.000000 linpgtoolbox-22.12/src/linpgtoolbox/zipper.pyi
-drwxrwxrwx   0        0        0        0 2022-12-17 21:35:26.339486 linpgtoolbox-22.12/src/linpgtoolbox.egg-info/
--rw-rw-rw-   0        0        0     2207 2022-12-17 21:35:26.000000 linpgtoolbox-22.12/src/linpgtoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      834 2022-12-17 21:35:26.000000 linpgtoolbox-22.12/src/linpgtoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-17 21:35:26.000000 linpgtoolbox-22.12/src/linpgtoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-12-17 21:35:26.000000 linpgtoolbox-22.12/src/linpgtoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-17 21:35:26.000000 linpgtoolbox-22.12/src/linpgtoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 20:44:16.075862 linpgtoolbox-23.6/
+-rw-rw-rw-   0        0        0    35803 2023-05-16 03:38:47.000000 linpgtoolbox-23.6/LICENSE
+-rw-rw-rw-   0        0        0     2456 2023-06-02 20:44:16.074862 linpgtoolbox-23.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2023-05-27 16:58:11.000000 linpgtoolbox-23.6/README.md
+-rw-rw-rw-   0        0        0     1145 2023-05-27 05:48:48.000000 linpgtoolbox-23.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:44:16.075862 linpgtoolbox-23.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 20:44:16.048862 linpgtoolbox-23.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:44:16.068862 linpgtoolbox-23.6/src/linpgtoolbox/
+-rw-rw-rw-   0        0        0     5349 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0    35803 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/LICENSE
+-rw-rw-rw-   0        0        0     1789 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/README.md
+-rw-rw-rw-   0        0        0    18944 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/__init__.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-02 20:44:16.073862 linpgtoolbox-23.6/src/linpgtoolbox/__pyinstaller/
+-rw-rw-rw-   0        0        0       90 2023-05-16 03:38:47.000000 linpgtoolbox-23.6/src/linpgtoolbox/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      850 2023-05-16 03:38:47.000000 linpgtoolbox-23.6/src/linpgtoolbox/__pyinstaller/hook.py
+-rw-rw-rw-   0        0        0   131584 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/builder.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0      931 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/builder.pyi
+-rw-rw-rw-   0        0        0     4655 2023-05-16 03:51:26.000000 linpgtoolbox-23.6/src/linpgtoolbox/compiler.py
+-rw-rw-rw-   0        0        0    51200 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/organizer.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0       96 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/organizer.pyi
+-rw-rw-rw-   0        0        0    51712 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/pkginstaller.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0      318 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/pkginstaller.pyi
+-rw-rw-rw-   0        0        0      119 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/py.typed
+-rw-rw-rw-   0        0        0    59392 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/pyinstaller.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0      126 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/pyinstaller.pyi
+-rw-rw-rw-   0        0        0    65536 2023-06-02 20:43:58.000000 linpgtoolbox-23.6/src/linpgtoolbox/zipper.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0       68 2023-06-02 20:43:59.000000 linpgtoolbox-23.6/src/linpgtoolbox/zipper.pyi
+drwxrwxrwx   0        0        0        0 2023-06-02 20:44:16.072862 linpgtoolbox-23.6/src/linpgtoolbox.egg-info/
+-rw-rw-rw-   0        0        0     2456 2023-06-02 20:44:16.000000 linpgtoolbox-23.6/src/linpgtoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      922 2023-06-02 20:44:16.000000 linpgtoolbox-23.6/src/linpgtoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:44:16.000000 linpgtoolbox-23.6/src/linpgtoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-02 20:44:16.000000 linpgtoolbox-23.6/src/linpgtoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 20:44:16.000000 linpgtoolbox-23.6/src/linpgtoolbox.egg-info/top_level.txt
```

### Comparing `linpgtoolbox-22.12/LICENSE` & `linpgtoolbox-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linpgtoolbox-22.12/PKG-INFO` & `linpgtoolbox-23.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: linpgtoolbox
-Version: 22.12
+Version: 23.6
 Summary: A set of tools for managing, compiling, and uploading your own package.
-Home-page: https://github.com/LinpgFoundation/linpg-toolbox
-Author: Linpg Foundation
-Author-email: yudong9912@gmail.com
+Author-email: Linpg Foundation <yudong9912@gmail.com>
+Project-URL: Homepage, https://github.com/LinpgFoundation/linpg-toolbox
 Project-URL: Bug Tracker, https://github.com/LinpgFoundation/linpg-toolbox/issues
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # linpg-toolbox
 
@@ -26,25 +27,29 @@
 
 **Builder** - Automates the process of compiling and uploading your personal library.
 
 - compiler.py - A python script that is called by the Builder. Supports multi-processing.
 
 **Organizer** - A organizing tool that organizes your gitignore files
 
+**pkginstaller** - A simple package install and uninstall tool.
+
 **Pyinstaller** - Generate a Pyinstaller template for your personal repository on the fly. Typically, the template no longer requires any further changes.
 
 **Zipper** - Pack file and directory according to the linpg.zipscript file
 
 
 
 工具包包含以下程序：
 
 **Builder** - 自动化编译并上传你个人库的流程
 
 - compiler.py - 被Builder调用的编译脚本，支持多进程
 
 **Organizer** - 整理工具，可以整理你的gitignore文件
 
+**pkginstaller** - 第三方库安装以及卸载
+
 **Pyinstaller** - 为你的个人库快速生成一个__pyinstaller模板。一般情况下，该模板不再需要任何的变动
 
 **Zipper** - 根据linpg.zipscript文件打包数据
```

### Comparing `linpgtoolbox-22.12/README.md` & `linpgtoolbox-23.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 
 **Builder** - Automates the process of compiling and uploading your personal library.
 
 - compiler.py - A python script that is called by the Builder. Supports multi-processing.
 
 **Organizer** - A organizing tool that organizes your gitignore files
 
+**pkginstaller** - A simple package install and uninstall tool.
+
 **Pyinstaller** - Generate a Pyinstaller template for your personal repository on the fly. Typically, the template no longer requires any further changes.
 
 **Zipper** - Pack file and directory according to the linpg.zipscript file
 
 
 
 工具包包含以下程序：
 
 **Builder** - 自动化编译并上传你个人库的流程
 
 - compiler.py - 被Builder调用的编译脚本，支持多进程
 
 **Organizer** - 整理工具，可以整理你的gitignore文件
 
+**pkginstaller** - 第三方库安装以及卸载
+
 **Pyinstaller** - 为你的个人库快速生成一个__pyinstaller模板。一般情况下，该模板不再需要任何的变动
 
 **Zipper** - 根据linpg.zipscript文件打包数据
```

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox/CODE_OF_CONDUCT.md` & `linpgtoolbox-23.6/src/linpgtoolbox/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox/LICENSE` & `linpgtoolbox-23.6/src/linpgtoolbox/LICENSE`

 * *Files identical despite different names*

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox/README.md` & `linpgtoolbox-23.6/src/linpgtoolbox/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 
 **Builder** - Automates the process of compiling and uploading your personal library.
 
 - compiler.py - A python script that is called by the Builder. Supports multi-processing.
 
 **Organizer** - A organizing tool that organizes your gitignore files
 
+**pkginstaller** - A simple package install and uninstall tool.
+
 **Pyinstaller** - Generate a Pyinstaller template for your personal repository on the fly. Typically, the template no longer requires any further changes.
 
 **Zipper** - Pack file and directory according to the linpg.zipscript file
 
 
 
 工具包包含以下程序：
 
 **Builder** - 自动化编译并上传你个人库的流程
 
 - compiler.py - 被Builder调用的编译脚本，支持多进程
 
 **Organizer** - 整理工具，可以整理你的gitignore文件
 
+**pkginstaller** - 第三方库安装以及卸载
+
 **Pyinstaller** - 为你的个人库快速生成一个__pyinstaller模板。一般情况下，该模板不再需要任何的变动
 
 **Zipper** - 根据linpg.zipscript文件打包数据
```

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox/__pyinstaller/hook.py` & `linpgtoolbox-23.6/src/linpgtoolbox/__pyinstaller/hook.py`

 * *Files identical despite different names*

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox/builder.pyi` & `linpgtoolbox-23.6/src/linpgtoolbox/builder.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from .pkginstaller import PackageInstaller as PackageInstaller
 from .pyinstaller import Pyinstaller as Pyinstaller
 from _typeshed import Incomplete
 from enum import IntEnum
-from typing import Optional
 
 class SmartAutoModuleCombineMode(IntEnum):
     DISABLE: Incomplete
     FOLDER_ONLY: Incomplete
     ALL_INTO_ONE: Incomplete
 
 class Builder:
     @staticmethod
     def delete_file_if_exist(path: str) -> None: ...
     @staticmethod
     def copy(files: tuple, target_folder: str) -> None: ...
     @classmethod
     def compile(cls, source_folder: str, target_folder: str = ..., additional_files: tuple = ..., ignore_key_words: tuple = ..., smart_auto_module_combine: SmartAutoModuleCombineMode = ..., remove_building_cache: bool = ..., update_the_one_in_sitepackages: bool = ..., include_pyinstaller_program: bool = ..., options: dict = ...) -> None: ...
     @classmethod
-    def upload_package(cls, python_ver: Optional[str] = ...) -> None: ...
+    def upload_package(cls, python_ver: str | None = ...) -> None: ...
```

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox/compiler.py` & `linpgtoolbox-23.6/src/linpgtoolbox/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import path as OS_PATH
 from os import remove as OS_REMOVE
 from subprocess import check_call
 
-from setuptools import setup  # setuptools.setup import不可以在Cython.Build之后
+# setuptools.setup import不可以在Cython.Build之后
+from setuptools import setup  # type: ignore
 from Cython.Build import cythonize  # type: ignore
 
 
 # 编译方法
 def _compile_file(
     _source_folder: str,
     _path: str,
@@ -29,15 +30,14 @@
     # 生成pyi后缀的typing提示文件
     check_call(["stubgen", _path, "-o", OS_PATH.dirname(_source_folder)])
     # 删除原始py文件
     OS_REMOVE(_path)
 
 
 if __name__ == "__main__":
-
     import json
     from glob import glob
     from multiprocessing import Process
 
     # 加载全局参数
     with open("builder_data_cache.json", "r", encoding="utf-8") as f:
         Data: dict = json.load(f)
@@ -55,15 +55,14 @@
         _ignore_key_words: tuple = tuple(Data["ignore_key_words"])
 
     # 移除参数文件
     OS_REMOVE("builder_data_cache.json")
 
     # 编译进程管理模组
     class _CompileProcessManager:
-
         # 储存进程的列表
         __processes: list[Process] = []
 
         # 是否忽略文件
         @classmethod
         def __if_ignore(cls, _path: str) -> bool:
             for key_word in _ignore_key_words:
```

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox.egg-info/PKG-INFO` & `linpgtoolbox-23.6/src/linpgtoolbox.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: linpgtoolbox
-Version: 22.12
+Version: 23.6
 Summary: A set of tools for managing, compiling, and uploading your own package.
-Home-page: https://github.com/LinpgFoundation/linpg-toolbox
-Author: Linpg Foundation
-Author-email: yudong9912@gmail.com
+Author-email: Linpg Foundation <yudong9912@gmail.com>
+Project-URL: Homepage, https://github.com/LinpgFoundation/linpg-toolbox
 Project-URL: Bug Tracker, https://github.com/LinpgFoundation/linpg-toolbox/issues
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # linpg-toolbox
 
@@ -26,25 +27,29 @@
 
 **Builder** - Automates the process of compiling and uploading your personal library.
 
 - compiler.py - A python script that is called by the Builder. Supports multi-processing.
 
 **Organizer** - A organizing tool that organizes your gitignore files
 
+**pkginstaller** - A simple package install and uninstall tool.
+
 **Pyinstaller** - Generate a Pyinstaller template for your personal repository on the fly. Typically, the template no longer requires any further changes.
 
 **Zipper** - Pack file and directory according to the linpg.zipscript file
 
 
 
 工具包包含以下程序：
 
 **Builder** - 自动化编译并上传你个人库的流程
 
 - compiler.py - 被Builder调用的编译脚本，支持多进程
 
 **Organizer** - 整理工具，可以整理你的gitignore文件
 
+**pkginstaller** - 第三方库安装以及卸载
+
 **Pyinstaller** - 为你的个人库快速生成一个__pyinstaller模板。一般情况下，该模板不再需要任何的变动
 
 **Zipper** - 根据linpg.zipscript文件打包数据
```

### Comparing `linpgtoolbox-22.12/src/linpgtoolbox.egg-info/SOURCES.txt` & `linpgtoolbox-23.6/src/linpgtoolbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 src/linpgtoolbox/CODE_OF_CONDUCT.md
 src/linpgtoolbox/LICENSE
 src/linpgtoolbox/README.md
-src/linpgtoolbox/__init__.cp310-win_amd64.pyd
+src/linpgtoolbox/__init__.cp311-win_amd64.pyd
 src/linpgtoolbox/__init__.pyi
-src/linpgtoolbox/builder.cp310-win_amd64.pyd
+src/linpgtoolbox/builder.cp311-win_amd64.pyd
 src/linpgtoolbox/builder.pyi
 src/linpgtoolbox/compiler.py
-src/linpgtoolbox/organizer.cp310-win_amd64.pyd
+src/linpgtoolbox/organizer.cp311-win_amd64.pyd
 src/linpgtoolbox/organizer.pyi
-src/linpgtoolbox/pyinstaller.cp310-win_amd64.pyd
+src/linpgtoolbox/pkginstaller.cp311-win_amd64.pyd
+src/linpgtoolbox/pkginstaller.pyi
+src/linpgtoolbox/py.typed
+src/linpgtoolbox/pyinstaller.cp311-win_amd64.pyd
 src/linpgtoolbox/pyinstaller.pyi
-src/linpgtoolbox/zipper.cp310-win_amd64.pyd
+src/linpgtoolbox/zipper.cp311-win_amd64.pyd
 src/linpgtoolbox/zipper.pyi
 src/linpgtoolbox.egg-info/PKG-INFO
 src/linpgtoolbox.egg-info/SOURCES.txt
 src/linpgtoolbox.egg-info/dependency_links.txt
 src/linpgtoolbox.egg-info/requires.txt
 src/linpgtoolbox.egg-info/top_level.txt
 src/linpgtoolbox/__pyinstaller/__init__.py
```

