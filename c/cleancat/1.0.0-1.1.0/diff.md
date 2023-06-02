# Comparing `tmp/cleancat-1.0.0.tar.gz` & `tmp/cleancat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancat-1.0.0.tar", last modified: Mon Jun 29 17:08:53 2020, max compression
+gzip compressed data, was "cleancat-1.1.0.tar", last modified: Fri Jun  2 07:17:02 2023, max compression
```

## Comparing `cleancat-1.0.0.tar` & `cleancat-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 wojcikstefan   (501) staff       (20)        0 2020-06-29 17:08:53.000000 cleancat-1.0.0/
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      947 2020-06-29 17:08:53.000000 cleancat-1.0.0/PKG-INFO
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      729 2018-07-30 13:56:33.000000 cleancat-1.0.0/README.md
-drwxr-xr-x   0 wojcikstefan   (501) staff       (20)        0 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat/
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      656 2020-06-29 16:20:16.000000 cleancat-1.0.0/cleancat/__init__.py
--rw-r--r--   0 wojcikstefan   (501) staff       (20)    34190 2020-06-29 16:15:39.000000 cleancat-1.0.0/cleancat/base.py
--rw-r--r--   0 wojcikstefan   (501) staff       (20)     2497 2019-10-28 06:38:56.000000 cleancat-1.0.0/cleancat/mongo.py
--rw-r--r--   0 wojcikstefan   (501) staff       (20)     2055 2019-10-28 06:38:56.000000 cleancat-1.0.0/cleancat/sqla.py
-drwxr-xr-x   0 wojcikstefan   (501) staff       (20)        0 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat.egg-info/
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      947 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat.egg-info/PKG-INFO
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      306 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat.egg-info/SOURCES.txt
--rw-r--r--   0 wojcikstefan   (501) staff       (20)        1 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat.egg-info/dependency_links.txt
--rw-r--r--   0 wojcikstefan   (501) staff       (20)        1 2020-06-29 17:03:01.000000 cleancat-1.0.0/cleancat.egg-info/not-zip-safe
--rw-r--r--   0 wojcikstefan   (501) staff       (20)       89 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat.egg-info/requires.txt
--rw-r--r--   0 wojcikstefan   (501) staff       (20)        9 2020-06-29 17:08:53.000000 cleancat-1.0.0/cleancat.egg-info/top_level.txt
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      108 2019-10-28 06:38:56.000000 cleancat-1.0.0/pyproject.toml
--rw-r--r--   0 wojcikstefan   (501) staff       (20)      119 2020-06-29 17:08:53.000000 cleancat-1.0.0/setup.cfg
--rw-r--r--   0 wojcikstefan   (501) staff       (20)     1619 2020-06-29 16:15:39.000000 cleancat-1.0.0/setup.py
+drwxr-xr-x   0 tsx        (501) staff       (20)        0 2023-06-02 07:17:02.444598 cleancat-1.1.0/
+-rw-r--r--   0 tsx        (501) staff       (20)     1094 2023-06-01 11:23:30.000000 cleancat-1.1.0/LICENSE
+-rw-r--r--   0 tsx        (501) staff       (20)      798 2023-06-02 07:17:02.444662 cleancat-1.1.0/PKG-INFO
+-rw-r--r--   0 tsx        (501) staff       (20)      729 2023-06-01 11:23:30.000000 cleancat-1.1.0/README.md
+drwxr-xr-x   0 tsx        (501) staff       (20)        0 2023-06-02 07:17:02.443396 cleancat-1.1.0/cleancat/
+-rw-r--r--   0 tsx        (501) staff       (20)      656 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat/__init__.py
+-rw-r--r--   0 tsx        (501) staff       (20)    34560 2023-06-02 07:14:50.000000 cleancat-1.1.0/cleancat/base.py
+-rw-r--r--   0 tsx        (501) staff       (20)     2490 2023-06-02 07:14:50.000000 cleancat-1.1.0/cleancat/mongo.py
+-rw-r--r--   0 tsx        (501) staff       (20)     2036 2023-06-02 07:14:50.000000 cleancat-1.1.0/cleancat/sqla.py
+drwxr-xr-x   0 tsx        (501) staff       (20)        0 2023-06-02 07:17:02.444097 cleancat-1.1.0/cleancat.egg-info/
+-rw-r--r--   0 tsx        (501) staff       (20)      798 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat.egg-info/PKG-INFO
+-rw-r--r--   0 tsx        (501) staff       (20)      372 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat.egg-info/SOURCES.txt
+-rw-r--r--   0 tsx        (501) staff       (20)        1 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat.egg-info/dependency_links.txt
+-rw-r--r--   0 tsx        (501) staff       (20)        1 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat.egg-info/not-zip-safe
+-rw-r--r--   0 tsx        (501) staff       (20)       89 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat.egg-info/requires.txt
+-rw-r--r--   0 tsx        (501) staff       (20)        9 2023-06-02 07:17:02.000000 cleancat-1.1.0/cleancat.egg-info/top_level.txt
+-rw-r--r--   0 tsx        (501) staff       (20)      309 2023-06-02 07:14:50.000000 cleancat-1.1.0/pyproject.toml
+-rw-r--r--   0 tsx        (501) staff       (20)      119 2023-06-02 07:17:02.444904 cleancat-1.1.0/setup.cfg
+-rw-r--r--   0 tsx        (501) staff       (20)     1454 2023-06-02 07:14:50.000000 cleancat-1.1.0/setup.py
+drwxr-xr-x   0 tsx        (501) staff       (20)        0 2023-06-02 07:17:02.444500 cleancat-1.1.0/tests/
+-rw-r--r--   0 tsx        (501) staff       (20)    40556 2023-06-02 07:14:50.000000 cleancat-1.1.0/tests/test_base.py
+-rw-r--r--   0 tsx        (501) staff       (20)     4364 2023-06-02 07:14:50.000000 cleancat-1.1.0/tests/test_mongo.py
+-rw-r--r--   0 tsx        (501) staff       (20)     3774 2023-06-02 07:14:50.000000 cleancat-1.1.0/tests/test_sqla.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cleancat-1.0.0/README.md` & `cleancat-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cleancat
+CleanCat
 ========
 
 [![Build Status](https://travis-ci.org/closeio/cleancat.svg?branch=master)](https://travis-ci.org/closeio/cleancat)
 
 Validation library for Python designed to be used with JSON REST frameworks
```

### Comparing `cleancat-1.0.0/cleancat/__init__.py` & `cleancat-1.1.0/cleancat/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from cleancat.base import (
+    URL,
     Bool,
     Choices,
     DateTime,
     Dict,
     Email,
     Embedded,
     EmbeddedReference,
@@ -13,35 +14,34 @@
     Regex,
     RelaxedURL,
     Schema,
     SortedSet,
     StopValidation,
     String,
     TrimmedString,
-    URL,
     ValidationError,
 )
 
 __all__ = [
-    'Bool',
-    'Choices',
-    'DateTime',
-    'Dict',
-    'Email',
-    'Embedded',
-    'EmbeddedReference',
-    'Enum',
-    'Field',
-    'Integer',
-    'List',
-    'Regex',
-    'RelaxedURL',
-    'Schema',
-    'SortedSet',
-    'StopValidation',
-    'String',
-    'TrimmedString',
-    'URL',
-    'ValidationError',
+    "Bool",
+    "Choices",
+    "DateTime",
+    "Dict",
+    "Email",
+    "Embedded",
+    "EmbeddedReference",
+    "Enum",
+    "Field",
+    "Integer",
+    "List",
+    "Regex",
+    "RelaxedURL",
+    "Schema",
+    "SortedSet",
+    "StopValidation",
+    "String",
+    "TrimmedString",
+    "URL",
+    "ValidationError",
 ]
 
-__version__ = '1.0.0'
+__version__ = "1.1.0"
```

### Comparing `cleancat-1.0.0/cleancat/base.py` & `cleancat-1.1.0/cleancat/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import datetime
 import inspect
 import re
+from operator import attrgetter
 from uuid import UUID as PythonUUID
 
 import pytz
 from dateutil import parser
 
-
 # Sentinel value which means "pick the default value" when encountered.
 default_sentinel = object()
 
 
 class ValidationError(Exception):
     pass
 
 
 class StopValidation(Exception):
     pass
 
 
-class Field(object):
-
+class Field:
     # If specified, the field ensures that the supplied value is an instance
     # of this type. Can be either a single specific type (e.g. int) or a tuple
     # of multiple types.
     base_type = None
 
     # Value to be used when there was no specific value supplied for this
     # field and the field is not required.
@@ -64,26 +63,26 @@
         if (
             self.base_type is not None
             and value is not None
             and not isinstance(value, self.base_type)
         ):
             if isinstance(self.base_type, tuple):
                 allowed_types = [typ.__name__ for typ in self.base_type]
-                allowed_types_text = ' or '.join(allowed_types)
+                allowed_types_text = " or ".join(allowed_types)
             else:
                 allowed_types_text = self.base_type.__name__
-            err_msg = 'Value must be of %s type.' % allowed_types_text
+            err_msg = "Value must be of %s type." % allowed_types_text
             raise ValidationError(err_msg)
 
         if not self.has_value(value):
             if self.default is not None:
                 raise StopValidation(self.default)
 
             if self.required:
-                raise ValidationError('This field is required.')
+                raise ValidationError("This field is required.")
             else:
                 raise StopValidation(self.blank_value)
 
         return value
 
     def serialize(self, value):
         """
@@ -93,50 +92,50 @@
         might be None.
         """
         return value
 
 
 class String(Field):
     base_type = str
-    blank_value = ''
+    blank_value = ""
     min_length = None
     max_length = None
 
     def __init__(self, min_length=None, max_length=None, **kwargs):
         if min_length is not None:
             self.min_length = min_length
         if max_length is not None:
             self.max_length = max_length
-        super(String, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def _check_length(self, value):
         if self.max_length is not None and len(value) > self.max_length:
-            err_msg = 'The value must be no longer than %s characters.' % (
+            err_msg = "The value must be no longer than %s characters." % (
                 self.max_length
             )
             raise ValidationError(err_msg)
 
         if self.min_length is not None and len(value) < self.min_length:
-            err_msg = 'The value must be at least %s characters long.' % (
+            err_msg = "The value must be at least %s characters long." % (
                 self.min_length
             )
             raise ValidationError(err_msg)
 
     def clean(self, value):
-        value = super(String, self).clean(value)
+        value = super().clean(value)
         self._check_length(value)
         return value
 
     def has_value(self, value):
         return bool(value)
 
 
 class TrimmedString(String):
     base_type = str
-    blank_value = ''
+    blank_value = ""
 
     def clean(self, value):
         # XXX we skip a level of inheritance so that we can perform length
         # checks *after* trimming.
         value = super(String, self).clean(value)
 
         if value:
@@ -152,257 +151,264 @@
     base_type = bool
     blank_value = False
 
 
 class Regex(String):
     regex = None
     regex_flags = 0
-    regex_message = 'Invalid input.'
+    regex_message = "Invalid input."
 
     def __init__(
         self, regex=None, regex_flags=None, regex_message=None, **kwargs
     ):
-        super(Regex, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         if regex is not None:
             self.regex = regex
         if regex_flags is not None:
             self.regex_flags = regex_flags
         if regex_message is not None:
             self.regex_message = regex_message
 
     def get_regex(self):
-        if not getattr(self, '_compiled_regex', None):
+        if not getattr(self, "_compiled_regex", None):
             self._compiled_regex = re.compile(self.regex, self.regex_flags)
         return self._compiled_regex
 
     def clean(self, value):
-        value = super(Regex, self).clean(value)
+        value = super().clean(value)
 
         if not self.get_regex().match(value):
             raise ValidationError(self.regex_message)
 
         return value
 
 
 class DateTime(Regex):
     """ISO 8601 from http://www.pelagodesign.com/blog/2009/05/20/iso-8601-date-validation-that-doesnt-suck/"""
 
     regex = "^([\\+-]?\\d{4}(?!\\d{2}\\b))((-?)((0[1-9]|1[0-2])(\\3([12]\\d|0[1-9]|3[01]))?|W([0-4]\\d|5[0-2])(-?[1-7])?|(00[1-9]|0[1-9]\\d|[12]\\d{2}|3([0-5]\\d|6[1-6])))([T\\s]((([01]\\d|2[0-3])((:?)[0-5]\\d)?|24\\:?00)([\\.,]\\d+(?!:))?)?(\\17[0-5]\\d([\\.,]\\d+)?)?([zZ]|([\\+-])([01]\\d|2[0-3]):?([0-5]\\d)?)?)?)?$"
-    regex_message = 'Invalid ISO 8601 datetime.'
+    regex_message = "Invalid ISO 8601 datetime."
     blank_value = None
+    _force_datetime: bool
 
-    def __init__(self, *args, **kwargs):
-        self.min_date = kwargs.pop('min_date', None)
-        super(DateTime, self).__init__(*args, **kwargs)
+    def __init__(self, *args, force_datetime: bool = False, **kwargs):
+        """
+        Args:
+            force_datetime: If True, always return a datetime object, even if
+                the input does not specify a time.
+        """
+        self.min_date = kwargs.pop("min_date", None)
+        self._force_datetime = force_datetime
+        super().__init__(*args, **kwargs)
 
     def clean(self, value):
         # XXX we're skipping a level of inheritance so that we can reuse
         # the regex match later in this method.
         value = super(Regex, self).clean(value)
         match = self.get_regex().match(value)
         if not match:
             raise ValidationError(self.regex_message)
         try:
             dt = parser.parse(value)
-        except ValueError:
-            raise ValidationError('Could not parse datetime')
+        except ValueError as e:
+            raise ValidationError("Could not parse datetime") from e
         if self.min_date:
             if dt.tzinfo is not None and self.min_date.tzinfo is None:
                 min_date = self.min_date.replace(tzinfo=pytz.utc)
             else:
                 min_date = self.min_date
             if dt < min_date:
-                err_msg = 'Date cannot be earlier than %s.' % (
-                    self.min_date.strftime('%Y-%m-%d')
+                err_msg = "Date cannot be earlier than %s." % (
+                    self.min_date.strftime("%Y-%m-%d")
                 )
                 raise ValidationError(err_msg)
 
+        if self._force_datetime:  # don't convert to a date
+            return dt
+
         time_group = match.groups()[11]
         if time_group and len(time_group) > 1:
             return dt
         return dt.date()
 
     def serialize(self, value):
         if value is not None:
             return value.isoformat()
 
 
 class Email(Regex):
     regex = (
-        r'^(?:[^\.@\s]|[^\.@\s]\.(?!\.))*[^.@\s]@'
-        r'[^.@\s](?:[^\.@\s]|\.(?!\.))*\.[a-z]{2,63}$'
+        r"^(?:[^\.@\s]|[^\.@\s]\.(?!\.))*[^.@\s]@"
+        r"[^.@\s](?:[^\.@\s]|\.(?!\.))*\.[a-z]{2,63}$"
     )
     regex_flags = re.IGNORECASE
-    regex_message = 'Invalid email address.'
+    regex_message = "Invalid email address."
     max_length = 254
 
     def clean(self, value):
         # trim any leading/trailing whitespace before validating the email
         if isinstance(value, str):
             value = value.strip()
-        return super(Email, self).clean(value)
+        return super().clean(value)
 
 
 class URL(Regex):
     blank_value = None
 
     def __init__(
         self,
         require_tld=True,
         default_scheme=None,
         allowed_schemes=None,
         disallowed_schemes=None,
-        **kwargs
+        **kwargs,
     ):
         def normalize_scheme(sch):
-            if sch.endswith('://') or sch.endswith(':'):
+            if sch.endswith(("://", ":")):
                 return sch
-            return sch + '://'
+            return sch + "://"
 
         # FQDN validation similar to https://github.com/chriso/validator.js/blob/master/src/lib/isFQDN.js
 
         # ff01-ff5f -> full-width chars, not allowed
-        alpha_numeric_and_symbols_ranges = u'0-9a-z\u00a1-\uff00\uff5f-\uffff'
+        alpha_numeric_and_symbols_ranges = "0-9a-z\u00a1-\uff00\uff5f-\uffff"
 
         tld_part = (
             require_tld
-            and r'\.[%s-]{2,63}' % alpha_numeric_and_symbols_ranges
-            or ''
+            and r"\.[%s-]{2,63}" % alpha_numeric_and_symbols_ranges
+            or ""
         )
-        scheme_part = '[a-z]+://'
+        scheme_part = "[a-z]+://"
         self.default_scheme = default_scheme
         if self.default_scheme:
             self.default_scheme = normalize_scheme(self.default_scheme)
-        self.scheme_regex = re.compile('^' + scheme_part, re.IGNORECASE)
+        self.scheme_regex = re.compile("^" + scheme_part, re.IGNORECASE)
         if default_scheme:
-            scheme_part = '(%s)?' % scheme_part
-        regex = (
-            r'^%s([-%s@:%%_+.~#?&/\\=]{1,256}%s|([0-9]{1,3}\.){3}[0-9]{1,3})(:[0-9]+)?([/?].*)?$'
-            % (scheme_part, alpha_numeric_and_symbols_ranges, tld_part)
-        )
-        super(URL, self).__init__(
+            scheme_part = "(%s)?" % scheme_part
+        regex = rf"^{scheme_part}([-{alpha_numeric_and_symbols_ranges}@:%_+.~#?&/\\=]{{1,256}}{tld_part}|([0-9]{{1,3}}\.){{3}}[0-9]{{1,3}})(:[0-9]+)?([/?].*)?$"
+        super().__init__(
             regex=regex,
             regex_flags=re.IGNORECASE | re.UNICODE,
-            regex_message='Invalid URL.',
-            **kwargs
+            regex_message="Invalid URL.",
+            **kwargs,
         )
 
         def compile_schemes_to_regexes(schemes):
             return [
-                re.compile('^' + normalize_scheme(sch) + '.*', re.IGNORECASE)
+                re.compile("^" + normalize_scheme(sch) + ".*", re.IGNORECASE)
                 for sch in schemes
             ]
 
         self.allowed_schemes = allowed_schemes or []
         self.allowed_schemes_regexes = compile_schemes_to_regexes(
             self.allowed_schemes
         )
 
         self.disallowed_schemes = disallowed_schemes or []
         self.disallowed_schemes_regexes = compile_schemes_to_regexes(
             self.disallowed_schemes
         )
 
     def clean(self, value):
-        value = super(URL, self).clean(value)
+        value = super().clean(value)
         if not self.scheme_regex.match(value):
             value = self.default_scheme + value
 
-        if self.allowed_schemes:
-            if not any(
-                allowed_regex.match(value)
-                for allowed_regex in self.allowed_schemes_regexes
-            ):
-                allowed_schemes_text = ' or '.join(self.allowed_schemes)
-                err_msg = (
-                    "This URL uses a scheme that's not allowed. You can only "
-                    "use %s." % allowed_schemes_text
-                )
-                raise ValidationError(err_msg)
+        if self.allowed_schemes and not any(
+            allowed_regex.match(value)
+            for allowed_regex in self.allowed_schemes_regexes
+        ):
+            allowed_schemes_text = " or ".join(self.allowed_schemes)
+            err_msg = (
+                "This URL uses a scheme that's not allowed. You can only "
+                "use %s." % allowed_schemes_text
+            )
+            raise ValidationError(err_msg)
 
-        if self.disallowed_schemes:
-            if any(
-                disallowed_regex.match(value)
-                for disallowed_regex in self.disallowed_schemes_regexes
-            ):
-                err_msg = "This URL uses a scheme that's not allowed."
-                raise ValidationError(err_msg)
+        if self.disallowed_schemes and any(
+            disallowed_regex.match(value)
+            for disallowed_regex in self.disallowed_schemes_regexes
+        ):
+            err_msg = "This URL uses a scheme that's not allowed."
+            raise ValidationError(err_msg)
 
         return value
 
 
 class RelaxedURL(URL):
     """Like URL but will just ignore values like "http://" and treat them
     as blank.
     """
 
     def clean(self, value):
         if not self.required and value == self.default_scheme:
             return None
-        value = super(RelaxedURL, self).clean(value)
+        value = super().clean(value)
         return value
 
 
 class Integer(Field):
     base_type = int
 
     def __init__(self, min_value=None, max_value=None, **kwargs):
         self.max_value = max_value
         self.min_value = min_value
-        super(Integer, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def _check_value(self, value):
         if self.max_value is not None and value > self.max_value:
-            err_msg = 'The value must not be larger than %d.' % self.max_value
+            err_msg = "The value must not be larger than %d." % self.max_value
             raise ValidationError(err_msg)
 
         if self.min_value is not None and value < self.min_value:
-            err_msg = 'The value must be at least %d.' % self.min_value
+            err_msg = "The value must be at least %d." % self.min_value
             raise ValidationError(err_msg)
 
     def clean(self, value):
-        value = super(Integer, self).clean(value)
+        value = super().clean(value)
         self._check_value(value)
         return value
 
 
 class List(Field):
     base_type = list
     blank_value = []
 
     def __init__(self, field_instance, max_length=None, **kwargs):
         self.max_length = max_length
-        super(List, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.field_instance = field_instance
 
     def has_value(self, value):
         return bool(value)
 
     def clean(self, value):
-        value = super(List, self).clean(value)
+        value = super().clean(value)
 
         item_cnt = len(value)
         if self.required and not item_cnt:
-            raise ValidationError('List must not be empty.')
+            raise ValidationError("List must not be empty.")
 
         if self.max_length and item_cnt > self.max_length:
-            raise ValidationError('List is too long.')
+            raise ValidationError("List is too long.")
 
         errors = {}
         data = []
         for n, item in enumerate(value):
             try:
                 cleaned_data = self.field_instance.clean(item)
             except ValidationError as e:
                 errors[n] = e.args and e.args[0]
+            except StopValidation as e:
+                data.append(e.args and e.args[0])
             else:
                 data.append(cleaned_data)
 
         if errors:
-            raise ValidationError({'errors': errors})
+            raise ValidationError({"errors": errors})
 
         return data
 
     def serialize(self, value):
         # Serialize all falsy values as an empty list.
         if not value:
             return []
@@ -418,19 +424,19 @@
     def serialize(self, value):
         # Serialize all falsy values as an empty dict.
         return value or {}
 
 
 class Embedded(Dict):
     def __init__(self, schema_class, **kwargs):
-        super(Embedded, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.schema_class = schema_class
 
     def clean(self, value):
-        value = super(Embedded, self).clean(value)
+        value = super().clean(value)
         try:
             cleaned_value = self.schema_class(value).full_clean()
         except ValidationError as e:
             raise e
         else:
             return cleaned_value
 
@@ -456,23 +462,23 @@
 
     This field allows one to submit a dict of values which will then create
     a new instance of the object, or it will update fields of an existing
     object if a field representing its ID (called `pk_field`) was included
     in the submitted dict.
     """
 
-    def __init__(self, object_class, schema_class, pk_field='id', **kwargs):
+    def __init__(self, object_class, schema_class, pk_field="id", **kwargs):
         self.object_class = object_class
         self.schema_class = schema_class
         self.pk_field = pk_field
-        super(EmbeddedReference, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def clean(self, value):
         # Clean the dict first.
-        value = super(EmbeddedReference, self).clean(value)
+        value = super().clean(value)
 
         # Then, depending on whether `pk_field` is in the dict of submitted
         # values or not, update an existing object or create a new one.
         if value and self.pk_field in value:
             return self.clean_existing(value)
         return self.clean_new(value)
 
@@ -493,16 +499,16 @@
     def clean_existing(self, value):
         """Clean the data and return an existing document with its fields
         updated based on the cleaned values.
         """
         existing_pk = value[self.pk_field]
         try:
             obj = self.fetch_existing(existing_pk)
-        except ReferenceNotFoundError:
-            raise ValidationError('Object does not exist.')
+        except ReferenceNotFoundError as e:
+            raise ValidationError("Object does not exist.") from e
         orig_data = self.get_orig_data_from_existing(obj)
 
         # Clean the data (passing the new data dict and the original data to
         # the schema).
         value = self.schema_class(value, orig_data).full_clean()
 
         # Set cleaned data on the object (except for the pk_field).
@@ -552,22 +558,22 @@
     # The ID is assumed to be supplied as a string. However, subclasses can
     # change this field if need be (e.g. it's common for objects persisted in
     # relational databases to use integers as IDs).
     base_type = str
 
     def __init__(self, object_class, **kwargs):
         self.object_class = object_class
-        super(Reference, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def clean(self, value):
-        obj_id = super(Reference, self).clean(value)
+        obj_id = super().clean(value)
         try:
             return self.fetch_object(obj_id)
-        except ReferenceNotFoundError:
-            raise ValidationError('Object does not exist.')
+        except ReferenceNotFoundError as e:
+            raise ValidationError("Object does not exist.") from e
 
     def fetch_object(self, ref_id):
         """Fetch an existing object that corresponds to a given ID.
 
         This needs to be subclassed since, depending on the object class,
         the fetching mechanism might be different. See implementations of
         SQLAReference and MongoReference for a concrete example of fetching
@@ -586,41 +592,41 @@
     """
 
     def __init__(
         self,
         choices,
         case_insensitive=False,
         error_invalid_choice=None,
-        **kwargs
+        **kwargs,
     ):
-        super(Choices, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.choices = choices
         self.case_insensitive = case_insensitive
         self.error_invalid_choice = (
-            error_invalid_choice or 'Not a valid choice.'
+            error_invalid_choice or "Not a valid choice."
         )
 
     def get_choices(self):
         return self.choices
 
     def format_invalid_choice_msg(self, value):
         return self.error_invalid_choice.format(
-            value=value, valid_choices=', '.join(self.get_choices())
+            value=value, valid_choices=", ".join(self.get_choices())
         )
 
     def clean(self, value):
-        value = super(Choices, self).clean(value)
+        value = super().clean(value)
 
         choices = self.get_choices()
 
         if self.case_insensitive:
             choices = {choice.lower(): choice for choice in choices}
 
             if not isinstance(value, str):
-                raise ValidationError(u'Value needs to be a string.')
+                raise ValidationError("Value needs to be a string.")
 
             if value.lower() not in choices:
                 err_msg = self.format_invalid_choice_msg(value)
                 raise ValidationError(err_msg)
 
             return choices[value.lower()]
 
@@ -645,44 +651,44 @@
           more than one choice in this list and *all* of the choices must
           belong to the same enum class.
         """
         is_cls = inspect.isclass(choices)
         if is_cls:
             self.enum_cls = choices
         else:
-            assert choices, 'You need to provide at least one enum choice.'
+            assert choices, "You need to provide at least one enum choice."
             self.enum_cls = choices[0].__class__
-        return super(Enum, self).__init__(choices, **kwargs)
+        super().__init__(choices, **kwargs)
 
     def get_choices(self):
         return [choice.value for choice in self.choices]
 
     def clean(self, value):
-        value = super(Enum, self).clean(value)
+        value = super().clean(value)
         return self.enum_cls(value)
 
     def serialize(self, choice):
         if choice is not None:
             return choice.value
 
 
 class SortedSet(List):
     """Sorted, unique set of values represented as a list."""
 
     def __init__(self, field_instance, max_length=None, key=None, **kwargs):
-        super(SortedSet, self).__init__(field_instance, max_length, **kwargs)
+        super().__init__(field_instance, max_length, **kwargs)
+        if isinstance(field_instance, Enum) and key is None:
+            key = attrgetter("value")
         self.key = key
 
     def clean(self, value):
-        return list(
-            sorted(set(super(SortedSet, self).clean(value)), key=self.key)
-        )
+        return sorted(set(super().clean(value)), key=self.key)
 
 
-class Schema(object):
+class Schema:
     """
     Base Schema class. Provides core behavior like fields declaration
     and construction, validation, and data and error proxying.
 
     There are 3 steps to using a Schema:
 
     1. Define the Schema, e.g.
@@ -766,45 +772,51 @@
             if callable(value):
                 value = value()
             data[field_name] = value
 
         return data
 
     def __init__(self, raw_data=None, data=None):
-        conflicting_fields = set(
-            [
-                'raw_data',
-                'orig_data',
-                'data',
-                'errors',
-                'field_errors',
-                'fields',
-            ]
-        ).intersection(dir(self))
+        conflicting_fields = {
+            "raw_data",
+            "orig_data",
+            "data",
+            "errors",
+            "field_errors",
+            "fields",
+        }.intersection(dir(self))
         if conflicting_fields:
             raise Exception(
-                'The following field names are reserved and need to be renamed: %s. '
-                'Please use the field_name keyword to use them.'
+                "The following field names are reserved and need to be renamed: %s. "
+                "Please use the field_name keyword to use them."
                 % list(conflicting_fields)
             )
 
         self.raw_data = raw_data or {}
         self.orig_data = data or None
         self.data = data and dict(data) or {}
         self.field_errors = {}
         self.errors = []
         self.fields = self.get_fields()
 
     def clean(self):
-        pass
+        """
+        Override to add additional validations.
 
-    def full_clean(self):
+        Always called at the end of `full_clean()` method, even if validation
+        failed for some fields.
+        Cleaned input data are available in `self.data` dict.
+        Keys that failed validation won't be set. Use conditional dictionary
+        access or return early `if self.errors or self.field_errors`.
+        """
+
+    def full_clean(self):  # noqa: C901
         if not isinstance(self.raw_data, dict):
             raise ValidationError(
-                {'errors': ['Invalid request: JSON dictionary expected.']}
+                {"errors": ["Invalid request: JSON dictionary expected."]}
             )
 
         for field_name, field in self.fields.items():
             if field.read_only:
                 continue
             raw_field_name = field.raw_field_name or field_name
             try:
@@ -815,15 +827,14 @@
                 ):
                     value = field.clean(self.raw_data.get(raw_field_name))
                     if (
                         not field.mutable
                         and self.orig_data
                         and field_name in self.orig_data
                     ):
-
                         old_value = self.orig_data[field_name]
 
                         # compare datetimes properly, regardless of whether they're offset-naive or offset-aware
                         if isinstance(value, datetime.datetime) and isinstance(
                             old_value, datetime.datetime
                         ):
                             value = value.replace(tzinfo=None) + (
@@ -832,15 +843,15 @@
                             )
                             old_value = old_value.replace(tzinfo=None) + (
                                 old_value.utcoffset()
                                 or datetime.timedelta(seconds=0)
                             )
 
                         if value != old_value:
-                            raise ValidationError('Value cannot be changed.')
+                            raise ValidationError("Value cannot be changed.")
 
                     self.data[field_name] = value
 
             except ValidationError as e:
                 self.field_errors[raw_field_name] = e.args and e.args[0]
             except StopValidation as e:
                 self.data[field_name] = e.args and e.args[0]
@@ -852,43 +863,43 @@
 
         self.raise_on_errors()
         return self.data
 
     def raise_on_errors(self):
         if self.field_errors or self.errors:
             raise ValidationError(
-                {'field-errors': self.field_errors, 'errors': self.errors}
+                {"field-errors": self.field_errors, "errors": self.errors}
             )
 
     def external_clean(self, cls, raise_on_errors=True):
         try:
             # Instantiate the external schema with the right raw_data/data.
             external_schema = cls(raw_data=self.raw_data, data=self.data)
 
             # Make sure its orig_data is the same as this schema's
             external_schema.orig_data = self.orig_data
 
             # Validate the schema and update self.data with its results.
             self.data.update(external_schema.full_clean())
         except ValidationError as e:
-            self.field_errors.update(e.args[0]['field-errors'])
-            self.errors += e.args[0]['errors']
+            self.field_errors.update(e.args[0]["field-errors"])
+            self.errors += e.args[0]["errors"]
             if raise_on_errors:
                 self.raise_on_errors()
 
     def serialize(self):
         data = {}
         for field_name, field in self.fields.items():
             raw_field_name = field.raw_field_name or field_name
             value = self.data[field_name]
             data[raw_field_name] = field.serialize(value)
         return data
 
 
-DEFAULT_TYPE_FIELD = 'type'
+DEFAULT_TYPE_FIELD = "type"
 
 
 class PolymorphicField(Dict):
     """A field that can be validated with one of multiple schemas,
     depending on type provided in input values.
 
     Requires a dictionary-shaped value.
@@ -905,32 +916,32 @@
     in dispatched schemas' data.
     """
 
     base_type = dict
 
     def __init__(
         self,
-        type_map={},
+        type_map=None,
         type_field=DEFAULT_TYPE_FIELD,
         keep_type_field=False,
         *args,
-        **kwargs
+        **kwargs,
     ):
-        super(PolymorphicField, self).__init__(*args, **kwargs)
-        self.type_map = type_map
+        super().__init__(*args, **kwargs)
+        self.type_map = type_map or {}
         self.type_field = type_field
         self.keep_type_field = keep_type_field
 
     def clean(self, value):
-        clean = super(PolymorphicField, self).clean(value)
+        clean = super().clean(value)
         field_type = clean.get(self.type_field)
         if field_type not in self.type_map:
             raise ValidationError(
-                '{} must be one of {}'.format(
-                    self.type_field, ','.join(self.type_map.keys())
+                "{} must be one of {}".format(
+                    self.type_field, ",".join(self.type_map.keys())
                 )
             )
 
         return self.type_map[field_type].clean(
             {
                 k: v
                 for k, v in value.items()
@@ -945,56 +956,56 @@
     It handles deserialization from a string to a Python UUID object
     and serialization from a Python UUID object to a string.
     """
 
     blank_value = None
 
     def clean(self, value):
-        value = super(UUID, self).clean(value)
+        value = super().clean(value)
         try:
             return PythonUUID(value)
-        except ValueError:
-            raise ValidationError('Not a UUID.')
+        except ValueError as e:
+            raise ValidationError("Not a UUID.") from e
 
     def serialize(self, value):
         return str(value)
 
 
 class CleanDict(Dict):
     """A dictionary in which both keys and values are validated with separate schema fields."""
 
     def __init__(self, key_schema, value_schema, max_length=None, **kwargs):
-        super(CleanDict, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.key_schema = key_schema
         self.value_schema = value_schema
         self.max_length = max_length
 
     def clean(self, value):
-        value = super(CleanDict, self).clean(value)
+        value = super().clean(value)
 
         if self.max_length and len(value) > self.max_length:
-            raise ValidationError('Dict is too long.')
+            raise ValidationError("Dict is too long.")
 
         errors = {}
         data = {}
-        for key, value in value.items():
+        for key, item_value in value.items():
             try:
                 cleaned_key = self.key_schema.clean(key)
             except ValidationError as e:
                 errors[key] = e.args and e.args[0]
             else:
                 try:
-                    cleaned_value = self.value_schema.clean(value)
+                    data[cleaned_key] = self.value_schema.clean(item_value)
                 except ValidationError as e:
                     errors[key] = e.args and e.args[0]
-                else:
-                    data[cleaned_key] = cleaned_value
+                except StopValidation as e:
+                    data[cleaned_key] = e.args and e.args[0]
 
         if errors:
-            raise ValidationError({'errors': errors})
+            raise ValidationError({"errors": errors})
 
         return data
 
     def serialize(self, value):
         # Serialize all falsy values as an empty dict.
         if not value:
             return {}
@@ -1010,21 +1021,21 @@
     It generates the object using provided factory function.
     Kwargs for the factory function is the input dict, validated
     validated with schema_class (from Embedded field).
     """
 
     def __init__(self, factory, *args, **kwargs):
         self.factory = factory
-        super(EmbeddedFactory, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def clean(self, value):
         """Clean the provided dict of values and then return an
         an object created using a factory.
         """
-        value = super(EmbeddedFactory, self).clean(value)
+        value = super().clean(value)
         return self.factory(**value)
 
 
 class LazyField(Field):
     """A field which is instantiated later.
 
     Useful for resolving circular dependencies in code.
```

### Comparing `cleancat-1.0.0/cleancat/mongo.py` & `cleancat-1.1.0/cleancat/mongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     """
     Represents MongoEngine's EmbeddedDocument. Expects the document's
     contents as an input dict.
     """
 
     def __init__(self, document_class=None, *args, **kwargs):
         self.document_class = document_class
-        super(MongoEmbedded, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def clean(self, value):
         """Clean the provided dict of values and then return an
         EmbeddedDocument instantiated with them.
         """
-        value = super(MongoEmbedded, self).clean(value)
+        value = super().clean(value)
         return self.document_class(**value)
 
 
 class MongoEmbeddedReference(EmbeddedReference):
     """
     Represents an embedded reference where the object class is a MongoEngine
     document.
@@ -44,22 +44,22 @@
     {'foo': 'bar'} -> creates a new document instance
     """
 
     def fetch_existing(self, pk):
         doc_cls = self.object_class
         try:
             return doc_cls.objects.get(pk=pk)
-        except doc_cls.DoesNotExist:
-            raise ReferenceNotFoundError
+        except doc_cls.DoesNotExist as e:
+            raise ReferenceNotFoundError from e
         except MongoValidationError as e:
-            raise ValidationError(str(e))
+            raise ValidationError(str(e)) from e
 
     def get_orig_data_from_existing(self, obj):
         # Get a dict of existing document's field names and values.
-        if getattr(obj, 'to_dict', None):
+        if getattr(obj, "to_dict", None):
             # MongoMallard
             return obj.to_dict()
         else:
             # Upstream MongoEngine
             return dict(obj._data)
 
 
@@ -70,13 +70,13 @@
     first).
     """
 
     def fetch_object(self, doc_id):
         """Fetch the document by its PK."""
         try:
             return self.object_class.objects.get(pk=doc_id)
-        except self.object_class.DoesNotExist:
-            raise ReferenceNotFoundError
+        except self.object_class.DoesNotExist as e:
+            raise ReferenceNotFoundError from e
 
     def serialize(self, doc):
         if doc:
             return doc.pk
```

### Comparing `cleancat-1.0.0/cleancat/sqla.py` & `cleancat-1.1.0/cleancat/sqla.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 class SQLAReference(Reference):
     """
     Represents a reference to an SQLAlchemy model. Expects an ID string as
     input and returns a cleaned model instance (verifying that it exists
     first).
     """
 
-    def __init__(self, object_class, pk_field='id', **kwargs):
+    def __init__(self, object_class, pk_field="id", **kwargs):
         self.pk_field = pk_field
-        super(SQLAReference, self).__init__(object_class, **kwargs)
+        super().__init__(object_class, **kwargs)
 
     def fetch_object(self, model_id):
         """Fetch the model by its ID."""
         pk_field_instance = getattr(self.object_class, self.pk_field)
         qs = self.object_class.query.filter(pk_field_instance == model_id)
         model = qs.one_or_none()
         if not model:
```

### Comparing `cleancat-1.0.0/setup.py` & `cleancat-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,46 @@
-import io
 import re
+
 from setuptools import setup
 
-install_requirements = ['python-dateutil', 'pytz']
+install_requirements = ["python-dateutil", "pytz"]
 test_requirements = install_requirements + [
-    'pytest',
-    'coverage',
-    'mongoengine',
-    'sqlalchemy',
+    "pytest",
+    "coverage",
+    "mongoengine",
+    "sqlalchemy",
 ]
 
 VERSION_FILE = "cleancat/__init__.py"
-with io.open(VERSION_FILE, "rt", encoding="utf8") as f:
+with open(VERSION_FILE, encoding="utf8") as f:
     version = re.search(r'__version__ = ([\'"])(.*?)\1', f.read()).group(2)
 
 setup(
-    name='cleancat',
+    name="cleancat",
     version=version,
-    url='http://github.com/elasticsales/cleancat',
-    license='MIT',
-    author='Thomas Steinacher',
-    author_email='engineering@close.io',
-    maintainer='Thomas Steinacher',
-    maintainer_email='engineering@close.io',
-    description='Validation library for Python designed to be used with JSON REST frameworks',
+    url="http://github.com/elasticsales/cleancat",
+    license="MIT",
+    author="Thomas Steinacher",
+    author_email="engineering@close.io",
+    maintainer="Thomas Steinacher",
+    maintainer_email="engineering@close.io",
+    description="Validation library for Python designed to be used with JSON REST frameworks",
     long_description=__doc__,
-    packages=['cleancat'],
+    packages=["cleancat"],
     zip_safe=False,
-    platforms='any',
+    platforms="any",
     install_requires=install_requirements,
-    setup_requires=['pytest-runner'],
-    test_suite='tests',
+    setup_requires=["pytest-runner"],
+    test_suite="tests",
     tests_require=test_requirements,
-    extras_require={'test': test_requirements},
+    extras_require={"test": test_requirements},
     classifiers=[
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Environment :: Web Environment",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

