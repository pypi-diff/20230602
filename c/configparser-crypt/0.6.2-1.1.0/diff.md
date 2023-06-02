# Comparing `tmp/configparser_crypt-0.6.2.tar.gz` & `tmp/configparser_crypt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\configparser_crypt-0.6.2.tar", last modified: Tue Mar 16 14:02:43 2021, max compression
+gzip compressed data, was "configparser_crypt-1.1.0.tar", last modified: Fri Jun  2 15:05:17 2023, max compression
```

## Comparing `configparser_crypt-0.6.2.tar` & `configparser_crypt-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-03-16 14:02:43.854475 configparser_crypt-0.6.2/
--rw-rw-rw-   0        0        0     4183 2021-03-16 14:02:43.852502 configparser_crypt-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2435 2021-03-16 13:53:09.000000 configparser_crypt-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2021-03-16 14:02:43.833553 configparser_crypt-0.6.2/configparser_crypt/
--rw-rw-rw-   0        0        0     7986 2021-03-16 13:31:07.000000 configparser_crypt-0.6.2/configparser_crypt/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-16 14:02:43.849488 configparser_crypt-0.6.2/configparser_crypt.egg-info/
--rw-rw-rw-   0        0        0     4183 2021-03-16 14:02:43.000000 configparser_crypt-0.6.2/configparser_crypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2021-03-16 14:02:43.000000 configparser_crypt-0.6.2/configparser_crypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-16 14:02:43.000000 configparser_crypt-0.6.2/configparser_crypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2021-03-16 14:02:43.000000 configparser_crypt-0.6.2/configparser_crypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2021-03-16 14:02:43.000000 configparser_crypt-0.6.2/configparser_crypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-16 14:02:43.854475 configparser_crypt-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     3688 2021-03-16 13:53:09.000000 configparser_crypt-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:05:17.042210 configparser_crypt-1.1.0/
+-rw-rw-rw-   0        0        0     1590 2022-10-28 09:38:06.000000 configparser_crypt-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7344 2023-06-02 15:05:17.042210 configparser_crypt-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6053 2023-06-01 21:43:07.000000 configparser_crypt-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 15:05:17.031210 configparser_crypt-1.1.0/configparser_crypt/
+-rw-rw-rw-   0        0        0     7792 2023-06-02 15:04:07.000000 configparser_crypt-1.1.0/configparser_crypt/__init__.py
+-rw-rw-rw-   0        0        0     1901 2022-10-28 09:38:06.000000 configparser_crypt-1.1.0/configparser_crypt/dict_convert.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:05:17.040210 configparser_crypt-1.1.0/configparser_crypt.egg-info/
+-rw-rw-rw-   0        0        0     7344 2023-06-02 15:05:16.000000 configparser_crypt-1.1.0/configparser_crypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-02 15:05:16.000000 configparser_crypt-1.1.0/configparser_crypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:05:16.000000 configparser_crypt-1.1.0/configparser_crypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-02 15:05:16.000000 configparser_crypt-1.1.0/configparser_crypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-02 15:05:16.000000 configparser_crypt-1.1.0/configparser_crypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:05:17.042210 configparser_crypt-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3688 2022-10-28 09:38:06.000000 configparser_crypt-1.1.0/setup.py
```

### Comparing `configparser_crypt-0.6.2/configparser_crypt/__init__.py` & `configparser_crypt-1.1.0/configparser_crypt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #! /usr/bin/env python
 #  -*- coding: utf-8 -*-
 
 # This file is part of configparser_crypt package
 
 """
-The configparser_crypt package is a dropin replacement for configparser
+The configparser_crypt package is a drop-in replacement for configparser
 that allows read/write of symmetric encrypted ini files
 """
 
-__intname__ = 'configparser_crypt'
-__author__ = 'Orsiris de Jong'
-__copyright__ = 'Copyright (C) 2016-2020 Orsiris de Jong'
-__description__ = 'Drop-in replacement for ConfigParser with encryption support'
-__licence__ = 'BSD 3 Clause'
-__version__ = '0.6.2'
-__build__ = '2021031601'
+__intname__ = "configparser_crypt"
+__author__ = "Orsiris de Jong"
+__copyright__ = "Copyright (C) 2016-2022 Orsiris de Jong"
+__description__ = "Drop-in replacement for ConfigParser with encryption support"
+__licence__ = "BSD 3 Clause"
+__version__ = "1.1.0"
+__build__ = "2022102801"
+__compat__ = "python3.5+"
 
 import os
 from configparser import ConfigParser
 
 import cryptidy.symmetric_encryption as symmetric_encryption
 from Cryptodome.Random import get_random_bytes
 
@@ -38,66 +39,64 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # By default, configparser sets all strings to lowercase, this option let's keep the case
         self.optionxform = str
-        self.to_write_data = ''
+        self.to_write_data = ""
 
         # AES cypto key with optional added random bytes
         self._aes_key = None
         self._header_length = 0
         self._footer_length = 0
-        self.random_header = get_random_bytes(self._header_length)
-        self.random_footer = get_random_bytes(self._footer_length)
 
     @property
     def aes_key(self):
         return self._aes_key
 
     @aes_key.setter
     def aes_key(self, aes_key):
         if len(aes_key) not in [16, 32]:
-            raise ValueError('AES Key should be 16 or 32 bytes, %s bytes given.' % len(aes_key))
+            raise ValueError(
+                "AES Key should be 16 or 32 bytes, %s bytes given." % len(aes_key)
+            )
         self._aes_key = aes_key
 
     def generate_key(self, size=32):
         """
         Generate a fresh AES 256 bits key by default (32 bytes)
         """
         try:
             self.aes_key = symmetric_encryption.generate_key(size=size)
             return self.aes_key
         except Exception as exc:
-            raise ValueError('Cannot generate AES key: %s' % exc)
+            raise ValueError("Cannot generate AES key: %s" % exc)
 
     @property
     def header_length(self):
         return self._header_length
 
     @header_length.setter
     def header_length(self, value):
         if isinstance(value, int):
-            self.random_header = get_random_bytes(value)
             self._header_length = value
         else:
-            raise ValueError('Header length must be an int')
+            raise ValueError("Header length must be an int")
 
     @property
     def footer_length(self):
         return self._footer_length
 
     @footer_length.setter
     def footer_length(self, value):
         if isinstance(value, int):
-            self.random_footer = get_random_bytes(value)
             self._footer_length = value
         else:
-            raise ValueError('Header length must be an int')
+            raise ValueError("Header length must be an int")
 
     def read_encrypted(self, filenames, encoding=None, aes_key=None):
         """Read and parse a filename or an iterable of filenames.
 
         Files that cannot be opened are silently ignored; this is
         designed so that you can specify an iterable of potential
         configuration file locations (e.g. current directory, user's
@@ -118,15 +117,15 @@
         except AttributeError:
             if isinstance(filenames, str):
                 filenames = [filenames]
 
         read_ok = []
         for filename in filenames:
             try:
-                with open(filename, 'rb') as file_handle:
+                with open(filename, "rb") as file_handle:
                     self._read_encrypted(file_handle, filename, aes_key)
             except OSError:
                 continue
             # Same here, we'll get a AttributeError since os.fspath does not exist in Python 3.5
             # Original ConfigParser did not have that part of the code, let's fallback to ignoring it
             try:
                 if isinstance(filename, os.PathLike):
@@ -134,71 +133,79 @@
             except AttributeError:
                 pass
             read_ok.append(filename)
         return read_ok
 
     def _read_encrypted(self, file_handle, filename, aes_key):
         try:
-
-            if aes_key is not None:
-                _, raw_data = symmetric_encryption.decrypt_message(file_handle.read(), aes_key)
-            elif self.aes_key is not None:
-                _, raw_data = symmetric_encryption.decrypt_message(file_handle.read(), self.aes_key)
-            else:
-                raise ValueError('No aes key provided.')
+            if aes_key is None and self.aes_key is None:
+                raise ValueError("No aes key provided.")
+            if aes_key is None:
+                # on the fly provided aes key has precedence over class aes key
+                aes_key = self.aes_key
+            _, raw_data = symmetric_encryption.decrypt_message_hf(
+                file_handle.read(),
+                aes_key,
+                random_header_len=self._header_length,
+                random_footer_len=self._footer_length,
+            )
+            # Don't keep optional aes_key in memory if not needed
             aes_key = None
-            # Remove extra bytes, decode bytes to string, split into list as if lines were read from file
-            # Don't remove footer when footer len = 0 since the [:footer_len] will result in 0 len
-            if self.footer_length > 0:
-                data = (raw_data[self.header_length:][:-self.footer_length]).decode('utf-8').split('\n')
-            else:
-                data = (raw_data[self.header_length:]).decode('utf-8').split('\n')
+            data = raw_data.decode("utf-8").split("\n")
         except Exception as exc:
-            raise ValueError('Cannot read AES data: %s' % exc)
+            raise ValueError("Cannot read AES data: %s" % exc)
         self._read(data, filename)
 
     def write_encrypted(self, file_handle, space_around_delimiters=True, aes_key=None):
         """Write an .ini-format representation of the configuration state.
 
         If `space_around_delimiters' is True (the default), delimiters
         between keys and values are surrounded by spaces.
         """
 
-        self.to_write_data = ''
+        self.to_write_data = ""
 
         if space_around_delimiters:
             delim = " {} ".format(self._delimiters[0])
         else:
             delim = self._delimiters[0]
         if self._defaults:
-            self._write_section_encrypted(self.default_section, self._defaults.items(), delim)
+            self._write_section_encrypted(
+                self.default_section, self._defaults.items(), delim
+            )
         for section in self._sections:
-            self._write_section_encrypted(section, self._sections[section].items(), delim)
+            self._write_section_encrypted(
+                section, self._sections[section].items(), delim
+            )
 
         self.commit_write(file_handle, aes_key=aes_key)
 
     def _write_section_encrypted(self, section_name, section_items, delimiter):
         """Write a single section to the specified `fp'."""
         self.to_write_data += "[{}]\n".format(section_name)
         for key, value in section_items:
-            value = self._interpolation.before_write(self, section_name, key,
-                                                     value)
+            value = self._interpolation.before_write(self, section_name, key, value)
             if value is not None or not self._allow_no_value:
-                value = delimiter + str(value).replace('\n', '\n\t')
+                value = delimiter + str(value).replace("\n", "\n\t")
             else:
                 value = ""
             self.to_write_data += "{}{}\n".format(key, value)
         self.to_write_data += "\n"
 
     def commit_write(self, file_handle, aes_key=None):
         try:
-            data = self.random_header + self.to_write_data.encode('utf-8') + self.random_footer
-            if aes_key is not None:
-                enc = symmetric_encryption.encrypt_message(data, aes_key)
-            elif self.aes_key is not None:
-                enc = symmetric_encryption.encrypt_message(data, self.aes_key)
-            else:
-                raise ValueError('No AES key provided.')
+            data = self.to_write_data.encode("utf-8")
+            if aes_key is None and self.aes_key is None:
+                raise ValueError("No aes key provided.")
+            if aes_key is None:
+                # on the fly provided aes key has precedence over class aes key
+                aes_key = self.aes_key
+            enc = symmetric_encryption.encrypt_message_hf(
+                data,
+                aes_key,
+                random_header_len=self._header_length,
+                random_footer_len=self._footer_length,
+            )
             aes_key = None
             file_handle.write(enc)
         except Exception as exc:
-            raise ValueError('Cannot write AES data: %s' % exc)
+            raise ValueError("Cannot write AES data: %s" % exc)
```

### Comparing `configparser_crypt-0.6.2/setup.py` & `configparser_crypt-1.1.0/setup.py`

 * *Files identical despite different names*

