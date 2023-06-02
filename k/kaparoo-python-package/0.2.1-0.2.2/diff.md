# Comparing `tmp/kaparoo_python_package-0.2.1.tar.gz` & `tmp/kaparoo_python_package-0.2.2.tar.gz`

## Comparing `kaparoo_python_package-0.2.1.tar` & `kaparoo_python_package-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/py.typed
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    21066 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/utils/optional.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/utils/singleton.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/LICENSE
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/README.md
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/py.typed
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/path.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/utils/singleton.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/README.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/PKG-INFO
```

### Comparing `kaparoo_python_package-0.2.1/kaparoo/filesystem/path.py` & `kaparoo_python_package-0.2.2/kaparoo/filesystem/path.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,36 +8,40 @@
     "check_if_path_exists",
     "check_if_paths_exist",
     "check_if_file_exists",
     "check_if_files_exist",
     "check_if_dir_exists",
     "check_if_dirs_exist",
     "get_paths",
-    "get_file_paths",
-    "get_dir_paths",
+    "get_files",
+    "get_dirs",
+    "is_empty_dir",
+    "is_empty_dir_unsafe",
+    "are_empty_dirs",
+    "are_empty_dirs_unsafe",
 )
 
 import os
 import random
 from collections.abc import Callable, Sequence
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, overload
 
 from kaparoo.filesystem.exceptions import DirectoryNotFoundError, NotAFileError
 
 if TYPE_CHECKING:
-    from kaparoo.filesystem.types import StrPath
+    from kaparoo.filesystem.types import StrPath, StrPaths
 
 
 def stringify_path(path: StrPath) -> str:
     """Convert a path to a string representation."""
     return os.fspath(path)
 
 
-def stringify_paths(paths: Sequence[StrPath]) -> Sequence[str]:
+def stringify_paths(paths: StrPaths) -> Sequence[str]:
     """Convert a sequence of paths to a sequence of string representations."""
     return [stringify_path(p) for p in paths]
 
 
 @overload
 def check_if_path_exists(path: StrPath, *, stringify: Literal[False] = False) -> Path:
     ...
@@ -71,38 +75,38 @@
         raise FileNotFoundError(f"no such path: {path}")
 
     return stringify_path(path) if stringify else path
 
 
 @overload
 def check_if_paths_exist(
-    paths: Sequence[StrPath],
+    paths: StrPaths,
     *,
     root: StrPath | None = None,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def check_if_paths_exist(
-    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: Literal[True]
+    paths: StrPaths, *, root: StrPath | None = None, stringify: Literal[True]
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def check_if_paths_exist(
-    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool
+    paths: StrPaths, *, root: StrPath | None = None, stringify: bool
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_paths_exist(
-    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool = False
+    paths: StrPaths, *, root: StrPath | None = None, stringify: bool = False
 ) -> Sequence[Path] | Sequence[str]:
     """Check if multiple paths exist and return them as a sequence of `Path` objects.
 
     Args:
         paths: A sequence of paths to check for existence.
         root: The root directory to resolve relative paths. If provided, the `paths`
             will be resolved relative to the `root` directory. Defaults to `None`.
@@ -163,38 +167,38 @@
         raise NotAFileError(f"not a file: {path}")
 
     return stringify_path(path) if stringify else path
 
 
 @overload
 def check_if_files_exist(
-    paths: Sequence[StrPath],
+    paths: StrPaths,
     *,
     root: StrPath | None = None,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def check_if_files_exist(
-    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: Literal[True]
+    paths: StrPaths, *, root: StrPath | None = None, stringify: Literal[True]
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def check_if_files_exist(
-    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool
+    paths: StrPaths, *, root: StrPath | None = None, stringify: bool
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_files_exist(
-    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool = False
+    paths: StrPaths, *, root: StrPath | None = None, stringify: bool = False
 ) -> Sequence[Path] | Sequence[str]:
     """Check if multiple files exist and return them as a sequence of `Path` objects.
 
     Args:
         paths: A sequence of file paths to check for existence.
         root: The root directory to resolve relative paths. If provided, the `paths`
             will be resolved relative to the `root` directory. Defaults to `None`.
@@ -268,47 +272,47 @@
         raise NotADirectoryError(f"not a directory: {path}")
 
     return stringify_path(path) if stringify else path
 
 
 @overload
 def check_if_dirs_exist(
-    paths: Sequence[StrPath],
+    paths: StrPaths,
     *,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def check_if_dirs_exist(
-    paths: Sequence[StrPath],
+    paths: StrPaths,
     *,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def check_if_dirs_exist(
-    paths: Sequence[StrPath],
+    paths: StrPaths,
     *,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_dirs_exist(
-    paths: Sequence[StrPath],
+    paths: StrPaths,
     *,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Check if multiple directories exist and return them as a sequence of `Path` objects.
 
@@ -342,56 +346,56 @@
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files or directories in a given directory.
 
     Args:
@@ -451,61 +455,61 @@
             raise ValueError("`num_samples` must be a positive int")
         paths = random.sample(paths, num_samples)
 
     return stringify_paths(paths) if stringify else paths
 
 
 @overload
-def get_file_paths(
+def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
-def get_file_paths(
+def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
-def get_file_paths(
+def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
-def get_file_paths(
+def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files in a given directory.
 
     Args:
@@ -550,61 +554,61 @@
         stringify=stringify,
     )
 
     return file_paths
 
 
 @overload
-def get_dir_paths(
+def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
-def get_dir_paths(
+def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
-def get_dir_paths(
+def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
-def get_dir_paths(
+def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
-    ignores: Sequence[StrPath] | None = None,
+    ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of directories in a given directory.
 
     Args:
@@ -646,7 +650,81 @@
         ignores=ignores,
         condition=dir_condition,
         recursive=recursive,
         stringify=stringify,
     )
 
     return dir_paths
+
+
+def is_empty_dir_unsafe(path: StrPath) -> bool:
+    """Check if a directory is empty.
+
+    Unlike the function `is_empty_dir()`, this function does not check the existence of
+    the input argument `path`. Use this function only if you are sure it exists.
+
+    Args:
+        path: The path to the directory.
+
+    Returns:
+        A boolean indicating whether the directory is empty.
+    """
+    return not os.listdir(path)
+
+
+def is_empty_dir(path: StrPath) -> bool:
+    """Check if a directory is empty.
+
+    Args:
+        path: The path to the directory.
+
+    Returns:
+        A boolean indicating whether the directory is empty.
+
+    Raises:
+        DirectoryNotFoundError: If the directory does not exist.
+        NotADirectoryError: If `path` exists but is not a directory.
+    """
+
+    path = check_if_dir_exists(path)
+    return is_empty_dir_unsafe(path)
+
+
+def are_empty_dirs_unsafe(paths: StrPaths, *, root: StrPath | None = None) -> bool:
+    """Check if multiple directories are empty.
+
+    Unlike the function `are_empty_dirs()`, this function does not check the existence
+    of the input arguments `paths` and `root`. Use this function only if you are sure
+    they exist.
+
+    Args:
+        paths: A sequence of directory paths to check.
+        root: The root directory to resolve relative paths. Defaults to `None`.
+
+    Returns:
+        A boolean indicating whether all directories are empty.
+    """
+
+    if root is not None:
+        paths = [os.path.join(root, p) for p in paths]
+    return all(is_empty_dir_unsafe(p) for p in paths)
+
+
+def are_empty_dirs(paths: StrPaths, *, root: StrPath | None = None) -> bool:
+    """Check if multiple directories are empty.
+
+    Args:
+        paths: A sequence of directory paths to check.
+        root: The root directory to resolve relative paths. Defaults to `None`.
+
+    Returns:
+        A boolean indicating whether all directories are empty.
+
+    Raises:
+        DirectoryNotFoundError: If the `root` directory does not exist.
+        DirectoryNotFoundError: If any of the directory paths does not exist.
+        NotADirectoryError: If `root` exists but is not a directory.
+        NotADirectoryError: If any of the paths exists but is not a directory.
+    """
+
+    paths = check_if_dirs_exist(paths, root=root)
+    return all(is_empty_dir_unsafe(p) for p in paths)
```

### Comparing `kaparoo_python_package-0.2.1/kaparoo/utils/optional.py` & `kaparoo_python_package-0.2.2/kaparoo/utils/optional.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.1/kaparoo/utils/singleton.py` & `kaparoo_python_package-0.2.2/kaparoo/utils/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 __all__ = ("Singleton", "SingletonMeta", "singleton")
 
 from collections.abc import Callable
+from functools import wraps
 from typing import Type, TypeVar
 
 from typing_extensions import Self
 
 T = TypeVar("T")
 
 
@@ -65,13 +66,14 @@
         >>> obj2 = MyClass()
         >>> obj1 is obj2
         True
     """
 
     _instances: dict[Type[T], T] = {}
 
+    @wraps(cls)
     def wrapper(*args, **kwargs) -> T:
         if cls not in _instances:
             _instances[cls] = cls(*args, **kwargs)
         return _instances[cls]
 
     return wrapper
```

### Comparing `kaparoo_python_package-0.2.1/.gitignore` & `kaparoo_python_package-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.1/LICENSE` & `kaparoo_python_package-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.1/README.md` & `kaparoo_python_package-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.1/pyproject.toml` & `kaparoo_python_package-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.1/PKG-INFO` & `kaparoo_python_package-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python-package
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

