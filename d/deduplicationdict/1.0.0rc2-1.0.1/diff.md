# Comparing `tmp/deduplicationdict-1.0.0rc2.tar.gz` & `tmp/deduplicationdict-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deduplicationdict-1.0.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deduplicationdict-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deduplicationdict-1.0.0rc2.tar` & `deduplicationdict-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-27 08:06:02.215188 deduplicationdict-1.0.0rc2/README.md
--rw-r--r--   0        0        0    10020 2023-05-27 06:44:12.394368 deduplicationdict-1.0.0rc2/deduplicationdict/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-27 08:09:53.417806 deduplicationdict-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 deduplicationdict-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4095 2023-06-02 01:57:49.631690 deduplicationdict-1.0.1/README.md
+-rw-r--r--   0        0        0    10826 2023-05-27 23:42:44.735005 deduplicationdict-1.0.1/deduplicationdict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.1/deduplicationdict/py.typed
+-rw-r--r--   0        0        0     4026 2023-05-27 23:51:47.853909 deduplicationdict-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.1/PKG-INFO
```

### Comparing `deduplicationdict-1.0.0rc2/LICENSE` & `deduplicationdict-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.0rc2/deduplicationdict/__init__.py` & `deduplicationdict-1.0.1/deduplicationdict/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,29 +67,34 @@
 
         self.key_dict: Dict[str, Union[str, DeDuplicationDict]] = {}
         self.value_dict: Dict[str, Any] = {} if _value_dict is None else _value_dict
 
         for k, v in dict(*args, **kwargs).items():
             self[k] = v
 
-    def _set_value_dict(self, value_dict: dict) -> None:
+    def _set_value_dict(self, value_dict: dict) -> DeDuplicationDict:
         """Update the value dictionary and propagate the changes to nested DeDuplicationDict instances.
 
         Args:
             value_dict (dict): The new value dictionary to use for deduplication.
+
+        Return:
+            DeDuplicationDict: self
         """
 
         value_dict.update(self.value_dict)
         self.value_dict = value_dict
         for v in self.key_dict.values():
             if isinstance(v, str):
                 continue
 
             v._set_value_dict(value_dict)
 
+        return self
+
     def __setitem__(self, key: KT, value: VT) -> None:
         """Set the value for the given key, deduplicating the value if necessary.
 
         Args:
             key (KT): The key to set the value for.
             value (VT): The value to set for the given key.
         """
@@ -101,15 +106,17 @@
             self.key_dict[key] = DeDuplicationDict(value, _value_dict=self.value_dict)
         elif isinstance(value, DeDuplicationDict):
             self.key_dict[key] = value
             value._set_value_dict(self.value_dict)
         else:
             hash_id = sha256(pickle.dumps(value)).hexdigest()[:self.hash_length]
             self.key_dict[key] = hash_id
-            self.value_dict[hash_id] = value
+
+            if hash_id not in self.value_dict:
+                self.value_dict[hash_id] = value
 
     def __getitem__(self, key: KT) -> VT_co:
         """Get the value for the given key.
 
         Args:
             key (KT): The key to get the value for.
 
@@ -144,41 +151,53 @@
         for v in self.key_dict.values():
             if isinstance(v, str):
                 all_hashes_in_use.add(v)
             else:
                 all_hashes_in_use.update(v.all_hashes_in_use())
         return all_hashes_in_use
 
-    def clean_up(self) -> None:
-        """Remove unused hash values from the value dictionary."""
+    def clean_up(self) -> DeDuplicationDict:
+        """Remove unused hash values from the value dictionary.
+
+        Return:
+            DeDuplicationDict: self
+        """
 
         all_hashes_in_use = self.all_hashes_in_use()
         all_hashes = set(self.value_dict.keys())
         not_in_use = all_hashes - all_hashes_in_use
         for hash_id in not_in_use:
             del self.value_dict[hash_id]
 
+        return self
+
     def detach(self) -> DeDuplicationDict:
         """Detach the DeDuplicationDict instance from its value dictionary, creating a standalone instance.
 
         Returns:
             DeDuplicationDict: A new DeDuplicationDict instance with its own value dictionary.
         """
 
         return self.from_json_save_dict(self.to_json_save_dict())
 
-    def _del_detach(self) -> None:
-        """Detach the DeDuplicationDict instance from its value dictionary and clean up unused hash values."""
+    def _del_detach(self) -> DeDuplicationDict:
+        """Detach the DeDuplicationDict instance from its value dictionary and clean up unused hash values.
+
+        Return:
+            DeDuplicationDict: self
+        """
 
         self._set_value_dict({})
         self.clean_up()
 
         for k, v in self.value_dict.items():
             self.value_dict[k] = copy.deepcopy(v)
 
+        return self
+
     def __delitem__(self, key: KT) -> None:
         """Delete the item with the given key.
 
         Args:
             key (KT): The key of the item to delete.
 
         Raises:
@@ -262,14 +281,35 @@
         """
 
         return {
             'key_dict': self._get_key_dict(),
             'value_dict': self.value_dict
         }
 
+    def _set_key_dict(self, key_dict: dict) -> DeDuplicationDict:
+        """Set the key dictionary of the DeDuplicationDict instance from a normal dictionary format.
+
+        Args:
+            key_dict (dict): The key dictionary to set.
+
+        Returns:
+            DeDuplicationDict: self
+        """
+
+        for k, v in key_dict.items():
+            if isinstance(v, dict):
+                new_dict = self.__class__()
+                new_dict.value_dict = self.value_dict
+                new_dict._set_key_dict(v)
+                self.key_dict[k] = new_dict
+            else:
+                self.key_dict[k] = v
+
+        return self
+
     @classmethod
     def from_json_save_dict(cls, d: dict, _v: dict = None) -> DeDuplicationDict:
         """Create a DeDuplicationDict instance from a dictionary that was saved to a JSON file.
 
         Args:
             d (dict): The dictionary that was saved to a JSON file.
             _v (dict, optional): The value dictionary to use. Defaults to None.
@@ -278,17 +318,10 @@
             DeDuplicationDict: A new DeDuplicationDict instance with the same key-value pairs as the given dictionary.
         """
 
         if _v is None:
             return cls.from_json_save_dict(d['key_dict'], _v=d['value_dict'])
 
         new_dict = cls()
-        new_dict.key_dict = {}
         new_dict.value_dict = _v
-
-        for k, v in d.items():
-            if isinstance(v, dict):
-                new_dict.key_dict[k] = cls.from_json_save_dict(v, _v=_v)
-            else:
-                new_dict.key_dict[k] = v
-
+        new_dict._set_key_dict(d)
         return new_dict
```

### Comparing `deduplicationdict-1.0.0rc2/pyproject.toml` & `deduplicationdict-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,24 @@
 
 [tool.flit.module]
 name = "deduplicationdict"
 
 [tool.setuptools]
 py-modules = ['deduplicationdict']
 
+[tool.setuptools.package-data]
+"deduplicationdict" = ["py.typed"]
+
+[tool.setuptools.packages.find]
+where = ["deduplicationdict"]
+
 [project]
 # $ pip install deduplicationdict
 name = "deduplicationdict"
-version = "1.0.0rc2"
+version = "1.0.1"
 description = "A dictionary that de-duplicates values."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["python", "dict", "deduplication", "optimization", ]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
@@ -106,7 +112,12 @@
 [project.urls]
 "Author" = "https://vivswan.github.io/"
 "Bug Reports" = "https://github.com/Vivswan/DeDuplicationDict/issues"
 "Documentation" = "https://deduplicationdict.readthedocs.io/en/latest/"
 "Homepage" = "https://github.com/Vivswan/DeDuplicationDict"
 "Say Thanks!" = "https://vivswan.github.io/"
 "Source" = "https://github.com/Vivswan/DeDuplicationDict"
+
+# pytest configuration
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "--cov=deduplicationdict --cov-report=xml --cov-report=html"
```

