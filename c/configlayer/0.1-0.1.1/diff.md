# Comparing `tmp/configlayer-0.1.tar.gz` & `tmp/configlayer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configlayer-0.1.tar", last modified: Sun Apr 30 19:58:41 2023, max compression
+gzip compressed data, was "configlayer-0.1.1.tar", last modified: Thu Jun  1 19:00:42 2023, max compression
```

## Comparing `configlayer-0.1.tar` & `configlayer-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 19:58:41.518434 configlayer-0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-25 13:59:31.000000 configlayer-0.1/LICENSE
--rw-rw-rw-   0        0        0     5189 2023-04-30 19:58:41.517435 configlayer-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4573 2023-04-29 20:12:16.000000 configlayer-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 19:58:41.477458 configlayer-0.1/configlayer/
--rw-rw-rw-   0        0        0    12241 2023-04-29 18:03:53.000000 configlayer-0.1/configlayer/__init__.py
--rw-rw-rw-   0        0        0     8406 2023-04-08 11:00:25.000000 configlayer-0.1/configlayer/_config.py
--rw-rw-rw-   0        0        0     4586 2023-04-14 16:18:09.000000 configlayer-0.1/configlayer/_file.py
--rw-rw-rw-   0        0        0    17423 2023-04-12 14:46:06.000000 configlayer-0.1/configlayer/_io.py
--rw-rw-rw-   0        0        0    12616 2023-04-12 12:12:49.000000 configlayer-0.1/configlayer/_profiles.py
--rw-rw-rw-   0        0        0      272 2022-10-16 11:29:22.000000 configlayer-0.1/configlayer/constants.py
--rw-rw-rw-   0        0        0     4592 2023-04-12 14:47:46.000000 configlayer-0.1/configlayer/exceptions.py
--rw-rw-rw-   0        0        0     1917 2023-04-14 15:15:30.000000 configlayer-0.1/configlayer/types.py
--rw-rw-rw-   0        0        0    57123 2023-04-11 12:11:09.000000 configlayer-0.1/configlayer/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 19:58:41.498447 configlayer-0.1/configlayer.egg-info/
--rw-rw-rw-   0        0        0     5189 2023-04-30 19:58:41.000000 configlayer-0.1/configlayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-04-30 19:58:41.000000 configlayer-0.1/configlayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 19:58:41.000000 configlayer-0.1/configlayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 19:58:41.000000 configlayer-0.1/configlayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      695 2023-04-26 12:34:13.000000 configlayer-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 19:58:41.518434 configlayer-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 19:58:41.514437 configlayer-0.1/tests/
--rw-rw-rw-   0        0        0     6243 2023-04-06 16:09:09.000000 configlayer-0.1/tests/test_1_exceptions.py
--rw-rw-rw-   0        0        0    76602 2023-04-05 11:38:59.000000 configlayer-0.1/tests/test_2_utils.py
--rw-rw-rw-   0        0        0     8198 2023-04-12 12:10:55.000000 configlayer-0.1/tests/test_3_main.py
--rw-rw-rw-   0        0        0    12839 2023-04-12 12:10:55.000000 configlayer-0.1/tests/test_4_config.py
--rw-rw-rw-   0        0        0    19814 2023-04-12 12:12:28.000000 configlayer-0.1/tests/test_5_profiles.py
--rw-rw-rw-   0        0        0    32059 2023-04-12 12:10:55.000000 configlayer-0.1/tests/test_6_io.py
--rw-rw-rw-   0        0        0     5904 2023-04-12 09:02:37.000000 configlayer-0.1/tests/test_7_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:42.329370 configlayer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-01 19:00:30.000000 configlayer-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-01 19:00:42.329370 configlayer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-01 19:00:30.000000 configlayer-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:42.329370 configlayer-0.1.1/configlayer/
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55927 2023-06-01 19:00:30.000000 configlayer-0.1.1/configlayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:42.329370 configlayer-0.1.1/configlayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-01 19:00:42.000000 configlayer-0.1.1/configlayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-01 19:00:42.000000 configlayer-0.1.1/configlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:00:42.000000 configlayer-0.1.1/configlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 19:00:42.000000 configlayer-0.1.1/configlayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-01 19:00:30.000000 configlayer-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:00:42.329370 configlayer-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:42.329370 configlayer-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_1_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74953 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_2_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_3_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_4_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19308 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_5_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31241 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_6_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-01 19:00:30.000000 configlayer-0.1.1/tests/test_7_file.py
```

### Comparing `configlayer-0.1/configlayer/__init__.py` & `configlayer-0.1.1/configlayer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,240 +1,241 @@
-"""Config layer main
-    todo: Remove check_type(s) 'obj_t_check' (annotation provided, himself an evil Pinocchio)
-    todo: Rework profiles.active_fields to profiles dict with active fields (and it's set method)
-    todo: Add 'name' param to io.import_section (import single section to config possibility)
-
-    note: Think about pydantic: seems checks can be delegated, and added more possibilities
-    note: Think about fast is_holder - check only __iter__, without __getitem__ iter detection
-
-    note: "type: ignore" (mypy) is better than "typing.cast()", type hinting must stay type hinting
-    note: "bug mypy" is not necessarily a bug, but that's what it's supposed to be
-    note: "noqa" is mostly for silencing pycharm bugs or corrected side effects"""
-from copy import deepcopy
-from weakref import ref
-from dataclasses import replace
-
-from ._config import ConfigSupport, Options
-from ._profiles import Profiles
-from ._io import IO
-from ._file import File
-
-from .types import path_t, Field
-from .utils import (init_reraise, get_attrs, check_type, check_items, check_types, safe, GetName,
-                    split, is_dunder, with_type, as_holder, is_exception)
-from .constants import DEFAULT_SECTION, DEFAULT_ID
-from .exceptions import InternalError, InputError, CheckTypeError, FieldError
-
-
-__all__ = ['ConfigBase', 'LanguageBase', 'Field', 'Options']
-
-
-class ConfigBase:
-    """Config base
-    Must be inherited with providing configuration fields"""
-    cfg: ConfigSupport
-
-    @init_reraise('config', doc=True)
-    def __init__(self, path: path_t | None = None, *,
-                 profiles: bool | None = None, io: bool | None = None, group: str | None = None,
-                 default_section: str = DEFAULT_SECTION, options: Options | None = None,
-                 type_name: str = 'config'):
-        """
-        :arg path:              Current configuration file path to load from or save to
-        :arg profiles:          Enable profiles support for current configuration
-        :arg io:                Enable input/output operations for current configuration
-        :arg group:             Group name for current configuration, if group changes needed
-        :arg default_section:   Default section name for current configuration
-        :arg options:           More precise behavior options for current configuration
-        :arg type_name:         Internal current configuration type name for error message
-        :raise InitError:       If something goes wrong"""
-        _ = GetName(self, doc=True, full=True)
-        _name, name = str(_.attrs.cls), str(_)  # noqa
-
-        # Check that call is inherited
-        if type(self) == ConfigBase:
-            raise InputError(must_be='inherited')
-
-        # Assign or check options
-        if options is None:
-            options = Options()
-        elif not isinstance(options, Options):
-            raise InputError('options', must_be='Options type', received=with_type(options))
-
-        # Assign states of profiles if they are not provided and check bound settings
-        profiles = profiles if profiles is not None else group is not None
-        if group is not None and not profiles:
-            raise InputError('profiles', must_be=f"True or unfilled when {group=!r} provided")
-
-        # Assign states of io if they are not provided and check bound settings
-        io = io if io is not None else path is not None
-        if path is not None and not io:
-            raise InputError('io', must_be=f'True or unfilled when {path=!r} provided')
-
-        # Get fields names with declared types and values, including multiple inherited configs
-        attrs = get_attrs(self, 1, internal=True, dunder=True)  # dunder for merged __annotations__
-        cfg_values = {k: v for k, v in attrs.items() if not is_dunder(k)}
-        cfg_types = attrs.get('__annotations__', {})
-
-        # Check for empty config, reserved 'cfg' field name and that all values/types was provided
-        if not cfg_types and not cfg_values:
-            raise InputError(must_be='at least one field', received='empty config')
-        if 'cfg' in cfg_types | cfg_values:
-            raise InputError('cfg', item_name='field',
-                             reserved="for ConfigSupport structure, use another field name")
-        if cfg_values.keys() != cfg_types.keys():
-            if wrong_names := [x for x in cfg_types if x not in cfg_values and is_dunder(x)]:
-                raise InputError(*wrong_names, item_name='field', dunder='names are forbidden')
-            check_items(cfg_values, cfg_types, 'field', str, input_exc=('',),
-                        extra_template='{} without type: ',
-                        absent_template='{} without factory default: ',
-                        must_be='', received='', fields=cfg_values, types=cfg_types)
-
-        # Prepare fields and default values
-        fields, defaults = {}, {}
-        for k, v in cfg_values.items():
-
-            # Check that field types is actually types, and set info if possibly shadowing detected
-            if isinstance(check_type(t := cfg_types[k], type, raw=True), CheckTypeError):
-                msg = f"Field {k!r} type {with_type(t)} - is not a type"
-                if t == v:
-                    msg += (", and is equal to a value. "
-                            "If shadowing - regular scoping rules applied (cpython issue #98876)")
-                raise InputError(msg=msg)
-
-            # Fill default values for type checking and fields for usage
-            if isinstance(v, Field):
-                defaults[k] = d = deepcopy(v.default)
-                fields[k] = replace(v, default=d, type=t)
-            else:
-                defaults[k] = d = deepcopy(v)
-                fields[k] = Field(d, type=t)
-
-        # Check and set default values
-        self.__dict__ |= check_types(defaults, cfg_types, item_name='field', obj_t_check=False,
-                                     input_exc=('',))
-
-        # Init config support structure with additional functionality (with - unlocks structure)
-        data = ref(self)()
-        with ConfigSupport(data, fields, _name, name, default_section, options, type_name) as cfg:
-            self.cfg, cfg = cfg, ref(cfg)()
-            self.cfg.profiles = Profiles(cfg, data, group) if profiles else None
-            self.cfg.io = IO(cfg, data, fields) if io else None
-            self.cfg.file = File(cfg, path) if path is not None else None
-
-    def __del__(self):
-        """Remove path from used at object deletion by garbage collector
-        Warning: del keyword deletes only link to object from local area, not object itself!"""
-        if (cfg := getattr(self, 'cfg', None)) and (file := getattr(cfg, 'file', None)):
-            file.__del__()
-
-    def __repr__(self):
-        """Class name in code"""
-        return self.cfg._name  # noqa
-
-    def __str__(self):
-        """Config name for user + fields names and values"""
-        return '\n\t'.join((f'{self.cfg.name!r} {self.cfg.type_name}:',
-                            *(f'{k}: {field.type.__name__} = {getattr(self, k)!r}'
-                              for k, field in self.cfg.get_fields.items())))
-
-    def __eq__(self, other):
-        """Only fields compared! Profiles and any other functionalities are ignored!"""
-        if issubclass(type(other), ConfigBase) and self.cfg.get_fields == other.cfg.get_fields:
-            return self.cfg.get_data == other.cfg.get_data
-        return False
-
-    def __set_field__(self, key, value, cfg, field, options, *, check=True, revert=False):
-        if value == DEFAULT_ID:
-            value = field.default
-        elif not revert and check and options.typecheck:
-            value = check_type(value, field.type, options.typecast)
-
-        # Set user default value in default profile if default section is active
-        if profiles := cfg.profiles:
-            if profiles.active == cfg.def_sect:
-                field.default = value
-            if key not in profiles.active_fields:
-                raise FieldError('Set', cfg.name, key, value, getattr(self, key),
-                                 type_name=cfg.type_name,
-                                 reason=f'it is fixed by {profiles.active!r} profile. '
-                                        f'Available fields: {", ".join(profiles.active_fields)}')
-
-        # Get previous and set current value
-        prev_value = getattr(self, key)
-        object.__setattr__(self, key, value)
-
-        # Run on_set handlers
-        errors = []
-        for name, (f_name, run_if_equal, partial_func) in cfg.get_on_set.items():
-            if f_name is None or f_name == key:
-                if run_if_equal or prev_value != value:
-                    if is_exception(error := safe(partial_func, key, prev_value, value)):
-                        errors.append(f'{name!r} handler ({GetName(partial_func.func)}): {error}')
-        errors = '\n\t'.join(('on_set handlers errors:', *errors)) if errors else ''
-
-        # Return revert if called with it (must be only internal call)
-        if revert:
-            return f"Revert completed{f', but {errors}' if errors else ''}"
-
-        # Handle on_set errors
-        if errors:
-            if options.revert_fails:
-                add_msg = self.__set_field__(key, prev_value, cfg, field, options, revert=True)
-            else:
-                add_msg = 'Revert option is disabled - field value is left changed'
-            raise FieldError('Set', cfg.name, key, value, prev_value, type_name=cfg.type_name,
-                             reason=f'{errors}\n{add_msg}', failed=False)
-
-    def __setattr__(self, key, value):
-        """Set field (or attribute if config is not initialized yet)"""
-        # RAW write if ConfigSupport is not inited yet
-        if (cfg := getattr(self, 'cfg', None)) is None:
-            return super().__setattr__(key, value)
-
-        # Check for exists field name
-        if key not in (fields := cfg.get_fields):
-            raise FieldError('Set', cfg.name, key, value, type_name=cfg.type_name,
-                             reason=f"it is not field. Available: {', '.join(fields)}")
-
-        # Set field value
-        self.__set_field__(key, value, cfg, fields[key], cfg.options)
-
-    def __delattr__(self, key):
-        """Clear field (replaces field value to user default)"""
-        cfg = self.cfg
-        if key not in cfg.get_fields:
-            raise FieldError('Delete', cfg.name, key, type_name=cfg.type_name,
-                             reason='it is not field. Attributes cannot be deleted')
-        self.__setattr__(key, DEFAULT_ID)
-
-
-class LanguageBase(ConfigBase):
-    """Language base
-    Must be inherited with providing language str fields"""
-    @init_reraise('language', doc=True)
-    def __init__(self, *args, **kwargs):
-        if type(self) == LanguageBase:
-            raise InputError(must_be='inherited')
-
-        # Get all fields from multiple inherited configs
-        attrs = get_attrs(self, 2, internal=True, dunder=True)  # dunder for merged __annotations__
-
-        # Language fields must not have types provided
-        if cfg_types := attrs.get('__annotations__', {}):
-            msg = 'No need to annotate language fields, only str type allowed'
-            raise InputError(*cfg_types, item_name='field', msg=msg)
-
-        # Force all fields to str type
-        self.__annotations__ = {k: str for k in attrs if not is_dunder(k)}
-
-        # Group is fixed for language config
-        if (group := kwargs.get('group', None)) is not None:
-            raise InputError('group', reserved=f"for LanguageBase ({group!r} will be 'Language')")
-
-        # Init config as language group for synchronized translations changing
-        super().__init__(*args, **kwargs, group='Language', type_name='language')
-
-    def __str__(self):
-        """Language name for user + fields names and values"""
-        return '\n\t'.join((f'{self.cfg.name!r} {self.cfg.type_name}:',
-                            *(f'{k}: {getattr(self, k)!r}' for k in self.cfg.get_fields)))
+"""Config layer main
+    todo: Remove check_type(s) 'obj_t_check' (annotation provided, himself an evil Pinocchio)
+    todo: Rework profiles.active_fields to profiles dict with active fields (and it's set method)
+    todo: Add 'name' param to io.import_section (import single section to config possibility)
+    todo: Reduce complexity (Flake8 C901 error disabled by changing max-complexity from 10 to 20)
+
+    note: Think about pydantic: seems checks can be delegated, and added more possibilities
+    note: Think about fast is_holder - check only __iter__, without __getitem__ iter detection
+
+    note: "type: ignore" (mypy) is better than "typing.cast()", type hinting must stay type hinting
+    note: "bug mypy" is not necessarily a bug, but that's what it's supposed to be
+    note: "noqa" is mostly for silencing pycharm bugs or corrected side effects"""
+from copy import deepcopy
+from weakref import ref
+from dataclasses import replace
+
+from ._config import ConfigSupport, Options
+from ._profiles import Profiles
+from ._io import IO
+from ._file import File
+
+from .types import path_t, Field
+from .utils import (init_reraise, get_attrs, check_type, check_items, check_types, safe, GetName,
+                    is_dunder, with_type, is_exception)
+from .constants import DEFAULT_SECTION, DEFAULT_ID
+from .exceptions import InputError, CheckTypeError, FieldError
+
+
+__all__ = ['ConfigBase', 'LanguageBase', 'Field', 'Options']
+
+
+class ConfigBase:
+    """Config base
+    Must be inherited with providing configuration fields"""
+    cfg: ConfigSupport
+
+    @init_reraise('config', doc=True)
+    def __init__(self, path: path_t | None = None, *,
+                 profiles: bool | None = None, io: bool | None = None, group: str | None = None,
+                 default_section: str = DEFAULT_SECTION, options: Options | None = None,
+                 type_name: str = 'config'):
+        """
+        :arg path:              Current configuration file path to load from or save to
+        :arg profiles:          Enable profiles support for current configuration
+        :arg io:                Enable input/output operations for current configuration
+        :arg group:             Group name for current configuration, if group changes needed
+        :arg default_section:   Default section name for current configuration
+        :arg options:           More precise behavior options for current configuration
+        :arg type_name:         Internal current configuration type name for error message
+        :raise InitError:       If something goes wrong"""
+        _ = GetName(self, doc=True, full=True)
+        _name, name = str(_.attrs.cls), str(_)  # noqa
+
+        # Check that call is inherited
+        if type(self) == ConfigBase:
+            raise InputError(must_be='inherited')
+
+        # Assign or check options
+        if options is None:
+            options = Options()
+        elif not isinstance(options, Options):
+            raise InputError('options', must_be='Options type', received=with_type(options))
+
+        # Assign states of profiles if they are not provided and check bound settings
+        profiles = profiles if profiles is not None else group is not None
+        if group is not None and not profiles:
+            raise InputError('profiles', must_be=f"True or unfilled when {group=!r} provided")
+
+        # Assign states of io if they are not provided and check bound settings
+        io = io if io is not None else path is not None
+        if path is not None and not io:
+            raise InputError('io', must_be=f'True or unfilled when {path=!r} provided')
+
+        # Get fields names with declared types and values, including multiple inherited configs
+        attrs = get_attrs(self, 1, internal=True, dunder=True)  # dunder for merged __annotations__
+        cfg_values = {k: v for k, v in attrs.items() if not is_dunder(k)}
+        cfg_types = attrs.get('__annotations__', {})
+
+        # Check for empty config, reserved 'cfg' field name and that all values/types was provided
+        if not cfg_types and not cfg_values:
+            raise InputError(must_be='at least one field', received='empty config')
+        if 'cfg' in cfg_types | cfg_values:
+            raise InputError('cfg', item_name='field',
+                             reserved="for ConfigSupport structure, use another field name")
+        if cfg_values.keys() != cfg_types.keys():
+            if wrong_names := [x for x in cfg_types if x not in cfg_values and is_dunder(x)]:
+                raise InputError(*wrong_names, item_name='field', dunder='names are forbidden')
+            check_items(cfg_values, cfg_types, 'field', str, input_exc=('',),
+                        extra_template='{} without type: ',
+                        absent_template='{} without factory default: ',
+                        must_be='', received='', fields=cfg_values, types=cfg_types)
+
+        # Prepare fields and default values
+        fields, defaults = {}, {}
+        for k, v in cfg_values.items():
+
+            # Check that field types is actually types, and set info if possibly shadowing detected
+            if isinstance(check_type(t := cfg_types[k], type, raw=True), CheckTypeError):
+                msg = f"Field {k!r} type {with_type(t)} - is not a type"
+                if t == v:
+                    msg += (", and is equal to a value. "
+                            "If shadowing - regular scoping rules applied (cpython issue #98876)")
+                raise InputError(msg=msg)
+
+            # Fill default values for type checking and fields for usage
+            if isinstance(v, Field):
+                defaults[k] = d = deepcopy(v.default)
+                fields[k] = replace(v, default=d, type=t)
+            else:
+                defaults[k] = d = deepcopy(v)
+                fields[k] = Field(d, type=t)
+
+        # Check and set default values
+        self.__dict__ |= check_types(defaults, cfg_types, item_name='field', obj_t_check=False,
+                                     input_exc=('',))
+
+        # Init config support structure with additional functionality (with - unlocks structure)
+        data = ref(self)()
+        with ConfigSupport(data, fields, _name, name, default_section, options, type_name) as cfg:
+            self.cfg, cfg = cfg, ref(cfg)()
+            self.cfg.profiles = Profiles(cfg, data, group) if profiles else None
+            self.cfg.io = IO(cfg, data, fields) if io else None
+            self.cfg.file = File(cfg, path) if path is not None else None
+
+    def __del__(self):
+        """Remove path from used at object deletion by garbage collector
+        Warning: del keyword deletes only link to object from local area, not object itself!"""
+        if (cfg := getattr(self, 'cfg', None)) and (file := getattr(cfg, 'file', None)):
+            file.__del__()
+
+    def __repr__(self):
+        """Class name in code"""
+        return self.cfg._name  # noqa
+
+    def __str__(self):
+        """Config name for user + fields names and values"""
+        return '\n\t'.join((f'{self.cfg.name!r} {self.cfg.type_name}:',
+                            *(f'{k}: {field.type.__name__} = {getattr(self, k)!r}'
+                              for k, field in self.cfg.get_fields.items())))
+
+    def __eq__(self, other):
+        """Only fields compared! Profiles and any other functionalities are ignored!"""
+        if issubclass(type(other), ConfigBase) and self.cfg.get_fields == other.cfg.get_fields:
+            return self.cfg.get_data == other.cfg.get_data
+        return False
+
+    def __set_field__(self, key, value, cfg, field, options, *, check=True, revert=False):
+        if value == DEFAULT_ID:
+            value = field.default
+        elif not revert and check and options.typecheck:
+            value = check_type(value, field.type, options.typecast)
+
+        # Set user default value in default profile if default section is active
+        if profiles := cfg.profiles:
+            if profiles.active == cfg.def_sect:
+                field.default = value
+            if key not in profiles.active_fields:
+                raise FieldError('Set', cfg.name, key, value, getattr(self, key),
+                                 type_name=cfg.type_name,
+                                 reason=f'it is fixed by {profiles.active!r} profile. '
+                                        f'Available fields: {", ".join(profiles.active_fields)}')
+
+        # Get previous and set current value
+        prev_value = getattr(self, key)
+        object.__setattr__(self, key, value)
+
+        # Run on_set handlers
+        errors = []
+        for name, (f_name, run_if_equal, partial_func) in cfg.get_on_set.items():
+            if f_name is None or f_name == key:
+                if run_if_equal or prev_value != value:
+                    if is_exception(error := safe(partial_func, key, prev_value, value)):
+                        errors.append(f'{name!r} handler ({GetName(partial_func.func)}): {error}')
+        errors = '\n\t'.join(('on_set handlers errors:', *errors)) if errors else ''
+
+        # Return revert if called with it (must be only internal call)
+        if revert:
+            return f"Revert completed{f', but {errors}' if errors else ''}"
+
+        # Handle on_set errors
+        if errors:
+            if options.revert_fails:
+                add_msg = self.__set_field__(key, prev_value, cfg, field, options, revert=True)
+            else:
+                add_msg = 'Revert option is disabled - field value is left changed'
+            raise FieldError('Set', cfg.name, key, value, prev_value, type_name=cfg.type_name,
+                             reason=f'{errors}\n{add_msg}', failed=False)
+
+    def __setattr__(self, key, value):
+        """Set field (or attribute if config is not initialized yet)"""
+        # RAW write if ConfigSupport is not inited yet
+        if (cfg := getattr(self, 'cfg', None)) is None:
+            return super().__setattr__(key, value)
+
+        # Check for exists field name
+        if key not in (fields := cfg.get_fields):
+            raise FieldError('Set', cfg.name, key, value, type_name=cfg.type_name,
+                             reason=f"it is not field. Available: {', '.join(fields)}")
+
+        # Set field value
+        self.__set_field__(key, value, cfg, fields[key], cfg.options)
+
+    def __delattr__(self, key):
+        """Clear field (replaces field value to user default)"""
+        cfg = self.cfg
+        if key not in cfg.get_fields:
+            raise FieldError('Delete', cfg.name, key, type_name=cfg.type_name,
+                             reason='it is not field. Attributes cannot be deleted')
+        self.__setattr__(key, DEFAULT_ID)
+
+
+class LanguageBase(ConfigBase):
+    """Language base
+    Must be inherited with providing language str fields"""
+    @init_reraise('language', doc=True)
+    def __init__(self, *args, **kwargs):
+        if type(self) == LanguageBase:
+            raise InputError(must_be='inherited')
+
+        # Get all fields from multiple inherited configs
+        attrs = get_attrs(self, 2, internal=True, dunder=True)  # dunder for merged __annotations__
+
+        # Language fields must not have types provided
+        if cfg_types := attrs.get('__annotations__', {}):
+            msg = 'No need to annotate language fields, only str type allowed'
+            raise InputError(*cfg_types, item_name='field', msg=msg)
+
+        # Force all fields to str type
+        self.__annotations__ = {k: str for k in attrs if not is_dunder(k)}
+
+        # Group is fixed for language config
+        if (group := kwargs.get('group', None)) is not None:
+            raise InputError('group', reserved=f"for LanguageBase ({group!r} will be 'Language')")
+
+        # Init config as language group for synchronized translations changing
+        super().__init__(*args, **kwargs, group='Language', type_name='language')
+
+    def __str__(self):
+        """Language name for user + fields names and values"""
+        return '\n\t'.join((f'{self.cfg.name!r} {self.cfg.type_name}:',
+                            *(f'{k}: {getattr(self, k)!r}' for k in self.cfg.get_fields)))
```

### Comparing `configlayer-0.1/configlayer/_config.py` & `configlayer-0.1.1/configlayer/_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-"""Internal config layer support structure"""
-from types import MappingProxyType
-from typing import Any, Callable
-from functools import partial
-
-from ._profiles import Profiles
-from ._io import IO
-from ._file import File
-
-from .types import fields_t, on_set_t, Field
-from .utils import Locker, check_extra, check_types, set_slots_defaults, fmt_exc
-from .exceptions import OptionsCheckError, InputError
-
-
-_get_raw = object.__getattribute__
-
-
-@set_slots_defaults(fields_t=bool)
-class Options:
-    """Config options defaults
-    There is 2 ways to change it:
-        1. Fill instance and provide it at Config init (options keyword)
-        2. Change in inited config directly (<config_data>.cfg.options.<option_name>)"""
-    typecheck = True        # Check field data for type at each field set
-    typecast = True         # Try to cast type if type check enabled and failed
-    revert_fails = False    # Field value revert if on_set get some error
-
-    def __post_init__(self):
-        if msg := self._check():
-            raise OptionsCheckError(msg)
-
-    def __setattr__(self, key, value, revert=False):
-        if not isinstance(value, bool):
-            raise OptionsCheckError('Options accepting only booleans')
-        if value == (prev_value := getattr(self, key, None)):
-            return
-
-        object.__setattr__(self, key, value)
-        if msg := self._check():
-            if revert:
-                return f'Some options changed in wrong way, check failed: {msg}'
-            msg = f'Set option {key!r} to {value!r} failed: {msg}'
-            if msg2 := self.__setattr__(key, prev_value, revert=True):
-                raise OptionsCheckError(f'{msg}. Revert to {prev_value!r} also failed: {msg2}')
-            raise OptionsCheckError(f'{msg}. Reverted to {prev_value!r} successfully')
-
-    def _check(self):
-        if self.typecast and not self.typecheck:
-            return 'Type checking is disabled, type casting cannot be enabled'
-
-
-class ConfigSupport(Locker):
-    """Config support structure
-    Holds a lot of functionality for config operations"""
-    __slots__ = ('__weakref__', '_data', '_fields', '_on_set', '_name',
-                 'name', 'type_name', 'def_sect', 'options', 'version', 'profiles', 'io', 'file')
-    _data:      Any
-    _fields:    dict[str, Field]
-    _on_set:    dict[str, on_set_t]
-    name:       str
-    type_name:  str
-    def_sect:   str
-    options:    Options
-    version:    None | int
-    profiles:   None | Profiles
-    io:         None | IO
-    file:       None | File
-
-    def __init__(self, data, fields, _name, name, default_section, options, type_name):
-        self._data = data
-        self._fields = fields
-        self._on_set = {}
-        self._name = _name
-        self.name = name
-        self.type_name = type_name
-        self.def_sect = default_section
-        self.options = options
-        self.version = self.profiles = self.io = self.file = None
-
-        # Locks structure for changes with disabling attribute deletion
-        super().__init__(del_attr=False, name=str(self))
-
-    def __repr__(self):
-        return f'{self._name}.cfg'  # noqa
-
-    def __str__(self):
-        return f'{self.name!r} {self.type_name} support structure'
-
-    def add_on_set(self, name: str, field_name: str | None, run_if_equal: bool,
-                   func: Callable, *args, **kwargs):
-        """Add function call on specified or any (if None provided) config field set
-        :arg name:          Handler name
-        :arg field_name:    Field name or None (if all fields handler provided)
-        :arg run_if_equal:  Run handler anyway (if field value is not changed)
-        :arg func:          Handler function
-        :arg args:          :arg func: positional arguments before: key, prev_value, value
-        :arg kwargs:        :arg func: keyword arguments
-        :raise InputError:  If wrong arguments provided"""
-        if name in self._on_set:
-            raise InputError('name', func_name=f'{self!r}.add_on_set()',
-                             msg=f'Cannot add {name!r} handler, it already exists')
-        if field_name is not None and field_name not in self._fields:
-            raise InputError('field_name', func_name=f'{self!r}.add_on_set()',
-                             msg=f'Cannot add {name!r} handler, not exists {field_name = }')
-        self._on_set.update({name: (field_name, run_if_equal, partial(func, *args, **kwargs))})
-
-    def del_on_set(self, name: str):
-        """Delete on_set handler by its name
-        :arg name:  Handler name"""
-        del self._on_set[name]
-
-    @property
-    def get_on_set(self) -> MappingProxyType[str, on_set_t]:
-        """Get exists on_set handlers as a dict view"""
-        return MappingProxyType(self._on_set)
-
-    @property
-    def get_fields(self) -> MappingProxyType[str, Field]:
-        """Get fields descriptors as dict"""
-        return MappingProxyType(self._fields)
-
-    @property
-    def get_data(self) -> fields_t:
-        """Get fields data as dict"""
-        data = self._data
-        return {k: getattr(data, k) for k in self._fields}
-
-    @property
-    def get_changed(self) -> fields_t[bool]:
-        """Get changed fields states as dict"""
-        data = self._data
-        return {k: getattr(data, k) != v.default for k, v in self._fields.items()}
-
-    @property
-    def get_types(self) -> fields_t[type]:
-        """Get fields types as dict"""
-        return {k: v.type for k, v in self._fields.items()}
-
-    @property
-    def get_defaults(self) -> fields_t:
-        """Get fields defaults as dict"""
-        return {k: v.default for k, v in self._fields.items()}
-
-    @property
-    def get_factory_defaults(self) -> fields_t:
-        """Get fields defaults provided at config declaration as dict"""
-        c = type(self._data)
-        return {k: f.default if isinstance(f := getattr(c, k), Field) else f for k in self._fields}
-
-    def _check_fields(self, input_exc, fields: fields_t, types=True, typecast=False):
-        if not fields:
-            raise fmt_exc(input_exc, 'Empty fields provided')
-
-        check_extra(fields, self._fields, 'field', input_exc=input_exc)
-
-        if types:
-            _types = self.get_types
-            # bug mypy: dict[str, type] is type, not str.. and it is also holder_t..
-            return check_types(fields, {k: _types[k] for k in fields}, typecast,                    # type: ignore[misc]
-                               input_exc=input_exc, obj_t_check=False)
-        return fields
-
-    def _set_fields(self, fields: fields_t):
-        data = self._data
-        # bug mypy: return value is not used
-        [setattr(data, k, v) for k, v in fields.items()]                                            # type: ignore[func-returns-value]
-
-    def _set_defaults(self, fields: fields_t):
-        _fields = self._fields
-        # bug mypy: return value is not used
-        [setattr(_fields[k], 'default', v) for k, v in fields.items()]                              # type: ignore[func-returns-value]
-
-    def set_fields(self, fields: fields_t, typecheck=True, typecast=False):
-        """Set current fields by dict with type check and cast possibility
-        :arg fields:        Dict with data to set fields
-        :arg typecheck:     Data types check
-        :arg typecast:      Data types cast (if check failed)
-        :raise InputError:  If wrong arguments provided"""
-        input_exc = (f'{self!r}.set_fields()', 'fields')
-        self._set_fields(self._check_fields(input_exc, fields, typecheck, typecast))
-        if self.profiles:
-            self.profiles.update()
-
-    def set_defaults(self, fields: fields_t, typecheck=True, typecast=False):
-        """Set defaults by dict with type check and cast possibility
-        :arg fields:        Dict with data to set defaults
-        :arg typecheck:     Data types check
-        :arg typecast:      Data types cast (if check failed)
-        :raise InputError:  If wrong arguments provided"""
-        input_exc = (f'{self!r}.set_defaults()', 'fields')
-        fields = self._check_fields(input_exc, fields, typecheck, typecast)
-        if self.profiles and self.profiles.active == self.def_sect:
-            self._set_fields(fields)
-        self._set_defaults(fields)
+"""Internal config layer support structure"""
+from types import MappingProxyType
+from typing import Any, Callable
+from functools import partial
+
+from ._profiles import Profiles
+from ._io import IO
+from ._file import File
+
+from .types import fields_t, on_set_t, Field
+from .utils import Locker, check_extra, check_types, set_slots_defaults, fmt_exc
+from .exceptions import OptionsCheckError, InputError
+
+
+_get_raw = object.__getattribute__
+
+
+@set_slots_defaults(fields_t=bool)
+class Options:
+    """Config options defaults
+    There is 2 ways to change it:
+        1. Fill instance and provide it at Config init (options keyword)
+        2. Change in inited config directly (<config_data>.cfg.options.<option_name>)"""
+    typecheck = True        # Check field data for type at each field set
+    typecast = True         # Try to cast type if type check enabled and failed
+    revert_fails = False    # Field value revert if on_set get some error
+
+    def __post_init__(self):
+        if msg := self._check():
+            raise OptionsCheckError(msg)
+
+    def __setattr__(self, key, value, revert=False):
+        if not isinstance(value, bool):
+            raise OptionsCheckError('Options accepting only booleans')
+        if value == (prev_value := getattr(self, key, None)):
+            return
+
+        object.__setattr__(self, key, value)
+        if msg := self._check():
+            if revert:
+                return f'Some options changed in wrong way, check failed: {msg}'
+            msg = f'Set option {key!r} to {value!r} failed: {msg}'
+            if msg2 := self.__setattr__(key, prev_value, revert=True):
+                raise OptionsCheckError(f'{msg}. Revert to {prev_value!r} also failed: {msg2}')
+            raise OptionsCheckError(f'{msg}. Reverted to {prev_value!r} successfully')
+
+    def _check(self):
+        if self.typecast and not self.typecheck:
+            return 'Type checking is disabled, type casting cannot be enabled'
+
+
+class ConfigSupport(Locker):
+    """Config support structure
+    Holds a lot of functionality for config operations"""
+    __slots__ = ('__weakref__', '_data', '_fields', '_on_set', '_name',
+                 'name', 'type_name', 'def_sect', 'options', 'version', 'profiles', 'io', 'file')
+    _data:      Any
+    _fields:    dict[str, Field]
+    _on_set:    dict[str, on_set_t]
+    name:       str
+    type_name:  str
+    def_sect:   str
+    options:    Options
+    version:    None | int
+    profiles:   None | Profiles
+    io:         None | IO
+    file:       None | File
+
+    def __init__(self, data, fields, _name, name, default_section, options, type_name):
+        self._data = data
+        self._fields = fields
+        self._on_set = {}
+        self._name = _name
+        self.name = name
+        self.type_name = type_name
+        self.def_sect = default_section
+        self.options = options
+        self.version = self.profiles = self.io = self.file = None
+
+        # Locks structure for changes with disabling attribute deletion
+        super().__init__(del_attr=False, name=str(self))
+
+    def __repr__(self):
+        return f'{self._name}.cfg'  # noqa
+
+    def __str__(self):
+        return f'{self.name!r} {self.type_name} support structure'
+
+    def add_on_set(self, name: str, field_name: str | None, run_if_equal: bool,
+                   func: Callable, *args, **kwargs):
+        """Add function call on specified or any (if None provided) config field set
+        :arg name:          Handler name
+        :arg field_name:    Field name or None (if all fields handler provided)
+        :arg run_if_equal:  Run handler anyway (if field value is not changed)
+        :arg func:          Handler function
+        :arg args:          :arg func: positional arguments before: key, prev_value, value
+        :arg kwargs:        :arg func: keyword arguments
+        :raise InputError:  If wrong arguments provided"""
+        if name in self._on_set:
+            raise InputError('name', func_name=f'{self!r}.add_on_set()',
+                             msg=f'Cannot add {name!r} handler, it already exists')
+        if field_name is not None and field_name not in self._fields:
+            raise InputError('field_name', func_name=f'{self!r}.add_on_set()',
+                             msg=f'Cannot add {name!r} handler, not exists {field_name = }')
+        self._on_set.update({name: (field_name, run_if_equal, partial(func, *args, **kwargs))})
+
+    def del_on_set(self, name: str):
+        """Delete on_set handler by its name
+        :arg name:  Handler name"""
+        del self._on_set[name]
+
+    @property
+    def get_on_set(self) -> MappingProxyType[str, on_set_t]:
+        """Get exists on_set handlers as a dict view"""
+        return MappingProxyType(self._on_set)
+
+    @property
+    def get_fields(self) -> MappingProxyType[str, Field]:
+        """Get fields descriptors as dict"""
+        return MappingProxyType(self._fields)
+
+    @property
+    def get_data(self) -> fields_t:
+        """Get fields data as dict"""
+        data = self._data
+        return {k: getattr(data, k) for k in self._fields}
+
+    @property
+    def get_changed(self) -> fields_t[bool]:
+        """Get changed fields states as dict"""
+        data = self._data
+        return {k: getattr(data, k) != v.default for k, v in self._fields.items()}
+
+    @property
+    def get_types(self) -> fields_t[type]:
+        """Get fields types as dict"""
+        return {k: v.type for k, v in self._fields.items()}
+
+    @property
+    def get_defaults(self) -> fields_t:
+        """Get fields defaults as dict"""
+        return {k: v.default for k, v in self._fields.items()}
+
+    @property
+    def get_factory_defaults(self) -> fields_t:
+        """Get fields defaults provided at config declaration as dict"""
+        c = type(self._data)
+        return {k: f.default if isinstance(f := getattr(c, k), Field) else f for k in self._fields}
+
+    def _check_fields(self, input_exc, fields: fields_t, types=True, typecast=False):
+        if not fields:
+            raise fmt_exc(input_exc, 'Empty fields provided')
+
+        check_extra(fields, self._fields, 'field', input_exc=input_exc)
+
+        if types:
+            _types = self.get_types
+            # bug mypy: dict[str, type] is type, not str.. and it is also holder_t..
+            return check_types(fields, {k: _types[k] for k in fields}, typecast,                    # type: ignore[misc]
+                               input_exc=input_exc, obj_t_check=False)
+        return fields
+
+    def _set_fields(self, fields: fields_t):
+        data = self._data
+        # bug mypy: return value is not used
+        [setattr(data, k, v) for k, v in fields.items()]                                     # type: ignore[func-returns-value]
+
+    def _set_defaults(self, fields: fields_t):
+        _fields = self._fields
+        # bug mypy: return value is not used
+        [setattr(_fields[k], 'default', v) for k, v in fields.items()]                       # type: ignore[func-returns-value]
+
+    def set_fields(self, fields: fields_t, typecheck=True, typecast=False):
+        """Set current fields by dict with type check and cast possibility
+        :arg fields:        Dict with data to set fields
+        :arg typecheck:     Data types check
+        :arg typecast:      Data types cast (if check failed)
+        :raise InputError:  If wrong arguments provided"""
+        input_exc = (f'{self!r}.set_fields()', 'fields')
+        self._set_fields(self._check_fields(input_exc, fields, typecheck, typecast))
+        if self.profiles:
+            self.profiles.update()
+
+    def set_defaults(self, fields: fields_t, typecheck=True, typecast=False):
+        """Set defaults by dict with type check and cast possibility
+        :arg fields:        Dict with data to set defaults
+        :arg typecheck:     Data types check
+        :arg typecast:      Data types cast (if check failed)
+        :raise InputError:  If wrong arguments provided"""
+        input_exc = (f'{self!r}.set_defaults()', 'fields')
+        fields = self._check_fields(input_exc, fields, typecheck, typecast)
+        if self.profiles and self.profiles.active == self.def_sect:
+            self._set_fields(fields)
+        self._set_defaults(fields)
```

### Comparing `configlayer-0.1/configlayer/_file.py` & `configlayer-0.1.1/configlayer/_file.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-"""Internal config layer file support structure"""
-from pathlib import Path
-from configparser import ConfigParser
-
-from .utils import Locker
-from .types import path_t, mb_holder_t
-from .exceptions import InitError, FileError
-
-
-class File(Locker):
-    """File optional structure
-    Used in config support structure if file path provided, for local storage of configs"""
-    __slots__ = ('_cfg', 'path')
-    _used_paths: dict = dict()    # Common fixed class variable (dict methods only)
-    path: Path
-
-    def __init__(self, cfg, path: path_t):
-        self._cfg = cfg
-        if (path := Path(path)) in self._used_paths:
-            raise InitError(f'Path "{path}" is already used in {self._used_paths[path]!r} config')
-
-        self.path = path
-        if path.exists():
-            self.load()
-        else:
-            self.save()     # Create "empty" file for path correctness check, folder is not created
-            path.unlink()   # Remove "empty" file
-        self._used_paths[path] = cfg.name
-
-        # Locks structure for changes with disabling attribute deletion
-        super().__init__(del_attr=False)
-
-    def __del__(self):
-        """Remove path from used at config deletion"""
-        if hasattr(self, 'path'):
-            self._used_paths.pop(self.path, None)
-
-    def __repr__(self):
-        return f'{self._cfg!r}.file'
-
-    def __str__(self):
-        return f'{self._cfg.name!r} {self._cfg.type_name} file support structure'
-
-    @staticmethod
-    def _exc(op):
-        def init_wrapper(func):
-            def method_wrapper(self, *args, **kwargs):
-                try:
-                    return func(self, *args, **kwargs)
-                except FileNotFoundError as e:
-                    msg = e.args[1]
-                except FileError as e:
-                    msg = e
-                except Exception as e:
-                    raise FileError(f'{op} "{self.path}" failed. {e!r}') from e
-                raise FileError(f'{op} "{self.path}" failed. {msg}')
-            return method_wrapper
-        return init_wrapper
-
-    def _get_config(self):
-        config = ConfigParser(default_section=f'_{self._cfg.def_sect}')  # hidden reserved name
-        config.optionxform = str
-        return config
-
-    @_exc('Save to')
-    def save(self, sections: mb_holder_t[str] | None = None, *,
-             strict_defaults=False, strict_data=False):
-        """Save config to file (or only selected sections, excepting internal)
-        :arg sections:          Selected section name(s) or all (if not provided)
-        :arg strict_defaults:   Save all fields from default section (not skip equal to factory)
-        :arg strict_data:       Save all fields from data sections (not skip equal to default)
-        :raise InputError:      If wrong arguments provided
-        :raise IOExportError:   If errors during export_config"""
-        config = self._get_config()
-        config.read_dict(self._cfg.io.export_config(sections, strict_defaults=strict_defaults,
-                                                    strict_data=strict_data, typecast=True))
-        with self.path.open('w') as file:
-            config.write(file)
-
-    @_exc('Load from')
-    def load(self, sections: mb_holder_t[str] | None = None):
-        """Load config from file (or only selected sections, excepting internal)
-        :arg sections:          Selected section name(s) or all (if not provided)
-        :raise InputError:      If wrong arguments provided
-        :raise IOImportError:   If errors during import_config
-        :raise FileError:       If file contains forbidden default section"""
-        config = self._get_config()
-        hidden_default_sect = f'_{self._cfg.def_sect}'
-
-        # Raw check for provided real default section (not used due to internal section impact)
-        error = False
-        with self.path.open() as file:
-            config.read_file(file)
-            file.seek(0)
-            for line in file.readlines():
-                if line.startswith(f'[{hidden_default_sect}]'):
-                    error = True
-                    break
-
-        # Process data as dicts and raise an error if real default section provided
-        data = {k: dict(v) for k, v in config.items()}
-        if (wrong := data.pop(hidden_default_sect)) or error:
-            details = f'. Data: {wrong}' if wrong else ''
-            raise FileError(f'{hidden_default_sect!r} section is forbidden, but provided{details}')
-        self._cfg.io.import_config(data, sections)
+"""Internal config layer file support structure"""
+from pathlib import Path
+from configparser import ConfigParser
+
+from .utils import Locker
+from .types import path_t, mb_holder_t
+from .exceptions import InitError, FileError
+
+
+class File(Locker):
+    """File optional structure
+    Used in config support structure if file path provided, for local storage of configs"""
+    __slots__ = ('_cfg', 'path')
+    _used_paths: dict = dict()    # Common fixed class variable (dict methods only)
+    path: Path
+
+    def __init__(self, cfg, path: path_t):
+        self._cfg = cfg
+        if (path := Path(path)) in self._used_paths:
+            raise InitError(f'Path "{path}" is already used in {self._used_paths[path]!r} config')
+
+        self.path = path
+        if path.exists():
+            self.load()
+        else:
+            self.save()     # Create "empty" file for path correctness check, folder is not created
+            path.unlink()   # Remove "empty" file
+        self._used_paths[path] = cfg.name
+
+        # Locks structure for changes with disabling attribute deletion
+        super().__init__(del_attr=False)
+
+    def __del__(self):
+        """Remove path from used at config deletion"""
+        if hasattr(self, 'path'):
+            self._used_paths.pop(self.path, None)
+
+    def __repr__(self):
+        return f'{self._cfg!r}.file'
+
+    def __str__(self):
+        return f'{self._cfg.name!r} {self._cfg.type_name} file support structure'
+
+    @staticmethod
+    def _exc(op):
+        def init_wrapper(func):
+            def method_wrapper(self, *args, **kwargs):
+                try:
+                    return func(self, *args, **kwargs)
+                except FileNotFoundError as e:
+                    msg = e.args[1]
+                except FileError as e:
+                    msg = e
+                except Exception as e:
+                    raise FileError(f'{op} "{self.path}" failed. {e!r}') from e
+                raise FileError(f'{op} "{self.path}" failed. {msg}')
+            return method_wrapper
+        return init_wrapper
+
+    def _get_config(self):
+        config = ConfigParser(default_section=f'_{self._cfg.def_sect}')  # hidden reserved name
+        config.optionxform = str
+        return config
+
+    @_exc('Save to')
+    def save(self, sections: mb_holder_t[str] | None = None, *,
+             strict_defaults=False, strict_data=False):
+        """Save config to file (or only selected sections, excepting internal)
+        :arg sections:          Selected section name(s) or all (if not provided)
+        :arg strict_defaults:   Save all fields from default section (not skip equal to factory)
+        :arg strict_data:       Save all fields from data sections (not skip equal to default)
+        :raise InputError:      If wrong arguments provided
+        :raise IOExportError:   If errors during export_config"""
+        config = self._get_config()
+        config.read_dict(self._cfg.io.export_config(sections, strict_defaults=strict_defaults,
+                                                    strict_data=strict_data, typecast=True))
+        with self.path.open('w') as file:
+            config.write(file)
+
+    @_exc('Load from')
+    def load(self, sections: mb_holder_t[str] | None = None):
+        """Load config from file (or only selected sections, excepting internal)
+        :arg sections:          Selected section name(s) or all (if not provided)
+        :raise InputError:      If wrong arguments provided
+        :raise IOImportError:   If errors during import_config
+        :raise FileError:       If file contains forbidden default section"""
+        config = self._get_config()
+        hidden_default_sect = f'_{self._cfg.def_sect}'
+
+        # Raw check for provided real default section (not used due to internal section impact)
+        error = False
+        with self.path.open() as file:
+            config.read_file(file)
+            file.seek(0)
+            for line in file.readlines():
+                if line.startswith(f'[{hidden_default_sect}]'):
+                    error = True
+                    break
+
+        # Process data as dicts and raise an error if real default section provided
+        data = {k: dict(v) for k, v in config.items()}
+        if (wrong := data.pop(hidden_default_sect)) or error:
+            details = f'. Data: {wrong}' if wrong else ''
+            raise FileError(f'{hidden_default_sect!r} section is forbidden, but provided{details}')
+        self._cfg.io.import_config(data, sections)
```

### Comparing `configlayer-0.1/configlayer/_io.py` & `configlayer-0.1.1/configlayer/_io.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,355 +1,355 @@
-"""Internal config layer IO support structure"""
-from ast import literal_eval
-from typing import Any, Mapping
-
-from .exceptions import CheckValueError, InputError, FieldError, IOExportError, IOImportError
-from .types import mb_holder_t, fields_t, Field
-from .utils import (Locker, GetName, as_holder, check_input, check_extra, check_items, check_type,
-                    with_type, fmt_exc, as_dict)
-
-
-_UNIQUE = object()
-
-
-# Error templates
-_TEMPL_FIELD_DESC = "Field {}={} by {}: {!r}"
-_TEMPL_CONFIG = "Cannot {} {!r} config"
-
-# Exceptions holder
-_EXC_LIST = {'import': IOImportError, 'export': IOExportError}
-
-
-class IO(Locker):
-    """IO optional structure
-    Used in config support structure if enabled, for any IO operations"""
-    __slots__ = ('_cfg', '_data')
-    _key_section = '_CONFIG_LAYER'  # Class constant
-    _key_version = 'version'        # Class constant
-    _key_profile = 'profile'        # Class constant
-    _key_fields = 'fields'          # Class constant
-
-    def __init__(self, cfg, data, fields):
-        self._cfg = cfg
-        self._data = data
-
-        # Config IO check (rewrite to export/import section with all fields)
-        errors = []
-        for name, field in fields.items():
-            exported = self.export_field(name, field.default)
-            imported = self.import_field(name, exported)
-            if field.default != imported:
-                export_func = GetName(field.export_func)
-                import_func = GetName(field.import_func)
-                errors.append(f'Field {name}={with_type(field.default)} must be equal '
-                              f'imported={with_type(imported)}: '
-                              f'{export_func = }, {exported = }, {import_func = }')
-        if errors:
-            raise CheckValueError('\n\t'.join((f'{cfg.name!r} config IO check failed:', *errors)))
-
-        # Locks structure for changes with disabling attribute deletion
-        super().__init__(del_attr=False, name=str(self))
-
-    def __repr__(self):
-        return f'{self._cfg!r}.io'
-
-    def __str__(self):
-        return f'{self._cfg.name!r} {self._cfg.type_name} I/O support structure'
-
-    def _exc(self, op, exc, section=_UNIQUE):
-        section = '' if section == _UNIQUE else f' section {section!r}' if section else ' section'
-        return _EXC_LIST[op](f"{_TEMPL_CONFIG.format(op, self._cfg.name)}{section}. {exc}")
-
-    @staticmethod
-    def _export_field(field: Field, value: str, typecast: bool) -> str:
-        return check_type(field.export_func(value), str, typecast, 'field', False)
-
-    def export_field(self, name: str, value: Any = None, typecast=True) -> str:
-        """Export single field to raw str type
-        :arg name:          Field name
-        :arg value:         Field value (if override needed)
-        :arg typecast:      Force str type if field export_func result is not str
-        :return:            Field raw value
-        :raise FieldError:  Any error"""
-        field = None
-        try:
-            field = self._cfg.get_fields[name]
-            value = getattr(self._data, name) if value is None else value
-            return self._export_field(field, value, typecast)
-        except Exception as e:
-            kw = {} if field is None else {'by_func': GetName(field.export_func, code=True)}
-            kw |= {} if value is None else {'from_value': value}
-            raise FieldError('Export', self._cfg.name, name, **kw, type_name=self._cfg.type_name,
-                             reason=repr(e)) from e
-
-    def export_section(self, section: str | fields_t | None = None, strict=False, typecast=True
-                       ) -> fields_t[str]:
-        """Export single section to dict with raw str type values
-        :arg section:           Section name, fields dict, or active section (if not provided)
-        :arg strict:            Export all fields (not skip equal to default)
-        :arg typecast:          Force str type if field export_func result is not str
-        :return:                Fields raw values
-        :raise InputError:      If wrong arguments provided
-        :raise IOExportError:   Any other error"""
-        cfg = self._cfg
-        profiles = cfg.profiles
-        fields = cfg.get_fields
-        active_fields = tuple(fields)
-        name, section = (section, None) if isinstance(section, str) else (None, section)
-        ie = (f'{self!r}.export_section()', 'section')
-
-        try:
-            # Provided section select
-            if section is not None:
-                check_type(section, Mapping, input_exc=ie)
-                check_extra(section, fields, 'field', input_exc=ie)
-                items, defaults = section, cfg.get_defaults
-
-            # Internal section direct export
-            elif name == self._key_section:
-                support = {}
-                if cfg.version:
-                    support[self._key_version] = repr(cfg.version)
-                if profiles:
-                    support[self._key_profile] = repr(profiles.active)
-                    if fields := {k: tuple(v) for k, v in profiles.get.items()
-                                  if isinstance(v, dict)}:
-                        support[self._key_fields] = repr(fields)
-                return support
-
-            # Default section select
-            elif (name == cfg.def_sect or
-                  name is None and profiles and profiles.active == cfg.def_sect):
-                name, items, defaults = cfg.def_sect, cfg.get_defaults, cfg.get_factory_defaults
-
-            # Profile section select
-            elif profiles:
-                if name is None:
-                    name = profiles.active
-                elif name not in profiles:
-                    p = ", ".join(map(repr, profiles.get))
-                    details = f'available profiles: {p}' if p else 'there is no profiles'
-                    raise fmt_exc(ie, f'Profile is not exists, {details}')
-                items, defaults = as_dict(profiles[name], fields), cfg.get_defaults
-                active_fields = tuple(items)
-
-            # Config section select
-            else:
-                if name is None or name == cfg.name:
-                    name, items, defaults = cfg.name, cfg.get_data, cfg.get_defaults
-                else:
-                    raise fmt_exc(ie, must_be=repr(cfg.name), received=repr(name))
-
-            # Export section
-            _export = self._export_field
-            result, errors = {}, []
-            for key, field in fields.items():
-                default = defaults[key]
-                value = items.get(key, default)
-                if key in active_fields and strict or value != default:
-                    try:
-                        result[key] = _export(field, value, typecast)
-                    except Exception as e:
-                        fn = GetName(field.export_func, code=True)
-                        errors.append(_TEMPL_FIELD_DESC.format(key, with_type(value), fn, e))
-            if errors:
-                raise CheckValueError('\n\t'.join(('Errors:', *errors)))
-            return result
-
-        except InputError:
-            raise
-        except CheckValueError as e:
-            raise self._exc('export', str(e), name)
-        except Exception as e:
-            raise self._exc('export', repr(e), name) from e  # not tested extreme case exception
-
-    def export_config(self, sections: mb_holder_t[str] | None = None, *, strict_defaults=False,
-                      strict_data=False, typecast=True) -> dict[str, fields_t[str]]:
-        """Export whole config or specified profile(s) (if profiles enabled).
-        Also, by defaults, export only changed by user default and data fields
-        :arg sections:          Selected section name(s) or all (if not provided)
-        :arg strict_defaults:   Export all fields from default section (not skip equal to factory)
-        :arg strict_data:       Export all fields from data sections (not skip equal to default)
-        :arg typecast:          Force str type if field export_func result is not str
-        :return:                Sections with fields raw values
-        :raise InputError:      If wrong arguments provided
-        :raise IOExportError:   Any other error"""
-        cfg = self._cfg
-        ie = (f'{self!r}.export_config()', 'profiles')
-        try:
-            result = {}
-            if sections is not None and cfg.profiles is None:
-                raise fmt_exc(ie, f'Profiles disabled, but provided: {sections!r}')
-
-            # Export config support fields
-            if support := self.export_section(self._key_section):
-                result[self._key_section] = support
-
-            # Export config defaults
-            cds = cfg.def_sect
-            result[cds] = self.export_section(cds, strict=strict_defaults, typecast=typecast)
-
-            # Export config data
-            if cfg.profiles:
-                exists = cfg.profiles.get
-                # bug mypy: profiles cannot be None here
-                if (selected := as_holder(sections, exists)) != exists:                             # type: ignore[arg-type]
-                    check_extra(selected, exists, 'profile', input_exc=ie)
-                # bug mypy: k cannot be None here
-                result |= {k: self.export_section(k, strict=strict_data, typecast=typecast)         # type: ignore[misc]
-                           for k in selected}
-            else:
-                result[cfg.name] = self.export_section(strict=strict_data, typecast=typecast)
-            return result
-
-        except (InputError, IOExportError):
-            raise
-        except Exception as e:
-            raise self._exc('export', repr(e)) from e  # not tested extreme case exception
-
-    @staticmethod
-    def _import_field(field: Field, raw_value: str, typecast: bool) -> Any:
-        return check_type(field.import_func(raw_value), field.type, typecast, 'field', False)
-
-    def import_field(self, name: str, raw_value: str, typecast=True) -> Any:
-        """Import single field to field type
-        :arg name:          Field name
-        :arg raw_value:     Field raw value
-        :arg typecast:      Force field type if field import_func result has any other type
-        :return:            Field value
-        :raise FieldError:  Any error"""
-        try:
-            return self._import_field(self._cfg.get_fields[name], raw_value, typecast)
-        except Exception as e:
-            field = self._cfg.get_fields.get(name, None)
-            kwargs = {} if field is None else {'by_func': GetName(field.import_func, code=True)}
-            raise FieldError('Import', self._cfg.name, name, from_value=raw_value, **kwargs,
-                             type_name=self._cfg.type_name, reason=repr(e)) from e
-
-    def import_section(self, raw_section: fields_t[str], name: str | None = None, typecast=True
-                       ) -> fields_t:
-        """Import single section to dict with fields values
-        note: Import section directly into the config is not available and may not be!
-        :arg raw_section:       Fields raw values
-        :arg name:              Section name (only for error message)
-        :arg typecast:          Force field type if field import_func result has any other type
-        :return:                Fields values
-        :raise InputError:      If wrong arguments provided
-        :raise IOImportError:   Any other error"""
-        cfg = self._cfg
-        fields = cfg.get_fields
-        ie = (f'{self!r}.import_section()', 'raw_section')
-        check_type(raw_section, Mapping, input_exc=ie)
-        check_extra(raw_section, fields, 'field', input_exc=ie)
-        try:
-            result, errors = {}, []
-            _import = self._import_field
-            for key, raw_value in raw_section.items():
-                field = fields[key]
-                try:
-                    result[key] = _import(field, raw_value, typecast)
-                except Exception as e:
-                    fn = GetName(field.import_func, code=True)
-                    errors.append(_TEMPL_FIELD_DESC.format(key, with_type(raw_value), fn, e))
-            if errors:
-                raise CheckValueError("\n\t".join(('Errors:', *errors)))
-            return result
-
-        except CheckValueError as e:
-            raise self._exc('import', str(e), name)
-        except Exception as e:
-            raise self._exc('import', repr(e), name) from e  # not tested extreme case exception
-
-    def import_config(self, raw_config: Mapping[str, fields_t[str]],
-                      sections: mb_holder_t[str] | None = None, typecast=True):
-        """Import whole config, or specified section(s) from it
-        :arg raw_config:        Sections with fields raw values
-        :arg sections:          Selected section name(s) to import or all (if not provided)
-        :arg typecast:          Force field type if field import_func result has any other type
-        :return:                Sections with fields values
-        :raise InputError:      If wrong arguments provided
-        :raise IOImportError:   Any other error"""
-        cfg = self._cfg
-        def_sect = cfg.def_sect
-        profiles = cfg.profiles
-        fields = tuple(cfg.get_fields)
-        ie_func = f'{self!r}.import_config()'
-        ie_cfg = (ie_func, 'raw_config')
-        ie_sect = (ie_func, 'sections')
-        try:
-            raw_config = dict(raw_config)
-
-            # Import config support structure fields
-            active = None
-            active_fields = {}
-            support = raw_config.pop(self._key_section, None)
-            check_input(support, cfg.version or profiles, f'{self._key_section!r} section',
-                        input_exc=ie_cfg)
-            if support is not None:
-                version = support.get(self._key_version)
-                if version:
-                    version = str(literal_eval(version))
-                if check_input(version, cfg.version, 'version', input_exc=ie_cfg):
-                    raise NotImplementedError('Version import is not available yet')
-
-                active = support.get(self._key_profile)
-                if active:
-                    active = str(literal_eval(active))
-                if check_input(active, profiles, 'profile', input_exc=ie_cfg):
-                    if active not in raw_config and active != def_sect:
-                        raise fmt_exc(ie_cfg, f'Active profile is not provided: {active!r}')
-
-                    if self._key_fields in support:
-                        active_fields_raw = support[self._key_fields]
-                        try:
-                            active_fields = dict(literal_eval(active_fields_raw))
-                        except Exception as e:
-                            raise fmt_exc(ie_cfg, 'Active fields dict is not parsed: '
-                                                  f'{active_fields_raw!r}') from e
-                        check_extra(active_fields, raw_config, 'active fields profile',
-                                    input_exc=ie_cfg)
-                        [check_extra(v, fields, f'{k!r} profile active field', input_exc=ie_cfg)
-                         for k, v in active_fields.items()]
-
-            # Check sections
-            if sections:
-                sections = as_holder(sections)
-                if profiles:
-                    selected = tuple(raw_config)
-                else:
-                    selected = ((def_sect,) if def_sect in raw_config else ()) + (cfg.name,)
-                check_extra(sections, selected, 'section', input_exc=ie_sect)
-                raw_config = {k: raw_config[k] for k in sections}
-
-            # Import defaults
-            if defaults := raw_config.pop(def_sect, {}):
-                check_extra(defaults, fields, 'default field', input_exc=ie_cfg)
-                defaults = self.import_section(defaults, def_sect, typecast)
-            defaults = cfg.get_factory_defaults | defaults
-
-            # Import data
-            profiles_data = {}
-            if profiles:
-                for k, v in raw_config.items():
-                    p_data = self.import_section(v, k, typecast)
-                    if af := active_fields.get(k):
-                        check_items(p_data, af, f'{k!r} profile field', input_exc=ie_cfg)
-                        profiles_data[k] = {k: v for k, v in p_data.items() if k in af}
-                    else:
-                        profiles_data[k] = defaults | p_data
-            else:
-                data = defaults | self.import_section(raw_config[cfg.name], cfg.name, typecast)
-
-            # Apply successfully imported data
-            cfg.set_defaults(defaults, typecheck=False)
-            if profiles:
-                profiles.clear()
-                [profiles.set(name, profile, defaults=False, typecheck=False)
-                 for name, profile in profiles_data.items()]
-                profiles.switch(active)
-            else:
-                cfg._set_fields(data)   # noqa
-
-        except (InputError, IOImportError):
-            raise
-        except Exception as e:
-            raise self._exc('import', repr(e)) from e
+"""Internal config layer IO support structure"""
+from ast import literal_eval
+from typing import Any, Mapping
+
+from .exceptions import CheckValueError, InputError, FieldError, IOExportError, IOImportError
+from .types import mb_holder_t, fields_t, Field
+from .utils import (Locker, GetName, as_holder, check_input, check_extra, check_items, check_type,
+                    with_type, fmt_exc, as_dict)
+
+
+_UNIQUE = object()
+
+
+# Error templates
+_TEMPL_FIELD_DESC = "Field {}={} by {}: {!r}"
+_TEMPL_CONFIG = "Cannot {} {!r} config"
+
+# Exceptions holder
+_EXC_LIST = {'import': IOImportError, 'export': IOExportError}
+
+
+class IO(Locker):
+    """IO optional structure
+    Used in config support structure if enabled, for any IO operations"""
+    __slots__ = ('_cfg', '_data')
+    _key_section = '_CONFIG_LAYER'  # Class constant
+    _key_version = 'version'        # Class constant
+    _key_profile = 'profile'        # Class constant
+    _key_fields = 'fields'          # Class constant
+
+    def __init__(self, cfg, data, fields):
+        self._cfg = cfg
+        self._data = data
+
+        # Config IO check (rewrite to export/import section with all fields)
+        errors = []
+        for name, field in fields.items():
+            exported = self.export_field(name, field.default)
+            imported = self.import_field(name, exported)
+            if field.default != imported:
+                export_func = GetName(field.export_func)
+                import_func = GetName(field.import_func)
+                errors.append(f'Field {name}={with_type(field.default)} must be equal '
+                              f'imported={with_type(imported)}: '
+                              f'{export_func = }, {exported = }, {import_func = }')
+        if errors:
+            raise CheckValueError('\n\t'.join((f'{cfg.name!r} config IO check failed:', *errors)))
+
+        # Locks structure for changes with disabling attribute deletion
+        super().__init__(del_attr=False, name=str(self))
+
+    def __repr__(self):
+        return f'{self._cfg!r}.io'
+
+    def __str__(self):
+        return f'{self._cfg.name!r} {self._cfg.type_name} I/O support structure'
+
+    def _exc(self, op, exc, section=_UNIQUE):
+        section = '' if section == _UNIQUE else f' section {section!r}' if section else ' section'
+        return _EXC_LIST[op](f"{_TEMPL_CONFIG.format(op, self._cfg.name)}{section}. {exc}")
+
+    @staticmethod
+    def _export_field(field: Field, value: str, typecast: bool) -> str:
+        return check_type(field.export_func(value), str, typecast, 'field', False)
+
+    def export_field(self, name: str, value: Any = None, typecast=True) -> str:
+        """Export single field to raw str type
+        :arg name:          Field name
+        :arg value:         Field value (if override needed)
+        :arg typecast:      Force str type if field export_func result is not str
+        :return:            Field raw value
+        :raise FieldError:  Any error"""
+        field = None
+        try:
+            field = self._cfg.get_fields[name]
+            value = getattr(self._data, name) if value is None else value
+            return self._export_field(field, value, typecast)
+        except Exception as e:
+            kw = {} if field is None else {'by_func': GetName(field.export_func, code=True)}
+            kw |= {} if value is None else {'from_value': value}
+            raise FieldError('Export', self._cfg.name, name, **kw, type_name=self._cfg.type_name,
+                             reason=repr(e)) from e
+
+    def export_section(self, section: str | fields_t | None = None, strict=False, typecast=True
+                       ) -> fields_t[str]:
+        """Export single section to dict with raw str type values
+        :arg section:           Section name, fields dict, or active section (if not provided)
+        :arg strict:            Export all fields (not skip equal to default)
+        :arg typecast:          Force str type if field export_func result is not str
+        :return:                Fields raw values
+        :raise InputError:      If wrong arguments provided
+        :raise IOExportError:   Any other error"""
+        cfg = self._cfg
+        profiles = cfg.profiles
+        fields = cfg.get_fields
+        active_fields = tuple(fields)
+        name, section = (section, None) if isinstance(section, str) else (None, section)
+        ie = (f'{self!r}.export_section()', 'section')
+
+        try:
+            # Provided section select
+            if section is not None:
+                check_type(section, Mapping, input_exc=ie)
+                check_extra(section, fields, 'field', input_exc=ie)
+                items, defaults = section, cfg.get_defaults
+
+            # Internal section direct export
+            elif name == self._key_section:
+                support = {}
+                if cfg.version:
+                    support[self._key_version] = repr(cfg.version)
+                if profiles:
+                    support[self._key_profile] = repr(profiles.active)
+                    if fields := {k: tuple(v) for k, v in profiles.get.items()
+                                  if isinstance(v, dict)}:
+                        support[self._key_fields] = repr(fields)
+                return support
+
+            # Default section select
+            elif (name == cfg.def_sect or
+                  name is None and profiles and profiles.active == cfg.def_sect):
+                name, items, defaults = cfg.def_sect, cfg.get_defaults, cfg.get_factory_defaults
+
+            # Profile section select
+            elif profiles:
+                if name is None:
+                    name = profiles.active
+                elif name not in profiles:
+                    p = ", ".join(map(repr, profiles.get))
+                    details = f'available profiles: {p}' if p else 'there is no profiles'
+                    raise fmt_exc(ie, f'Profile is not exists, {details}')
+                items, defaults = as_dict(profiles[name], fields), cfg.get_defaults
+                active_fields = tuple(items)
+
+            # Config section select
+            else:
+                if name is None or name == cfg.name:
+                    name, items, defaults = cfg.name, cfg.get_data, cfg.get_defaults
+                else:
+                    raise fmt_exc(ie, must_be=repr(cfg.name), received=repr(name))
+
+            # Export section
+            _export = self._export_field
+            result, errors = {}, []
+            for key, field in fields.items():
+                default = defaults[key]
+                value = items.get(key, default)
+                if key in active_fields and strict or value != default:
+                    try:
+                        result[key] = _export(field, value, typecast)
+                    except Exception as e:
+                        fn = GetName(field.export_func, code=True)
+                        errors.append(_TEMPL_FIELD_DESC.format(key, with_type(value), fn, e))
+            if errors:
+                raise CheckValueError('\n\t'.join(('Errors:', *errors)))
+            return result
+
+        except InputError:
+            raise
+        except CheckValueError as e:
+            raise self._exc('export', str(e), name)
+        except Exception as e:
+            raise self._exc('export', repr(e), name) from e  # not tested extreme case exception
+
+    def export_config(self, sections: mb_holder_t[str] | None = None, *, strict_defaults=False,
+                      strict_data=False, typecast=True) -> dict[str, fields_t[str]]:
+        """Export whole config or specified profile(s) (if profiles enabled).
+        Also, by defaults, export only changed by user default and data fields
+        :arg sections:          Selected section name(s) or all (if not provided)
+        :arg strict_defaults:   Export all fields from default section (not skip equal to factory)
+        :arg strict_data:       Export all fields from data sections (not skip equal to default)
+        :arg typecast:          Force str type if field export_func result is not str
+        :return:                Sections with fields raw values
+        :raise InputError:      If wrong arguments provided
+        :raise IOExportError:   Any other error"""
+        cfg = self._cfg
+        ie = (f'{self!r}.export_config()', 'profiles')
+        try:
+            result = {}
+            if sections is not None and cfg.profiles is None:
+                raise fmt_exc(ie, f'Profiles disabled, but provided: {sections!r}')
+
+            # Export config support fields
+            if support := self.export_section(self._key_section):
+                result[self._key_section] = support
+
+            # Export config defaults
+            cds = cfg.def_sect
+            result[cds] = self.export_section(cds, strict=strict_defaults, typecast=typecast)
+
+            # Export config data
+            if cfg.profiles:
+                exists = cfg.profiles.get
+                # bug mypy: profiles cannot be None here
+                if (selected := as_holder(sections, exists)) != exists:                             # type: ignore[arg-type]
+                    check_extra(selected, exists, 'profile', input_exc=ie)
+                # bug mypy: k cannot be None here
+                result |= {k: self.export_section(k, strict=strict_data, typecast=typecast)         # type: ignore[misc]
+                           for k in selected}
+            else:
+                result[cfg.name] = self.export_section(strict=strict_data, typecast=typecast)
+            return result
+
+        except (InputError, IOExportError):
+            raise
+        except Exception as e:
+            raise self._exc('export', repr(e)) from e  # not tested extreme case exception
+
+    @staticmethod
+    def _import_field(field: Field, raw_value: str, typecast: bool) -> Any:
+        return check_type(field.import_func(raw_value), field.type, typecast, 'field', False)
+
+    def import_field(self, name: str, raw_value: str, typecast=True) -> Any:
+        """Import single field to field type
+        :arg name:          Field name
+        :arg raw_value:     Field raw value
+        :arg typecast:      Force field type if field import_func result has any other type
+        :return:            Field value
+        :raise FieldError:  Any error"""
+        try:
+            return self._import_field(self._cfg.get_fields[name], raw_value, typecast)
+        except Exception as e:
+            field = self._cfg.get_fields.get(name, None)
+            kwargs = {} if field is None else {'by_func': GetName(field.import_func, code=True)}
+            raise FieldError('Import', self._cfg.name, name, from_value=raw_value, **kwargs,
+                             type_name=self._cfg.type_name, reason=repr(e)) from e
+
+    def import_section(self, raw_section: fields_t[str], name: str | None = None, typecast=True
+                       ) -> fields_t:
+        """Import single section to dict with fields values
+        note: Import section directly into the config is not available and may not be!
+        :arg raw_section:       Fields raw values
+        :arg name:              Section name (only for error message)
+        :arg typecast:          Force field type if field import_func result has any other type
+        :return:                Fields values
+        :raise InputError:      If wrong arguments provided
+        :raise IOImportError:   Any other error"""
+        cfg = self._cfg
+        fields = cfg.get_fields
+        ie = (f'{self!r}.import_section()', 'raw_section')
+        check_type(raw_section, Mapping, input_exc=ie)
+        check_extra(raw_section, fields, 'field', input_exc=ie)
+        try:
+            result, errors = {}, []
+            _import = self._import_field
+            for key, raw_value in raw_section.items():
+                field = fields[key]
+                try:
+                    result[key] = _import(field, raw_value, typecast)
+                except Exception as e:
+                    fn = GetName(field.import_func, code=True)
+                    errors.append(_TEMPL_FIELD_DESC.format(key, with_type(raw_value), fn, e))
+            if errors:
+                raise CheckValueError("\n\t".join(('Errors:', *errors)))
+            return result
+
+        except CheckValueError as e:
+            raise self._exc('import', str(e), name)
+        except Exception as e:
+            raise self._exc('import', repr(e), name) from e  # not tested extreme case exception
+
+    def import_config(self, raw_config: Mapping[str, fields_t[str]],
+                      sections: mb_holder_t[str] | None = None, typecast=True):
+        """Import whole config, or specified section(s) from it
+        :arg raw_config:        Sections with fields raw values
+        :arg sections:          Selected section name(s) to import or all (if not provided)
+        :arg typecast:          Force field type if field import_func result has any other type
+        :return:                Sections with fields values
+        :raise InputError:      If wrong arguments provided
+        :raise IOImportError:   Any other error"""
+        cfg = self._cfg
+        def_sect = cfg.def_sect
+        profiles = cfg.profiles
+        fields = tuple(cfg.get_fields)
+        ie_func = f'{self!r}.import_config()'
+        ie_cfg = (ie_func, 'raw_config')
+        ie_sect = (ie_func, 'sections')
+        try:
+            raw_config = dict(raw_config)
+
+            # Import config support structure fields
+            active = None
+            active_fields = {}
+            support = raw_config.pop(self._key_section, None)
+            check_input(support, cfg.version or profiles, f'{self._key_section!r} section',
+                        input_exc=ie_cfg)
+            if support is not None:
+                version = support.get(self._key_version)
+                if version:
+                    version = str(literal_eval(version))
+                if check_input(version, cfg.version, 'version', input_exc=ie_cfg):
+                    raise NotImplementedError('Version import is not available yet')
+
+                active = support.get(self._key_profile)
+                if active:
+                    active = str(literal_eval(active))
+                if check_input(active, profiles, 'profile', input_exc=ie_cfg):
+                    if active not in raw_config and active != def_sect:
+                        raise fmt_exc(ie_cfg, f'Active profile is not provided: {active!r}')
+
+                    if self._key_fields in support:
+                        active_fields_raw = support[self._key_fields]
+                        try:
+                            active_fields = dict(literal_eval(active_fields_raw))
+                        except Exception as e:
+                            raise fmt_exc(ie_cfg, 'Active fields dict is not parsed: '
+                                                  f'{active_fields_raw!r}') from e
+                        check_extra(active_fields, raw_config, 'active fields profile',
+                                    input_exc=ie_cfg)
+                        [check_extra(v, fields, f'{k!r} profile active field', input_exc=ie_cfg)
+                         for k, v in active_fields.items()]
+
+            # Check sections
+            if sections:
+                sections = as_holder(sections)
+                if profiles:
+                    selected = tuple(raw_config)
+                else:
+                    selected = ((def_sect,) if def_sect in raw_config else ()) + (cfg.name,)
+                check_extra(sections, selected, 'section', input_exc=ie_sect)
+                raw_config = {k: raw_config[k] for k in sections}
+
+            # Import defaults
+            if defaults := raw_config.pop(def_sect, {}):
+                check_extra(defaults, fields, 'default field', input_exc=ie_cfg)
+                defaults = self.import_section(defaults, def_sect, typecast)
+            defaults = cfg.get_factory_defaults | defaults
+
+            # Import data
+            profiles_data = {}
+            if profiles:
+                for k, v in raw_config.items():
+                    p_data = self.import_section(v, k, typecast)
+                    if af := active_fields.get(k):
+                        check_items(p_data, af, f'{k!r} profile field', input_exc=ie_cfg)
+                        profiles_data[k] = {k: v for k, v in p_data.items() if k in af}
+                    else:
+                        profiles_data[k] = defaults | p_data
+            else:
+                data = defaults | self.import_section(raw_config[cfg.name], cfg.name, typecast)
+
+            # Apply successfully imported data
+            cfg.set_defaults(defaults, typecheck=False)
+            if profiles:
+                profiles.clear()
+                [profiles.set(name, profile, defaults=False, typecheck=False)
+                 for name, profile in profiles_data.items()]
+                profiles.switch(active)
+            else:
+                cfg._set_fields(data)   # noqa
+
+        except (InputError, IOImportError):
+            raise
+        except Exception as e:
+            raise self._exc('import', repr(e)) from e
```

### Comparing `configlayer-0.1/configlayer/_profiles.py` & `configlayer-0.1.1/configlayer/_profiles.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-"""Internal config layer profiles support structure"""
-from __future__ import annotations
-
-from copy import deepcopy
-from types import MappingProxyType
-from typing import Any, Optional, Callable, Iterable
-
-from .types import fields_t
-from .utils import Locker, check_items, check_types, as_dict_stated, check_lengths, fmt_exc
-from .exceptions import InputError, ProfilesError
-
-
-class Profiles(Locker):
-    """Profiles optional structure
-    Used in config support structure if enabled, for config profiles operations"""
-    __slots__ = ('_cfg', '_data', '_profiles', '_group', 'active', 'active_fields',
-                 'before_switch', 'after_switch')
-    _groups: dict[str, list[Profiles]] = dict()  # Common fixed class variable (dict methods only)
-    _cfg: Any
-    _data: Any
-    _profiles: dict[str, tuple | dict]
-    _group: str | None
-    active: str
-    active_fields: tuple
-    before_switch: Optional[Callable]
-    after_switch: Optional[Callable]
-
-    def __init__(self, cfg, data, group: str | None = None):
-        self._cfg = cfg
-        self._data = data
-        self._profiles = {}
-        self._group = group
-        self.before_switch = self.after_switch = None
-        self.active = cfg.def_sect
-        self.active_fields = tuple(cfg.get_fields)
-        if group is not None:
-            if group in self._groups:
-                curr_group = self._groups[group]
-                if (curr_active := curr_group[0].active) != self.active:
-                    next(self._switch(curr_active, True, False))
-                curr_group.append(self)
-            else:
-                self._groups[group] = [self]
-
-        # Locks structure for changes with disabling attribute deletion and unlocked switch funcs
-        super().__init__('before_switch', 'after_switch', del_attr=False, name=str(self))
-
-    def __repr__(self):
-        return f'{self._cfg!r}.profiles'
-
-    def __str__(self):
-        return f'{self._cfg.name!r} {self._cfg.type_name} profiles support structure'
-
-    def __contains__(self, key):
-        return self._profiles.__contains__(key)
-
-    def __getitem__(self, key):
-        cfg = self._cfg
-        if key == cfg.def_sect:
-            return tuple(cfg.get_defaults.values())
-        if key == self.active:
-            self.update()
-        return self._profiles[key]
-
-    def __delitem__(self, key):
-        if key == self.active:
-            if len(self._profiles) > 1:
-                indexed = tuple(self._profiles)
-                new_key = indexed[1 if (new := indexed.index(key)) == 0 else (new - 1)]  # -> or <-
-            else:
-                new_key = self._cfg.def_sect
-            self.switch(new_key)
-        del self._profiles[key]
-
-    def clear(self):
-        """Delete all profiles"""
-        if self.active != (default := self._cfg.def_sect):
-            self.switch(default)
-        self._profiles.clear()
-
-    @property
-    def get(self) -> MappingProxyType[str, Any]:
-        """Get profiles dict view"""
-        self.update()
-        return MappingProxyType(self._profiles)
-
-    def set(self, name: str, data: fields_t | Iterable = (), *,
-            defaults=True, typecheck=True, typecast=False):
-        """Set profile data by name, with optional defaults filling, type checking and casting
-        :arg name:              Target profile name
-        :arg data:              Target profile data
-        :arg defaults:          Fill missing fields by defaults and store strictly as tuple
-        :arg typecheck:         Data types check
-        :arg typecast:          Data types cast (if check failed)
-        :raise InputError:      If wrong arguments provided
-        :raise ProfilesError:   Any other error"""
-        cfg = self._cfg
-        fields = cfg.get_fields
-        default_profile = name == cfg.def_sect
-        func_name = f'{self!r}.set()'
-        try:
-            if data:
-                mapping, items = as_dict_stated(data, fields)
-                if not mapping:
-                    check_lengths(tuple(data), fields, absent=False, input_exc=(func_name, 'data'))
-                check_items(items, fields, 'field', str, absent=not (defaults or mapping),
-                            input_exc=(func_name, 'data'))
-                if typecheck:
-                    items = check_types(items, {k: fields[k].type for k in items}, typecast,
-                                        input_exc=(func_name, 'data'))
-                if defaults:
-                    items = cfg.get_defaults | items
-            elif default_profile:
-                raise InputError('data', func_name=func_name,
-                                 msg='Cannot overwrite profile defaults with empty data')
-            elif not defaults:
-                raise InputError('data', func_name=func_name,
-                                 msg='Cannot set profile with empty data and disabled defaults')
-            else:
-                items = cfg.get_defaults
-
-            if default_profile:
-                cfg.set_defaults(items)
-            else:
-                result = tuple(items.values()) if len(fields) == len(items) else items
-                # bug mypy: no Sequence type, tuple or fields_t in previous line
-                self._profiles[name] = deepcopy(result)                                             # type: ignore[assignment]
-                if name == self.active:
-                    with self:
-                        self.active_fields = tuple(items)
-                    cfg.set_fields(items)
-
-        except InputError:
-            raise
-        except Exception as e:
-            raise ProfilesError(f'Cannot set {name!r} profile to {cfg.name!r} config') from e
-
-    def update(self):
-        """Copy current config values to active profile. Used in self.switch() or manually"""
-        cfg = self._cfg
-        if self.active == cfg.def_sect:
-            return  # Realized faster and automatically in ConfigBase.__set_field__
-
-        data = cfg.get_data
-        if len(profile := self._profiles[self.active]) != len(cfg.get_fields):
-            self._profiles[self.active] = {k: data[k] for k in profile}
-        else:
-            self._profiles[self.active] = tuple(data.values())
-
-    def _name_error(self, input_exc, name):
-        return fmt_exc(input_exc, f'{name!r} profile in {self._cfg.name!r} config is not exists',
-                       available=tuple(self._profiles))
-
-    def _group_call(self, func_name: str, *args, revert=True):
-        processed, errors = [], []
-        # note mypy: self._group is not None if _group_call called
-        for profile in self._groups[self._group]:                                                   # type: ignore[index]
-            try:
-                next(gen := getattr(profile, func_name)(*args))
-                processed.append((profile._cfg.name, gen))
-            except StopIteration:
-                continue
-            except Exception as e:
-                errors.append(f'{profile._cfg.name}: {e!r}')
-        if not errors:
-            return
-
-        # Prepare error message
-        msg = '\n\t'.join((f'Some profiles in group {self._group!r} failed ' + '{}:', *errors))
-        if not revert:
-            return msg + '\nRevert disabled'
-
-        # Revert processed profiles
-        errors = []
-        for profile_name, yielded in processed:
-            try:
-                next(yielded)
-            except StopIteration:
-                continue
-            except Exception as e:
-                errors.append(f'{profile_name}: {e!r}')
-        return msg + '\nRevert ' + ('\n\t'.join(('failed:', *errors)) if errors else 'successful')
-
-    def _rename_raw(self, new_name, old_name):
-        if old_name == self.active:
-            self.active = new_name
-        self._profiles = {new_name if k == old_name else k: v for k, v in self._profiles.items()}
-
-    def _rename(self, new_name, old_name):
-        if old_name not in self._profiles:
-            raise self._name_error((f'{self!r}.rename()', 'old_name'), old_name)
-        with self:
-            try:
-                self._rename_raw(new_name, old_name)
-            except Exception:
-                self._rename_raw(old_name, new_name)
-                raise
-            yield
-            return self._rename_raw(old_name, new_name)
-
-    def rename(self, new_name: str, old_name: str | None = None):
-        """Rename active or selected profile. Profiles in groups will also be renamed
-        :arg new_name:          New profile name
-        :arg old_name:          Target, or active (if not provided) profile name
-        :raise InputError:      If wrong arguments provided
-        :raise ProfilesError:   If any error at group operations"""
-        # Check input
-        if old_name is None:
-            old_name = self.active
-        if old_name == self._cfg.def_sect:
-            raise InputError(msg=f'Cannot rename default profile to {new_name!r}',
-                             func_name=f'{self!r}.rename()')
-
-        # Single config profile rename
-        if self._group is None:
-            return next(self._rename(new_name, old_name))
-
-        # Group configs profile rename
-        if error := self._group_call('_rename', new_name, old_name):
-            raise ProfilesError(error.format(f'rename from {old_name!r} to {new_name!r}'))
-
-    def _switch_raw(self, name, cfg, data):
-        if self.before_switch is not None:
-            self.before_switch()
-
-        fields = cfg.get_fields
-        mapping, data_dict = as_dict_stated(self[name], fields, strict=True)
-        with self:
-            self.active = name
-            self.active_fields = tuple(data_dict if mapping else fields)
-        [setattr(data, *kv) for kv in data_dict.items()]
-
-        if self.after_switch is not None:
-            self.after_switch()
-
-    def _switch_check(self, name, add, cfg):
-        if (absent := name not in self and name != cfg.def_sect) and not add:
-            raise self._name_error((f'{self!r}.switch()', 'name'), name)
-        return absent
-
-    def _switch(self, name, add, add_current, absent=None):
-        cfg = self._cfg
-        if (prev_name := self.active) == name:
-            yield
-            return
-
-        # Check input and add data from default or current profile if enabled and profile is absent
-        if absent is None:
-            absent = self._switch_check(name, add, cfg)
-        if absent and add:
-            self.set(name, self.get[prev_name] if add_current else None, typecheck=False)
-
-        # Save current profile values and switch with revert at fail
-        self.update()
-        try:
-            self._switch_raw(name, cfg, self._data)
-        except Exception:
-            self._switch_raw(prev_name, cfg, self._data)
-            raise
-        yield
-        return self._switch_raw(prev_name, cfg, self._data)
-
-    def switch(self, name: str, add=False, add_current=False):
-        """Switch active profile. Profiles in groups will also be switched
-        :arg name:              Exists or new profile name (if :arg add: enabled)
-        :arg add:               Adds profile with provided :arg name: if it not exists
-        :arg add_current:       Replaces defaults with the active profile values, when it is added
-        :raise InputError:      If wrong arguments provided
-        :raise ProfilesError:   If any error at group operations"""
-        # Check input
-        if add_current and not add:
-            raise InputError('add', 'add_current',
-                             msg="Param 'add' must be True, when 'add_current' is True")
-        absent = self._switch_check(name, add, self._cfg)
-
-        # Single config profile switch
-        if self._group is None:
-            return next(self._switch(name, add, add_current, absent))
-
-        # Group configs profile switch
-        if error := self._group_call('_switch', name, add, add_current):
-            raise ProfilesError(error.format(f'switch to {name!r}'))
-
-    @property
-    def get_groups(self) -> MappingProxyType[str, Any]:
-        """Get groups dict view"""
-        return MappingProxyType(self._groups)
-
-    def del_group(self, name: str) -> list | None:
-        """Delete provided group name
-        :arg name:          Deleting group name
-        :return:            List of deleted group config profiles
-        :raise KeyError:    If :arg name: is not exists"""
-        return self._groups.pop(name)
+"""Internal config layer profiles support structure"""
+from __future__ import annotations
+
+from copy import deepcopy
+from types import MappingProxyType
+from typing import Any, Optional, Callable, Iterable
+
+from .types import fields_t
+from .utils import Locker, check_items, check_types, as_dict_stated, check_lengths, fmt_exc
+from .exceptions import InputError, ProfilesError
+
+
+class Profiles(Locker):
+    """Profiles optional structure
+    Used in config support structure if enabled, for config profiles operations"""
+    __slots__ = ('_cfg', '_data', '_profiles', '_group', 'active', 'active_fields',
+                 'before_switch', 'after_switch')
+    _groups: dict[str, list[Profiles]] = dict()  # Common fixed class variable (dict methods only)
+    _cfg: Any
+    _data: Any
+    _profiles: dict[str, tuple | dict]
+    _group: str | None
+    active: str
+    active_fields: tuple
+    before_switch: Optional[Callable]
+    after_switch: Optional[Callable]
+
+    def __init__(self, cfg, data, group: str | None = None):
+        self._cfg = cfg
+        self._data = data
+        self._profiles = {}
+        self._group = group
+        self.before_switch = self.after_switch = None
+        self.active = cfg.def_sect
+        self.active_fields = tuple(cfg.get_fields)
+        if group is not None:
+            if group in self._groups:
+                curr_group = self._groups[group]
+                if (curr_active := curr_group[0].active) != self.active:
+                    next(self._switch(curr_active, True, False))
+                curr_group.append(self)
+            else:
+                self._groups[group] = [self]
+
+        # Locks structure for changes with disabling attribute deletion and unlocked switch funcs
+        super().__init__('before_switch', 'after_switch', del_attr=False, name=str(self))
+
+    def __repr__(self):
+        return f'{self._cfg!r}.profiles'
+
+    def __str__(self):
+        return f'{self._cfg.name!r} {self._cfg.type_name} profiles support structure'
+
+    def __contains__(self, key):
+        return self._profiles.__contains__(key)
+
+    def __getitem__(self, key):
+        cfg = self._cfg
+        if key == cfg.def_sect:
+            return tuple(cfg.get_defaults.values())
+        if key == self.active:
+            self.update()
+        return self._profiles[key]
+
+    def __delitem__(self, key):
+        if key == self.active:
+            if len(self._profiles) > 1:
+                indexed = tuple(self._profiles)
+                new_key = indexed[1 if (new := indexed.index(key)) == 0 else (new - 1)]  # -> or <-
+            else:
+                new_key = self._cfg.def_sect
+            self.switch(new_key)
+        del self._profiles[key]
+
+    def clear(self):
+        """Delete all profiles"""
+        if self.active != (default := self._cfg.def_sect):
+            self.switch(default)
+        self._profiles.clear()
+
+    @property
+    def get(self) -> MappingProxyType[str, Any]:
+        """Get profiles dict view"""
+        self.update()
+        return MappingProxyType(self._profiles)
+
+    def set(self, name: str, data: fields_t | Iterable = (), *,
+            defaults=True, typecheck=True, typecast=False):
+        """Set profile data by name, with optional defaults filling, type checking and casting
+        :arg name:              Target profile name
+        :arg data:              Target profile data
+        :arg defaults:          Fill missing fields by defaults and store strictly as tuple
+        :arg typecheck:         Data types check
+        :arg typecast:          Data types cast (if check failed)
+        :raise InputError:      If wrong arguments provided
+        :raise ProfilesError:   Any other error"""
+        cfg = self._cfg
+        fields = cfg.get_fields
+        default_profile = name == cfg.def_sect
+        func_name = f'{self!r}.set()'
+        try:
+            if data:
+                mapping, items = as_dict_stated(data, fields)
+                if not mapping:
+                    check_lengths(tuple(data), fields, absent=False, input_exc=(func_name, 'data'))
+                check_items(items, fields, 'field', str, absent=not (defaults or mapping),
+                            input_exc=(func_name, 'data'))
+                if typecheck:
+                    items = check_types(items, {k: fields[k].type for k in items}, typecast,
+                                        input_exc=(func_name, 'data'))
+                if defaults:
+                    items = cfg.get_defaults | items
+            elif default_profile:
+                raise InputError('data', func_name=func_name,
+                                 msg='Cannot overwrite profile defaults with empty data')
+            elif not defaults:
+                raise InputError('data', func_name=func_name,
+                                 msg='Cannot set profile with empty data and disabled defaults')
+            else:
+                items = cfg.get_defaults
+
+            if default_profile:
+                cfg.set_defaults(items)
+            else:
+                result = tuple(items.values()) if len(fields) == len(items) else items
+                # bug mypy: no Sequence type, tuple or fields_t in previous line
+                self._profiles[name] = deepcopy(result)                                             # type: ignore[assignment]
+                if name == self.active:
+                    with self:
+                        self.active_fields = tuple(items)
+                    cfg.set_fields(items)
+
+        except InputError:
+            raise
+        except Exception as e:
+            raise ProfilesError(f'Cannot set {name!r} profile to {cfg.name!r} config') from e
+
+    def update(self):
+        """Copy current config values to active profile. Used in self.switch() or manually"""
+        cfg = self._cfg
+        if self.active == cfg.def_sect:
+            return  # Realized faster and automatically in ConfigBase.__set_field__
+
+        data = cfg.get_data
+        if len(profile := self._profiles[self.active]) != len(cfg.get_fields):
+            self._profiles[self.active] = {k: data[k] for k in profile}
+        else:
+            self._profiles[self.active] = tuple(data.values())
+
+    def _name_error(self, input_exc, name):
+        return fmt_exc(input_exc, f'{name!r} profile in {self._cfg.name!r} config is not exists',
+                       available=tuple(self._profiles))
+
+    def _group_call(self, func_name: str, *args, revert=True):
+        processed, errors = [], []
+        # note mypy: self._group is not None if _group_call called
+        for profile in self._groups[self._group]:                                                   # type: ignore[index]
+            try:
+                next(gen := getattr(profile, func_name)(*args))
+                processed.append((profile._cfg.name, gen))
+            except StopIteration:
+                continue
+            except Exception as e:
+                errors.append(f'{profile._cfg.name}: {e!r}')
+        if not errors:
+            return
+
+        # Prepare error message
+        msg = '\n\t'.join((f'Some profiles in group {self._group!r} failed ' + '{}:', *errors))
+        if not revert:
+            return msg + '\nRevert disabled'
+
+        # Revert processed profiles
+        errors = []
+        for profile_name, yielded in processed:
+            try:
+                next(yielded)
+            except StopIteration:
+                continue
+            except Exception as e:
+                errors.append(f'{profile_name}: {e!r}')
+        return msg + '\nRevert ' + ('\n\t'.join(('failed:', *errors)) if errors else 'successful')
+
+    def _rename_raw(self, new_name, old_name):
+        if old_name == self.active:
+            self.active = new_name
+        self._profiles = {new_name if k == old_name else k: v for k, v in self._profiles.items()}
+
+    def _rename(self, new_name, old_name):
+        if old_name not in self._profiles:
+            raise self._name_error((f'{self!r}.rename()', 'old_name'), old_name)
+        with self:
+            try:
+                self._rename_raw(new_name, old_name)
+            except Exception:
+                self._rename_raw(old_name, new_name)
+                raise
+            yield
+            return self._rename_raw(old_name, new_name)
+
+    def rename(self, new_name: str, old_name: str | None = None):
+        """Rename active or selected profile. Profiles in groups will also be renamed
+        :arg new_name:          New profile name
+        :arg old_name:          Target, or active (if not provided) profile name
+        :raise InputError:      If wrong arguments provided
+        :raise ProfilesError:   If any error at group operations"""
+        # Check input
+        if old_name is None:
+            old_name = self.active
+        if old_name == self._cfg.def_sect:
+            raise InputError(msg=f'Cannot rename default profile to {new_name!r}',
+                             func_name=f'{self!r}.rename()')
+
+        # Single config profile rename
+        if self._group is None:
+            return next(self._rename(new_name, old_name))
+
+        # Group configs profile rename
+        if error := self._group_call('_rename', new_name, old_name):
+            raise ProfilesError(error.format(f'rename from {old_name!r} to {new_name!r}'))
+
+    def _switch_raw(self, name, cfg, data):
+        if self.before_switch is not None:
+            self.before_switch()
+
+        fields = cfg.get_fields
+        mapping, data_dict = as_dict_stated(self[name], fields, strict=True)
+        with self:
+            self.active = name
+            self.active_fields = tuple(data_dict if mapping else fields)
+        [setattr(data, *kv) for kv in data_dict.items()]
+
+        if self.after_switch is not None:
+            self.after_switch()
+
+    def _switch_check(self, name, add, cfg):
+        if (absent := name not in self and name != cfg.def_sect) and not add:
+            raise self._name_error((f'{self!r}.switch()', 'name'), name)
+        return absent
+
+    def _switch(self, name, add, add_current, absent=None):
+        cfg = self._cfg
+        if (prev_name := self.active) == name:
+            yield
+            return
+
+        # Check input and add data from default or current profile if enabled and profile is absent
+        if absent is None:
+            absent = self._switch_check(name, add, cfg)
+        if absent and add:
+            self.set(name, self.get[prev_name] if add_current else None, typecheck=False)
+
+        # Save current profile values and switch with revert at fail
+        self.update()
+        try:
+            self._switch_raw(name, cfg, self._data)
+        except Exception:
+            self._switch_raw(prev_name, cfg, self._data)
+            raise
+        yield
+        return self._switch_raw(prev_name, cfg, self._data)
+
+    def switch(self, name: str, add=False, add_current=False):
+        """Switch active profile. Profiles in groups will also be switched
+        :arg name:              Exists or new profile name (if :arg add: enabled)
+        :arg add:               Adds profile with provided :arg name: if it not exists
+        :arg add_current:       Replaces defaults with the active profile values, when it is added
+        :raise InputError:      If wrong arguments provided
+        :raise ProfilesError:   If any error at group operations"""
+        # Check input
+        if add_current and not add:
+            raise InputError('add', 'add_current',
+                             msg="Param 'add' must be True, when 'add_current' is True")
+        absent = self._switch_check(name, add, self._cfg)
+
+        # Single config profile switch
+        if self._group is None:
+            return next(self._switch(name, add, add_current, absent))
+
+        # Group configs profile switch
+        if error := self._group_call('_switch', name, add, add_current):
+            raise ProfilesError(error.format(f'switch to {name!r}'))
+
+    @property
+    def get_groups(self) -> MappingProxyType[str, Any]:
+        """Get groups dict view"""
+        return MappingProxyType(self._groups)
+
+    def del_group(self, name: str) -> list | None:
+        """Delete provided group name
+        :arg name:          Deleting group name
+        :return:            List of deleted group config profiles
+        :raise KeyError:    If :arg name: is not exists"""
+        return self._groups.pop(name)
```

### Comparing `configlayer-0.1/configlayer/exceptions.py` & `configlayer-0.1.1/configlayer/exceptions.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-"""Config layer exceptions"""
-from typing import Callable, Any
-
-
-_UNIQUE = object()
-
-
-# Common exceptions
-
-
-class InternalError(Exception):
-    """Something in code goes wrong, program works not as expected!"""
-
-
-class InputError(Exception):
-    """Input parameter(s) of func or class method is wrong
-    All parameters are optional, can be names or exceptions (if needed to override message)
-    Parameters must_be and received can be started from ':' sign, to join message without space"""
-    def __init__(self, *items: Exception | str,  msg='', item_name='parameter', func_name='',
-                 args=(), force_header=False, **kwargs: Any):
-        self.items = items
-        self.msg = msg
-        self.item_name = item_name
-        self.func_name = func_name
-        self.kwargs = kwargs
-        self.header = self.must_be = self.received = ''
-        self.sentences: tuple = ()
-
-        # Handle exceptions
-        if not all(isinstance(x, str) for x in items):
-            super().__init__('; '.join(map(repr, items)), *args)
-            return
-
-        # Make header
-        header = f'Provided wrong {item_name}'
-        func = f' to {func_name}' if func_name else ''
-        match len(items):
-            case 0: header = f'{header}(s){func}' if (force_header or func or
-                                                      not (msg or kwargs)) else ''
-            case 1: header = f'{header}{func}: {items[0]}'
-            # bug mypy: not see check for str at line 30, so type ignored
-            case _: header = f'{header}s{func}: {", ".join(items)}'                                 # type: ignore[arg-type]
-        self.header = header
-
-        # Make received, must_be and sentences
-        must_recv, sentences = [], []
-        for k, v in kwargs.items():
-            if k == 'sentences':
-                sentences.extend(v)
-                continue
-
-            # bug mypy: isinstance can accept Callable as type, so type ignored
-            if val := (v if isinstance(v, str) else
-                       v() if isinstance(v, Callable) else f': {v!r}'):                             # type: ignore[arg-type]
-                sentence = f'{k.replace("_", " ")}{"" if val[0] in ":,=" else " "}{val}'
-                if k == 'must_be' or k == 'received':
-                    setattr(self, k, v)
-                    must_recv.append(sentence)
-                else:
-                    sentences.append(sentence)
-        self.sentences = tuple(sentences)
-
-        # Build message and fill exception
-        msgs = (header, msg, ', but '.join(must_recv), *sentences)
-        super().__init__('. '.join(x[0].upper() + x[1:] for x in msgs if x), *args)
-
-
-class InitError(Exception):
-    """Object initialization failed during class.__init__() method processing"""
-
-
-class CheckValueError(ValueError):
-    """Object value check failed"""
-
-
-class CheckTypeError(TypeError):
-    """Object type check failed"""
-
-
-# Config related exceptions
-
-
-class ConfigError(Exception):
-    """Any config-related error type"""
-
-
-class OptionsCheckError(ConfigError):
-    """Options check failed, planned set of values is invalid"""
-
-
-def _replace_unique(value, default=''):
-    if value != _UNIQUE:
-        try:
-            value = repr(value)
-        except Exception as e:
-            value = repr(e)
-    else:
-        value = default
-    return value
-
-
-class FieldError(ConfigError):
-    """Requested wrong field operation"""
-    def __init__(self, operation: str, config: str, field: str, to_value=_UNIQUE,
-                 from_value=_UNIQUE, by_func='', reason='', failed=True, type_name='config'):
-        from_value = f' from {from_value!r}' if (from_value := _replace_unique(from_value)) else ''
-        to_value = f' to {to_value!r}' if (to_value := _replace_unique(to_value)) else ''
-        by_func = f' by {by_func}' if by_func else ''
-        failed = f' {"failed" if failed else "completed"}'
-        reason = f',{"" if failed else " but"} {reason}' if reason else ''
-        super().__init__(f'{operation.capitalize()} {config!r} {type_name} field {field!r}'
-                         f'{from_value}{to_value}{by_func}{failed}{reason}')
-
-
-class ProfilesError(ConfigError):
-    """Requested wrong profiles operation"""
-
-
-class IOImportError(ConfigError):
-    """Requested wrong io import operation"""
-
-
-class IOExportError(ConfigError):
-    """Requested wrong io export operation"""
-
-
-class FileError(ConfigError):
-    """Requested wrong file operation"""
+"""Config layer exceptions"""
+from typing import Callable, Any
+
+
+_UNIQUE = object()
+
+
+# Common exceptions
+
+
+class InternalError(Exception):
+    """Something in code goes wrong, program works not as expected!"""
+
+
+class InputError(Exception):
+    """Input parameter(s) of func or class method is wrong
+    All parameters are optional, can be names or exceptions (if needed to override message)
+    Parameters must_be and received can be started from ':' sign, to join message without space"""
+    def __init__(self, *items: Exception | str,  msg='', item_name='parameter', func_name='',
+                 args=(), force_header=False, **kwargs: Any):
+        self.items = items
+        self.msg = msg
+        self.item_name = item_name
+        self.func_name = func_name
+        self.kwargs = kwargs
+        self.header = self.must_be = self.received = ''
+        self.sentences: tuple = ()
+
+        # Handle exceptions
+        if not all(isinstance(x, str) for x in items):
+            super().__init__('; '.join(map(repr, items)), *args)
+            return
+
+        # Make header
+        header = f'Provided wrong {item_name}'
+        func = f' to {func_name}' if func_name else ''
+        match len(items):
+            case 0: header = f'{header}(s){func}' if (force_header or func or
+                                                      not (msg or kwargs)) else ''
+            case 1: header = f'{header}{func}: {items[0]}'
+            # bug mypy: not see check for str at line 30, so type ignored
+            case _: header = f'{header}s{func}: {", ".join(items)}'                                 # type: ignore[arg-type]
+        self.header = header
+
+        # Make received, must_be and sentences
+        must_recv, sentences = [], []
+        for k, v in kwargs.items():
+            if k == 'sentences':
+                sentences.extend(v)
+                continue
+
+            # bug mypy: isinstance can accept Callable as type, so type ignored
+            if val := (v if isinstance(v, str) else
+                       v() if isinstance(v, Callable) else f': {v!r}'):                             # type: ignore[arg-type]
+                sentence = f'{k.replace("_", " ")}{"" if val[0] in ":,=" else " "}{val}'
+                if k == 'must_be' or k == 'received':
+                    setattr(self, k, v)
+                    must_recv.append(sentence)
+                else:
+                    sentences.append(sentence)
+        self.sentences = tuple(sentences)
+
+        # Build message and fill exception
+        msgs = (header, msg, ', but '.join(must_recv), *sentences)
+        super().__init__('. '.join(x[0].upper() + x[1:] for x in msgs if x), *args)
+
+
+class InitError(Exception):
+    """Object initialization failed during class.__init__() method processing"""
+
+
+class CheckValueError(ValueError):
+    """Object value check failed"""
+
+
+class CheckTypeError(TypeError):
+    """Object type check failed"""
+
+
+# Config related exceptions
+
+
+class ConfigError(Exception):
+    """Any config-related error type"""
+
+
+class OptionsCheckError(ConfigError):
+    """Options check failed, planned set of values is invalid"""
+
+
+def _replace_unique(value, default=''):
+    if value != _UNIQUE:
+        try:
+            value = repr(value)
+        except Exception as e:
+            value = repr(e)
+    else:
+        value = default
+    return value
+
+
+class FieldError(ConfigError):
+    """Requested wrong field operation"""
+    def __init__(self, operation: str, config: str, field: str, to_value=_UNIQUE,
+                 from_value=_UNIQUE, by_func='', reason='', failed=True, type_name='config'):
+        from_value = f' from {from_value!r}' if (from_value := _replace_unique(from_value)) else ''
+        to_value = f' to {to_value!r}' if (to_value := _replace_unique(to_value)) else ''
+        by_func = f' by {by_func}' if by_func else ''
+        failed = f' {"failed" if failed else "completed"}'
+        reason = f',{"" if failed else " but"} {reason}' if reason else ''
+        super().__init__(f'{operation.capitalize()} {config!r} {type_name} field {field!r}'
+                         f'{from_value}{to_value}{by_func}{failed}{reason}')
+
+
+class ProfilesError(ConfigError):
+    """Requested wrong profiles operation"""
+
+
+class IOImportError(ConfigError):
+    """Requested wrong io import operation"""
+
+
+class IOExportError(ConfigError):
+    """Requested wrong io export operation"""
+
+
+class FileError(ConfigError):
+    """Requested wrong file operation"""
```

### Comparing `configlayer-0.1/configlayer/types.py` & `configlayer-0.1.1/configlayer/types.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""Config layer type annotations and other types"""
-from __future__ import annotations
-from ast import literal_eval
-from typing import Any, Iterable, Sequence, NamedTuple, TypeVar, Callable, TypeAlias
-from pathlib import Path
-from dataclasses import dataclass
-
-
-__all__ = ('path_t', 'state_t', 'holder_t', 'mb_holder_t', 'fields_t', 'on_set_t',
-           'ClsObj', 'ItemError', 'ValidWrong', 'Field')
-
-
-T = TypeVar('T')
-
-path_t = str | Path                             # Generic path type
-state_t = bool | None                           # State is bool or None
-holder_t = Iterable[T] | Sequence[T]            # Any objects holder type (__iter__ or __getitem__)
-
-# bug mypy #14824: TypeAlias needed (Type variable "T" is invalid as target for type alias [misc])
-mb_holder_t: TypeAlias = T | Iterable[T] | Sequence[T]  # Maybe holder_t, as_holder() possible type
-
-fields_t = dict[str, T]                         # Fields holder type
-on_set_t = tuple[mb_holder_t[str] | None, bool, Callable[[str, Any, Any], None]]
-
-
-class ClsObj(NamedTuple):
-    cls: type | None
-    obj: object | None
-
-
-class ItemError(NamedTuple):
-    key: Any
-    value: Any
-    result: Any = ''
-
-
-class ValidWrong(tuple):
-    valid: Any
-    wrong: Any
-    errors: Iterable[ItemError]
-
-    def __new__(cls, valid, wrong, errors: Iterable[ItemError] = ()):
-        self = super().__new__(cls, (valid, wrong))
-        self.valid = valid
-        self.wrong = wrong
-        self.errors = errors
-        return self
-
-
-@dataclass(slots=True)
-class Field:
-    """Field additional descriptor's holder
-    Used if custom export/import functions needed at value declaration of inherited ConfigBase
-    Also used internally in ConfigBase"""
-    default: Any
-    export_func: Callable = repr
-    import_func: Callable = literal_eval
-    type: type = object  # internal usage, filled at ConfigBase init
+"""Config layer type annotations and other types"""
+from __future__ import annotations
+from ast import literal_eval
+from typing import Any, Iterable, Sequence, NamedTuple, TypeVar, Callable, TypeAlias
+from pathlib import Path
+from dataclasses import dataclass
+
+
+__all__ = ('path_t', 'state_t', 'holder_t', 'mb_holder_t', 'fields_t', 'on_set_t',
+           'ClsObj', 'ItemError', 'ValidWrong', 'Field')
+
+
+T = TypeVar('T')
+
+path_t = str | Path                             # Generic path type
+state_t = bool | None                           # State is bool or None
+holder_t = Iterable[T] | Sequence[T]            # Any objects holder type (__iter__ or __getitem__)
+
+# bug mypy #14824: TypeAlias needed (Type variable "T" is invalid as target for type alias [misc])
+mb_holder_t: TypeAlias = T | Iterable[T] | Sequence[T]  # Maybe holder_t, as_holder() possible type
+
+fields_t = dict[str, T]                         # Fields holder type
+on_set_t = tuple[mb_holder_t[str] | None, bool, Callable[[str, Any, Any], None]]
+
+
+class ClsObj(NamedTuple):
+    cls: type | None
+    obj: object | None
+
+
+class ItemError(NamedTuple):
+    key: Any
+    value: Any
+    result: Any = ''
+
+
+class ValidWrong(tuple):
+    valid: Any
+    wrong: Any
+    errors: Iterable[ItemError]
+
+    def __new__(cls, valid, wrong, errors: Iterable[ItemError] = ()):
+        self = super().__new__(cls, (valid, wrong))
+        self.valid = valid
+        self.wrong = wrong
+        self.errors = errors
+        return self
+
+
+@dataclass(slots=True)
+class Field:
+    """Field additional descriptor's holder
+    Used if custom export/import functions needed at value declaration of inherited ConfigBase
+    Also used internally in ConfigBase"""
+    default: Any
+    export_func: Callable = repr
+    import_func: Callable = literal_eval
+    type: type = object  # internal usage, filled at ConfigBase init
```

### Comparing `configlayer-0.1/configlayer/utils.py` & `configlayer-0.1.1/configlayer/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,1135 +1,1135 @@
-"""Config layer support classes and functions"""
-from types import MappingProxyType
-from typing import TypeVar, Iterable, Any, Callable, Sized, Union, get_origin, Sequence
-from itertools import chain
-from functools import partial
-from dataclasses import dataclass
-from collections import ChainMap
-from collections.abc import Mapping
-
-from .types import state_t, holder_t, mb_holder_t, ClsObj, ItemError, ValidWrong
-from .exceptions import InternalError, InputError, InitError, CheckValueError, CheckTypeError
-
-
-_T = TypeVar('_T')
-
-_TEMPL_INPUT = '{} is{} needed, but{} provided'
-_TEMPL_ABSENT = 'Absent {}: '
-_TEMPL_EXTRA = 'Extra {}: '
-
-_IE_CE__T = ('check_extra()', 'template')
-_IE_CA__T = ('check_absent()', 'template')
-_IE_CI_ET = ('check_items()', 'extra_template')
-_IE_CI_AT = ('check_items()', 'absent_template')
-_IE_CL__T = ('check_lengths()', 'template')
-
-_CE = 'not more than'
-_CA = 'not less than'
-_CI = 'equal to'
-
-_GN_ATTRS = ('name', '__name__')
-_GN_ORDER = ('doc_obj', 'code_obj', 'attrs_obj', 'doc_cls', 'attrs_cls',
-             'str_obj', 'str_cls', 'repr_cls', 'repr_obj')
-_GN_INTERNAL = ('cls', 'obj', 'full', 'order', 'none', 'unknown', 'kwargs')
-
-_CLS_OBJ = ('cls', 'obj')
-_UNIQUE = object()
-_FORCE_SET = object.__setattr__
-
-_LOCKER_IGNORED = ('_locker_state', '_locker_enter_state')
-
-
-# Internal
-
-
-def _field_func_default(k, v):  # noqa
-    return not callable(v)
-
-
-def _types(obj_t: mb_holder_t[type], func_name='', param_name='obj_t') -> holder_t[type]:
-    if isinstance(obj_t, type):
-        return obj_t,  # holder_t
-    if origin := get_origin(obj_t):
-        if origin is Union:
-            # bug mypy: Union origin is always has __args__
-            return obj_t.__args__                                                                   # type: ignore[attr-defined]
-        obj_t = origin
-
-    errors = []
-    holder, obj_types = as_holder_stated(obj_t)
-    mapping, items = as_dict_stated(obj_types)
-    if obj_types:
-        if not (errors := [ItemError(k, v) for k, v in items.items() if not isinstance(v, type)]):
-            return obj_types
-    received = ', '.join(fmt_obj_errors(obj_t, errors, bool(obj_types), holder, mapping))
-    raise InputError(param_name, must_be="type or types", received=received, func_name=func_name)
-
-
-# Bool checks
-
-
-def is_dunder(name: str) -> bool:
-    """Returns True only if a '__dunder__' name provided (double underscored from both sides)
-    :arg name:  Target name for check
-    :return:    bool"""
-    return len(name) > 4 and name[:2] == name[-2:] == '__' and name[2] != '_' and name[-3] != '_'
-
-
-def is_internal(name: str) -> bool:
-    """Returns True only if name is '_internal', excepting '__dunder__' name ('magic' methods)
-    :arg name:  Target name for check
-    :return:    bool"""
-    return name.startswith('_') and not is_dunder(name)
-
-
-def is_hidden(name: str) -> bool:
-    """Returns True if name is hidden - '_internal' or '__dunder__' name
-    :arg name:  Target name for check
-    :return:    bool"""
-    return name.startswith('_')
-
-
-def is_exception(obj, exc_t: type[Exception] = Exception) -> bool:
-    """Returns True only if obj is instance or subclass of provided exception type
-    :arg obj:   Target object for check
-    :arg exc_t: Exception type for instance or subclass check
-    :return:    bool"""
-    return isinstance(obj, exc_t) or issubclass(get_cls_obj(obj).cls or object, exc_t)
-
-
-def is_holder(obj, exclude: mb_holder_t[type] = ()) -> state_t:
-    """Returns True only if obj can hold objects of any possible type
-    :arg obj:       Target object for check
-    :arg exclude:   Type or types that must not be detected as holders
-    :return:        bool | None (if :arg obj: is None)"""
-    exclude = _types(exclude, 'is_holder()', 'exclude') if exclude else ()  # no RecursionError
-    if obj is None:
-        return None
-    if isinstance(obj, (str, bytes, bytearray) + tuple(exclude)):
-        return False
-    try:
-        iter(obj)  # Check iteration possibility through __iter__ or __getitem__ methods
-    except TypeError:
-        return False
-    return True
-
-
-# Type casting
-
-
-def as_holder(obj: mb_holder_t[_T], default=(), exclude: mb_holder_t[type] = ()) -> holder_t[_T]:
-    """Returns obj if it is holder type, or make holder from obj, or pass default if obj is None
-    :arg obj:       Target object or objects for cast
-    :arg default:   Any object that will be returned if :arg obj: is None
-    :arg exclude:   Type or types that must not be detected as holders
-    :return:        :arg obj: | (:arg obj:,) | :arg default:"""
-    # bug mypy: obj is always returned as holder_t, except default, that can be anything
-    return obj if (state := is_holder(obj, exclude)) else default if state is None else (obj,)      # type: ignore[return-value]
-
-
-def as_holder_stated(obj: mb_holder_t[_T], default=(), exclude: mb_holder_t[type] = ()
-                     ) -> tuple[bool, holder_t[_T]]:
-    """Returns obj if it is holder type, or make holder from obj, or pass default if obj is None.
-    Return is_holder() state before result
-    :arg obj:       Target object or objects for cast
-    :arg default:   Any object that will be returned if :arg obj: is None
-    :arg exclude:   Type or types that must not be detected as holders
-    :return:        bool, :arg obj: | (:arg obj:,) | :arg default:"""
-    # bug mypy: obj is always returned as holder_t, except default, that can be anything
-    return (st := is_holder(obj, exclude)), obj if st else default if st is None else (obj,)        # type: ignore[return-value]
-
-
-def as_dict(objs: holder_t, keys: holder_t | Callable = enumerate, strict=False) -> dict:
-    """Returns dict from objs if it is Mapping type or process by keys func or zip keys with objs
-    :arg objs:      Target objects for cast
-    :arg keys:      Used only if :arg objs: is not Mapping, as func(:arg objs:) or as dict keys
-    :arg strict:    Used only if :arg keys: used, and it is not Callable, as zip keyword
-    :return:        dict(:arg objs: | :arg keys:(:arg objs:) | zip(:arg keys:, :arg objs:,
-                    strict=:arg strict:))"""
-    s = isinstance(objs, Mapping)
-    return dict(objs if s else keys(objs) if callable(keys) else zip(keys, objs, strict=strict))
-
-
-def as_dict_stated(objs: holder_t, keys: holder_t | Callable = enumerate, strict=False
-                   ) -> tuple[bool, dict]:
-    """Returns dict from objs if it is Mapping type or process by keys func or zip keys with objs
-    Return isinstance(objs, Mapping) state before result
-    :arg objs:      Target objects for cast
-    :arg keys:      Used only if :arg objs: is not Mapping, as func(:arg objs:) or as dict keys
-    :arg strict:    Used only if :arg keys: used, and it is not Callable, as zip keyword
-    :return:        bool, dict(:arg objs: | :arg keys:(:arg objs:) | zip(:arg keys:,
-                    :arg objs:, strict=:arg strict:))"""
-    s = isinstance(objs, Mapping)
-    return s, dict(objs if s else keys(objs) if callable(keys) else zip(keys, objs, strict=strict))
-
-
-# Common
-
-
-def safe(func: Callable, /, *args, _res_: Any = _UNIQUE, _exc_: Any = _UNIQUE, **kwargs):
-    """Safe function execution, return result or exception object, if it raised.
-    Optional result and exception handlers or fillers could be provided (repr, 'some str', etc.)
-    :arg func:      Target function for safe call
-    :arg args:      Positional arguments for :arg func:
-    :arg _res_:     Used on :arg func: result if Callable provided, or returned instead of result
-    :arg _exc_:     Used on exception if Callable provided, or returned instead of exception
-    :arg kwargs:    Keyword arguments for :arg func:
-    :return:        Handled or unhandled :arg func: result or exception"""
-    try:
-        result = func(*args, **kwargs)
-        return result if _res_ is _UNIQUE else _res_(result) if callable(_res_) else _res_
-    except Exception as exc:
-        return exc if _exc_ is _UNIQUE else _exc_(exc) if callable(_exc_) else _exc_
-
-
-def with_type(obj, **kwargs) -> str:
-    """Adds type name to object representation with additional information, if needed
-    :arg obj:       Target for type and optional details
-    :arg kwargs:    Keyword arguments for optional details about :arg obj:
-    :return:        Formatted string with :arg obj: name or repr, type, and optional details"""
-    obj_t = type(obj).__name__
-    obj = obj.__name__ if isinstance(obj, type) else repr(obj)
-    if not kwargs:
-        return f'{obj} ({obj_t})'
-    kwargs = {k: repr(v) for k, v in kwargs.items()}
-    kwargs = kwargs | {'type': obj_t} if 'type' in kwargs else {'type': obj_t} | kwargs
-    return f"{obj} ({', '.join(fmt_dict(kwargs, value_func=str))})"
-
-
-# Formatters
-
-
-def fmt_dict(obj: Mapping, key_func=str, sep='=', value_func=repr) -> tuple[str, ...]:
-    """Format dict data to tuple of str per item by customizable formatting
-    :arg obj:           Target mapping for formatting
-    :arg key_func:      Function for keys handling
-    :arg sep:           String separator between key and value
-    :arg value_func:    Function for values handling
-    :return:            Formatted strings tuple of each element"""
-    return tuple(f'{key_func(k)}{sep}{value_func(v)}' for k, v in obj.items())
-
-
-def fmt_obj_errors(obj, errors: holder_t[ItemError], exists: bool, holder: bool, mapping: bool,
-                   result=False, result_name='result', key_handler=repr, kv_sep='='
-                   ) -> tuple[str, ...]:
-    """Format obj errors (ItemError objects) if they exist, or add obj details only
-    :arg obj:           Target object for formatting, if no :arg errors: provided
-    :arg errors:        Target errors list for formatting
-    :arg exists:        [Formatter switch] Errors list handling
-    :arg holder:        [Formatter switch] is_holder(:arg obj:) result
-    :arg mapping:       [Formatter switch] isinstance(:arg obj:, Mapping) result
-    :arg result:        Add error(s) result to formatted info
-    :arg result_name:   :arg result: key name for not holder or mapping formatters
-    :arg key_handler:   Key formatting function for mapping formatter
-    :arg kv_sep:        Key-value separator for mapping formatter
-    :return:            Formatted strings tuple from :arg errors: or :arg obj:"""
-    if exists and errors:
-        rn = result_name
-        if not holder:
-            error = next(x for x in errors)
-            return with_type(error.value, **({rn: error.result} if result else {})),
-        if mapping:
-            return tuple(f'{key_handler(k)}{kv_sep}{with_type(v, **({rn: r} if result else {}))}'
-                         for k, v, r in errors)
-        return tuple(f'{with_type(v)} at pos {i}' + (f' ({r})' if result else '')
-                     for i, v, r in errors)
-    return with_type(obj),
-
-
-def fmt_name(obj: Sized, item_name='item', default=_UNIQUE) -> str:
-    """Format name depending only on the obj size - singular or plural
-    :arg obj:       Target sized object for name formatting
-    :arg item_name: Base item name (without 's' postfix)
-    :arg default:   Override item name if no objects provided (by default :arg item_name: + 's')
-    :return:        Formatted name"""
-    if cnt := len(obj):
-        return f'{item_name}{"s" if item_name and cnt > 1 else ""}'
-    elif default == _UNIQUE:
-        return f'{item_name}s'
-    else:
-        return str(default)
-
-
-def fmt_exc(input_exc: tuple, msg='', default_exc_t: type[Exception] = Exception, *args, **kwargs
-            ) -> InputError | Exception:
-    """Format InputError (if input_exc provided) or default exception
-    :arg input_exc:     InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :arg msg:           Exception message
-    :arg default_exc_t: Exception type, used if :arg input_exc: is empty
-    :arg args:          InputError or default exception positional arguments
-    :arg kwargs:        InputError keyword arguments used as InputError result in default exception
-    :return:            Formatted InputError or :arg default_exc_t: exception"""
-    if input_exc:
-        name, *params, in_kw = (input_exc if isinstance(input_exc[-1], dict) else (*input_exc, {}))
-        return InputError(*params, msg=msg, func_name=name, args=args, **in_kw | kwargs | in_kw)
-
-    if kwargs:
-        msg = InputError(msg=msg, **kwargs).args[0]
-    return default_exc_t(msg, *args) if msg else default_exc_t(*args)
-
-
-# Split
-
-
-def split(items: Iterable, condition: Callable = bool, func: Callable | None = None, *,  # noqa
-          unpack=False, safely=False, modify=False, as_dicts=False,
-          cond_key: bool | None = None, cond_value: bool | None = None, cond_invert=False
-          ) -> ValidWrong:
-    """Split items to valid and wrong iterables by condition
-    Each item can be unpacked, safely called and/or modified by provided func
-    Key (or index) and/or value can be provided as condition parameter(s) (default: value only)
-    If provided only cond_key or only cond_value - another parameter will be in inverted state
-    If unpack enabled, but item is not iterable - unpack will be skipped!
-    :arg items:         Target objects for split
-    :arg condition:     Split function, bool (default) means that True - Valid, False - Wrong
-    :arg func:          Modify function that called with each item as positional argument
-    :arg unpack:        Unpack item for :arg func: call with multiple positional arguments
-    :arg safely:        Safe call :arg func:, at exception - item placed in Wrong
-    :arg modify:        :arg func: call results used in ValidWrong, instead of :arg items:
-    :arg as_dicts:      Fill ValidWrong by dicts, even if not dict provided (indexes used as keys)
-    :arg cond_key:      Add item key (or index) to condition positional arguments
-    :arg cond_value:    Add item value to condition positional arguments (default: True)
-    :arg cond_invert:   Invert :arg condition: bool result to swap Valid and Wrong
-    :return:            ValidWrong instance with filled valid, wrong and errors attributes
-    :raise InputError:  When input parameters has wrong data or used not correct"""
-    if not cond_key and cond_value is None:
-        cond_value = True
-    elif not cond_value and cond_key is None:
-        cond_key = True
-    elif not cond_key and not cond_value:
-        raise fmt_exc(('split()', 'cond_key', 'cond_value'),
-                      must_be=f'at least one True or not filled',
-                      received=f'{cond_key = }, {cond_value = }')
-
-    valid, wrong, errors = {}, {}, []
-    mapping, named = as_dict_stated(items)
-    for k, raw_item in named.items():
-        args = as_holder(raw_item, default=(None,)) if unpack else (raw_item,)
-        item = raw_item if func is None else safe(func, *args) if safely else func(*args)
-        cond_args = [x for x, state in ((k, cond_key), (item, cond_value)) if state]
-        result = item if modify else raw_item
-        if safely and is_exception(item) or bool(item := condition(*cond_args)) == cond_invert:
-            wrong[k] = result
-            errors.append(ItemError(k, raw_item, item))
-        else:
-            valid[k] = result
-
-    # Return result items depending on the source items type
-    if as_dicts or mapping:
-        return ValidWrong(valid, wrong, errors)
-    return ValidWrong(tuple(valid.values()), tuple(wrong.values()), errors)
-
-
-# Joins
-
-
-def join(*items, sep=', ', typecast=True, skip_false=True) -> str:
-    """Advanced str.join() method with str typecast and skip false-values possibilities
-    :arg items:         Target items to join
-    :arg sep:           Items separator
-    :arg typecast:      Cast each item from :arg items: to str
-    :arg skip_false:    Skip each item from :arg items: if it False at bool check
-    :return:            Joined string"""
-    if skip_false:
-        items = tuple(filter(bool, items))
-    if typecast:
-        items = tuple(map(str, items))
-    return sep.join(items)
-
-
-def sentence(*items, sep=' ', typecast=True, skip_false=True) -> str:
-    """Make a single sentence from provided items (capitalize first letter in result)
-    :arg items:         Target items to join (mostly words or phrases)
-    :arg sep:           Items separator
-    :arg typecast:      Cast each item from :arg args: to str
-    :arg skip_false:    Skip each item from :arg args: if it False at bool check
-    :return:            Joined sentence"""
-    phrase = join(*items, sep=sep, typecast=typecast, skip_false=skip_false)
-    return f'{phrase[0].upper()}{phrase[1:]}' if phrase else ''
-
-
-def sentences(*items, sep='. ', typecast=True, skip_false=True) -> str:
-    """Make a multiple sentences from provided items (capitalize first letter in each item)
-    :arg items:         Target items to join (mostly finished sentences)
-    :arg sep:           Items separator
-    :arg typecast:      Cast each item from :arg args: to str
-    :arg skip_false:    Skip each item from :arg args: if it False at bool check
-    :return:            Joined sentences"""
-    phrases = tuple(sentence(x, typecast=typecast, skip_false=skip_false) for x in items)
-    return join(*phrases, sep=sep, typecast=typecast, skip_false=skip_false)
-
-
-# Data checks
-
-
-def check_input(provided: Any | None, needed: Any | None, item_name='Item', template=_TEMPL_INPUT,
-                input_exc=()) -> bool:
-    """Check provided input correctness. Error if provided XOR needed (None == False, Any == True)
-    :arg provided:  Target object to check
-    :arg needed:    Target object to check with
-    :arg item_name: Object name for error message
-    :arg template:  String with 3 placeholders: :arg item_name:, 'not' provided, 'not' needed
-    :arg input_exc: InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :return:        False if provided is None else True"""
-    if (is_provided := (provided is not None)) != (needed is not None):
-        args = (' not', '') if is_provided else ('', ' not')
-        msg = sentence(template.format(item_name, *args).lstrip())
-        raise fmt_exc(input_exc, msg, CheckValueError)
-    return is_provided
-
-
-def _fmt_template(template, items, item_name, item_func, sep, input_exc=()) -> str:
-    msg = sep.join(map(item_func, items))
-    match template.count('{'):
-        case 0: return template + msg
-        case 1: return template.format(fmt_name(items, item_name)) + msg
-        case 2: return template.format(fmt_name(items, item_name), msg)
-        case _: raise fmt_exc(input_exc, must_be='not more than 2 data places',
-                              received=repr(template))
-
-
-def _items_out(msg1, msg2, provided, as_text, input_exc, sep='. ', **kwargs) -> holder_t | str:
-    if msg := sentences(msg1, msg2, sep=sep, typecast=False) if msg2 else msg1:
-        exc = fmt_exc(input_exc, msg, CheckValueError, **kwargs)
-        if as_text:
-            return str(exc)
-        raise exc
-    return msg if as_text else provided
-
-
-def _add_info(msg, provided, expected, item_func):
-    return {'must_be': f"{msg} expected ({', '.join(map(item_func, expected))})",
-            'received': f": {', '.join(map(item_func, provided))}"}
-
-
-def check_extra(provided: holder_t, expected: holder_t, item_name='item', item_func=repr, *,
-                item_sep=', ', as_text=False, template=_TEMPL_EXTRA, input_exc=(), **kwargs
-                ) -> holder_t | str:
-    """Check for not exists items provided (if all provided is expected)
-    :arg provided:  Target objects to check
-    :arg expected:  Target objects to check with
-    :arg item_name: Object name for error message
-    :arg item_func: Function to show item information for error message
-    :arg item_sep:  Items separator for error message
-    :arg as_text:   Not raise exception, return formatted str
-    :arg template:  String with 0-2 placeholders: formatted item_name, wrong items message
-    :arg input_exc: InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :arg kwargs:    InputError additional keyword arguments
-    :return:        :arg provided: | str (if :arg as_text:)"""
-    if msg := [x for x in provided if x not in expected] or '':
-        msg = _fmt_template(template, msg, item_name, item_func, item_sep, _IE_CE__T)
-        kwargs = _add_info(_CE, provided, expected, item_func) | kwargs
-    return _items_out(msg, '', provided, as_text, input_exc, **kwargs)
-
-
-def check_absent(provided: holder_t, expected: holder_t, item_name='item', item_func=repr, *,
-                 item_sep=', ', as_text=False, template=_TEMPL_ABSENT, input_exc=(), **kwargs
-                 ) -> holder_t | str:
-    """Check for not enough items provided (if all expected is provided)
-    :arg provided:  Target objects to check
-    :arg expected:  Target objects to check with
-    :arg item_name: Object name for error message
-    :arg item_func: Function to show item information for error message
-    :arg item_sep:  Items separator for error message
-    :arg as_text:   Not raise exception, return formatted str
-    :arg template:  String with 0-2 placeholders: formatted item_name, wrong items message
-    :arg input_exc: InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :arg kwargs:    InputError additional keyword arguments
-    :return:        :arg provided: | str (if :arg as_text:)"""
-    if msg := [x for x in expected if x not in provided] or '':
-        msg = _fmt_template(template, msg, item_name, item_func, item_sep, _IE_CA__T)
-        kwargs = _add_info(_CA, provided, expected, item_func) | kwargs
-    return _items_out(msg, '', provided, as_text, input_exc, **kwargs)
-
-
-def check_items(provided: holder_t, expected: holder_t, item_name='item', item_func=repr, *,
-                item_sep=', ', check_sep='. ', as_text=False, input_exc=(),
-                extra=True, extra_template=_TEMPL_EXTRA,
-                absent=True, absent_template=_TEMPL_ABSENT, **kwargs) -> holder_t | str:
-    """Check for not enough and not exists items provided with customizable output
-    Both checks can be disabled by absent and extra keywords and each can have custom header    
-    :arg provided:          Target objects to check
-    :arg expected:          Target objects to check with
-    :arg item_name:         Object name for error message
-    :arg item_func:         Function to show item information for error message
-    :arg item_sep:          Items separator for error message
-    :arg check_sep:         Checks separator for error message
-    :arg as_text:           Not raise exception, return formatted str
-    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :arg extra:             Extra check state
-    :arg extra_template:    String with 0-2 placeholders: formatted item_name, wrong items message
-    :arg absent:            Absent check state
-    :arg absent_template:   String with 0-2 placeholders: formatted item_name, wrong items message
-    :arg kwargs:            InputError additional keyword arguments
-    :return:                :arg provided: | str (if :arg as_text:)"""
-    msg1, msg2 = ('', '')
-    if extra and (items := [x for x in provided if x not in expected]):
-        msg1 = _fmt_template(extra_template, items, item_name, item_func, item_sep, _IE_CI_ET)
-    if absent and (items := [x for x in expected if x not in provided]):
-        msg2 = _fmt_template(absent_template, items, item_name, item_func, item_sep, _IE_CI_AT)
-    if msg1 or msg2:
-        msg_part = _CI if extra and absent else _CE if extra else _CA
-        kwargs = _add_info(msg_part, provided, expected, item_func) | kwargs
-    return _items_out(msg1, msg2, provided, as_text, input_exc, check_sep, **kwargs)
-
-
-def check_lengths(provided: Sequence, expected: Sequence, item_name='value', item_func=repr, *,
-                  item_sep=', ', as_text=False, input_exc=(),
-                  extra=True, extra_template=_TEMPL_EXTRA,
-                  absent=True, absent_template=_TEMPL_ABSENT, **kwargs):
-    """Check for length equality of provided and expected with customizable output
-    Both checks can be disabled by absent and extra keywords and each can have custom header
-    :arg provided:          Target objects sequence to check
-    :arg expected:          Target objects sequence to check with
-    :arg item_name:         Object name for error message
-    :arg item_func:         Function to show item information for error message
-    :arg item_sep:          Items separator for error message
-    :arg as_text:           Not raise exception, return formatted str
-    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :arg extra:             Extra check state
-    :arg extra_template:    String with 0-2 placeholders: formatted item_name, wrong items message
-    :arg absent:            Absent check state
-    :arg absent_template:   String with 0-2 placeholders: formatted item_name, wrong items message
-    :arg kwargs:            InputError additional keyword arguments
-    :return:                :arg provided: | str (if :arg as_text:)"""
-    msg = ''
-    if (pl := len(provided)) != (nl := len(expected)):
-        state, template, obj, i = ((extra, extra_template, provided, nl) if pl > nl else
-                                   (absent, absent_template, expected, pl))
-        if state:
-            msg = _fmt_template(template, obj[i:], item_name, item_func, item_sep, _IE_CL__T)
-            kwargs = {'must_be': f'{nl} {fmt_name(expected, item_name, f"{item_name}s")} long',
-                      'received': str(pl)} | kwargs
-    return _items_out(msg, '', provided, as_text, input_exc, **kwargs)
-
-
-def check_type(obj: object, obj_t: mb_holder_t[type], typecast=False, name='', obj_t_check=True,
-               input_exc=(), raw=False, *raw_args):
-    """Check object type(s), with optional typecast if other type provided, dicts NOT supported
-    :arg obj:               Target object to check
-    :arg obj_t:             Target object type or types to check with
-    :arg typecast:          :arg obj: type casting to :arg obj_t: (if wrong type)
-    :arg name:              :arg obj: name ('object', 'item', etc.) for error message
-    :arg obj_t_check:       Check :arg obj_t: that types provided
-    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :arg raw:               Return not raised exception at error, with not formatted parts in args
-    :arg raw_args:          Additional args before not formatted parts in args (if :arg raw:)
-    :return:                :arg obj: | typecast-ed :arg obj: (if :arg typecast:) | CheckTypeError
-    :raise InputError:      If wrong arguments provided
-    :raise InputError:      If check failed and filled :arg input_exc: provided (upper-level error)
-    :raise CheckTypeError:  If check failed and :arg input_exc: not (or empty) provided"""
-    # Check simple
-    # bug mypy: valid type or types for isinstance
-    if isinstance(obj, obj_types := _types(obj_t, 'check_type()') if obj_t_check else obj_t):       # type: ignore[arg-type]
-        return obj
-
-    # Check with typecast if enabled
-    error = ''
-    obj_types = as_holder(obj_types)
-    if typecast:
-        for obj_type in obj_types:
-            if isinstance(result := safe(obj_type, obj), obj_type):
-                return result
-
-            error += f', typecast to {obj_type.__name__}: {result!r}'
-            if not isinstance(result, Exception):
-                error += f' ({type(obj).__name__})'
-
-    # Format error
-    name = sentence(f'{name} ') if name else ''
-    must_be = f'{" or ".join(x.__name__ for x in obj_types)} {fmt_name(tuple(obj_types), "type")}'
-    msg = f"{name}{with_type(obj)} must be {must_be}{error}"
-    if raw:
-        return CheckTypeError(*raw_args, obj, obj_t, msg, name, must_be, error)
-    raise fmt_exc(input_exc, msg, CheckTypeError)
-
-
-def _build_ct_ie_kw(no_info):
-    return {
-        'input_exc': ('check_types()', 'obj', {'must_be': '', 'received': ''} if no_info else {}),
-        'extra_template': "Extra {} (without type): ",
-        'absent_template': "Absent {} (type provided): "}
-
-
-_CT_IE_MAPS = _build_ct_ie_kw(True)
-_CT_IE_PAIRS = _build_ct_ie_kw(False)
-
-
-def check_types(obj: mb_holder_t[object], obj_t: mb_holder_t[type], typecast=False, item_name='',
-                *, one_obj=False, pairs=False, strict=True, obj_t_check=True, input_exc=()):
-    """Check object(s) type(s), with optional typecast if other type provided, dicts supported
-    :arg obj:               Target object or objects to check
-    :arg obj_t:             Target object type or types to check with
-    :arg typecast:          :arg obj: type casting to :arg obj_t: (if wrong type)
-    :arg item_name:         Common item name ('object', 'item', etc.) for error message
-    :arg one_obj:           Check :arg obj: as single object, even if any holder type provided
-    :arg pairs:             Zip :arg obj: and :arg obj_t: for pairs check (must be strict lengths)
-    :arg strict:            At :arg pairs: or both mappings detect :arg obj: absent keys/values
-    :arg obj_t_check:       Check :arg obj_t: that types provided
-    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
-    :return:                :arg obj: | typecast-ed :arg obj: (if :arg typecast:) | CheckTypeError
-    :raise InputError:      If wrong arguments provided
-    :raise InputError:      If check failed and filled :arg input_exc: provided (upper-level error)
-    :raise CheckTypeError:  If check failed and :arg input_exc: not (or empty) provided"""
-    # Check mutually exclusive input parameters
-    if one_obj and pairs:
-        raise fmt_exc(('check_types()', 'one_obj', 'pairs'),
-                      must_be='not more than one True', received='both')
-
-    # Check input obj
-    obj_is_holder, objects = (False, (obj,)) if one_obj else as_holder_stated(obj)
-    if not objects or any(x is None for x in objects):
-        raise fmt_exc(('check_types()', 'obj'), must_be='one or more objects without None',
-                      received=f"{obj = !r}{'' if obj == objects else f' ({objects = !r})'}")
-
-    # Check single object
-    if not obj_is_holder:
-        if obj_t_check:
-            _types(obj_t, 'check_types()')
-        return check_type(obj, obj_t, typecast, item_name, False, input_exc)
-
-    # Prepare common part for datasets
-    obj_types = _types(obj_t, 'check_types()') if obj_t_check else as_holder(obj_t)
-    obj_t_mapping = isinstance(obj_t, Mapping)
-    obj_mapping, named = as_dict_stated(objects)
-    maps = obj_mapping and obj_t_mapping
-
-    # Add args to check_type: typecast, name, obj_t_check, input_exc, raw
-    add_args = (typecast, item_name, False, (), True)
-
-    # Build dataset
-    if maps:        # Value-type pairs by its names if both are mappings
-        check_items(named, obj_types, absent=strict, item_name='key', **_CT_IE_MAPS)
-        # bug mypy: obj_types is Mapping in that case, so it has get method
-        dataset = [(v, obj_types.get(k), *add_args, k) for k, v in named.items()]                   # type: ignore[attr-defined]
-
-    elif pairs:     # Value-type pairs by lengths if enabled
-        # bug mypy: obj_types is Mapping in that case, so it has values method
-        obj_t_vals = obj_types.values() if obj_t_mapping else obj_types                             # type: ignore[attr-defined]
-        check_lengths(tuple(objects), obj_t_vals, absent=strict, item_name='value', **_CT_IE_PAIRS)
-        dataset = [(v, t, *add_args, ki) for (ki, v), t in zip(named.items(), obj_t_vals)]
-
-    else:           # Common type(s) for all values
-        dataset = [(v, obj_types, *add_args, ki) for ki, v in named.items()]
-
-    # Check multiple objects
-    exceptions, valid = split(dataset, is_exception, check_type, unpack=True, modify=True)
-
-    # Raise formatted error message if errors exists
-    if exceptions:
-        msg = f'Several {item_name or "object"}s'
-        errors = [ItemError(*x.args[:2]) for x in exceptions]
-        raw = exceptions[0].args
-
-        # Format error(s)
-        if len(exceptions) == 1:    # Single error - as single
-            info = fmt_obj_errors(obj, errors, True, True, obj_mapping)
-            msg = f'{raw[-3]}{info[0]} must be {raw[-2]}{raw[-1]}'
-
-        elif maps or pairs:         # Several errors, separate type - as newline
-            info = fmt_obj_errors(obj, errors, True, True, obj_mapping, False, '', str, ': ')
-            msg += '\n\t'.join((' has a wrong type:',
-                                *[f'{raw[-3]}{x} must be {e.args[-2]}{e.args[-1]}'
-                                  for x, e in zip(info, exceptions, strict=True)]))
-
-        else:                       # Several errors, common type(s) - as inline
-            info = fmt_obj_errors(obj, errors, True, True, obj_mapping, False, '', repr, '=')
-            result = ", ".join(f"{x}{e.args[-1]}" for x, e in zip(info, exceptions, strict=True))
-            msg += f' are not {raw[-2]}: {result}'
-
-        raise fmt_exc(input_exc, msg, CheckTypeError)
-
-    # Return input (or typecast-ed) value
-    if not typecast:
-        return obj
-    # note mypy: typecast is user selectable, so if an error occurs - it is considered as scheduled
-    return type(obj)(zip((x[-1] for x in dataset), valid, strict=True) if obj_mapping else valid)   # type: ignore[call-arg]
-
-
-# Decorators
-
-
-def decorate_methods(decorator: Callable, exclude: mb_holder_t[str] | Callable = is_hidden):
-    """Class decorator to apply provided decorator to non-excluded methods
-    :arg decorator: Target decorator for methods
-    :arg exclude:   Excluded from decoration class methods (default: hidden methods are excluded)
-    :return:        Class with decorated methods"""
-    if callable(exclude):
-        excluded = exclude
-    else:
-        exclude = as_holder(exclude)
-
-        def excluded(x):
-            return x in exclude
-
-    def decorate(cls):
-        for name, attr in cls.__dict__.items():
-            if not excluded(name) and callable(attr):
-                setattr(cls, name, decorator(attr))
-        return cls
-
-    # Decorator is called only (usage without calling is useless and wrong)
-    return decorate
-
-
-def init_reraise(entity_name: str, *get_name_args, **get_name_kwargs):
-    """Decorator for __init__ method (reraise basic error info at exception with InitError)
-    :arg entity_name:       Class objects common name, for error message
-    :arg get_name_args:     Class object GetName args, for error message
-    :arg get_name_kwargs:   Class object GetName kwargs, for error message
-    :return:                Decorated __init__ method
-    :raise InitError:       If error in __init__ method occurred"""
-    def init_decorator(__init__):
-        def init_wrapper(self, *args, **kwargs):
-            try:
-                __init__(self, *args, **kwargs)
-            except Exception as e:
-                target_name = GetName(self, *get_name_args, **get_name_kwargs)
-                view = ", ".join((*map(repr, args), *fmt_dict(kwargs)))
-                msg = f'Cannot init {entity_name} {target_name!r} (self.__init__({view}))'
-                raise InitError(msg) from e
-        return init_wrapper
-
-    # Decorator is not called - entity_name is class
-    if not isinstance(entity_name, str) and not get_name_args and not get_name_kwargs:
-        cls, entity_name = entity_name, 'class'
-        return init_decorator(cls)
-
-    # Decorator is called
-    return init_decorator
-
-
-def set_slots_defaults(field_names: mb_holder_t[str] = (),
-                       field_func: Callable = _field_func_default,
-                       fields_t: type | None = None):
-    """@dataclass(slots=True) alternative, that allows set slots with provided default values
-    :arg field_names:   Strict field name or names (if needed)
-    :arg field_func:    Condition for getting fields from class attributes
-    :arg fields_t:      Common fields type
-    :return:            Decorated class with slots defaults
-    :raise InputError:  If wrong arguments provided"""
-    def decorator(cls: type):
-        name = cls.__name__
-        # bug mypy: mapping proxy is support '|' operand with dict
-        base = type.__dict__ | {'__weakref__': None}                                                # type: ignore[operator]
-        differ = {k: v for k, v in cls.__dict__.items() if k not in base or base[k] != v}
-        condition = lambda k, v: k in field_names or k not in base and field_func(k, v)  # noqa
-        fields, attrs = split(differ, cond_key=True, cond_value=True, condition=condition)
-
-        types = {k: fields_t for k in fields} if fields_t else getattr(cls, '__annotations__', {})
-        type_kw = {'__slots__': tuple(fields)} | ({'__annotations__': types} if types else {})
-
-        def __repr__(self):
-            return f'{name}({", ".join(f"{k}={getattr(self, k, None)}" for k in fields)})'
-
-        def __eq__(self, other):
-            return repr(self) == repr(other)
-
-        def __init__(self, *args, **kwargs):
-            # Input checks
-            check_lengths(args, fields, absent=False, input_exc=(f'{name}()', '*args'))
-            if kwargs:
-                check_extra(kwargs, fields, input_exc=(f'{name}()', '**kwargs'))
-
-            if args and kwargs:
-                unfilled = tuple(fields)[len(args):]
-                if left := [x for x in kwargs if x not in unfilled]:
-                    raise fmt_exc((f'{name}()', '*args', '**kwargs'),
-                                  f'Already provided item in args: {", ".join(left)}')
-
-            if fields_t:
-                if args:
-                    check_types(args, fields_t, input_exc=(f'{name}()', '*args'))
-                if kwargs:
-                    check_types(kwargs, fields_t, input_exc=(f'{name}()', '**kwargs'))
-
-            # Fill fields by defaults | args | kwargs
-            if args:
-                kwargs = dict(zip(fields, args)) | kwargs
-            [_FORCE_SET(self, k, v) for k, v in (fields | kwargs).items()]
-
-            # Call post init as in dataclass
-            if post_init := attrs.get('__post_init__'):
-                post_init(self)
-
-        new_cls = type(cls.__name__, (), attrs | type_kw)
-        # note mypy: skip static checks
-        new_cls.__repr__ = __repr__                                                                 # type: ignore[method-assign, assignment]
-        new_cls.__init__ = __init__                                                                 # type: ignore[misc]
-        new_cls.__eq__ = __eq__                                                                     # type: ignore[method-assign, assignment]
-        return new_cls
-
-    # Decorator is not called
-    if isinstance(field_names, type) and field_func == _field_func_default and fields_t is None:
-        _cls, field_names = field_names, ()
-        return decorator(_cls)
-
-    # Decorator is called with or without parameters
-    if field_names:
-        check_types(field_names, str, input_exc=('@set_slots_defaults()', 'field_names'))
-        field_names = as_holder(field_names)
-    if field_func != _field_func_default:
-        # bug mypy: Special forms is not supported yet (https://github.com/python/mypy/issues/9773)
-        check_type(field_func, Callable, input_exc=('@set_slots_defaults()', 'field_func'))         # type: ignore[arg-type]
-    if fields_t:
-        check_type(fields_t, type, input_exc=('@set_slots_defaults()', 'fields_t'))
-    return decorator
-
-
-# Getters
-
-
-def get_cls_obj(obj: object | type) -> ClsObj:
-    """Get class and object from target class or object, as NamedTuple with cls and obj attrs
-    :arg obj:   Target object for getting
-    :return:    NamedTuple with cls and obj attrs"""
-    if obj is None:
-        return ClsObj(None, None)
-    elif isinstance(obj, type):
-        return ClsObj(obj, None)
-    return ClsObj(type(obj), obj)
-
-
-def get_cls_attr(obj: object | type, attr: str):
-    """Get class attribute from target class or object
-    :arg obj:   Target object for getting
-    :arg attr:  Class attribute name
-    :return:    Class attribute value | None (if not exists)"""
-    return None if (cls := get_cls_obj(obj).cls) is None else getattr(cls, attr)
-
-
-def get_attrs(obj: object | type, skip_parent: int = 0, skip_child: int = 0, *,
-              internal=False, dunder=False, ignored: Iterable[type] = (type, object),
-              merge: Iterable[str] = ('__annotations__', '__slots__')) -> dict[str, Any]:
-    """Get attributes by exploring method resolution order, with optional parent coerce
-    By default merges __annotations__ dict and __slots__ tuple
-    :arg obj:           Target object for getting
-    :arg skip_parent:   Classes count starting from parent to skip
-    :arg skip_child:    Classes count starting from child to skip
-    :arg internal:      Include internal attrs (starting from '_', except __dunder__)
-    :arg dunder:        Include __dunder__ attrs
-    :arg ignored:       Ignored classes (default: type and object)
-    :arg merge:         Merge provided methods values from several classes
-    :return:            Dict with attributes
-    :raise InputError:  If wrong arguments provided"""
-    if obj is None:
-        raise fmt_exc(('get_attrs()', 'obj'), must_be='not None', received='None')
-    if ignored != (type, object) and ignored:
-        check_types(ignored, type, input_exc=('get_attrs()', 'ignored'))
-
-    # Prepare MRO
-    obj_t = obj if (is_cls := isinstance(obj, type)) else type(obj)
-    mro = [x for x in type.mro(obj_t) if x not in ignored]
-
-    # Check for skip correctness
-    if (parents := len(mro)) <= (skip_total := skip_parent + skip_child):
-        if not parents:
-            raise fmt_exc(('get_attrs()', 'obj'),
-                          must_be='not ignored type', received=with_type(obj),
-                          ignored_types=f': {", ".join(x.__name__ for x in ignored)}')
-        raise fmt_exc(('get_attrs()', 'skip_parent', 'skip_child'),
-                      must_be=f'less than {parents} skipped in total',
-                      skipped=f': {skip_total} ({skip_parent = }, {skip_child = })')
-
-    # Build filtered MRO from coerced MRO and from object (if not class provided) in first order
-    mro_flt = [x.__dict__ for x in mro[skip_child:len(mro) - skip_parent]]
-    if not is_cls:
-        # bug mypy: Union[Any, Dict[Any, Any]]?..
-        mro_flt.insert(0, getattr(obj, '__dict__',                                                  # type: ignore[arg-type]
-                                  {k: v for k in obj.__dir__()
-                                   if (v := getattr(obj, k, _UNIQUE)) is not _UNIQUE}))
-    # bug mypy: Why MutableMapping?..
-    coerced: ChainMap[str, Any] = ChainMap(*mro_flt)                                                # type: ignore[arg-type]
-
-    # Filter hidden if needed
-    if dunder and internal:
-        result = dict(coerced)
-    else:
-        result = {k: v for k, v in coerced.items()
-                  if (dunder or not is_dunder(k)) and (internal or not is_internal(k))}
-
-    # Merge provided dicts or iterables
-    for k in merge:
-        if k in result and (attrs := [y for x in coerced.maps if is_holder(y := x.get(k))]):
-            if isinstance(attrs[-1], Mapping):
-                # bug mypy: Why MutableMapping?..
-                result[k] = dict(ChainMap(*attrs))                                                  # type: ignore[arg-type]
-            else:
-                # bug mypy: Optional? Type[None]?..
-                result[k] = type(attrs[-1])(dict.fromkeys(chain(*attrs[::-1])))                     # type: ignore[arg-type, misc]
-    return result
-
-
-class _GNMethod(str):
-    # bug mypy: MappingProxyType as default dict arg
-    def __new__(cls, first_or_cls, obj=_UNIQUE, attrs: dict = MappingProxyType({})):                # type: ignore[assignment]
-        inst = str.__new__(cls, obj or first_or_cls if (pair := obj != _UNIQUE) else first_or_cls)
-        inst.__dict__ |= attrs | (dict(zip(_CLS_OBJ, (first_or_cls, obj))) if pair else {})
-        return inst
-
-
-class _GNClassMethod:
-    def __init__(self, decorated):
-        self.func = decorated
-        self.args = decorated.__code__.co_argcount - 1
-
-    def __call__(self, target, *args):
-        cls_args, obj_args = args, args
-        if (received := len(args)) and received != self.args:
-            if received != self.args * 2:
-                args_names = self.func.__code__.co_varnames[1:self.args + 1]
-                must_be = (f'{self.args} (same for both) or {self.args * 2} (separately) '
-                           'provided for cls and obj') if self.args else 'no arguments'
-                raise fmt_exc((f'GetName.{self.func.__code__.co_name}()', *args_names),
-                              force_header=True, must_be=must_be,
-                              received=f'{received}: {", ".join(map(repr, args))}')
-            cls_args, obj_args = args[:self.args], args[self.args:]
-
-        cls, obj = get_cls_obj(target)
-        return _GNMethod('' if cls is None else self.func(cls, *cls_args),
-                         '' if obj is None else self.func(obj, *obj_args))
-
-    def __repr__(self):
-        return f'GetName.{self.func.__code__.co_name}'
-
-
-def _flt_std_name(target: object | type, name: str) -> str:
-    return '' if get_cls_attr(target, '__qualname__') in name else name
-
-
-@decorate_methods(_GNClassMethod)
-class _GNMethods:
-    def doc(self: Any) -> str:
-        """Get first line in __doc__ attr as name"""
-        return doc.split('\n')[0] if (doc := getattr(self, '__doc__', None)) else ''
-
-    def code(self: Any) -> str:
-        """Get __code__.co_name attr as name"""
-        return getattr(co, 'co_name', '') if (co := getattr(self, '__code__', None)) else ''
-
-    def attrs(self: Any, attrs: Iterable[str] = _GN_ATTRS) -> str:
-        """Get first from default or provided attrs as name"""
-        if attrs:
-            if attrs != _GN_ATTRS:
-                check_types(attrs, str)
-
-            for attr in attrs:
-                if result := getattr(self, attr, ''):
-                    if result := safe(str, result, _exc_=''):
-                        return result
-        return ''
-
-    def repr(self: Any) -> str:
-        """Get __str__ attr as name"""
-        return safe(self.__repr__, _res_=partial(_flt_std_name, self), _exc_='')
-
-    def str(self: Any) -> str:
-        """Get __repr__ attr as name"""
-        return safe(self.__str__, _res_=partial(_flt_std_name, self), _exc_='')
-
-
-_GN_METHODS = get_attrs(_GNMethods)
-_GN_METHODS_EMPTY = {k: _GNMethod('', '') for k in _GN_METHODS}
-_GN_POSSIBLE_PARAMS = {'possible_parameters': f': {", ".join(_GN_ORDER)}'}
-
-
-@dataclass(slots=True)
-class _GNMethodHolder:
-    value: str
-    state: bool
-    args: tuple
-    method: _GNClassMethod
-
-
-class GetName(str, _GNMethods):
-    """Get first available name from provided target using multiple configurable ways
-    By default - only first of cls and obj names will be received (full=False)
-    Order of get methods can be changed, set of all get methods names is not required
-    Any get method can be enabled/disabled by bool ('{method}', '{method}_cls', '{method}_obj')
-    Attrs get method ('attrs', 'attrs_cls', 'attrs_obj') can have names tuple instead of bool
-    If None obj provided - 'none' arg value will be returned, as GetName (if str type)
-    All get methods failed - 'unknown' arg value will be returned, as GetName (if str type)"""
-    cls: _GNMethod
-    obj: _GNMethod
-
-    def __new__(cls, obj, doc=False, code=False, attrs: bool | tuple[holder_t[str]] = True,
-                str=True, repr=True, *, full=False, order=_GN_ORDER, none='', unknown='',  # noqa
-                **kwargs):
-        """
-        :arg obj:       Target object for getting
-        :arg doc:       Enable cls and obj get method, first line in __doc__ attr as name
-        :arg code:      Enable cls and obj get method, __code__.co_name attr as name
-        :arg attrs:     Enable cls and obj get method, first from default or provided attrs as name
-        :arg str:       Enable cls and obj get method, __str__ attr as name
-        :arg repr:      Enable cls and obj get method, __repr__ attr as name
-        :arg full:      Get all enabled methods and fill (default: only first in cls and obj)
-        :arg order:     Get methods order, cls or obj required ('{method}_cls', '{method}_obj')
-        :arg none:      Return value if :arg obj: is None, typecast-ed to GetName (if str type)
-        :arg unknown:   Return value if all methods failed, typecast-ed to GetName (if str type)
-        :arg kwargs:    Enable cls or obj get method separately ('{method}_cls', '{method}_obj')"""
-
-        # Filter only methods states/args from internally used arguments
-        left = {k: v for k, v in locals().items() if k not in _GN_INTERNAL}
-        holders: dict[str, _GNMethodHolder] = {}
-        for k, method in _GN_METHODS.items():
-            value = cls._get_method_holder(k, method, left.pop(k))
-            value2 = _GNMethodHolder(value.value, value.state, value.args, value.method)  # copy
-            holders |= {f'{k}_cls': value, f'{k}_obj': value2}
-        if left:
-            raise InternalError(f'Found not used args in GetName with {obj=!r}: {left}')
-
-        # Rewrite separately (cls/obj) provided methods states/args
-        if kwargs:
-            if wrongs := {k: v for k, v in kwargs.items() if k not in holders.keys()}:
-                # bug mypy: unpacked keyword arguments is not a positional argument..
-                raise fmt_exc(('GetName()', *wrongs.keys()), **_GN_POSSIBLE_PARAMS)                 # type: ignore[arg-type]
-            for k, v in kwargs.items():
-                holders[k] = cls._get_method_holder(k, holders[k].method, v)
-
-        # Check order
-        if order != _GN_ORDER:
-            check_extra(order, _GN_ORDER, item_name='method', template='Not exists {}: ',
-                        input_exc=('GetName()', 'order', {'must_be': ''} | _GN_POSSIBLE_PARAMS))
-
-        # Return none if None target provided
-        if obj is None:
-            return cls._try_type_cast(none, full)
-
-        # Get names (all or only first in cls and obj) by enabled methods in provided order
-        first, first_cls_obj, left_set = '', dict.fromkeys(_CLS_OBJ, ''), set(_CLS_OBJ)
-        targets = get_cls_obj(obj)
-        if targets.obj is None:
-            left_set.discard('obj')
-        for method_name in order:
-            if (cls_or_obj := method_name.rsplit('_', 1)[1]) in left_set:
-                if (holder := holders[method_name]).state:
-                    if name := holder.method.func(getattr(targets, cls_or_obj), *holder.args):
-                        holder.value = name
-                        if not first:
-                            first = name
-                        if not first_cls_obj[cls_or_obj]:
-                            first_cls_obj[cls_or_obj] = name
-                        if not full:
-                            left_set.discard(cls_or_obj)
-                            if not left_set:
-                                break
-
-        # Return unknown if no name found
-        if not first:
-            return cls._try_type_cast(unknown, full)
-
-        # Fast names receive way (only first in cls and obj methods), without GetName instance fill
-        if not full:
-            methods = {k: '' for k in _GN_METHODS}
-            # note mypy: that's planned
-            return _GNMethod.__new__(cls, first, attrs=first_cls_obj | methods)                     # type: ignore[arg-type]
-
-        # GetName instance fill by first cls and obj methods and each method separately
-        methods = {k: _GNMethod(holders[f'{k}_cls'].value, holders[f'{k}_obj'].value)
-                   for k in _GN_METHODS}
-        # note mypy: that's planned
-        return _GNMethod.__new__(cls, first, attrs=first_cls_obj | methods)                         # type: ignore[arg-type]
-
-    @staticmethod
-    def _get_method_holder(k, method, value) -> _GNMethodHolder:
-        check_type(value, (bool, tuple) if method.args else bool, input_exc=('GetName()', k))
-        return _GNMethodHolder('', bool(value), value if isinstance(value, tuple) else (), method)
-
-    @classmethod
-    def _try_type_cast(cls, value, full):
-        if isinstance(value, str):
-            attrs = _GN_METHODS_EMPTY if full else {}
-            return _GNMethod.__new__(cls, value, attrs=attrs | dict.fromkeys(_CLS_OBJ, ''))  # noqa
-        return value
-
-
-# Uncategorized
-
-
-class UID:
-    """Unique ID instances used as filler for detecting by comparison"""
-    __slots__ = ('name',)
-    name: str
-    exists: list[str] = []
-
-    def __init__(self, name: str):
-        """
-        :arg name:  Unique name for ID"""
-        if (name := str(name)) in self.exists:
-            raise ValueError(f'{name!r} unique ID cannot be created, it already exists')
-        self.exists.append(name)
-        self.name = name
-
-    def __repr__(self):
-        return f'UID({self.name!r})'
-
-    def __str__(self):
-        return f'{self.name} ID'
-
-
-class Locker:
-    """Lock child class from attributes manipulations with internal unlock possibility
-    Can be unlocked during active context manager, as it finished - class will be also locked"""
-    __slots__ = ('_locker_state', '_locker_enter_state', '_locker_set_attr', '_locker_del_attr',
-                 '_locker_ignored', '_locker_name')
-    _locker_state: bool
-    _locker_enter_state: bool
-    _locker_set_attr: bool
-    _locker_del_attr: bool
-    _locker_ignored: tuple
-    _locker_name: str
-
-    def __new__(cls, *args, **kwargs):
-        obj = object.__new__(cls)
-        [_FORCE_SET(obj, *x) for x in zip(Locker.__slots__, (False, False, True, True, ()))]
-        return obj
-
-    def __init__(self, *ignored_attrs: str, set_attr=True, del_attr=True, name: str | None = None):
-        """
-        :arg ignored_attrs: Attributes names that will not be locked at all
-        :arg set_attr:      Allow __set__ unlocked attributes
-        :arg del_attr:      Allow __del__ unlocked attributes
-        :arg name:          Set locker name for error message"""
-        self._locker_ignored += ignored_attrs
-        name = f'{GetName(self)!r} object' if name is None else str(name)
-        _FORCE_SET(self, '_locker_name', name)
-        _FORCE_SET(self, '_locker_set_attr', set_attr)
-        _FORCE_SET(self, '_locker_del_attr', del_attr)
-        self._locker_state = True
-
-    @staticmethod
-    def _get_exc_msg(is_set, allowed):
-        if allowed:
-            return is_set, 'is locked for changes'
-        else:
-            return is_set, f'does not support {"setting" if is_set else "deleting"} attributes'
-
-    def _make_exc(self, is_set, msg, key, value=None):
-        op, value = ('set', f', {value!r}') if is_set else ('del', '')
-        return TypeError(f'{self._locker_name} {msg} (self.__{op}attr__({key!r}{value}))')
-
-    def is_unlocked(self, key):
-        """Get True if provided attribute is unlocked"""
-        return not self._locker_state or key in self._locker_ignored
-
-    def __setattr__(self, key, value):
-        if key in _LOCKER_IGNORED or self._locker_set_attr and self.is_unlocked(key):
-            return _FORCE_SET(self, key, value)
-        raise self._make_exc(*self._get_exc_msg(True, self._locker_set_attr), key, value)
-
-    def __delattr__(self, key):
-        if not hasattr(self, key):  # msg as at set any new attrs in slotted class
-            raise AttributeError(f'{self._locker_name} has no attribute {key!r}')
-        if key in Locker.__slots__:
-            raise self._make_exc(False, 'Locker attrs deletion is forbidden', key)
-        if self._locker_del_attr and self.is_unlocked(key):
-            return object.__delattr__(self, key)
-        raise self._make_exc(*self._get_exc_msg(False, self._locker_del_attr), key)
-
-    def __enter__(self):
-        self._locker_enter_state, self._locker_state = self._locker_state, False
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._locker_enter_state:
-            self._locker_state = True
+"""Config layer support classes and functions"""
+from types import MappingProxyType
+from typing import TypeVar, Iterable, Any, Callable, Sized, Union, get_origin, Sequence
+from itertools import chain
+from functools import partial
+from dataclasses import dataclass
+from collections import ChainMap
+from collections.abc import Mapping
+
+from .types import state_t, holder_t, mb_holder_t, ClsObj, ItemError, ValidWrong
+from .exceptions import InternalError, InputError, InitError, CheckValueError, CheckTypeError
+
+
+_T = TypeVar('_T')
+
+_TEMPL_INPUT = '{} is{} needed, but{} provided'
+_TEMPL_ABSENT = 'Absent {}: '
+_TEMPL_EXTRA = 'Extra {}: '
+
+_IE_CE__T = ('check_extra()', 'template')
+_IE_CA__T = ('check_absent()', 'template')
+_IE_CI_ET = ('check_items()', 'extra_template')
+_IE_CI_AT = ('check_items()', 'absent_template')
+_IE_CL__T = ('check_lengths()', 'template')
+
+_CE = 'not more than'
+_CA = 'not less than'
+_CI = 'equal to'
+
+_GN_ATTRS = ('name', '__name__')
+_GN_ORDER = ('doc_obj', 'code_obj', 'attrs_obj', 'doc_cls', 'attrs_cls',
+             'str_obj', 'str_cls', 'repr_cls', 'repr_obj')
+_GN_INTERNAL = ('cls', 'obj', 'full', 'order', 'none', 'unknown', 'kwargs')
+
+_CLS_OBJ = ('cls', 'obj')
+_UNIQUE = object()
+_FORCE_SET = object.__setattr__
+
+_LOCKER_IGNORED = ('_locker_state', '_locker_enter_state')
+
+
+# Internal
+
+
+def _field_func_default(k, v):  # noqa
+    return not callable(v)
+
+
+def _types(obj_t: mb_holder_t[type], func_name='', param_name='obj_t') -> holder_t[type]:
+    if isinstance(obj_t, type):
+        return obj_t,  # holder_t
+    if origin := get_origin(obj_t):
+        if origin is Union:
+            # bug mypy: Union origin is always has __args__
+            return obj_t.__args__                                                                  # type: ignore[attr-defined]
+        obj_t = origin
+
+    errors = []
+    holder, obj_types = as_holder_stated(obj_t)
+    mapping, items = as_dict_stated(obj_types)
+    if obj_types:
+        if not (errors := [ItemError(k, v) for k, v in items.items() if not isinstance(v, type)]):
+            return obj_types
+    received = ', '.join(fmt_obj_errors(obj_t, errors, bool(obj_types), holder, mapping))
+    raise InputError(param_name, must_be="type or types", received=received, func_name=func_name)
+
+
+# Bool checks
+
+
+def is_dunder(name: str) -> bool:
+    """Returns True only if a '__dunder__' name provided (double underscored from both sides)
+    :arg name:  Target name for check
+    :return:    bool"""
+    return len(name) > 4 and name[:2] == name[-2:] == '__' and name[2] != '_' and name[-3] != '_'
+
+
+def is_internal(name: str) -> bool:
+    """Returns True only if name is '_internal', excepting '__dunder__' name ('magic' methods)
+    :arg name:  Target name for check
+    :return:    bool"""
+    return name.startswith('_') and not is_dunder(name)
+
+
+def is_hidden(name: str) -> bool:
+    """Returns True if name is hidden - '_internal' or '__dunder__' name
+    :arg name:  Target name for check
+    :return:    bool"""
+    return name.startswith('_')
+
+
+def is_exception(obj, exc_t: type[Exception] = Exception) -> bool:
+    """Returns True only if obj is instance or subclass of provided exception type
+    :arg obj:   Target object for check
+    :arg exc_t: Exception type for instance or subclass check
+    :return:    bool"""
+    return isinstance(obj, exc_t) or issubclass(get_cls_obj(obj).cls or object, exc_t)
+
+
+def is_holder(obj, exclude: mb_holder_t[type] = ()) -> state_t:
+    """Returns True only if obj can hold objects of any possible type
+    :arg obj:       Target object for check
+    :arg exclude:   Type or types that must not be detected as holders
+    :return:        bool | None (if :arg obj: is None)"""
+    exclude = _types(exclude, 'is_holder()', 'exclude') if exclude else ()  # no RecursionError
+    if obj is None:
+        return None
+    if isinstance(obj, (str, bytes, bytearray) + tuple(exclude)):
+        return False
+    try:
+        iter(obj)  # Check iteration possibility through __iter__ or __getitem__ methods
+    except TypeError:
+        return False
+    return True
+
+
+# Type casting
+
+
+def as_holder(obj: mb_holder_t[_T], default=(), exclude: mb_holder_t[type] = ()) -> holder_t[_T]:
+    """Returns obj if it is holder type, or make holder from obj, or pass default if obj is None
+    :arg obj:       Target object or objects for cast
+    :arg default:   Any object that will be returned if :arg obj: is None
+    :arg exclude:   Type or types that must not be detected as holders
+    :return:        :arg obj: | (:arg obj:,) | :arg default:"""
+    # bug mypy: obj is always returned as holder_t, except default, that can be anything
+    return obj if (state := is_holder(obj, exclude)) else default if state is None else (obj,)     # type: ignore[return-value]
+
+
+def as_holder_stated(obj: mb_holder_t[_T], default=(), exclude: mb_holder_t[type] = ()
+                     ) -> tuple[bool, holder_t[_T]]:
+    """Returns obj if it is holder type, or make holder from obj, or pass default if obj is None.
+    Return is_holder() state before result
+    :arg obj:       Target object or objects for cast
+    :arg default:   Any object that will be returned if :arg obj: is None
+    :arg exclude:   Type or types that must not be detected as holders
+    :return:        bool, :arg obj: | (:arg obj:,) | :arg default:"""
+    # bug mypy: obj is always returned as holder_t, except default, that can be anything
+    return (st := is_holder(obj, exclude)), obj if st else default if st is None else (obj,)       # type: ignore[return-value]
+
+
+def as_dict(objs: holder_t, keys: holder_t | Callable = enumerate, strict=False) -> dict:
+    """Returns dict from objs if it is Mapping type or process by keys func or zip keys with objs
+    :arg objs:      Target objects for cast
+    :arg keys:      Used only if :arg objs: is not Mapping, as func(:arg objs:) or as dict keys
+    :arg strict:    Used only if :arg keys: used, and it is not Callable, as zip keyword
+    :return:        dict(:arg objs: | :arg keys:(:arg objs:) | zip(:arg keys:, :arg objs:,
+                    strict=:arg strict:))"""
+    s = isinstance(objs, Mapping)
+    return dict(objs if s else keys(objs) if callable(keys) else zip(keys, objs, strict=strict))
+
+
+def as_dict_stated(objs: holder_t, keys: holder_t | Callable = enumerate, strict=False
+                   ) -> tuple[bool, dict]:
+    """Returns dict from objs if it is Mapping type or process by keys func or zip keys with objs
+    Return isinstance(objs, Mapping) state before result
+    :arg objs:      Target objects for cast
+    :arg keys:      Used only if :arg objs: is not Mapping, as func(:arg objs:) or as dict keys
+    :arg strict:    Used only if :arg keys: used, and it is not Callable, as zip keyword
+    :return:        bool, dict(:arg objs: | :arg keys:(:arg objs:) | zip(:arg keys:,
+                    :arg objs:, strict=:arg strict:))"""
+    s = isinstance(objs, Mapping)
+    return s, dict(objs if s else keys(objs) if callable(keys) else zip(keys, objs, strict=strict))
+
+
+# Common
+
+
+def safe(func: Callable, /, *args, _res_: Any = _UNIQUE, _exc_: Any = _UNIQUE, **kwargs):
+    """Safe function execution, return result or exception object, if it raised.
+    Optional result and exception handlers or fillers could be provided (repr, 'some str', etc.)
+    :arg func:      Target function for safe call
+    :arg args:      Positional arguments for :arg func:
+    :arg _res_:     Used on :arg func: result if Callable provided, or returned instead of result
+    :arg _exc_:     Used on exception if Callable provided, or returned instead of exception
+    :arg kwargs:    Keyword arguments for :arg func:
+    :return:        Handled or unhandled :arg func: result or exception"""
+    try:
+        result = func(*args, **kwargs)
+        return result if _res_ is _UNIQUE else _res_(result) if callable(_res_) else _res_
+    except Exception as exc:
+        return exc if _exc_ is _UNIQUE else _exc_(exc) if callable(_exc_) else _exc_
+
+
+def with_type(obj, **kwargs) -> str:
+    """Adds type name to object representation with additional information, if needed
+    :arg obj:       Target for type and optional details
+    :arg kwargs:    Keyword arguments for optional details about :arg obj:
+    :return:        Formatted string with :arg obj: name or repr, type, and optional details"""
+    obj_t = type(obj).__name__
+    obj = obj.__name__ if isinstance(obj, type) else repr(obj)
+    if not kwargs:
+        return f'{obj} ({obj_t})'
+    kwargs = {k: repr(v) for k, v in kwargs.items()}
+    kwargs = kwargs | {'type': obj_t} if 'type' in kwargs else {'type': obj_t} | kwargs
+    return f"{obj} ({', '.join(fmt_dict(kwargs, value_func=str))})"
+
+
+# Formatters
+
+
+def fmt_dict(obj: Mapping, key_func=str, sep='=', value_func=repr) -> tuple[str, ...]:
+    """Format dict data to tuple of str per item by customizable formatting
+    :arg obj:           Target mapping for formatting
+    :arg key_func:      Function for keys handling
+    :arg sep:           String separator between key and value
+    :arg value_func:    Function for values handling
+    :return:            Formatted strings tuple of each element"""
+    return tuple(f'{key_func(k)}{sep}{value_func(v)}' for k, v in obj.items())
+
+
+def fmt_obj_errors(obj, errors: holder_t[ItemError], exists: bool, holder: bool, mapping: bool,
+                   result=False, result_name='result', key_handler=repr, kv_sep='='
+                   ) -> tuple[str, ...]:
+    """Format obj errors (ItemError objects) if they exist, or add obj details only
+    :arg obj:           Target object for formatting, if no :arg errors: provided
+    :arg errors:        Target errors list for formatting
+    :arg exists:        [Formatter switch] Errors list handling
+    :arg holder:        [Formatter switch] is_holder(:arg obj:) result
+    :arg mapping:       [Formatter switch] isinstance(:arg obj:, Mapping) result
+    :arg result:        Add error(s) result to formatted info
+    :arg result_name:   :arg result: key name for not holder or mapping formatters
+    :arg key_handler:   Key formatting function for mapping formatter
+    :arg kv_sep:        Key-value separator for mapping formatter
+    :return:            Formatted strings tuple from :arg errors: or :arg obj:"""
+    if exists and errors:
+        rn = result_name
+        if not holder:
+            error = next(x for x in errors)
+            return with_type(error.value, **({rn: error.result} if result else {})),
+        if mapping:
+            return tuple(f'{key_handler(k)}{kv_sep}{with_type(v, **({rn: r} if result else {}))}'
+                         for k, v, r in errors)
+        return tuple(f'{with_type(v)} at pos {i}' + (f' ({r})' if result else '')
+                     for i, v, r in errors)
+    return with_type(obj),
+
+
+def fmt_name(obj: Sized, item_name='item', default=_UNIQUE) -> str:
+    """Format name depending only on the obj size - singular or plural
+    :arg obj:       Target sized object for name formatting
+    :arg item_name: Base item name (without 's' postfix)
+    :arg default:   Override item name if no objects provided (by default :arg item_name: + 's')
+    :return:        Formatted name"""
+    if cnt := len(obj):
+        return f'{item_name}{"s" if item_name and cnt > 1 else ""}'
+    elif default == _UNIQUE:
+        return f'{item_name}s'
+    else:
+        return str(default)
+
+
+def fmt_exc(input_exc: tuple, msg='', default_exc_t: type[Exception] = Exception, *args, **kwargs
+            ) -> InputError | Exception:
+    """Format InputError (if input_exc provided) or default exception
+    :arg input_exc:     InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :arg msg:           Exception message
+    :arg default_exc_t: Exception type, used if :arg input_exc: is empty
+    :arg args:          InputError or default exception positional arguments
+    :arg kwargs:        InputError keyword arguments used as InputError result in default exception
+    :return:            Formatted InputError or :arg default_exc_t: exception"""
+    if input_exc:
+        name, *params, in_kw = (input_exc if isinstance(input_exc[-1], dict) else (*input_exc, {}))
+        return InputError(*params, msg=msg, func_name=name, args=args, **in_kw | kwargs | in_kw)
+
+    if kwargs:
+        msg = InputError(msg=msg, **kwargs).args[0]
+    return default_exc_t(msg, *args) if msg else default_exc_t(*args)
+
+
+# Split
+
+
+def split(items: Iterable, condition: Callable = bool, func: Callable | None = None, *,  # noqa
+          unpack=False, safely=False, modify=False, as_dicts=False,
+          cond_key: bool | None = None, cond_value: bool | None = None, cond_invert=False
+          ) -> ValidWrong:
+    """Split items to valid and wrong iterables by condition
+    Each item can be unpacked, safely called and/or modified by provided func
+    Key (or index) and/or value can be provided as condition parameter(s) (default: value only)
+    If provided only cond_key or only cond_value - another parameter will be in inverted state
+    If unpack enabled, but item is not iterable - unpack will be skipped!
+    :arg items:         Target objects for split
+    :arg condition:     Split function, bool (default) means that True - Valid, False - Wrong
+    :arg func:          Modify function that called with each item as positional argument
+    :arg unpack:        Unpack item for :arg func: call with multiple positional arguments
+    :arg safely:        Safe call :arg func:, at exception - item placed in Wrong
+    :arg modify:        :arg func: call results used in ValidWrong, instead of :arg items:
+    :arg as_dicts:      Fill ValidWrong by dicts, even if not dict provided (indexes used as keys)
+    :arg cond_key:      Add item key (or index) to condition positional arguments
+    :arg cond_value:    Add item value to condition positional arguments (default: True)
+    :arg cond_invert:   Invert :arg condition: bool result to swap Valid and Wrong
+    :return:            ValidWrong instance with filled valid, wrong and errors attributes
+    :raise InputError:  When input parameters has wrong data or used not correct"""
+    if not cond_key and cond_value is None:
+        cond_value = True
+    elif not cond_value and cond_key is None:
+        cond_key = True
+    elif not cond_key and not cond_value:
+        raise fmt_exc(('split()', 'cond_key', 'cond_value'),
+                      must_be='at least one True or not filled',
+                      received=f'{cond_key = }, {cond_value = }')
+
+    valid, wrong, errors = {}, {}, []
+    mapping, named = as_dict_stated(items)
+    for k, raw_item in named.items():
+        args = as_holder(raw_item, default=(None,)) if unpack else (raw_item,)
+        item = raw_item if func is None else safe(func, *args) if safely else func(*args)
+        cond_args = [x for x, state in ((k, cond_key), (item, cond_value)) if state]
+        result = item if modify else raw_item
+        if safely and is_exception(item) or bool(item := condition(*cond_args)) == cond_invert:
+            wrong[k] = result
+            errors.append(ItemError(k, raw_item, item))
+        else:
+            valid[k] = result
+
+    # Return result items depending on the source items type
+    if as_dicts or mapping:
+        return ValidWrong(valid, wrong, errors)
+    return ValidWrong(tuple(valid.values()), tuple(wrong.values()), errors)
+
+
+# Joins
+
+
+def join(*items, sep=', ', typecast=True, skip_false=True) -> str:
+    """Advanced str.join() method with str typecast and skip false-values possibilities
+    :arg items:         Target items to join
+    :arg sep:           Items separator
+    :arg typecast:      Cast each item from :arg items: to str
+    :arg skip_false:    Skip each item from :arg items: if it False at bool check
+    :return:            Joined string"""
+    if skip_false:
+        items = tuple(filter(bool, items))
+    if typecast:
+        items = tuple(map(str, items))
+    return sep.join(items)
+
+
+def sentence(*items, sep=' ', typecast=True, skip_false=True) -> str:
+    """Make a single sentence from provided items (capitalize first letter in result)
+    :arg items:         Target items to join (mostly words or phrases)
+    :arg sep:           Items separator
+    :arg typecast:      Cast each item from :arg args: to str
+    :arg skip_false:    Skip each item from :arg args: if it False at bool check
+    :return:            Joined sentence"""
+    phrase = join(*items, sep=sep, typecast=typecast, skip_false=skip_false)
+    return f'{phrase[0].upper()}{phrase[1:]}' if phrase else ''
+
+
+def sentences(*items, sep='. ', typecast=True, skip_false=True) -> str:
+    """Make a multiple sentences from provided items (capitalize first letter in each item)
+    :arg items:         Target items to join (mostly finished sentences)
+    :arg sep:           Items separator
+    :arg typecast:      Cast each item from :arg args: to str
+    :arg skip_false:    Skip each item from :arg args: if it False at bool check
+    :return:            Joined sentences"""
+    phrases = tuple(sentence(x, typecast=typecast, skip_false=skip_false) for x in items)
+    return join(*phrases, sep=sep, typecast=typecast, skip_false=skip_false)
+
+
+# Data checks
+
+
+def check_input(provided: Any | None, needed: Any | None, item_name='Item', template=_TEMPL_INPUT,
+                input_exc=()) -> bool:
+    """Check provided input correctness. Error if provided XOR needed (None == False, Any == True)
+    :arg provided:  Target object to check
+    :arg needed:    Target object to check with
+    :arg item_name: Object name for error message
+    :arg template:  String with 3 placeholders: :arg item_name:, 'not' provided, 'not' needed
+    :arg input_exc: InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :return:        False if provided is None else True"""
+    if (is_provided := (provided is not None)) != (needed is not None):
+        args = (' not', '') if is_provided else ('', ' not')
+        msg = sentence(template.format(item_name, *args).lstrip())
+        raise fmt_exc(input_exc, msg, CheckValueError)
+    return is_provided
+
+
+def _fmt_template(template, items, item_name, item_func, sep, input_exc=()) -> str:
+    msg = sep.join(map(item_func, items))
+    match template.count('{'):
+        case 0: return template + msg
+        case 1: return template.format(fmt_name(items, item_name)) + msg
+        case 2: return template.format(fmt_name(items, item_name), msg)
+        case _: raise fmt_exc(input_exc, must_be='not more than 2 data places',
+                              received=repr(template))
+
+
+def _items_out(msg1, msg2, provided, as_text, input_exc, sep='. ', **kwargs) -> holder_t | str:
+    if msg := sentences(msg1, msg2, sep=sep, typecast=False) if msg2 else msg1:
+        exc = fmt_exc(input_exc, msg, CheckValueError, **kwargs)
+        if as_text:
+            return str(exc)
+        raise exc
+    return msg if as_text else provided
+
+
+def _add_info(msg, provided, expected, item_func):
+    return {'must_be': f"{msg} expected ({', '.join(map(item_func, expected))})",
+            'received': f": {', '.join(map(item_func, provided))}"}
+
+
+def check_extra(provided: holder_t, expected: holder_t, item_name='item', item_func=repr, *,
+                item_sep=', ', as_text=False, template=_TEMPL_EXTRA, input_exc=(), **kwargs
+                ) -> holder_t | str:
+    """Check for not exists items provided (if all provided is expected)
+    :arg provided:  Target objects to check
+    :arg expected:  Target objects to check with
+    :arg item_name: Object name for error message
+    :arg item_func: Function to show item information for error message
+    :arg item_sep:  Items separator for error message
+    :arg as_text:   Not raise exception, return formatted str
+    :arg template:  String with 0-2 placeholders: formatted item_name, wrong items message
+    :arg input_exc: InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :arg kwargs:    InputError additional keyword arguments
+    :return:        :arg provided: | str (if :arg as_text:)"""
+    if msg := [x for x in provided if x not in expected] or '':
+        msg = _fmt_template(template, msg, item_name, item_func, item_sep, _IE_CE__T)
+        kwargs = _add_info(_CE, provided, expected, item_func) | kwargs
+    return _items_out(msg, '', provided, as_text, input_exc, **kwargs)
+
+
+def check_absent(provided: holder_t, expected: holder_t, item_name='item', item_func=repr, *,
+                 item_sep=', ', as_text=False, template=_TEMPL_ABSENT, input_exc=(), **kwargs
+                 ) -> holder_t | str:
+    """Check for not enough items provided (if all expected is provided)
+    :arg provided:  Target objects to check
+    :arg expected:  Target objects to check with
+    :arg item_name: Object name for error message
+    :arg item_func: Function to show item information for error message
+    :arg item_sep:  Items separator for error message
+    :arg as_text:   Not raise exception, return formatted str
+    :arg template:  String with 0-2 placeholders: formatted item_name, wrong items message
+    :arg input_exc: InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :arg kwargs:    InputError additional keyword arguments
+    :return:        :arg provided: | str (if :arg as_text:)"""
+    if msg := [x for x in expected if x not in provided] or '':
+        msg = _fmt_template(template, msg, item_name, item_func, item_sep, _IE_CA__T)
+        kwargs = _add_info(_CA, provided, expected, item_func) | kwargs
+    return _items_out(msg, '', provided, as_text, input_exc, **kwargs)
+
+
+def check_items(provided: holder_t, expected: holder_t, item_name='item', item_func=repr, *,
+                item_sep=', ', check_sep='. ', as_text=False, input_exc=(),
+                extra=True, extra_template=_TEMPL_EXTRA,
+                absent=True, absent_template=_TEMPL_ABSENT, **kwargs) -> holder_t | str:
+    """Check for not enough and not exists items provided with customizable output
+    Both checks can be disabled by absent and extra keywords and each can have custom header
+    :arg provided:          Target objects to check
+    :arg expected:          Target objects to check with
+    :arg item_name:         Object name for error message
+    :arg item_func:         Function to show item information for error message
+    :arg item_sep:          Items separator for error message
+    :arg check_sep:         Checks separator for error message
+    :arg as_text:           Not raise exception, return formatted str
+    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :arg extra:             Extra check state
+    :arg extra_template:    String with 0-2 placeholders: formatted item_name, wrong items message
+    :arg absent:            Absent check state
+    :arg absent_template:   String with 0-2 placeholders: formatted item_name, wrong items message
+    :arg kwargs:            InputError additional keyword arguments
+    :return:                :arg provided: | str (if :arg as_text:)"""
+    msg1, msg2 = ('', '')
+    if extra and (items := [x for x in provided if x not in expected]):
+        msg1 = _fmt_template(extra_template, items, item_name, item_func, item_sep, _IE_CI_ET)
+    if absent and (items := [x for x in expected if x not in provided]):
+        msg2 = _fmt_template(absent_template, items, item_name, item_func, item_sep, _IE_CI_AT)
+    if msg1 or msg2:
+        msg_part = _CI if extra and absent else _CE if extra else _CA
+        kwargs = _add_info(msg_part, provided, expected, item_func) | kwargs
+    return _items_out(msg1, msg2, provided, as_text, input_exc, check_sep, **kwargs)
+
+
+def check_lengths(provided: Sequence, expected: Sequence, item_name='value', item_func=repr, *,
+                  item_sep=', ', as_text=False, input_exc=(),
+                  extra=True, extra_template=_TEMPL_EXTRA,
+                  absent=True, absent_template=_TEMPL_ABSENT, **kwargs):
+    """Check for length equality of provided and expected with customizable output
+    Both checks can be disabled by absent and extra keywords and each can have custom header
+    :arg provided:          Target objects sequence to check
+    :arg expected:          Target objects sequence to check with
+    :arg item_name:         Object name for error message
+    :arg item_func:         Function to show item information for error message
+    :arg item_sep:          Items separator for error message
+    :arg as_text:           Not raise exception, return formatted str
+    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :arg extra:             Extra check state
+    :arg extra_template:    String with 0-2 placeholders: formatted item_name, wrong items message
+    :arg absent:            Absent check state
+    :arg absent_template:   String with 0-2 placeholders: formatted item_name, wrong items message
+    :arg kwargs:            InputError additional keyword arguments
+    :return:                :arg provided: | str (if :arg as_text:)"""
+    msg = ''
+    if (pl := len(provided)) != (nl := len(expected)):
+        state, template, obj, i = ((extra, extra_template, provided, nl) if pl > nl else
+                                   (absent, absent_template, expected, pl))
+        if state:
+            msg = _fmt_template(template, obj[i:], item_name, item_func, item_sep, _IE_CL__T)
+            kwargs = {'must_be': f'{nl} {fmt_name(expected, item_name, f"{item_name}s")} long',
+                      'received': str(pl)} | kwargs
+    return _items_out(msg, '', provided, as_text, input_exc, **kwargs)
+
+
+def check_type(obj: object, obj_t: mb_holder_t[type], typecast=False, name='', obj_t_check=True,
+               input_exc=(), raw=False, *raw_args):
+    """Check object type(s), with optional typecast if other type provided, dicts NOT supported
+    :arg obj:               Target object to check
+    :arg obj_t:             Target object type or types to check with
+    :arg typecast:          :arg obj: type casting to :arg obj_t: (if wrong type)
+    :arg name:              :arg obj: name ('object', 'item', etc.) for error message
+    :arg obj_t_check:       Check :arg obj_t: that types provided
+    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :arg raw:               Return not raised exception at error, with not formatted parts in args
+    :arg raw_args:          Additional args before not formatted parts in args (if :arg raw:)
+    :return:                :arg obj: | typecast-ed :arg obj: (if :arg typecast:) | CheckTypeError
+    :raise InputError:      If wrong arguments provided
+    :raise InputError:      If check failed and filled :arg input_exc: provided (upper-level error)
+    :raise CheckTypeError:  If check failed and :arg input_exc: not (or empty) provided"""
+    # Check simple
+    # bug mypy: valid type or types for isinstance
+    if isinstance(obj, obj_types := _types(obj_t, 'check_type()') if obj_t_check else obj_t):       # type: ignore[arg-type]
+        return obj
+
+    # Check with typecast if enabled
+    error = ''
+    obj_types = as_holder(obj_types)
+    if typecast:
+        for obj_type in obj_types:
+            if isinstance(result := safe(obj_type, obj), obj_type):
+                return result
+
+            error += f', typecast to {obj_type.__name__}: {result!r}'
+            if not isinstance(result, Exception):
+                error += f' ({type(obj).__name__})'
+
+    # Format error
+    name = sentence(f'{name} ') if name else ''
+    must_be = f'{" or ".join(x.__name__ for x in obj_types)} {fmt_name(tuple(obj_types), "type")}'
+    msg = f"{name}{with_type(obj)} must be {must_be}{error}"
+    if raw:
+        return CheckTypeError(*raw_args, obj, obj_t, msg, name, must_be, error)
+    raise fmt_exc(input_exc, msg, CheckTypeError)
+
+
+def _build_ct_ie_kw(no_info):
+    return {
+        'input_exc': ('check_types()', 'obj', {'must_be': '', 'received': ''} if no_info else {}),
+        'extra_template': "Extra {} (without type): ",
+        'absent_template': "Absent {} (type provided): "}
+
+
+_CT_IE_MAPS = _build_ct_ie_kw(True)
+_CT_IE_PAIRS = _build_ct_ie_kw(False)
+
+
+def check_types(obj: mb_holder_t[object], obj_t: mb_holder_t[type], typecast=False, item_name='',
+                *, one_obj=False, pairs=False, strict=True, obj_t_check=True, input_exc=()):
+    """Check object(s) type(s), with optional typecast if other type provided, dicts supported
+    :arg obj:               Target object or objects to check
+    :arg obj_t:             Target object type or types to check with
+    :arg typecast:          :arg obj: type casting to :arg obj_t: (if wrong type)
+    :arg item_name:         Common item name ('object', 'item', etc.) for error message
+    :arg one_obj:           Check :arg obj: as single object, even if any holder type provided
+    :arg pairs:             Zip :arg obj: and :arg obj_t: for pairs check (must be strict lengths)
+    :arg strict:            At :arg pairs: or both mappings detect :arg obj: absent keys/values
+    :arg obj_t_check:       Check :arg obj_t: that types provided
+    :arg input_exc:         InputError args tuple: (func_name: str, *items: str, kwargs: dict)
+    :return:                :arg obj: | typecast-ed :arg obj: (if :arg typecast:) | CheckTypeError
+    :raise InputError:      If wrong arguments provided
+    :raise InputError:      If check failed and filled :arg input_exc: provided (upper-level error)
+    :raise CheckTypeError:  If check failed and :arg input_exc: not (or empty) provided"""
+    # Check mutually exclusive input parameters
+    if one_obj and pairs:
+        raise fmt_exc(('check_types()', 'one_obj', 'pairs'),
+                      must_be='not more than one True', received='both')
+
+    # Check input obj
+    obj_is_holder, objects = (False, (obj,)) if one_obj else as_holder_stated(obj)
+    if not objects or any(x is None for x in objects):
+        raise fmt_exc(('check_types()', 'obj'), must_be='one or more objects without None',
+                      received=f"{obj = !r}{'' if obj == objects else f' ({objects = !r})'}")
+
+    # Check single object
+    if not obj_is_holder:
+        if obj_t_check:
+            _types(obj_t, 'check_types()')
+        return check_type(obj, obj_t, typecast, item_name, False, input_exc)
+
+    # Prepare common part for datasets
+    obj_types = _types(obj_t, 'check_types()') if obj_t_check else as_holder(obj_t)
+    obj_t_mapping = isinstance(obj_t, Mapping)
+    obj_mapping, named = as_dict_stated(objects)
+    maps = obj_mapping and obj_t_mapping
+
+    # Add args to check_type: typecast, name, obj_t_check, input_exc, raw
+    add_args = (typecast, item_name, False, (), True)
+
+    # Build dataset
+    if maps:        # Value-type pairs by its names if both are mappings
+        check_items(named, obj_types, absent=strict, item_name='key', **_CT_IE_MAPS)
+        # bug mypy: obj_types is Mapping in that case, so it has get method
+        dataset = [(v, obj_types.get(k), *add_args, k) for k, v in named.items()]                  # type: ignore[attr-defined]
+
+    elif pairs:     # Value-type pairs by lengths if enabled
+        # bug mypy: obj_types is Mapping in that case, so it has values method
+        obj_t_vals = obj_types.values() if obj_t_mapping else obj_types                            # type: ignore[attr-defined]
+        check_lengths(tuple(objects), obj_t_vals, absent=strict, item_name='value', **_CT_IE_PAIRS)
+        dataset = [(v, t, *add_args, ki) for (ki, v), t in zip(named.items(), obj_t_vals)]
+
+    else:           # Common type(s) for all values
+        dataset = [(v, obj_types, *add_args, ki) for ki, v in named.items()]
+
+    # Check multiple objects
+    exceptions, valid = split(dataset, is_exception, check_type, unpack=True, modify=True)
+
+    # Raise formatted error message if errors exists
+    if exceptions:
+        msg = f'Several {item_name or "object"}s'
+        errors = [ItemError(*x.args[:2]) for x in exceptions]
+        raw = exceptions[0].args
+
+        # Format error(s)
+        if len(exceptions) == 1:    # Single error - as single
+            info = fmt_obj_errors(obj, errors, True, True, obj_mapping)
+            msg = f'{raw[-3]}{info[0]} must be {raw[-2]}{raw[-1]}'
+
+        elif maps or pairs:         # Several errors, separate type - as newline
+            info = fmt_obj_errors(obj, errors, True, True, obj_mapping, False, '', str, ': ')
+            msg += '\n\t'.join((' has a wrong type:',
+                                *[f'{raw[-3]}{x} must be {e.args[-2]}{e.args[-1]}'
+                                  for x, e in zip(info, exceptions, strict=True)]))
+
+        else:                       # Several errors, common type(s) - as inline
+            info = fmt_obj_errors(obj, errors, True, True, obj_mapping, False, '', repr, '=')
+            result = ", ".join(f"{x}{e.args[-1]}" for x, e in zip(info, exceptions, strict=True))
+            msg += f' are not {raw[-2]}: {result}'
+
+        raise fmt_exc(input_exc, msg, CheckTypeError)
+
+    # Return input (or typecast-ed) value
+    if not typecast:
+        return obj
+    # note mypy: typecast is user selectable, so if an error occurs - it is considered as scheduled
+    return type(obj)(zip((x[-1] for x in dataset), valid, strict=True) if obj_mapping else valid)   # type: ignore[call-arg]
+
+
+# Decorators
+
+
+def decorate_methods(decorator: Callable, exclude: mb_holder_t[str] | Callable = is_hidden):
+    """Class decorator to apply provided decorator to non-excluded methods
+    :arg decorator: Target decorator for methods
+    :arg exclude:   Excluded from decoration class methods (default: hidden methods are excluded)
+    :return:        Class with decorated methods"""
+    if callable(exclude):
+        excluded = exclude
+    else:
+        exclude = as_holder(exclude)
+
+        def excluded(x):
+            return x in exclude
+
+    def decorate(cls):
+        for name, attr in cls.__dict__.items():
+            if not excluded(name) and callable(attr):
+                setattr(cls, name, decorator(attr))
+        return cls
+
+    # Decorator is called only (usage without calling is useless and wrong)
+    return decorate
+
+
+def init_reraise(entity_name: str, *get_name_args, **get_name_kwargs):
+    """Decorator for __init__ method (reraise basic error info at exception with InitError)
+    :arg entity_name:       Class objects common name, for error message
+    :arg get_name_args:     Class object GetName args, for error message
+    :arg get_name_kwargs:   Class object GetName kwargs, for error message
+    :return:                Decorated __init__ method
+    :raise InitError:       If error in __init__ method occurred"""
+    def init_decorator(__init__):
+        def init_wrapper(self, *args, **kwargs):
+            try:
+                __init__(self, *args, **kwargs)
+            except Exception as e:
+                target_name = GetName(self, *get_name_args, **get_name_kwargs)
+                view = ", ".join((*map(repr, args), *fmt_dict(kwargs)))
+                msg = f'Cannot init {entity_name} {target_name!r} (self.__init__({view}))'
+                raise InitError(msg) from e
+        return init_wrapper
+
+    # Decorator is not called - entity_name is class
+    if not isinstance(entity_name, str) and not get_name_args and not get_name_kwargs:
+        cls, entity_name = entity_name, 'class'
+        return init_decorator(cls)
+
+    # Decorator is called
+    return init_decorator
+
+
+def set_slots_defaults(field_names: mb_holder_t[str] = (),
+                       field_func: Callable = _field_func_default,
+                       fields_t: type | None = None):
+    """@dataclass(slots=True) alternative, that allows set slots with provided default values
+    :arg field_names:   Strict field name or names (if needed)
+    :arg field_func:    Condition for getting fields from class attributes
+    :arg fields_t:      Common fields type
+    :return:            Decorated class with slots defaults
+    :raise InputError:  If wrong arguments provided"""
+    def decorator(cls: type):
+        name = cls.__name__
+        # bug mypy: mapping proxy is support '|' operand with dict
+        base = type.__dict__ | {'__weakref__': None}                                                # type: ignore[operator]
+        differ = {k: v for k, v in cls.__dict__.items() if k not in base or base[k] != v}
+        condition = lambda k, v: k in field_names or k not in base and field_func(k, v)  # noqa
+        fields, attrs = split(differ, cond_key=True, cond_value=True, condition=condition)
+
+        types = {k: fields_t for k in fields} if fields_t else getattr(cls, '__annotations__', {})
+        type_kw = {'__slots__': tuple(fields)} | ({'__annotations__': types} if types else {})
+
+        def __repr__(self):
+            return f'{name}({", ".join(f"{k}={getattr(self, k, None)}" for k in fields)})'
+
+        def __eq__(self, other):
+            return repr(self) == repr(other)
+
+        def __init__(self, *args, **kwargs):
+            # Input checks
+            check_lengths(args, fields, absent=False, input_exc=(f'{name}()', '*args'))
+            if kwargs:
+                check_extra(kwargs, fields, input_exc=(f'{name}()', '**kwargs'))
+
+            if args and kwargs:
+                unfilled = tuple(fields)[len(args):]
+                if left := [x for x in kwargs if x not in unfilled]:
+                    raise fmt_exc((f'{name}()', '*args', '**kwargs'),
+                                  f'Already provided item in args: {", ".join(left)}')
+
+            if fields_t:
+                if args:
+                    check_types(args, fields_t, input_exc=(f'{name}()', '*args'))
+                if kwargs:
+                    check_types(kwargs, fields_t, input_exc=(f'{name}()', '**kwargs'))
+
+            # Fill fields by defaults | args | kwargs
+            if args:
+                kwargs = dict(zip(fields, args)) | kwargs
+            [_FORCE_SET(self, k, v) for k, v in (fields | kwargs).items()]
+
+            # Call post init as in dataclass
+            if post_init := attrs.get('__post_init__'):
+                post_init(self)
+
+        new_cls = type(cls.__name__, (), attrs | type_kw)
+        # note mypy: skip static checks
+        new_cls.__repr__ = __repr__                                                 # type: ignore[method-assign, assignment]
+        new_cls.__init__ = __init__                                                 # type: ignore[misc]
+        new_cls.__eq__ = __eq__                                                     # type: ignore[method-assign, assignment]
+        return new_cls
+
+    # Decorator is not called
+    if isinstance(field_names, type) and field_func == _field_func_default and fields_t is None:
+        _cls, field_names = field_names, ()
+        return decorator(_cls)
+
+    # Decorator is called with or without parameters
+    if field_names:
+        check_types(field_names, str, input_exc=('@set_slots_defaults()', 'field_names'))
+        field_names = as_holder(field_names)
+    if field_func != _field_func_default:
+        # bug mypy: Special forms is not supported yet (https://github.com/python/mypy/issues/9773)
+        check_type(field_func, Callable, input_exc=('@set_slots_defaults()', 'field_func'))         # type: ignore[arg-type]
+    if fields_t:
+        check_type(fields_t, type, input_exc=('@set_slots_defaults()', 'fields_t'))
+    return decorator
+
+
+# Getters
+
+
+def get_cls_obj(obj: object | type) -> ClsObj:
+    """Get class and object from target class or object, as NamedTuple with cls and obj attrs
+    :arg obj:   Target object for getting
+    :return:    NamedTuple with cls and obj attrs"""
+    if obj is None:
+        return ClsObj(None, None)
+    elif isinstance(obj, type):
+        return ClsObj(obj, None)
+    return ClsObj(type(obj), obj)
+
+
+def get_cls_attr(obj: object | type, attr: str):
+    """Get class attribute from target class or object
+    :arg obj:   Target object for getting
+    :arg attr:  Class attribute name
+    :return:    Class attribute value | None (if not exists)"""
+    return None if (cls := get_cls_obj(obj).cls) is None else getattr(cls, attr)
+
+
+def get_attrs(obj: object | type, skip_parent: int = 0, skip_child: int = 0, *,
+              internal=False, dunder=False, ignored: Iterable[type] = (type, object),
+              merge: Iterable[str] = ('__annotations__', '__slots__')) -> dict[str, Any]:
+    """Get attributes by exploring method resolution order, with optional parent coerce
+    By default merges __annotations__ dict and __slots__ tuple
+    :arg obj:           Target object for getting
+    :arg skip_parent:   Classes count starting from parent to skip
+    :arg skip_child:    Classes count starting from child to skip
+    :arg internal:      Include internal attrs (starting from '_', except __dunder__)
+    :arg dunder:        Include __dunder__ attrs
+    :arg ignored:       Ignored classes (default: type and object)
+    :arg merge:         Merge provided methods values from several classes
+    :return:            Dict with attributes
+    :raise InputError:  If wrong arguments provided"""
+    if obj is None:
+        raise fmt_exc(('get_attrs()', 'obj'), must_be='not None', received='None')
+    if ignored != (type, object) and ignored:
+        check_types(ignored, type, input_exc=('get_attrs()', 'ignored'))
+
+    # Prepare MRO
+    obj_t = obj if (is_cls := isinstance(obj, type)) else type(obj)
+    mro = [x for x in type.mro(obj_t) if x not in ignored]
+
+    # Check for skip correctness
+    if (parents := len(mro)) <= (skip_total := skip_parent + skip_child):
+        if not parents:
+            raise fmt_exc(('get_attrs()', 'obj'),
+                          must_be='not ignored type', received=with_type(obj),
+                          ignored_types=f': {", ".join(x.__name__ for x in ignored)}')
+        raise fmt_exc(('get_attrs()', 'skip_parent', 'skip_child'),
+                      must_be=f'less than {parents} skipped in total',
+                      skipped=f': {skip_total} ({skip_parent = }, {skip_child = })')
+
+    # Build filtered MRO from coerced MRO and from object (if not class provided) in first order
+    mro_flt = [x.__dict__ for x in mro[skip_child:len(mro) - skip_parent]]
+    if not is_cls:
+        # bug mypy: Union[Any, Dict[Any, Any]]?..
+        mro_flt.insert(0, getattr(obj, '__dict__',                                                  # type: ignore[arg-type]
+                                  {k: v for k in obj.__dir__()
+                                   if (v := getattr(obj, k, _UNIQUE)) is not _UNIQUE}))
+    # bug mypy: Why MutableMapping?..
+    coerced: ChainMap[str, Any] = ChainMap(*mro_flt)                                                # type: ignore[arg-type]
+
+    # Filter hidden if needed
+    if dunder and internal:
+        result = dict(coerced)
+    else:
+        result = {k: v for k, v in coerced.items()
+                  if (dunder or not is_dunder(k)) and (internal or not is_internal(k))}
+
+    # Merge provided dicts or iterables
+    for k in merge:
+        if k in result and (attrs := [y for x in coerced.maps if is_holder(y := x.get(k))]):
+            if isinstance(attrs[-1], Mapping):
+                # bug mypy: Why MutableMapping?..
+                result[k] = dict(ChainMap(*attrs))                                                  # type: ignore[arg-type]
+            else:
+                # bug mypy: Optional? Type[None]?..
+                result[k] = type(attrs[-1])(dict.fromkeys(chain(*attrs[::-1])))                  # type: ignore[arg-type, misc]
+    return result
+
+
+class _GNMethod(str):
+    # bug mypy: MappingProxyType as default dict arg
+    def __new__(cls, first_or_cls, obj=_UNIQUE, attrs: dict = MappingProxyType({})):                # type: ignore[assignment]
+        inst = str.__new__(cls, obj or first_or_cls if (pair := obj != _UNIQUE) else first_or_cls)
+        inst.__dict__ |= attrs | (dict(zip(_CLS_OBJ, (first_or_cls, obj))) if pair else {})
+        return inst
+
+
+class _GNClassMethod:
+    def __init__(self, decorated):
+        self.func = decorated
+        self.args = decorated.__code__.co_argcount - 1
+
+    def __call__(self, target, *args):
+        cls_args, obj_args = args, args
+        if (received := len(args)) and received != self.args:
+            if received != self.args * 2:
+                args_names = self.func.__code__.co_varnames[1:self.args + 1]
+                must_be = (f'{self.args} (same for both) or {self.args * 2} (separately) '
+                           'provided for cls and obj') if self.args else 'no arguments'
+                raise fmt_exc((f'GetName.{self.func.__code__.co_name}()', *args_names),
+                              force_header=True, must_be=must_be,
+                              received=f'{received}: {", ".join(map(repr, args))}')
+            cls_args, obj_args = args[:self.args], args[self.args:]
+
+        cls, obj = get_cls_obj(target)
+        return _GNMethod('' if cls is None else self.func(cls, *cls_args),
+                         '' if obj is None else self.func(obj, *obj_args))
+
+    def __repr__(self):
+        return f'GetName.{self.func.__code__.co_name}'
+
+
+def _flt_std_name(target: object | type, name: str) -> str:
+    return '' if get_cls_attr(target, '__qualname__') in name else name
+
+
+@decorate_methods(_GNClassMethod)
+class _GNMethods:
+    def doc(self: Any) -> str:
+        """Get first line in __doc__ attr as name"""
+        return doc.split('\n')[0] if (doc := getattr(self, '__doc__', None)) else ''
+
+    def code(self: Any) -> str:
+        """Get __code__.co_name attr as name"""
+        return getattr(co, 'co_name', '') if (co := getattr(self, '__code__', None)) else ''
+
+    def attrs(self: Any, attrs: Iterable[str] = _GN_ATTRS) -> str:
+        """Get first from default or provided attrs as name"""
+        if attrs:
+            if attrs != _GN_ATTRS:
+                check_types(attrs, str)
+
+            for attr in attrs:
+                if result := getattr(self, attr, ''):
+                    if result := safe(str, result, _exc_=''):
+                        return result
+        return ''
+
+    def repr(self: Any) -> str:
+        """Get __str__ attr as name"""
+        return safe(self.__repr__, _res_=partial(_flt_std_name, self), _exc_='')
+
+    def str(self: Any) -> str:
+        """Get __repr__ attr as name"""
+        return safe(self.__str__, _res_=partial(_flt_std_name, self), _exc_='')
+
+
+_GN_METHODS = get_attrs(_GNMethods)
+_GN_METHODS_EMPTY = {k: _GNMethod('', '') for k in _GN_METHODS}
+_GN_POSSIBLE_PARAMS = {'possible_parameters': f': {", ".join(_GN_ORDER)}'}
+
+
+@dataclass(slots=True)
+class _GNMethodHolder:
+    value: str
+    state: bool
+    args: tuple
+    method: _GNClassMethod
+
+
+class GetName(str, _GNMethods):
+    """Get first available name from provided target using multiple configurable ways
+    By default - only first of cls and obj names will be received (full=False)
+    Order of get methods can be changed, set of all get methods names is not required
+    Any get method can be enabled/disabled by bool ('{method}', '{method}_cls', '{method}_obj')
+    Attrs get method ('attrs', 'attrs_cls', 'attrs_obj') can have names tuple instead of bool
+    If None obj provided - 'none' arg value will be returned, as GetName (if str type)
+    All get methods failed - 'unknown' arg value will be returned, as GetName (if str type)"""
+    cls: _GNMethod
+    obj: _GNMethod
+
+    def __new__(cls, obj, doc=False, code=False, attrs: bool | tuple[holder_t[str]] = True,
+                str=True, repr=True, *, full=False, order=_GN_ORDER, none='', unknown='',  # noqa
+                **kwargs):
+        """
+        :arg obj:       Target object for getting
+        :arg doc:       Enable cls and obj get method, first line in __doc__ attr as name
+        :arg code:      Enable cls and obj get method, __code__.co_name attr as name
+        :arg attrs:     Enable cls and obj get method, first from default or provided attrs as name
+        :arg str:       Enable cls and obj get method, __str__ attr as name
+        :arg repr:      Enable cls and obj get method, __repr__ attr as name
+        :arg full:      Get all enabled methods and fill (default: only first in cls and obj)
+        :arg order:     Get methods order, cls or obj required ('{method}_cls', '{method}_obj')
+        :arg none:      Return value if :arg obj: is None, typecast-ed to GetName (if str type)
+        :arg unknown:   Return value if all methods failed, typecast-ed to GetName (if str type)
+        :arg kwargs:    Enable cls or obj get method separately ('{method}_cls', '{method}_obj')"""
+
+        # Filter only methods states/args from internally used arguments
+        left = {k: v for k, v in locals().items() if k not in _GN_INTERNAL}
+        holders: dict[str, _GNMethodHolder] = {}
+        for k, method in _GN_METHODS.items():
+            value = cls._get_method_holder(k, method, left.pop(k))
+            value2 = _GNMethodHolder(value.value, value.state, value.args, value.method)  # copy
+            holders |= {f'{k}_cls': value, f'{k}_obj': value2}
+        if left:
+            raise InternalError(f'Found not used args in GetName with {obj=!r}: {left}')
+
+        # Rewrite separately (cls/obj) provided methods states/args
+        if kwargs:
+            if wrongs := {k: v for k, v in kwargs.items() if k not in holders.keys()}:
+                # bug mypy: unpacked keyword arguments is not a positional argument..
+                raise fmt_exc(('GetName()', *wrongs.keys()), **_GN_POSSIBLE_PARAMS)                 # type: ignore[arg-type]
+            for k, v in kwargs.items():
+                holders[k] = cls._get_method_holder(k, holders[k].method, v)
+
+        # Check order
+        if order != _GN_ORDER:
+            check_extra(order, _GN_ORDER, item_name='method', template='Not exists {}: ',
+                        input_exc=('GetName()', 'order', {'must_be': ''} | _GN_POSSIBLE_PARAMS))
+
+        # Return none if None target provided
+        if obj is None:
+            return cls._try_type_cast(none, full)
+
+        # Get names (all or only first in cls and obj) by enabled methods in provided order
+        first, first_cls_obj, left_set = '', dict.fromkeys(_CLS_OBJ, ''), set(_CLS_OBJ)
+        targets = get_cls_obj(obj)
+        if targets.obj is None:
+            left_set.discard('obj')
+        for method_name in order:
+            if (cls_or_obj := method_name.rsplit('_', 1)[1]) in left_set:
+                if (holder := holders[method_name]).state:
+                    if name := holder.method.func(getattr(targets, cls_or_obj), *holder.args):
+                        holder.value = name
+                        if not first:
+                            first = name
+                        if not first_cls_obj[cls_or_obj]:
+                            first_cls_obj[cls_or_obj] = name
+                        if not full:
+                            left_set.discard(cls_or_obj)
+                            if not left_set:
+                                break
+
+        # Return unknown if no name found
+        if not first:
+            return cls._try_type_cast(unknown, full)
+
+        # Fast names receive way (only first in cls and obj methods), without GetName instance fill
+        if not full:
+            methods = {k: '' for k in _GN_METHODS}
+            # note mypy: that's planned
+            return _GNMethod.__new__(cls, first, attrs=first_cls_obj | methods)                     # type: ignore[arg-type]
+
+        # GetName instance fill by first cls and obj methods and each method separately
+        methods = {k: _GNMethod(holders[f'{k}_cls'].value, holders[f'{k}_obj'].value)
+                   for k in _GN_METHODS}
+        # note mypy: that's planned
+        return _GNMethod.__new__(cls, first, attrs=first_cls_obj | methods)                         # type: ignore[arg-type]
+
+    @staticmethod
+    def _get_method_holder(k, method, value) -> _GNMethodHolder:
+        check_type(value, (bool, tuple) if method.args else bool, input_exc=('GetName()', k))
+        return _GNMethodHolder('', bool(value), value if isinstance(value, tuple) else (), method)
+
+    @classmethod
+    def _try_type_cast(cls, value, full):
+        if isinstance(value, str):
+            attrs = _GN_METHODS_EMPTY if full else {}
+            return _GNMethod.__new__(cls, value, attrs=attrs | dict.fromkeys(_CLS_OBJ, ''))  # noqa
+        return value
+
+
+# Uncategorized
+
+
+class UID:
+    """Unique ID instances used as filler for detecting by comparison"""
+    __slots__ = ('name',)
+    name: str
+    exists: list[str] = []
+
+    def __init__(self, name: str):
+        """
+        :arg name:  Unique name for ID"""
+        if (name := str(name)) in self.exists:
+            raise ValueError(f'{name!r} unique ID cannot be created, it already exists')
+        self.exists.append(name)
+        self.name = name
+
+    def __repr__(self):
+        return f'UID({self.name!r})'
+
+    def __str__(self):
+        return f'{self.name} ID'
+
+
+class Locker:
+    """Lock child class from attributes manipulations with internal unlock possibility
+    Can be unlocked during active context manager, as it finished - class will be also locked"""
+    __slots__ = ('_locker_state', '_locker_enter_state', '_locker_set_attr', '_locker_del_attr',
+                 '_locker_ignored', '_locker_name')
+    _locker_state: bool
+    _locker_enter_state: bool
+    _locker_set_attr: bool
+    _locker_del_attr: bool
+    _locker_ignored: tuple
+    _locker_name: str
+
+    def __new__(cls, *args, **kwargs):
+        obj = object.__new__(cls)
+        [_FORCE_SET(obj, *x) for x in zip(Locker.__slots__, (False, False, True, True, ()))]
+        return obj
+
+    def __init__(self, *ignored_attrs: str, set_attr=True, del_attr=True, name: str | None = None):
+        """
+        :arg ignored_attrs: Attributes names that will not be locked at all
+        :arg set_attr:      Allow __set__ unlocked attributes
+        :arg del_attr:      Allow __del__ unlocked attributes
+        :arg name:          Set locker name for error message"""
+        self._locker_ignored += ignored_attrs
+        name = f'{GetName(self)!r} object' if name is None else str(name)
+        _FORCE_SET(self, '_locker_name', name)
+        _FORCE_SET(self, '_locker_set_attr', set_attr)
+        _FORCE_SET(self, '_locker_del_attr', del_attr)
+        self._locker_state = True
+
+    @staticmethod
+    def _get_exc_msg(is_set, allowed):
+        if allowed:
+            return is_set, 'is locked for changes'
+        else:
+            return is_set, f'does not support {"setting" if is_set else "deleting"} attributes'
+
+    def _make_exc(self, is_set, msg, key, value=None):
+        op, value = ('set', f', {value!r}') if is_set else ('del', '')
+        return TypeError(f'{self._locker_name} {msg} (self.__{op}attr__({key!r}{value}))')
+
+    def is_unlocked(self, key):
+        """Get True if provided attribute is unlocked"""
+        return not self._locker_state or key in self._locker_ignored
+
+    def __setattr__(self, key, value):
+        if key in _LOCKER_IGNORED or self._locker_set_attr and self.is_unlocked(key):
+            return _FORCE_SET(self, key, value)
+        raise self._make_exc(*self._get_exc_msg(True, self._locker_set_attr), key, value)
+
+    def __delattr__(self, key):
+        if not hasattr(self, key):  # msg as at set any new attrs in slotted class
+            raise AttributeError(f'{self._locker_name} has no attribute {key!r}')
+        if key in Locker.__slots__:
+            raise self._make_exc(False, 'Locker attrs deletion is forbidden', key)
+        if self._locker_del_attr and self.is_unlocked(key):
+            return object.__delattr__(self, key)
+        raise self._make_exc(*self._get_exc_msg(False, self._locker_del_attr), key)
+
+    def __enter__(self):
+        self._locker_enter_state, self._locker_state = self._locker_state, False
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self._locker_enter_state:
+            self._locker_state = True
```

### Comparing `configlayer-0.1/configlayer.egg-info/SOURCES.txt` & `configlayer-0.1.1/configlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configlayer-0.1/tests/test_1_exceptions.py` & `configlayer-0.1.1/tests/test_1_exceptions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from typing import Callable
-from itertools import product
-from collections import ChainMap
-
-from configlayer.exceptions import InputError, FieldError
-from configlayer.utils import fmt_name, safe
-
-from _utilities import subtest
-from _data import ReprError
-
-
-def test_input_error():
-    # Args
-    exc_set = ((KeyError('1'),), (ValueError('2', 3),), (KeyError(4, 5, '6'), ValueError('7', 8)))
-    items_set = ((), ('item',), ('item1', 'item2'))
-    msg_set = ('', 'message')
-    item_name_set = ('parameter', 'item')
-    func_name_set = ('', 'func()')
-    args_set = ((), (0,), (1, 2))
-    bools = (False, True)
-
-    # Kwarg: sentences
-    sentences_values = ((), ('sentence0',), ('sentence1', 'sentence2'))
-    sentences_set = ({}, *({'sentences': v} for v in sentences_values))
-
-    # Kwargs: must_be, received
-    must_kw = {'must_be': 'there'}
-    recv_kw = {'received': 'here'}
-    must_recv_set = ({}, must_kw, recv_kw, must_kw | recv_kw, recv_kw | must_kw)
-
-    # Kwarg type: str, Mapping, tuple, other
-    simple_kw_set = ({}, {'str': 'here'}, {'func': lambda: ': there'}, {'tuple': ('e', 6)})
-
-    # All kwargs
-    kw_params = (sentences_set, must_recv_set, simple_kw_set)
-    kw_set = tuple(dict(ChainMap(*dicts)) for dicts in product(*kw_params[::-1]))
-
-    common_set = (msg_set, item_name_set, func_name_set, args_set, bools, kw_set)
-
-    # Test provided exception
-    st = subtest('Exceptions test', 11520, product(exc_set, *common_set), {'repr': 3840})
-    for i, exc, msg, item_name, func_name, args, force_header, kwargs in st:
-        recv = InputError(*exc, msg=msg, item_name=item_name, func_name=func_name, args=args,
-                          force_header=force_header, **kwargs)
-        st.send(('', recv.items, exc))
-        st.send(('', recv.msg, msg))
-        st.send(('', recv.item_name, item_name))
-        st.send(('', recv.func_name, func_name))
-        st.send(('', recv.kwargs, kwargs))
-        st.send(('', recv.must_be, recv.received, recv.header, ''))
-        st.send(('', recv.sentences, ()))
-
-        ie_args = ("; ".join(map(repr, exc)), *args)
-        result = f'InputError({repr(ie_args)[1:-1 if len(ie_args) > 1 else -2]})'
-        st.send(('repr', repr(recv), result))
-
-    # Test InputError exception
-    st = subtest('InputError test', 11520, product(items_set, *common_set),
-                 {'header': 3840, 'kwargs sentences': 20, 'repr': 80})
-    for i, items, msg, item_name, func_name, args, force_header, kwargs in st:
-        recv = InputError(*items, msg=msg, item_name=item_name, func_name=func_name, args=args,
-                          force_header=force_header, **kwargs)
-        st.send(('', recv.items, items))
-        st.send(('', recv.msg, msg))
-        st.send(('', recv.item_name, item_name))
-        st.send(('', recv.func_name, func_name))
-        st.send(('', recv.kwargs, kwargs))
-
-        # Check header
-        h_func_name = f' to {func_name}' if func_name else ''
-        header = f'Provided wrong {fmt_name(items, item_name, item_name + "(s)")}{h_func_name}'
-        if items:
-            header = f'{header}: {items[0] if len(items) == 1 else ", ".join(items)}'
-        elif force_header or h_func_name or not (msg or kwargs):
-            pass
-        else:
-            header = ''
-        st.send(('header', recv.header, header))
-
-        # Check received, must_be and sentences
-        received = must_be = ''
-        must_recv, sentences = [], []
-        for k, v in kwargs.items():
-            if k == 'sentences':
-                sentences.extend(v)
-                continue
-
-            v_str = v if isinstance(v, str) else v() if isinstance(v, Callable) else f': {v!r}'
-            if not v_str:
-                continue
-
-            sentence = f'{k.replace("_", " ")}{"" if v_str[0] in ":,." else " "}{v_str}'
-
-            if k == 'must_be':
-                must_be = v
-                must_recv.append(sentence)
-            elif k == 'received':
-                received = v
-                must_recv.append(sentence)
-            else:
-                sentences.append(sentence)
-
-        mr = ', but '.join(must_recv)
-        st.send(('', recv.received, received))
-        st.send(('', recv.must_be, must_be))
-        st.send(('received, must_be', mr, mr))  # Show only
-
-        st.send(('kwargs sentences', ' | '.join(recv.sentences), ' | '.join(sentences)))
-
-        # Check repr
-        res_msg = '. '.join(f'{x[0].upper()}{x[1:]}' for x in (header, msg, mr, *sentences) if x)
-        result = f'InputError({repr((res_msg, *args))[1:-1 if args else -2]})'
-        st.send(('', repr(recv), result))
-
-
-def test_field_error():
-    def show(x):
-        return safe(repr, x, _exc_=repr)
-
-    # Constants
-    op, cfg, field = 'change amazing used'.split()
-    defaults = ('', '', '', '', ' failed', 'config')
-    kw_names = ('to_value', 'from_value', 'by_func', 'reason', 'failed', 'type_name')
-    kw_funcs = (lambda x: f' to {show(x)!r}', lambda x: f' from {show(x)!r}', lambda x: f' by {x}',
-                lambda x: ',{} ' + x, lambda x: ' failed' if x else ' completed', lambda x: x)
-
-    # Cases dicts
-    to_values = [{'to_value': ReprError(4)}, {}, {'to_value': 'value 4'}, ]
-    from_values = [{}, {'from_value': 3}, {'from_value': ReprError(3)}]
-    by_funcs = [{}, {'by_func': 'some func'}]
-    reasons = [{}, {'reason': 'some reason'}]
-    fails = [{}, {'failed': False}]
-    type_names = [{}, {'type_name': 'language'}]
-
-    # Check
-    cases = tuple(product(to_values, from_values, by_funcs, reasons, fails, type_names))
-    for i, kwargs in (st := subtest('', 144, ([dict(ChainMap(*dicts))] for dicts in cases))):
-        # Prepare
-        data = [f(safe(kwargs.get, k)) if k in kwargs else d
-                for k, f, d in zip(kw_names, kw_funcs, defaults, strict=True)]
-        to_value, from_value, by_func, reason, failed, type_name = data
-        reason_but = "" if failed else " but"
-        msg = f"Change 'amazing' {type_name} field 'used'{from_value}{to_value}{by_func}{failed}"
-
-        # Compare
-        st.send(('', str(FieldError(op, cfg, field, **kwargs)), msg + reason.format(reason_but)))
+from typing import Callable
+from itertools import product
+from collections import ChainMap
+
+from configlayer.exceptions import InputError, FieldError
+from configlayer.utils import fmt_name, safe
+
+from _utilities import subtest
+from _data import ReprError
+
+
+def test_input_error():
+    # Args
+    exc_set = ((KeyError('1'),), (ValueError('2', 3),), (KeyError(4, 5, '6'), ValueError('7', 8)))
+    items_set = ((), ('item',), ('item1', 'item2'))
+    msg_set = ('', 'message')
+    item_name_set = ('parameter', 'item')
+    func_name_set = ('', 'func()')
+    args_set = ((), (0,), (1, 2))
+    bools = (False, True)
+
+    # Kwarg: sentences
+    sentences_values = ((), ('sentence0',), ('sentence1', 'sentence2'))
+    sentences_set = ({}, *({'sentences': v} for v in sentences_values))
+
+    # Kwargs: must_be, received
+    must_kw = {'must_be': 'there'}
+    recv_kw = {'received': 'here'}
+    must_recv_set = ({}, must_kw, recv_kw, must_kw | recv_kw, recv_kw | must_kw)
+
+    # Kwarg type: str, Mapping, tuple, other
+    simple_kw_set = ({}, {'str': 'here'}, {'func': lambda: ': there'}, {'tuple': ('e', 6)})
+
+    # All kwargs
+    kw_params = (sentences_set, must_recv_set, simple_kw_set)
+    kw_set = tuple(dict(ChainMap(*dicts)) for dicts in product(*kw_params[::-1]))
+
+    common_set = (msg_set, item_name_set, func_name_set, args_set, bools, kw_set)
+
+    # Test provided exception
+    st = subtest('Exceptions test', 11520, product(exc_set, *common_set), {'repr': 3840})
+    for i, exc, msg, item_name, func_name, args, force_header, kwargs in st:
+        recv = InputError(*exc, msg=msg, item_name=item_name, func_name=func_name, args=args,
+                          force_header=force_header, **kwargs)
+        st.send(('', recv.items, exc))
+        st.send(('', recv.msg, msg))
+        st.send(('', recv.item_name, item_name))
+        st.send(('', recv.func_name, func_name))
+        st.send(('', recv.kwargs, kwargs))
+        st.send(('', recv.must_be, recv.received, recv.header, ''))
+        st.send(('', recv.sentences, ()))
+
+        ie_args = ("; ".join(map(repr, exc)), *args)
+        result = f'InputError({repr(ie_args)[1:-1 if len(ie_args) > 1 else -2]})'
+        st.send(('repr', repr(recv), result))
+
+    # Test InputError exception
+    st = subtest('InputError test', 11520, product(items_set, *common_set),
+                 {'header': 3840, 'kwargs sentences': 20, 'repr': 80})
+    for i, items, msg, item_name, func_name, args, force_header, kwargs in st:
+        recv = InputError(*items, msg=msg, item_name=item_name, func_name=func_name, args=args,
+                          force_header=force_header, **kwargs)
+        st.send(('', recv.items, items))
+        st.send(('', recv.msg, msg))
+        st.send(('', recv.item_name, item_name))
+        st.send(('', recv.func_name, func_name))
+        st.send(('', recv.kwargs, kwargs))
+
+        # Check header
+        h_func_name = f' to {func_name}' if func_name else ''
+        header = f'Provided wrong {fmt_name(items, item_name, item_name + "(s)")}{h_func_name}'
+        if items:
+            header = f'{header}: {items[0] if len(items) == 1 else ", ".join(items)}'
+        elif force_header or h_func_name or not (msg or kwargs):
+            pass
+        else:
+            header = ''
+        st.send(('header', recv.header, header))
+
+        # Check received, must_be and sentences
+        received = must_be = ''
+        must_recv, sentences = [], []
+        for k, v in kwargs.items():
+            if k == 'sentences':
+                sentences.extend(v)
+                continue
+
+            v_str = v if isinstance(v, str) else v() if isinstance(v, Callable) else f': {v!r}'
+            if not v_str:
+                continue
+
+            sentence = f'{k.replace("_", " ")}{"" if v_str[0] in ":,." else " "}{v_str}'
+
+            if k == 'must_be':
+                must_be = v
+                must_recv.append(sentence)
+            elif k == 'received':
+                received = v
+                must_recv.append(sentence)
+            else:
+                sentences.append(sentence)
+
+        mr = ', but '.join(must_recv)
+        st.send(('', recv.received, received))
+        st.send(('', recv.must_be, must_be))
+        st.send(('received, must_be', mr, mr))  # Show only
+
+        st.send(('kwargs sentences', ' | '.join(recv.sentences), ' | '.join(sentences)))
+
+        # Check repr
+        res_msg = '. '.join(f'{x[0].upper()}{x[1:]}' for x in (header, msg, mr, *sentences) if x)
+        result = f'InputError({repr((res_msg, *args))[1:-1 if args else -2]})'
+        st.send(('', repr(recv), result))
+
+
+def test_field_error():
+    def show(x):
+        return safe(repr, x, _exc_=repr)
+
+    # Constants
+    op, cfg, field = 'change amazing used'.split()
+    defaults = ('', '', '', '', ' failed', 'config')
+    kw_names = ('to_value', 'from_value', 'by_func', 'reason', 'failed', 'type_name')
+    kw_funcs = (lambda x: f' to {show(x)!r}', lambda x: f' from {show(x)!r}', lambda x: f' by {x}',
+                lambda x: ',{} ' + x, lambda x: ' failed' if x else ' completed', lambda x: x)
+
+    # Cases dicts
+    to_values = [{'to_value': ReprError(4)}, {}, {'to_value': 'value 4'}, ]
+    from_values = [{}, {'from_value': 3}, {'from_value': ReprError(3)}]
+    by_funcs = [{}, {'by_func': 'some func'}]
+    reasons = [{}, {'reason': 'some reason'}]
+    fails = [{}, {'failed': False}]
+    type_names = [{}, {'type_name': 'language'}]
+
+    # Check
+    cases = tuple(product(to_values, from_values, by_funcs, reasons, fails, type_names))
+    for i, kwargs in (st := subtest('', 144, ([dict(ChainMap(*dicts))] for dicts in cases))):
+        # Prepare
+        data = [f(safe(kwargs.get, k)) if k in kwargs else d
+                for k, f, d in zip(kw_names, kw_funcs, defaults, strict=True)]
+        to_value, from_value, by_func, reason, failed, type_name = data
+        reason_but = "" if failed else " but"
+        msg = f"Change 'amazing' {type_name} field 'used'{from_value}{to_value}{by_func}{failed}"
+
+        # Compare
+        st.send(('', str(FieldError(op, cfg, field, **kwargs)), msg + reason.format(reason_but)))
```

### Comparing `configlayer-0.1/tests/test_2_utils.py` & `configlayer-0.1.1/tests/test_2_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1706 +1,1707 @@
-from typing import Mapping, Iterable
-from itertools import product
-from functools import partial
-
-from configlayer.types import ItemError
-from configlayer.exceptions import InputError, InitError, CheckValueError, CheckTypeError
-from configlayer.utils import (
-    is_dunder, is_internal, is_hidden, is_exception, is_holder,                     # Bool checks
-    as_holder, as_holder_stated, as_dict, as_dict_stated,                           # Type casting
-    safe, with_type,                                                                # Common
-    fmt_dict, fmt_obj_errors, fmt_name, fmt_exc,                                    # Formatters
-    split,                                                                          # Split
-    join, sentence, sentences,                                                      # Joins
-    check_input, check_lengths, check_absent, check_extra, check_items, check_type, check_types,   # Data checks
-    decorate_methods, init_reraise, set_slots_defaults,                             # Decorators
-    get_cls_obj, get_cls_attr, get_attrs, GetName,                                  # Getters
-    UID, Locker)                                                                    # Uncategorized
-
-from _utilities import raises, subtest
-from _data import increment_str, wrong_func, wrong_func_3, WrongCast
-
-
-# Bool checks
-
-
-def test_is_dunder():
-    variants = ('', '_', '__', '___')
-    data = [f'{start}name{end}' for start in variants for end in variants]
-    data.remove('__name__')
-    assert is_dunder('__name__')
-    assert not any(map(is_dunder, data))
-
-
-def test_is_internal():
-    variants = ('_', '__', '___')
-    data = [f'{start}name{end}' for start in variants for end in variants]
-    data.remove('__name__')
-    assert all(map(is_internal, data))
-    assert not is_internal('name')
-    assert not is_internal('name_')
-    assert not is_internal('name__')
-    assert not is_internal('name___')
-    assert not is_internal('__name__')
-
-
-def test_is_hidden():
-    variants = ('_', '__', '___')
-    data = [f'{start}name{end}' for start in variants for end in variants]
-    assert all(map(is_hidden, data))
-    assert not is_hidden('name')
-    assert not is_hidden('name_')
-    assert not is_hidden('name__')
-    assert not is_hidden('name___')
-    assert is_hidden('__name__')
-
-
-def test_is_exception():
-    assert is_exception(Exception)
-    assert is_exception(Exception(''))
-    assert is_exception(ValueError)
-    assert is_exception(ValueError(''))
-    assert not is_exception(Exception, ValueError)
-    assert not is_exception(Exception(''), ValueError)
-    assert not is_exception(None)
-    assert not is_exception(None, ValueError)
-
-
-def test_is_holder():
-    holder_types = tuple, list, set, dict
-    not_holder_types = bool, int, float, str, bytes, bytearray
-
-    assert is_holder(None) is None
-    assert all(is_holder(x()) for x in holder_types) is True
-    assert any(is_holder(x()) for x in not_holder_types) is False
-    assert not any(is_holder(x(), holder_types) for x in holder_types)
-
-    exc = partial(InputError, 'exclude', must_be='type or types', func_name='is_holder()')
-    raises(exc(received='5 (int)'), is_holder, 5, 5)
-    raises(exc(received='5 (int) at pos 0'), is_holder, 5, (5, int))
-    raises(exc(received="'some'='string' (str)"), is_holder, 5, {'some': 'string', 'another': str})
-
-
-# Type casting
-
-
-def test_as_holder():
-    assert as_holder(None, default=None) is None
-    assert as_holder(None, None) is None
-    assert as_holder(None, [1]) == [1]
-    assert as_holder(None) == ()
-    assert as_holder('1') == ('1',)
-    assert as_holder([]) == []
-    assert as_holder([1]) == [1]
-    assert as_holder(['1']) == ['1']
-    assert as_holder(['1'], exclude=(list,)) == (['1'],)
-
-    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
-                      received="'1' (str) at pos 1"),
-           as_holder, ['1'], exclude=(list, '1'))
-
-    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
-                      received="'1' (str) at pos 1, 2.13 (float) at pos 2"),
-           as_holder, ['1'], exclude=(list, '1', 2.13))
-
-
-def test_as_holder_stated():
-    assert as_holder_stated(None, default=None) == (None, None)
-    assert as_holder_stated(None, None) == (None, None)
-    assert as_holder_stated(None, [1]) == (None, [1])
-    assert as_holder_stated(None) == (None, ())
-    assert as_holder_stated('1') == (False, ('1',))
-    assert as_holder_stated([]) == (True, [])
-    assert as_holder_stated([1]) == (True, [1])
-    assert as_holder_stated(['1']) == (True, ['1'])
-    assert as_holder_stated(['1'], exclude=(list,)) == (False, (['1'],))
-
-    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
-                      received="'1' (str) at pos 1"),
-           as_holder_stated, ['1'], exclude=(list, '1'))
-
-    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
-                      received="'1' (str) at pos 1, 2.13 (float) at pos 2"),
-           as_holder_stated, ['1'], exclude=(list, '1', 2.13))
-
-
-def test_as_mapping():
-    def modify(x):
-        return ((str(v), v) for v in x)
-
-    raises(TypeError("'int' object is not iterable"), as_dict, 5)
-    t1 = (0, '1')
-    t2 = ('0', '1')
-    t3 = ('0',)
-    t4 = ('0', 1, 2)
-    d1 = {0: 0, 1: '1'}
-    d2 = {'0': 0, '1': '1'}
-    d3 = {'0': 0}
-    d4 = {'0': 0, 1: '1'}
-
-    # input mapping
-    assert as_dict(d1) == d1                             # -> input
-    assert as_dict(d1, modify) == d1                     # -> input
-    assert as_dict(d1, t2) == d1                         # -> input
-    assert as_dict(d1, t3) == d1                         # -> input
-    assert as_dict(d1, t4) == d1                         # -> input
-    assert as_dict(d1, t2, strict=True) == d1            # -> input
-    assert as_dict(d1, t3, strict=True) == d1            # -> input
-    assert as_dict(d1, t4, strict=True) == d1            # -> input
-
-    # input not mapping iterable
-    assert as_dict(t1) == d1                             # -> default func
-    assert as_dict(t1, modify) == d2                     # -> modify func
-    assert as_dict(t1, t2) == d2                         # -> iterable
-    assert as_dict(t1, t3) == d3                         # -> iterable less
-    assert as_dict(t1, t4) == d4                         # -> iterable more
-    assert as_dict(t1, t2, strict=True) == d2            # -> iterable strict
-    raises(ValueError, as_dict, t1, t3, strict=True)     # -> iterable strict less error
-    raises(ValueError, as_dict, t1, t4, strict=True)     # -> iterable strict more error
-
-
-def test_as_mapping_stated():
-    def modify(x):
-        return ((str(v), v) for v in x)
-
-    raises(TypeError("'int' object is not iterable"), as_dict, 5)
-    t1 = (0, '1')
-    t2 = ('0', '1')
-    t3 = ('0',)
-    t4 = ('0', 1, 2)
-    d1 = {0: 0, 1: '1'}
-    d2 = {'0': 0, '1': '1'}
-    d3 = {'0': 0}
-    d4 = {'0': 0, 1: '1'}
-
-    # input mapping
-    assert as_dict_stated(d1) == (True, d1)                      # -> input state
-    assert as_dict_stated(d1, modify) == (True, d1)              # -> input state
-    assert as_dict_stated(d1, t2) == (True, d1)                  # -> input state
-    assert as_dict_stated(d1, t3) == (True, d1)                  # -> input state
-    assert as_dict_stated(d1, t4) == (True, d1)                  # -> input state
-    assert as_dict_stated(d1, t2, strict=True) == (True, d1)     # -> input state
-    assert as_dict_stated(d1, t3, strict=True) == (True, d1)     # -> input state
-    assert as_dict_stated(d1, t4, strict=True) == (True, d1)     # -> input state
-
-    # input not mapping iterable
-    assert as_dict_stated(t1) == (False, d1)                     # -> default func state
-    assert as_dict_stated(t1, modify) == (False, d2)             # -> modify func
-    assert as_dict_stated(t1, t2) == (False, d2)                 # -> iterable
-    assert as_dict_stated(t1, t3) == (False, d3)                 # -> iterable less
-    assert as_dict_stated(t1, t4) == (False, d4)                 # -> iterable more
-    assert as_dict_stated(t1, t2, strict=True) == (False, d2)    # -> iterable strict
-    raises(ValueError, as_dict_stated, t1, t3, strict=True)      # -> iterable strict less error
-    raises(ValueError, as_dict_stated, t1, t4, strict=True)      # -> iterable strict more error
-
-
-# Common
-
-
-def test_safe():
-    assert safe(increment_str, '5') == 6
-    assert safe(wrong_func_3, 'x', y=5).args == ("Cannot change value ('x',), {'y': 5}", )
-    assert safe(increment_str, '5', _res_=increment_str) == 7
-    assert safe(increment_str, '5', _res_=55) == 55
-    assert safe(wrong_func, 'x').args == ('Wrong func!', )
-    assert safe(wrong_func, 'x', _exc_=repr) == "TypeError('Wrong func!')"
-    assert safe(wrong_func, 'x', _exc_=55) == 55
-
-
-def test_with_type():
-    assert with_type(type) == "type (type)"
-    assert with_type(5) == "5 (int)"
-    assert with_type('any') == "'any' (str)"
-
-    assert with_type(type, key1='some') == "type (type=type, key1='some')"
-    assert with_type(5, key1='some', type=0.1) == "5 (key1='some', type=int)"
-    assert with_type('any', k=0, k3=False, k2=True) == "'any' (type=str, k=0, k3=False, k2=True)"
-
-
-# Formatters
-
-
-def test_fmt_dict():
-    obj = {0: 0, 1: '1', '2': 2, 'item': 'value'}
-    fmts = (str, repr)
-    seps = ('=', ': ')
-    for i, kf, sep, vf in (st := subtest('', 8, product(fmts, seps, fmts))):
-        st.send(('', fmt_dict(obj, kf, sep, vf),
-                 tuple(f'{kf(k)}{sep}{vf(v)}' for k, v in obj.items())))
-
-
-def test_fmt_obj_errors():
-    obj = object()
-    errors = [(ItemError('1', 1, ''),), (ItemError('1', 1, ''), ItemError(2, '2', '2'))]
-    rns = ({}, {'result_name': 'some name'})
-    khs = ({}, {'key_handler': str})
-    seps = ({}, {'kv_sep': ': '})
-    bools = [False, True]
-
-    # Check all Extra - 192 cases
-    cases = product([obj], [(), *errors], [False], bools, bools, bools, rns, khs, seps)
-    for i, o, *args, rn, kh, sep in (st := subtest('All Extra', 192, cases)):
-        st.send(('', fmt_obj_errors(o, *args, **rn, **kh, **sep), (with_type(o),)))
-
-    # Check all no errors - 128 cases
-    cases = product([obj], [()], bools, bools, bools, bools, rns, khs, seps)
-    for i, o, *args, rn, kh, sep in (st := subtest('All no errors', 128, cases)):
-        st.send(('', fmt_obj_errors(o, *args, **rn, **kh, **sep), (with_type(o),)))
-
-    # Check all not holders - 64 cases
-    cases = product([obj], errors, [True], [False], bools, bools, rns, khs, seps)
-    for i, o, e, *args, r, rn, kh, sep in (st := subtest('All not holders', 64, cases)):
-        res = with_type(e[0].value, **{rn.get('result_name', 'result'): e[0].result} if r else {})
-        st.send(('', fmt_obj_errors(o, e, *args, r, **rn, **kh, **sep), (res,)))
-
-    # Check all mappings - 32 cases
-    cases = product([obj], errors, [True], [True], [True], bools, rns, khs, seps)
-    for i, o, e, *args, r, rn, kh, sep in (st := subtest('All mappings', 32, cases)):
-        h = kh.get('key_handler', repr)
-        s = sep.get('kv_sep', '=')
-        res = (f"{h(k)}{s}{with_type(v, **{rn.get('result_name', 'result'): info} if r else {})}"
-               for k, v, info in e)
-        st.send(('', fmt_obj_errors(o, e, *args, r, **rn, **kh, **sep), tuple(res)))
-
-    # Check all left (not mapping holder that has errors and exists) - 32 cases
-    cases = product([obj], errors, [True], [True], [False], bools, rns, khs, seps)
-    for i, o, e, *args, r, rn, kh, sep in (st := subtest('All left', 32, cases)):
-        res = tuple(f"{with_type(v)} at pos {i}" + (f' ({info})' if r else '') for i, v, info in e)
-        st.send(('', fmt_obj_errors(o, e, *args, r, **rn, **kh, **sep), res))
-
-
-def test_fmt_name():
-    for results, kwargs in [
-        ('items item items',        {}),
-        ('params param params',     {'item_name': 'param'}),
-        ('param item items',        {'default': 'param'}),
-        ('param(s) param params',   {'item_name': 'param', 'default': 'param(s)'})
-    ]:
-        for obj, result in zip([(), ['a'], {'b': '1', 'c': 0}], results.split(), strict=True):
-            assert fmt_name(obj, **kwargs) == result
-
-
-def test_fmt_exc():
-    msg_set = ('', 'some message')
-    exc_set = (Exception, TypeError)
-    args_set = ((), (0,), (1, 2))
-    kwargs_set = ({}, {'str': 'here'}, {'sentences': ('msg1', 'msg2'), 'dict': {'k1': 1, 'k2': 2}})
-
-    def_set = (msg_set, exc_set, args_set, kwargs_set)
-
-    name_set = ('', 'name')
-    n_args_set = ((), ('arg',), ('arg1', 'arg2'))
-    in_kw_set = ((), *((x,) for x in kwargs_set))
-    input_exc_set = [(n, *a, *k) for n, a, k in product(name_set, n_args_set, in_kw_set)]
-
-    # Check default error exception, fixed empty input_exc param
-    st = subtest('Default exception', 36, product(*def_set))
-    for i, msg, exc, args, kwargs in st:
-        recv_exc = fmt_exc((), msg, exc, *args, **kwargs)
-
-        exc_msg = InputError(msg=msg, **kwargs).args[0] if kwargs else msg
-        wait_exc = exc(exc_msg, *args) if exc_msg else exc(*args)
-
-        st.send(('', type(recv_exc), exc))
-        r_msg, *r_left = recv_exc.args or ('',)
-        w_msg, *w_left = wait_exc.args or ('',)
-        st.send(('Message or arg - args[0]', r_msg, w_msg))
-        st.send(('', r_left, w_left))
-
-    # Check input error exception
-    st = subtest('Input exception', 864, product(input_exc_set, *def_set),
-                  {'Message - args[0]': 144})
-    for i, input_exc, msg, exc, args, kwargs in st:
-        recv_exc = fmt_exc(input_exc, msg, exc, *args, **kwargs)
-
-        name, *params, in_kw = (input_exc if isinstance(input_exc[-1], dict) else (*input_exc, {}))
-        in_kw |= {k: v for k, v in kwargs.items() if k not in in_kw}
-        wait_exc = InputError(*params, msg=msg, func_name=name, args=args, **in_kw)
-
-        st.send(('', type(recv_exc), InputError))
-        r_msg, *r_left = recv_exc.args
-        w_msg, *w_left = wait_exc.args
-        st.send(('Message - args[0]', r_msg, w_msg))
-        st.send(('', r_left, w_left))
-
-
-# Split
-
-
-def test_split():
-    e_value = ValueError('3')
-    data_dict = {'0': 0, '1': 1, 'E': e_value, 'T': (1, 2), 'L': [1, -1], 'F': False, 'N': None}
-    data_list = list(data_dict.values())
-
-    # support funcs
-    def to_tuples(values: Iterable[dict]):
-        return tuple(tuple(x.values()) for x in values)
-
-    # funcs for test
-    def change(x, val=1):
-        return (not x) if isinstance(x, bool) else (x + val) if isinstance(x, int) else x
-
-    def is_int_key(k, _):
-        return isinstance(k, int)
-
-    # data values (f - fixed, s - standard, m - modified)
-    fe, fn = {'E': e_value}, {'N': None}
-    s0, s1, st, sl, sf = {'0': 0}, {'1': 1}, {'T': (1, 2)}, {'L': [1, -1]}, {'F': False}
-    m0, m1, mt, ml, mf = {'0': 1}, {'1': 2}, {'T': 3}, {'L': 0}, {'F': True}
-
-    # possible bool condition results
-    b_______ = s1 | fe | st | sl, s0 | sf | fn
-    b____s__ = s1 | st | sl, s0 | fe | sf | fn
-
-    b_c_____ = s0 | s1 | fe | st | sl | sf, fn
-    b_c___m_ = m0 | m1 | fe | st | sl | mf, fn
-    b_c__s__ = s0 | s1 | st | sl | sf, fe | fn
-    b_c__sm_ = m0 | m1 | st | sl | mf, fe | fn
-    b_c_u___ = s0 | s1 | fe | st | sf, sl | fn
-    b_c_u_m_ = m0 | m1 | fe | mt | mf, ml | fn
-    b_c_us__ = s0 | s1 | st | sf, fe | sl | fn
-    b_c_usm_ = m0 | m1 | mt | mf, fe | ml | fn
-
-    b______i = b_______[::-1]
-
-    b_c____i = b_c_____[::-1]
-    b_c___mi = b_c___m_[::-1]
-    b_c_u__i = b_c_u___[::-1]
-    b_c_u_mi = b_c_u_m_[::-1]
-
-    # possible is_exception condition results
-    i_______ = fe, s0 | s1 | st | sl | sf | fn
-    i____s__ = {}, data_dict
-
-    i_c___m_ = fe, m0 | m1 | st | sl | mf | fn
-    i_c__sm_ = {}, m0 | m1 | fe | st | sl | mf | fn
-    i_c_u_m_ = fe, m0 | m1 | mt | ml | mf | fn
-    i_c_usm_ = {}, m0 | m1 | fe | mt | ml | mf | fn
-
-    i______i = i_______[::-1]
-    i_c___mi = i_c___m_[::-1]
-    i_c_u_mi = i_c_u_m_[::-1]
-
-    # defaults test
-    assert split(data_dict) == b_______
-    assert split(data_list) == to_tuples(b_______)
-
-    # general params tests
-    conditions = (bool, is_exception)
-    funcs = (None, change)
-    bool_keys = ('unpack', 'safely', 'modify', 'cond_invert')[::-1]
-    bool_kwargs = [dict(zip(bool_keys, x)) for x in product((False, True), repeat=len(bool_keys))]
-    for i, (args, results) in enumerate(zip(product(conditions, funcs), [
-        (b_______, b_______, b____s__, b____s__, b_______, b_______, b____s__, b____s__,
-         b______i, b______i, b______i, b______i, b______i, b______i, b______i, b______i),
-        (b_c_____, b_c_u___, b_c__s__, b_c_us__, b_c___m_, b_c_u_m_, b_c__sm_, b_c_usm_,
-         b_c____i, b_c_u__i, b_c____i, b_c_u__i, b_c___mi, b_c_u_mi, b_c___mi, b_c_u_mi),
-        (i_______, i_______, i____s__, i____s__, i_______, i_______, i____s__, i____s__,
-         i______i, i______i, i______i, i______i, i______i, i______i, i______i, i______i),
-        (i_______, i_______, i____s__, i____s__, i_c___m_, i_c_u_m_, i_c__sm_, i_c_usm_,
-         i______i, i______i, i______i, i______i, i_c___mi, i_c_u_mi, i_c___mi, i_c_u_mi)
-    ], strict=True)):
-        for j, (kwargs, expected) in enumerate(zip(bool_kwargs, results, strict=True)):
-            try:
-                assert split(data_dict, *args, **kwargs) == expected
-                assert split(data_list, *args, **kwargs) == to_tuples(expected)
-                vs, ws = split(data_list, *args, as_dicts=True, **kwargs)
-                ve, we = expected
-                assert all(isinstance(x, int) for x in tuple(vs.keys()) + tuple(ws.keys()))
-                assert tuple(vs.values()) == tuple(ve.values())
-                assert tuple(ws.values()) == tuple(we.values())
-            except Exception:
-                raise Exception(f"{i=} ({args = }), {j=} ({kwargs = })")
-
-    # cond_key and cond_value params test
-    e_kv____ = InputError('cond_key', 'cond_value', must_be='at least one True or not filled',
-                          func_name='split()', received='cond_key = False, cond_value = False')
-    b__vl___ = to_tuples(b_______)
-    b_k_d___ = (data_dict, {})
-    b_k_l___ = to_tuples((s1 | fe | st | sl | sf | fn, s0))
-    for (key, value), expected in zip(product((None, False, True), repeat=2), (
-        (b_______, b__vl___),                         # None  None  -> False, True
-        (b_k_d___, b_k_l___),                         # None  False -> True, False
-        (b_______, b__vl___),                         # None  True  -> False, True
-        (b_______, b__vl___),                         # False None  -> False, True
-        e_kv____,                                     # False False -> False, False (error)
-        (b_______, b__vl___),                         # False True  -> False, True
-        (b_k_d___, b_k_l___),                         # True  None  -> True, False
-        (b_k_d___, b_k_l___),                         # True  False -> True, False
-        (({}, data_dict), (tuple(data_list), ()))     # True  True  -> True,  True  (both)
-    ), strict=True):
-        if is_exception(expected):
-            raises(expected, split, data_dict, cond_key=key, cond_value=value)
-            raises(expected, split, data_list, cond_key=key, cond_value=value)
-        else:
-            args = (is_int_key,) if key == value and key is True else ()
-            assert split(data_dict, *args, cond_key=key, cond_value=value) == expected[0]
-            assert split(data_list, *args, cond_key=key, cond_value=value) == expected[1]
-
-
-# Joins
-
-join_dataset = [(0, '', 1, False),
-                (0, 'here is a sTrAnGe STRING', 1, False),
-                ('here is', 0, 'a sTrAnGe STRING', 1, False),
-                (None, 'here is', 0, 'a', False, 'sTrAnGe STRING', 1)]
-
-
-def _join_tests(func, results_set, sep=', '):
-    for typecast in True, False:
-        for skip_false, results in zip((True, False), results_set, strict=True):
-            kwargs = {'sep': sep, 'typecast': typecast, 'skip_false': skip_false}
-            for args, result in zip(join_dataset, results, strict=True):
-                if typecast:
-                    assert func(*args, **kwargs) == sep.join(result)
-                else:
-                    raises(TypeError, func, *args, **kwargs)
-
-
-def test_join():
-    results = ([('1',),
-                ('here is a sTrAnGe STRING', '1'),
-                ('here is', 'a sTrAnGe STRING', '1'),
-                ('here is', 'a', 'sTrAnGe STRING', '1')],
-               [('0', '', '1', 'False'),
-                ('0', 'here is a sTrAnGe STRING', '1', 'False'),
-                ('here is', '0', 'a sTrAnGe STRING', '1', 'False'),
-                ('None', 'here is', '0', 'a', 'False', 'sTrAnGe STRING', '1')])
-    _join_tests(join, results)
-
-
-def test_sentence():
-    results = ([('1',),
-                ('Here is a sTrAnGe STRING', '1'),
-                ('Here is', 'a sTrAnGe STRING', '1'),
-                ('Here is', 'a', 'sTrAnGe STRING', '1')],
-               [('0', '', '1', 'False'),
-                ('0', 'here is a sTrAnGe STRING', '1', 'False'),
-                ('Here is', '0', 'a sTrAnGe STRING', '1', 'False'),
-                ('None', 'here is', '0', 'a', 'False', 'sTrAnGe STRING', '1')])
-    _join_tests(sentence, results, ' ')
-
-
-def test_sentences():
-    results = ([('1',),
-                ('Here is a sTrAnGe STRING', '1'),
-                ('Here is', 'A sTrAnGe STRING', '1'),
-                ('Here is', 'A', 'STrAnGe STRING', '1')],
-               [('0', '', '1', 'False'),
-                ('0', 'Here is a sTrAnGe STRING', '1', 'False'),
-                ('Here is', '0', 'A sTrAnGe STRING', '1', 'False'),
-                ('None', 'Here is', '0', 'A', 'False', 'STrAnGe STRING', '1')])
-    _join_tests(sentences, results, '. ')
-
-
-# Data checks
-
-
-def test_check_input():
-    exc = CheckValueError
-    raises(exc("Item is needed, but not provided"), check_input, None, 1)
-    raises(exc("Item is not needed, but provided"), check_input, 1, None)
-    raises(exc("Some is needed, but not provided"), check_input, None, 1, 'Some')
-    raises(exc("Some is not needed, but provided"), check_input, 1, None, 'Some')
-    raises(exc("Is not needed, but provided"), check_input, 1, None, '')
-    raises(exc("- not"), check_input, 1, None, template='{2}-{1}')
-    assert check_input(None, None) is False
-    assert check_input(False, False) is True
-
-    exc1 = InputError('name1', msg="Some is not needed, but provided")
-    exc2 = InputError(msg="Some is not needed, but provided", func_name='str()')
-    raises(exc1, check_input, 1, None, 'Some', input_exc=('', 'name1'))
-    raises(exc2, check_input, 1, None, 'Some', input_exc=('str()',))
-    assert check_input(1, 1, 'Some', input_exc=('str()',))
-
-
-def test_check_extra():
-    exc = CheckValueError
-    vals = (1, '2', 3), [1]
-    add = ". Must be not more than expected (1), but received: 1, '2', 3"
-    raises(exc("Extra item: 2. Must be not more than expected (1), but received: 1, 2"),
-           check_extra, (1, 2), [1])
-    raises(exc("Extra items: '2', 3" + add), check_extra, *vals)
-    raises(exc("Extra vals: '2', 3" + add), check_extra, *vals, 'val')
-    raises(exc("E\n\t'2'\n\t3" + add), check_extra, *vals, template='E\n\t', item_sep='\n\t')
-    raises(exc("E items: '2' 3" + add), check_extra, *vals, template='E {}: ', item_sep=' ')
-    raises(exc("E items('2',3)" + add), check_extra, *vals, template='E {}({})', item_sep=',')
-    raises(exc("E xs('2',3)" + add), check_extra, *vals, 'x', template='E {}({})', item_sep=',')
-    raises(exc("E x('2',3)" + add), check_extra, *vals, '', template='E x{}({})', item_sep=',')
-
-    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
-                      func_name='check_extra()'),
-           check_extra, *vals, template='{}{}{}')     # with error
-    assert check_extra([1], (1, 2), template='{}{}{}')  # without error, but more pythonic
-
-    assert check_extra(*vals, as_text=True) == "Extra items: '2', 3" + add
-    assert check_extra((1, 2), (1, 2), as_text=True) == ""
-    assert check_extra((1, 2), (1, 2)) == (1, 2)
-
-    exc_inp = InputError('name1', msg="Extra items: '2', 3" + add)
-    raises(exc_inp, check_extra, *vals, input_exc=('', 'name1'))
-    assert check_extra(*vals, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
-
-    msg = "Extra strs: 2, 3. Must be not more than expected (1), but received: 1, 2, 3"
-    raises(exc(msg), check_extra, *vals, 'str', str)
-    raises(exc(msg + ". Some x"), check_extra, *vals, 'str', str, some='x')
-
-
-def test_check_absent():
-    exc = CheckValueError
-    vals = [1], (1, '2', 3)
-    add = ". Must be not less than expected (1, '2', 3), but received: 1"
-    raises(exc("Absent item: 2. Must be not less than expected (1, 2), but received: 1"),
-           check_absent, [1], (1, 2))
-    raises(exc("Absent items: '2', 3" + add), check_absent, *vals)
-    raises(exc("Absent vals: '2', 3" + add), check_absent, *vals, 'val')
-    raises(exc("A\n\t'2'\n\t3" + add), check_absent, *vals, template='A\n\t', item_sep='\n\t')
-    raises(exc("A items: '2' 3" + add), check_absent, *vals, template='A {}: ', item_sep=' ')
-    raises(exc("A items('2',3)" + add), check_absent, *vals, template='A {}({})', item_sep=',')
-    raises(exc("A xs('2',3)" + add), check_absent, *vals, 'x', template='A {}({})', item_sep=',')
-    raises(exc("A x('2',3)" + add), check_absent, *vals, '', template='A x{}({})', item_sep=',')
-
-    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
-                      func_name='check_absent()'),
-           check_absent, *vals, template='{}{}{}')        # with error
-    assert check_absent((1, 2), [1], template='{}{}{}')     # without error, but more pythonic
-
-    assert check_absent(*vals, as_text=True) == "Absent items: '2', 3" + add
-    assert check_absent((1, 2), [1], as_text=True) == ""
-    assert check_absent((1, 2), [1]) == (1, 2)
-
-    exc_inp = InputError('name1', msg="Absent items: '2', 3" + add)
-    raises(exc_inp, check_absent, *vals, input_exc=('', 'name1'))
-    assert check_absent(*vals, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
-
-    msg = "Absent strs: 2, 3. Must be not less than expected (1, 2, 3), but received: 1"
-    raises(exc(msg), check_absent, *vals, 'str', str)
-    raises(exc(msg + ". Some x"), check_absent, *vals, 'str', str, some='x')
-
-
-def test_check_items():
-    exc = CheckValueError
-    add1 = ". Must be equal to expected (1), but received: 1, '2', 3"
-    raises(exc("Extra item: 2. Must be equal to expected (1), but received: 1, 2"),
-           check_items, (1, 2), [1])
-    raises(exc("Extra items: '2', 3" + add1), check_items, (1, '2', 3), [1])
-    raises(exc("Extra vals: '2', 3" + add1), check_items, (1, '2', 3), [1], 'val')
-
-    add2 = ". Must be equal to expected (1, '2', 3), but received: 1"
-    raises(exc("Absent item: 2. Must be equal to expected (1, 2), but received: 1"),
-           check_items, [1], (1, 2))
-    raises(exc("Absent items: '2', 3" + add2), check_items, [1], (1, '2', 3))
-    raises(exc("Absent vals: '2', 3" + add2), check_items, [1], (1, '2', 3), 'val')
-
-    msg = "Extra item: 2. Absent item: 3"
-    raises(exc(msg + ". Must be equal to expected (3), but received: 2"), check_items, [2], [3])
-    raises(exc(msg + ". Must be equal to expected (1, 3), but received: 1, 2"),
-           check_items, (1, 2), (1, 3))
-
-    eav = (1, '2', 4), (1, '3', 5)
-    add3 = ". Must be equal to expected (1, '3', 5), but received: 1, '2', 4"
-    add4 = ". Must be equal to expected (1, 3, 5), but received: 1, 2, 4"
-    msg = "Extra items: '2', 4. Absent items: '3', 5"
-    msg2 = ("Extra items: 2, 4. Absent items: 3, 5. "
-            "Must be equal to expected (3, 5), but received: 2, 4")
-    raises(exc(msg2), check_items, (2, 4), (3, 5))
-    raises(exc(msg + add3), check_items, *eav)
-
-    raises(exc("Extra vals: '2', 4. Absent vals: '3', 5" + add3), check_items, *eav, 'val')
-
-    raises(exc("Extra strs: 2, 4. Absent strs: 3, 5" + add4), check_items, *eav, 'str', str)
-    raises(exc("Extra strs: 2, 4. Absent strs: 3, 5" + add4 + ". Some x"),
-           check_items, *eav, 'str', str, some='x')
-
-    raises(exc("E:\n\t'2'\n\t4\nA:\n\t'3'\n\t5" + add3), check_items, *eav,
-           extra_template='E:\n\t', absent_template='A:\n\t', check_sep='\n', item_sep='\n\t')
-    raises(exc("E items: '2' 4 | A items: '3' 5" + add3), check_items, *eav,
-           extra_template='E {}: ', absent_template='A {}: ', check_sep=' | ', item_sep=' ')
-    raises(exc("E items('2',4) | A items('3',5)" + add3), check_items, *eav,
-           extra_template='E {}({})', absent_template='A {}({})', check_sep=' | ', item_sep=',')
-    raises(exc("E coords('2',4) | A coords('3',5)" + add3), check_items, *eav, 'coord',
-           extra_template='E {}({})', absent_template='A {}({})', check_sep=' | ', item_sep=',')
-    raises(exc("E coord('2',4) | A coord('3',5)" + add3), check_items, *eav, '',
-           extra_template='E coord{}({})', absent_template='A {}coord({})', check_sep=' | ',
-           item_sep=',')
-
-    # Template error
-    exc = partial(InputError, must_be='not more than 2 data places', received="'{}{}{}'",
-                  func_name='check_items()')
-    error = exc('extra_template')
-    raises(error, check_items, (1, 2), (1, 3), extra_template='{}{}{}')
-    raises(error, check_items, (1, 2), (1, 3), extra_template='{}{}{}', absent_template='{}{}')
-    error = exc('absent_template')
-    raises(error, check_items, (1, 2), (1, 3), absent_template='{}{}{}')
-    raises(error, check_items, (1, 2), (1, 3), extra_template='{}{}', absent_template='{}{}{}')
-
-    # Without error, but more pythonic
-    assert check_items([1], [1], extra_template='{}{}{}')
-    assert check_items([1], [1], absent_template='{}{}{}')
-    assert check_items([1], [1], extra_template='{}{}{}', absent_template='{}{}')
-    assert check_items([1], [1], extra_template='{}{}', absent_template='{}{}{}')
-    assert check_items([1], [1], extra_template='{}{}{}', absent_template='{}{}{}')
-
-    extra_msg = "Extra items: '2', 4"
-    absent_msg = "Absent items: '3', 5"
-    add_extra = ". Must be not more than expected (1, '3', 5), but received: 1, '2', 4"
-    add_absent = ". Must be not less than expected (1, '3', 5), but received: 1, '2', 4"
-    assert check_items(*eav, as_text=True) == f'{extra_msg}. {absent_msg}' + add3
-    assert check_items(*eav, as_text=True, extra=False) == absent_msg + add_absent
-    assert check_items(*eav, as_text=True, absent=False) == extra_msg + add_extra
-    assert check_items(*eav, as_text=True, extra=False, absent=False) == ""
-    assert check_items(*eav, extra=False, absent=False) == (1, '2', 4)
-    assert check_items((1, 2), (1, 2), as_text=True) == ""
-    assert check_items((1, 2), (1, 2)) == (1, 2)
-
-    exc_inp = InputError('name1', msg=f'{extra_msg}. {absent_msg}' + add3)
-    raises(exc_inp, check_items, *eav, input_exc=('', 'name1'))
-    assert check_items(*eav, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
-
-
-def test_check_lengths():
-    assert check_lengths([1], [1])
-    assert check_lengths([2], [3])
-    assert check_lengths((1, 2, 4), (1, 3, 5))
-    exc = CheckValueError
-    ev = (1, '2', 3), [1]
-    av = ev[::-1]
-
-    # Extra values length
-    add1 = ". Must be 1 value long, but received 3"
-    raises(exc("Extra value: 2. Must be 1 value long, but received 2"),
-           check_lengths, (1, 2), [1])
-    raises(exc("Extra vals: '2', 3. Must be 1 val long, but received 3"),
-           check_lengths, *ev, 'val')
-    raises(exc("Extra values: '2', 3" + add1),
-           check_lengths, *ev)
-
-    raises(exc("E\n\t'2'\n\t3" + add1),
-           check_lengths, *ev, extra_template='E\n\t', item_sep='\n\t')
-    raises(exc("E values: '2' 3" + add1),
-           check_lengths, *ev, extra_template='E {}: ', item_sep=' ')
-    raises(exc("E values('2',3)" + add1),
-           check_lengths, *ev, extra_template='E {}({})', item_sep=',')
-    raises(exc("E xs('2',3). Must be 1 x long, but received 3"),
-           check_lengths, *ev, 'x', extra_template='E {}({})', item_sep=',')
-    raises(exc("E x('2',3). Must be 1  long, but received 3"),
-           check_lengths, *ev, '', extra_template='E x{}({})', item_sep=',')
-
-    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
-                      func_name='check_lengths()'),
-           check_lengths, *ev, extra_template='{}{}{}')  # with error
-
-    assert check_lengths(*ev, as_text=True) == "Extra values: '2', 3" + add1
-    assert check_lengths([1], (1, 2), absent=False, as_text=True) == ""
-    assert check_lengths([1], (1, 2), absent=False) == [1]
-
-    exc_inp = InputError('name1', msg="Extra values: '2', 3" + add1)
-    raises(exc_inp, check_lengths, *ev, input_exc=('', 'name1'))
-    assert check_lengths(*ev, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
-
-    raises(exc("Extra strs: 2, 3. Must be 1 str long, but received 3"),
-           check_lengths, *ev, 'str', str)
-    raises(exc("Extra strs: 2, 3. Must be 1 str long, but received 3. Some x"),
-           check_lengths, *ev, 'str', str, some='x')
-
-    # Absent values length
-    add2 = ". Must be 3 values long, but received 1"
-    raises(exc("Absent value: 2. Must be 2 values long, but received 1"),
-           check_lengths, [1], (1, 2))
-    raises(exc("Absent vals: '2', 3. Must be 3 vals long, but received 1"),
-           check_lengths, *av, 'val')
-    raises(exc("Absent values: '2', 3" + add2),
-           check_lengths, *av)
-    raises(exc("A\n\t'2'\n\t3" + add2),
-           check_lengths, *av, absent_template='A\n\t', item_sep='\n\t')
-    raises(exc("A values: '2' 3" + add2),
-           check_lengths, *av, absent_template='A {}: ', item_sep=' ')
-    raises(exc("A values('2',3)" + add2),
-           check_lengths, *av, absent_template='A {}({})', item_sep=',')
-    raises(exc("A xs('2',3). Must be 3 xs long, but received 1"),
-           check_lengths, *av, 'x', absent_template='A {}({})', item_sep=',')
-    raises(exc("A x('2',3). Must be 3  long, but received 1"),
-           check_lengths, *av, '', absent_template='A x{}({})', item_sep=',')
-
-    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
-                      func_name='check_lengths()'),
-           check_lengths, *av, absent_template='{}{}{}')     # with error
-
-    assert check_lengths(*av, as_text=True) == "Absent values: '2', 3" + add2
-    assert check_lengths((1, 2), [1], extra=False,  as_text=True) == ""
-    assert check_lengths((1, 2), [1], extra=False) == (1, 2)
-
-    exc_inp = InputError('name1', msg="Absent values: '2', 3" + add2)
-    raises(exc_inp, check_lengths, *av, input_exc=('', 'name1'))
-    assert check_lengths(*av, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
-
-    raises(exc("Absent strs: 2, 3. Must be 3 strs long, but received 1"),
-           check_lengths, *av, 'str', str)
-    raises(exc("Absent strs: 2, 3. Must be 3 strs long, but received 1. Some x"),
-           check_lengths, *av, 'str', str, some='x')
-
-    # Wrong template (without error, but more pythonic)
-    assert check_lengths([0], [0], extra_template='{}{}{}')
-    assert check_lengths([1], [1], absent_template='{}{}{}')
-    assert check_lengths([0], [1], extra_template='{}{}{}', absent_template='{}{}')
-    assert check_lengths([1], [0], extra_template='{}{}', absent_template='{}{}{}')
-    assert check_lengths([2], [3], extra_template='{}{}{}', absent_template='{}{}{}')
-
-
-def test_check_type():
-    # Check simple
-    assert check_type('some', str) == 'some'
-    raises(InputError('obj_t', must_be='type or types', received="'int' (str)",
-                      func_name='check_type()'),
-           check_type, 'some', 'int')
-
-    # Check with typecast if enabled
-    assert check_type('5', int, True) == check_type('5', int, typecast=True) == 5
-    assert check_type('some', (int, tuple), True) == ('s', 'o', 'm', 'e')
-
-    # Format error
-    raises(CheckTypeError("'some' (str) must be int type"), check_type, 'some', int)
-
-    assert isinstance(exc1 := safe(int, 'some'), ValueError)
-    raises(CheckTypeError(f"'some' (str) must be int type, typecast to int: {exc1!r}"),
-           check_type, 'some', int, True)
-
-    assert isinstance(exc2 := safe(dict, 'some'), ValueError)
-    msg = (f"'some' (str) must be int or dict types, typecast to int: {exc1!r}, "
-           f"typecast to dict: {exc2!r}")
-    raises(CheckTypeError(msg), check_type, 'some', (int, dict), True)
-
-    field_error = CheckTypeError('Field ' + msg)
-    raises(field_error, check_type, 'some', (int, dict), True, 'field')
-    raises(field_error, check_type, 'some', (int, dict), typecast=True, name='field')
-
-
-def test_check_types():
-    # Check mutually exclusive input parameters
-    raises(InputError('one_obj', 'pairs', must_be='not more than one True', received='both',
-                      func_name='check_types()'),
-           check_types, (), None, one_obj=True, pairs=True)
-
-    # Check input obj
-    obj_error = partial(InputError, 'obj', must_be='one or more objects without None',
-                        func_name='check_types()')
-    raises(obj_error(received="obj = None (objects = ())"), check_types, None, None)
-    raises(obj_error(received="obj = ()"), check_types, (), None)
-    raises(obj_error(received="obj = (<class 'tuple'>, None)"), check_types, (tuple, None), None)
-
-    # Check input obj_t
-    obj_t_error = partial(InputError, 'obj_t', must_be='type or types', func_name='check_types()')
-    raises(obj_t_error(received="() (tuple)"), check_types, 1, ())
-    raises(obj_t_error(received="None (NoneType)"), check_types, 1, None)
-    raises(obj_t_error(received="5 (int)"), check_types, 5, 5)
-    raises(obj_t_error(received="5 (int) at pos 0"), check_types, 5, (5, int))
-    raises(obj_t_error(received="5 (int) at pos 1"), check_types, 5, (int, 5))
-    raises(obj_t_error(received="5 (int) at pos 0, True (bool) at pos 3"),
-           check_types, 5, (5, int, str, True))
-
-    # Check typecast specific
-    msg = ("5 (int) must be WrongCast or tuple types, "
-           "typecast to WrongCast: 5 (int), "
-           "typecast to tuple: TypeError(\"'int' object is not iterable\")")
-    raises(CheckTypeError(msg), check_types, 5, (WrongCast, tuple), True)
-
-    # Check dicts specific
-    msg = "Extra key (without type): '2'. Absent keys (type provided): '3', '4'"
-    raises(InputError('obj', msg=msg, func_name='check_types()'),
-           check_types, {'1': 1, '2': 2}, {'1': int, '3': str, '4': str})
-
-    # Check pairs specific
-    msg = "Extra value (without type): '13'. Must be 1 value long, but received 2"
-    raises(InputError('obj', msg=msg, func_name='check_types()'),
-           check_types, (5, '13'), str, pairs=True)
-
-    # Check error in single objects
-    raises(CheckTypeError("5 (int) must be str type"), check_types, 5, str)
-    raises(CheckTypeError("5 (int) must be str or bool types"), check_types, 5, (str, bool))
-    raises(CheckTypeError("5 (int) at pos 0 must be str type"), check_types, (5, 'x'), str)
-    raises(CheckTypeError("5 (int) at pos 0 must be str or bool types"),
-           check_types, (5, 'x'), (str, bool))
-
-    # Check errors in multiple positional objects
-    msg = "Several objects are not bool type: 5 (int) at pos 0, 'x' (str) at pos 1"
-    raises(CheckTypeError(msg), check_types, (5, 'x'), bool)
-
-    msg = "Several objects are not bool or float types: 5 (int) at pos 0, 'x' (str) at pos 1"
-    raises(CheckTypeError(msg), check_types, (5, 'x'), (bool, float))
-
-    msg = ("Several objects has a wrong type:\n"
-           "\t5 (int) at pos 0 must be bool type\n"
-           "\t'x' (str) at pos 1 must be float type")
-    raises(CheckTypeError(msg), check_types, (5, 'x'), (bool, float), pairs=True)
-
-    msg = ("Several objects has a wrong type:\n"
-           "\t5 (int) at pos 0 must be bool type\n"
-           "\t'x' (str) at pos 1 must be float type")
-    raises(CheckTypeError(msg), check_types, (5, 'x'), {1: bool, 2: float}, pairs=True)
-
-    # Check errors in multiple named objects
-    dict_item, dict_items = {'name1': 5}, {'name1': 5, 2: '3'}
-    raises(CheckTypeError("'name1'=5 (int) must be str type"), check_types, dict_item, str)
-
-    msg = ("'name1'=5 (int) must be WrongCast or tuple types, "
-           "typecast to WrongCast: 5 (int), "
-           "typecast to tuple: TypeError(\"'int' object is not iterable\")")
-    raises(CheckTypeError(msg), check_types, dict_item, (WrongCast, tuple), True)
-
-    msg = "Several objects are not bool type: 'name1'=5 (int), 2='3' (str)"
-    raises(CheckTypeError(msg), check_types, dict_items, bool)
-
-    msg = ("Several objects has a wrong type:\n"
-           "\tname1: 5 (int) must be bool type\n"
-           "\t2: '3' (str) must be float type")
-    raises(CheckTypeError(msg), check_types, dict_items, (bool, float), pairs=True)
-
-    msg = ("Several objects has a wrong type:\n"
-           "\tname1: 5 (int) must be bool type\n"
-           "\t2: '3' (str) must be float type")
-    raises(CheckTypeError(msg), check_types, dict_items, {2: float, 'name1': bool})
-
-    # Check named params
-    name = 'item'
-    raises(CheckTypeError("Item 'name1'=5 (int) must be str type"),
-           check_types, dict_item, str, item_name=name)
-
-    msg = ("Item 'name1'=5 (int) must be WrongCast or tuple types, "
-           "typecast to WrongCast: 5 (int), "
-           "typecast to tuple: TypeError(\"'int' object is not iterable\")")
-    raises(CheckTypeError(msg), check_types, dict_item, (WrongCast, tuple), True, item_name=name)
-
-    msg = ("Several items has a wrong type:\n"
-           "\tItem name1: 5 (int) must be bool type\n"
-           "\tItem 2: '3' (str) must be float type")
-    raises(CheckTypeError(msg), check_types, dict_items, (bool, float), pairs=True, item_name=name)
-
-    msg = "Several items are not bool type: 5 (int) at pos 0, '3' (str) at pos 1"
-    raises(CheckTypeError(msg), check_types, (5, '3'), bool, item_name=name)
-
-    msg = "Several items are not bool type: 'name1'=5 (int), 2='3' (str)"
-    raises(CheckTypeError(msg), check_types, dict_items, bool, item_name=name)
-
-    # Positive check input obj
-    assert check_types((), tuple, one_obj=True) == ()
-    assert check_types((5,), int) == (5,)
-    assert check_types((5,), tuple, one_obj=True) == (5,)
-
-    # Positive check single objects
-    assert check_types(5, (str, bool, int)) == 5
-    assert check_types(5, (str, bool, int), True) == 5
-    assert check_types('5', int, True) == 5
-
-    # Positive check multiple objects
-    test_obj = (5, 'x', False)
-    assert check_types(test_obj, str, True) == ('5', 'x', 'False')
-    assert check_types(test_obj, (str, bool, int)) == test_obj
-    assert check_types(test_obj, (str, bool, int), True, pairs=True) == ('5', True, 0)
-    assert check_types(dict_items, (str, int)) == dict_items
-    assert check_types(dict_items, (str, int), True, pairs=True) == {'name1': '5', 2: 3}
-    assert check_types(dict_items, {2: int, 'name1': str}, True) == {'name1': '5', 2: 3}  # noqa
-
-    # Positive check mutually exclusive input parameters
-    assert check_types(test_obj, (tuple,), one_obj=True, pairs=False) == test_obj
-    assert check_types(test_obj, (int, str, bool), one_obj=False, pairs=True) == test_obj
-    assert check_types(test_obj, (int, str), one_obj=False, pairs=False) == test_obj
-
-
-# Decorators
-
-
-def test_decorate_methods():
-    class Fixed(str):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    def decorator(func):  # noqa
-        return 'Processed'
-
-    @decorate_methods(decorator)
-    class Empty(Fixed):
-        attr = 1
-
-    @decorate_methods(decorator)
-    class Visible(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude=is_hidden)
-    class Hidden1(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude=('_intern', '__dnd__'))
-    class Hidden2(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude=is_internal)
-    class Internal1(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude='_intern')
-    class Internal2(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude=is_dunder)
-    class Dunder1(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude='__dnd__')
-    class Dunder2(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude=lambda x: x)
-    class NoOne(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    @decorate_methods(decorator, exclude=lambda x: '')
-    class All(Fixed):
-        attr = 1
-        def visible(self): pass
-        def _intern(self): pass
-        def __dnd__(self): pass
-
-    for cls, v_state, h_state, d_state in [(Fixed, False, False, False),
-                                           (Empty, False, False, False),
-                                           (Visible, True, False, False),
-                                           (Hidden1, True, False, False),
-                                           (Hidden2, True, False, False),
-                                           (Internal1, True, False, True),
-                                           (Internal2, True, False, True),
-                                           (Dunder1, True, True, False),
-                                           (Dunder2, True, True, False),
-                                           (NoOne, False, False, False),
-                                           (All, True, True, True)]:
-        assert cls.attr == 1
-        assert (cls.visible == 'Processed') == v_state
-        assert (cls._intern == 'Processed') == h_state
-        assert (cls.__dnd__ == 'Processed') == d_state
-
-
-def test_init_reraise():
-    class Some1:
-        @init_reraise
-        def __init__(self, *args, **kwargs):  # noqa
-            if kwargs.get('no_exception'):
-                return
-            raise ValueError('Bad')
-
-    class Some2:
-        @init_reraise
-        def __init__(self):
-            raise ValueError('Bad')
-
-    class Cat:
-        @init_reraise('animal')
-        def __init__(self):
-            raise ValueError('Bad')
-
-    class Dog:
-        """Kristy, the dog"""
-        @init_reraise('animal', doc=True)
-        def __init__(self):
-            raise ValueError('Bad')
-
-    def error(view='', *, cn='Some1', tn='class'):
-        return InitError(f"Cannot init {tn} {cn!r} (self.__init__({view}))"), ValueError('Bad')
-
-    Some1(no_exception=True)
-    raises(error(), Some1)
-    raises(error(cn='Some2'), Some2)
-    raises(error(cn='Cat', tn='animal'), Cat)
-    raises(error(cn='Kristy, the dog', tn='animal'), Dog)
-
-    for kwv, _kwargs in (('', {}), ('x=3', {'x': 3}), ('x=3, y=4', {'x': 3, 'y': 4})):
-        for v, _args in (('', ()), ('1', (1,)), ('1, 2', (1, 2))):
-            raises(error(f'{v}, {kwv}' if v and kwv else v or kwv), Some1, *_args, **_kwargs)
-
-
-def test_set_slots_defaults():
-    def deco(*args, **kwargs):
-        @set_slots_defaults(*args, **kwargs)
-        class Deco:  # noqa
-            f1 = 1
-            f2 = '2'
-        return Deco
-
-    def error(params, msg, func_name):
-        return InputError(*as_holder(params), func_name=func_name, msg=msg)
-
-    def deco_error(params, msg):
-        return error(params, msg, '@set_slots_defaults()')
-
-    def init_error(params, msg):
-        return error(params, msg, 'Deco()')
-
-    # Decorator input params error
-    raises(deco_error('field_names', '5 (int) must be str type'), deco, 5)
-    raises(deco_error('field_names', '5 (int) at pos 2 must be str type'), deco, ('x', 'y', 5))
-    raises(deco_error('field_func', '5 (int) must be Callable type'), deco, 'x', 5)
-    raises(deco_error('fields_t', '5 (int) must be type type'), deco, 'x', lambda: True, 5)
-
-    # Decorator equality with different ways of fields declaring
-    @set_slots_defaults
-    class Deco:
-        f1 = 1
-        f2 = '2'
-        f3 = lambda x: x
-    assert Deco() == deco()() == deco('f1')() == deco(('f1', 'f2'), lambda k, v: False)()
-
-    # Decorator repr validity
-    assert Deco() == eval(repr(Deco()))
-
-    # Decorated class init error
-    raises(init_error('*args', "Extra value: 'x3'. Must be 2 values long, but received 3"),
-           Deco, 'x1', 'x2', 'x3')
-    err_msg = ". Must be not more than expected ('f1', 'f2'), but received: 'f1', 'f2', 'f3'"
-    raises(init_error('**kwargs', "Extra item: 'f3'" + err_msg), Deco, f1='x1', f2='x2', f3='x3')
-
-    err_msg = 'Already provided item in args: '
-    raises(init_error(('*args', '**kwargs'), err_msg + 'f2'), Deco, 'x1', 'x2', f2='x2')
-    raises(init_error(('*args', '**kwargs'), err_msg + 'f1'), Deco, 'x1', f1='x1')
-
-    raises(init_error('*args', "'x1' (str) at pos 0 must be int type"), deco(fields_t=int), 'x1')
-    raises(init_error('**kwargs', "'f1'='x1' (str) must be int type"), deco(fields_t=int), f1='x1')
-
-
-# Getters
-
-
-def test_get_cls_obj():
-    assert get_cls_obj(None) == (None, None)
-    assert get_cls_obj(int) == (int, None)
-    assert (x := get_cls_obj(5)) == (int, 5) == (x.cls, x.obj)
-
-
-def test_get_cls_attr():
-    class Something:
-        pass
-
-    assert get_cls_attr(None, '__qualname__') is None
-    assert get_cls_attr(Something, '__qualname__') == Something.__qualname__
-    assert get_cls_attr(Something(), '__qualname__') == Something.__qualname__
-    raises(AttributeError("type object 'Something' has no attribute 'asd'"),
-           get_cls_attr, Something, 'asd')
-
-
-def test_get_attrs():
-    # Checked classes
-    class C1:
-        """Class 1 (base)"""
-        x1: int                                                                      # type: ignore
-        x2: int = 12                                                                 # type: ignore
-        x3 = 13
-        x6: int                                                                      # type: ignore
-        _x7: int                                                                     # type: ignore
-        _x8 = 18
-
-    class C1S:
-        """Class 1 (base, slots)"""
-        __slots__ = ('x6', '_x7')
-        x1: int                                                                      # type: ignore
-        x2: int = 12                                                                 # type: ignore
-        x3 = 13
-        x6: int                                                                      # type: ignore
-        _x7: int                                                                     # type: ignore
-        _x8 = 18
-
-    class C2(C1):
-        """Class 2 (inherited)"""
-        x1 = 21
-        x2 = 22
-        x4 = 24
-        x5: int = 25                                                                 # type: ignore
-
-        def __init__(self, x6=36, x7=37, x9=39):
-            self.x6 = x6
-            self._x7 = x7
-            self.x9 = x9
-
-    class C2S(C1S):
-        """Class 2 (inherited, slots)"""
-        __slots__ = ('x9',)
-        x1 = 21
-        x2 = 22
-        x4 = 24
-        x5: int = 25                                                                 # type: ignore
-
-        def __init__(self, x6=36, x7=37, x9=39):
-            self.x6 = x6
-            self._x7 = x7
-            self.x9 = x9
-
-    # Skip args check
-    def skip_recv(total: int, parent: int, child: int):
-        return {'must_be': f'less than {total} skipped in total',
-                'skipped': f': {total} (skip_parent = {parent}, skip_child = {child})'}
-
-    exc = partial(InputError, 'skip_parent', 'skip_child', func_name='get_attrs()')
-    raises(exc(**skip_recv(2, 2, 0)), get_attrs, C2, 2)
-    raises(exc(**skip_recv(2, 1, 1)), get_attrs, C2, 1, 1)
-    raises(exc(**skip_recv(3, 3, 0)), get_attrs, C2, 3, ignored=())
-    raises(exc(**skip_recv(3, 2, 1)), get_attrs, C2, 2, 1, ignored=())
-
-    exc2 = InputError('ignored', func_name='get_attrs()', msg="1 (int) at pos 0 must be type type")
-    raises(exc2, get_attrs, C2, ignored=(1,))
-
-    # Helper functions
-    def merge_common(x, y, attrs=('__annotations__', '__slots__')) -> dict:
-        return {attr: (xa | ya if isinstance(xa or ya, Mapping) else (*xa, *ya)) for attr in attrs
-                if (xa := getattr(x, attr, {}), ya := getattr(y, attr, {})) and xa or ya}
-
-    def dict_build(obj) -> dict:
-        return {k: getattr(obj, k, None) for k in obj.__dir__()}
-
-    # Helper base objects
-    co = object                 # class <object>
-    cod = co.__dict__           # class <object> dict
-
-    ct = type                   # class <type>
-    ctd = cod | type.__dict__   # class <type> dict (type is inherited from object!)
-    cta = {'mro': type.mro}     # class <type> attributes
-
-    oo = co()                   # object <object>
-    ood = dict_build(oo)        # object <object> dict
-
-    # Helper exceptions
-    __e = partial(InputError, 'obj', must_be='not ignored type', func_name='get_attrs()',
-                  ignored_types=': type, object')
-    cte = __e(received="type (type)")
-    coe = __e(received="object (type)")
-    ooe = __e(received=f"{oo!r} (object)")
-
-    # Helper class 1 objects
-    c1_____ = {'x2': 12, 'x3': 13}      # class 1 attributes
-    c1__h__ = c1_____ | {'_x8': 18}     # class 1 internal
-    c1__hd_ = C1.__dict__               # class 1 hidden
-    c1___d_ = c1__hd_.copy()            # class 1 dunder
-    c1___d_.pop('_x8')                  # [-] remove internal
-    c1___di = cod | c1___d_             # class 1 dunder no_ignored
-    c1__hdi = cod | c1__hd_             # class 1 hidden no_ignored
-
-    o1 = C1()                           # object 1
-
-    # Helper class 1 slots objects
-    c1s____ = c1_____ | {'x6': C1S.x6}              # class 1 slots attributes
-    c1s_h__ = c1__h__ | c1s____ | {'_x7': C1S._x7}  # class 1 slots internal
-    c1s_hd_ = C1S.__dict__                          # class 1 slots hidden
-    c1s__d_ = c1s_hd_.copy()                        # class 1 slots dunder
-    c1s__d_.pop('_x7')                              # [-] remove internal
-    c1s__d_.pop('_x8')                              # [-] remove internal
-    c1s__di = cod | c1s__d_                         # class 1 slots dunder no_ignored
-    c1s_hdi = cod | c1s_hd_                         # class 1 slots hidden no_ignored
-
-    o1s = C1S()                                     # object 1 slots
-    o1s_hd_ = dict_build(o1s) | c1s_hd_             # object 1 slots hidden
-    o1s__d_ = o1s_hd_.copy()                        # object 1 slots dunder
-    o1s__d_.pop('_x7')                              # [-] remove internal
-    o1s__d_.pop('_x8')                              # [-] remove internal
-    o1s__di = cod | o1s__d_                         # object 1 slots dunder no_ignored
-    o1s_hdi = cod | o1s_hd_                         # object 1 slots hidden no_ignored
-
-    # Helper class 2 objects
-    c2_____ = c1_____ | {'x1': 21, 'x2': 22, 'x4': 24, 'x5': 25}    # class 2 attributes
-    c2__h__ = c1__h__ | c2_____                                     # class 2 internal
-    c2__hd_ = c1__hd_ | C2.__dict__ | merge_common(C1, C2)          # class 2 hidden
-    c2___d_ = c2__hd_.copy()                                        # class 2 dunder
-    c2___d_.pop('_x8')                                              # [-] remove internal
-    c2___di = cod | c2___d_                                         # class 2 dunder no_ignored
-    c2__hdi = cod | c2__hd_                                         # class 2 hidden no_ignored
-
-    o2 = C2()                                                       # object 2
-    o2_____ = c2_____ | {'x6': 36, 'x9': 39}                        # object 2 attributes
-    o2__h__ = c1__h__ | o2_____ | {'_x7': 37}                       # object 2 internal
-    o2___d_ = c1___d_ | c2___d_ | o2_____                           # object 2 dunder
-    o2__hd_ = o2__h__ | o2___d_                                     # object 2 hidden
-    o2___di = cod | o2___d_                                         # object 2 dunder no_ignored
-    o2__hdi = cod | o2__hd_                                         # object 2 hidden no_ignored
-
-    # Helper class 2 slots objects
-    c2s____ = c1s____ | c2_____ | {'x9': C2S.x9}                # class 2 slots attributes
-    c2s_h__ = c1s_h__ | c2s____                                 # class 2 slots internal
-    c2s_hd_ = c1s_hd_ | C2S.__dict__ | merge_common(C1S, C2S)   # class 2 slots hidden
-    c2s__d_ = c2s_hd_.copy()                                    # class 2 slots dunder
-    c2s__d_.pop('_x7')                                          # [-] remove internal
-    c2s__d_.pop('_x8')                                          # [-] remove internal
-    c2s__di = cod | c2s__d_                                     # class 2 dunder no_ignored
-    c2s_hdi = cod | c2s_hd_                                     # class 2 hidden no_ignored
-
-    o2s = C2S()
-    o2s_hd_ = dict_build(o2s) | merge_common(C1S, C2S)          # object 2 slots hidden
-    o2s__d_ = o2s_hd_.copy()                                    # object 2 slots dunder
-    o2s__d_.pop('_x7')                                          # [-] remove internal
-    o2s__d_.pop('_x8')                                          # [-] remove internal
-    o2s__di = cod | o2s__d_                                     # object 2 slots dunder no_ignored
-    o2s_hdi = cod | o2s_hd_                                     # object 2 slots hidden no_ignored
-
-    # Helper func kwargs
-    h__ = {'internal': True}
-    _d_ = {'dunder': True}
-    __i = {'ignored': ()}
-    hd_ = h__ | _d_
-    h_i = h__ | __i
-    _di = _d_ | __i
-    hdi = hd_ | __i
-
-    # All others checks, values: 0:empty, 1:internal, 2:dunder, 3:internal|dunder,
-    # 4:no_ignored, 5:no_ignored|internal, 6:no_ignored|dunder, 7:no_ignored|internal|dunder
-    for func, results in (
-            (None,  [InputError('obj', must_be='not None', received='None',
-                                func_name='get_attrs()')] * 8),
-            (ct,    [cte, cte, cte, cte, cta, cta, ctd, ctd]),
-            (co,    [coe, coe, coe, coe, {},  {},  cod, cod]),
-            (oo,    [ooe, ooe, ooe, ooe, {},  {},  ood, ood]),
-            (C1,    [c1_____, c1__h__, c1___d_, c1__hd_, c1_____, c1__h__, c1___di, c1__hdi]),
-            (o1,    [c1_____, c1__h__, c1___d_, c1__hd_, c1_____, c1__h__, c1___di, c1__hdi]),
-            (C1S,   [c1s____, c1s_h__, c1s__d_, c1s_hd_, c1s____, c1s_h__, c1s__di, c1s_hdi]),
-            (o1s,   [c1s____, c1s_h__, o1s__d_, o1s_hd_, c1s____, c1s_h__, o1s__di, o1s_hdi]),
-            (C2,    [c2_____, c2__h__, c2___d_, c2__hd_, c2_____, c2__h__, c2___di, c2__hdi]),
-            (o2,    [o2_____, o2__h__, o2___d_, o2__hd_, o2_____, o2__h__, o2___di, o2__hdi]),
-            (C2S,   [c2s____, c2s_h__, c2s__d_, c2s_hd_, c2s____, c2s_h__, c2s__di, c2s_hdi]),
-            (o2s,   [o2_____, o2__h__, o2s__d_, o2s_hd_, o2_____, o2__h__, o2s__di, o2s_hdi])):
-        for kwargs, result in zip(({}, h__, _d_, hd_, __i, h_i, _di, hdi), results, strict=True):
-            if isinstance(result, Exception) or result == InputError:
-                raises(result, get_attrs, func, **kwargs)
-            else:
-                assert get_attrs(func, **kwargs) == result
-
-
-def test_get_name():
-    test_funcs = (GetName, partial(GetName, full=True))
-
-    # Check wrong input
-    wrong_names = ("attr", "attr_cls", "attrs_", "attrs_cos")
-    order = ('some_obj', 'code_obj', 'not_exists')
-    possible_parameters = ("Possible parameters: doc_obj, code_obj, attrs_obj, doc_cls, "
-                           "attrs_cls, str_obj, str_cls, repr_cls, repr_obj")
-    details = f"Received: 'some_obj', 'code_obj', 'not_exists'. {possible_parameters}"
-    for kwargs, exc_kwargs in [
-        ({'doc': ()}, {"msg": "() (tuple) must be bool type"}),
-        ({'doc_cls': ()}, {"msg": "() (tuple) must be bool type"}),
-        ({'attrs': []}, {"msg": "[] (list) must be bool or tuple types"}),
-        ({'attrs_obj': []}, {"msg": "[] (list) must be bool or tuple types"}),
-        ({'order': order}, {"msg": f"Not exists methods: 'some_obj', 'not_exists'. {details}"}),
-        ({}.fromkeys(wrong_names), {"msg": possible_parameters})]:
-        for func in test_funcs:
-            raises(InputError(*kwargs, **exc_kwargs, func_name='GetName()'), func, '', **kwargs)
-
-    # Check method wrong input
-    msg = ("Provided wrong parameter to GetName.attrs(): attrs. Must be 1 (same for both) "
-           "or 2 (separately) provided for cls and obj, but received 3: 'some', 1, 2")
-    raises(InputError(msg=msg), GetName.attrs, 'obj', 'some', 1, 2)
-    msg = ("Provided wrong parameter(s) to GetName.doc(). "
-           "Must be no arguments, but received 1: 'some'")
-    raises(InputError(msg=msg), GetName.doc, 'obj', 'some')
-
-    # Check for None target
-    for func in test_funcs:
-        assert func(None, none=None) is None
-        assert (name_obj := func(None)) == ""
-        assert isinstance(name_obj, GetName)
-
-    # Check for unknown target
-    for func in test_funcs:
-        assert func('', unknown=None, attrs=False, repr=False) is None
-        assert (name_obj := func('', attrs=False, repr=False)) == ""
-        assert isinstance(name_obj, GetName)
-
-    # Prepare data for positive full=True check
-    def code_obj():
-        pass
-
-    class Non:
-        pass
-
-    class Cls:
-        """doc_cls"""
-        name = 'attrs_cls'
-        custom_name = 'attrs_custom_cls'
-
-        @classmethod
-        def __repr__(cls):
-            return 'repr_cls'
-
-        @classmethod
-        def __str__(cls):
-            return 'str_cls'
-
-    class Obj:
-        def __init__(self):
-            self.__doc__ = 'doc_obj'
-            self.__code__ = code_obj.__code__
-            self.name = 'attrs_obj'
-            self.__name__ = 'attrs_dunder_obj'
-            self.custom_name = 'attrs_custom_obj'
-            self.__repr__ = lambda: 'repr_obj'
-            self.__str__ = lambda: 'str_obj'
-
-    class COb(Cls, Obj):
-        pass
-
-    class All:
-        """doc_cls"""
-        name = 'attrs_cls'
-        custom_name = 'attrs_custom_cls'
-
-        @classmethod
-        def __repr__(cls):
-            return 'repr_cls'
-
-        @classmethod
-        def __str__(cls):
-            return 'str_cls'
-
-        def __init__(self):
-            self.__doc__ = 'doc_obj'
-            self.__code__ = code_obj.__code__
-            self.name = 'attrs_obj'
-            self.__name__ = 'attrs_dunder_obj'
-            self.custom_name = 'attrs_custom_obj'
-            self.__repr__ = lambda: 'repr_obj'
-            self.__str__ = lambda: 'str_obj'
-
-    def prepare_name(*prefixes):
-        def make_name(root=None):
-            if callable(root):  # set prefixes as fixed name if func provided
-                return root()
-            return join(*prefixes, root, sep='_') if root != '' else ''
-        return make_name
-
-    empty = ''
-    cls_s = 'cls'
-    obj_s = 'obj'
-    non_f = prepare_name('Non')         # fixed Non.__name__
-    cls_f = prepare_name('Cls')         # fixed Cls.__name__
-    obj_f = prepare_name('Obj')         # fixed Obj.__name__
-    cob_f = prepare_name('COb')         # fixed COb.__name__
-    all_f = prepare_name('All')         # fixed All.__name__
-
-    extension = (
-        ['default', '', ()],
-        ['empty', '', ([],)],
-        ['simple', '', (['name'],)],
-        ['dunder', 'dunder', (['__name__'],)],
-        ['custom', 'custom', (['custom_name'],)]
-    )
-
-    # [(attrs_default), (attrs_empty), (attrs_simple), (attrs_dunder), (attrs_custom)],
-    # [(doc)], [(code)], [(str)], [(repr)]
-    data = [
-        ([(non_f, empty), (empty, empty), (empty, empty), (non_f, empty), (empty, empty)],  # Non
-         [(empty, empty)], [(empty, empty)], [(empty, empty)], [(empty, empty)]),
-        ([(cls_s, cls_s), (empty, empty), (cls_s, cls_s), (cls_f, empty), (cls_s, cls_s)],  # Cls
-         [(cls_s, cls_s)], [(empty, empty)], [(cls_s, cls_s)], [(cls_s, cls_s)]),
-        ([(obj_f, obj_s), (empty, empty), (empty, obj_s), (obj_f, obj_s), (empty, obj_s)],  # Obj
-         [(empty, obj_s)], [(empty, obj_s)], [(empty, obj_s)], [(empty, obj_s)]),
-        ([(cls_s, obj_s), (empty, empty), (cls_s, obj_s), (cob_f, obj_s), (cls_s, obj_s)],  # COb
-         [(empty, obj_s)], [(empty, obj_s)], [(cls_s, obj_s)], [(cls_s, obj_s)]),
-        ([(cls_s, obj_s), (empty, empty), (cls_s, obj_s), (all_f, obj_s), (cls_s, obj_s)],  # All
-         [(cls_s, obj_s)], [(empty, obj_s)], [(cls_s, obj_s)], [(cls_s, obj_s)])
-    ]
-
-    # GetName.method(target, *args) + GetName(target, *args, full=True).method tests
-    errors = []
-    calls = ('GetName.{0}({1}{2}, {3})', 'GetName({1}{2}, full=True, {3}).{0}')
-    postfix = ('', '.cls', '.obj')
-    for cls, results in zip((Non, Cls, Obj, COb, All), data, strict=True):
-        for method, result in zip('attrs doc code str repr'.split(), results, strict=True):
-            cm = getattr(GetName, method)
-            args_str = ' || args set: ' if len(result) == len(extension) else ''
-            for (args_name, suffix, args), (val_cls, val_obj) in zip(extension, result):
-
-                # Must be
-                name = prepare_name(method, suffix)
-                name_cls, name_obj = name(val_cls), name(val_obj)
-                name_first = (name_obj or name_cls)
-                must_be_data = ((name_cls, name_cls, empty), (name_first, name_cls, name_obj))
-
-                # Received
-                kwargs = {method: args} if args else {method: True}
-                received_data = tuple((x, x.cls, x.obj) for x in (
-                    cm(cls, *args),
-                    cm(cls(), *args),
-                    getattr(GetName(cls, full=True, **kwargs), method),
-                    getattr(GetName(cls(), full=True, **kwargs), method)))
-
-                # Compare
-                if must_be_data * 2 != received_data:
-                    for i, (r, m) in enumerate(zip(received_data, must_be_data, strict=True)):
-                        for received, must_be, p in zip(r, m, postfix, strict=True):
-                            if received != must_be:
-                                obj_str = '()' if i % 2 else ''
-                                kw_str = ', '.join(fmt_dict(kwargs))
-                                sig = calls[i // 2].format(method, cls.__name__, obj_str, kw_str)
-                                add = args_str + args_name if args_str else ''
-                                msg = f'{sig}{p} == {received!r} || must be: {must_be!r}{add}'
-                                errors.append(msg)
-    if errors:
-        raise ValueError('\n\t'.join((f'Test failed, errors:', *errors)))
-
-
-# Uncategorized
-
-
-def test_uid():
-    id1 = UID('1')
-    id2 = UID('2')
-    raises(TypeError, UID)
-    raises(ValueError("'1' unique ID cannot be created, it already exists"), UID, 1)
-    assert repr(id1) == "UID('1')"
-    assert str(id1) == "1 ID"
-    assert id1 == id1
-    assert id1 != id2
-
-
-def test_locker():
-    class All(Locker):
-        def __init__(self):
-            self.a = 1
-            super().__init__('b')
-            self.b = 2
-            with self:
-                self.c = 3
-
-    class Add(Locker):
-        def __init__(self):
-            self.a = 1
-            super().__init__('b', del_attr=False)
-            self.b = 2
-            with self:
-                self.c = 3
-
-    class Del(Locker):
-        def __init__(self):
-            self.a = 1
-            super().__init__('b', set_attr=False)
-            exceptions = ''
-            try:
-                self.b = 2
-            except TypeError:
-                exceptions += 'b'
-            try:
-                with self:
-                    self.c = 3
-            except TypeError:
-                exceptions += 'c'
-
-            assert exceptions == 'bc'
-            object.__setattr__(self, 'b', 2)
-            object.__setattr__(self, 'c', 3)
-
-    class Non(Locker):
-        def __init__(self):
-            self.a = 1
-            super().__init__('b', set_attr=False, del_attr=False)
-            exceptions = ''
-            try:
-                self.b = 2
-            except TypeError:
-                exceptions += 'b'
-            try:
-                with self:
-                    self.c = 3
-            except TypeError:
-                exceptions += 'c'
-
-            assert exceptions == 'bc'
-            object.__setattr__(self, 'b', 2)
-            object.__setattr__(self, 'c', 3)
-
-    class AllSlot(Locker):
-        __slots__ = tuple('abcd')
-
-        def __init__(self):
-            self.a = 1
-            super().__init__('b')
-            self.b = 2
-            with self:
-                self.c = 3
-
-    class AddSlot(Locker):
-        __slots__ = tuple('abcd')
-
-        def __init__(self):
-            self.a = 1
-            super().__init__('b', del_attr=False)
-            self.b = 2
-            with self:
-                self.c = 3
-
-    class DelSlot(Locker):
-        __slots__ = tuple('abcd')
-
-        def __init__(self):
-            self.a = 1
-            super().__init__('b', set_attr=False)
-            exceptions = ''
-            try:
-                self.b = 2
-            except TypeError:
-                exceptions += 'b'
-            try:
-                with self:
-                    self.c = 3
-            except TypeError:
-                exceptions += 'c'
-
-            assert exceptions == 'bc'
-            object.__setattr__(self, 'b', 2)
-            object.__setattr__(self, 'c', 3)
-
-    class NonSlot(Locker):
-        __slots__ = tuple('abcd')
-
-        def __init__(self):
-            self.a = 1
-            super().__init__('b', set_attr=False, del_attr=False)
-            exceptions = ''
-            try:
-                self.b = 2
-            except TypeError:
-                exceptions += 'b'
-            try:
-                with self:
-                    self.c = 3
-            except TypeError:
-                exceptions += 'c'
-
-            assert exceptions == 'bc'
-            object.__setattr__(self, 'b', 2)
-            object.__setattr__(self, 'c', 3)
-
-    for data in (All, Add, Del, Non, AllSlot, AddSlot, DelSlot, NonSlot):
-        # Prepare message templates for set and del parts test
-        data = data()
-        obj = GetName(data)
-        name = f'{obj!r} object'
-        can_set = name + " is locked for changes (self.__setattr__('{}', {}))"
-        can_del = name + " is locked for changes (self.__delattr__('{}'))"
-        cant_set = name + " does not support setting attributes (self.__setattr__('{}', {}))"
-        cant_del = name + " does not support deleting attributes (self.__delattr__('{}'))"
-        not_exists = name + " has no attribute '{}'"
-        forbid = name + " Locker attrs deletion is forbidden (self.__delattr__('{}'))"
-
-        # [0. Init] Check locked object condition after init
-        assert data._locker_state is True
-        assert data._locker_ignored == ('b',)
-        assert data.a == 1
-        assert data.b == 2
-        assert data.c == 3
-        assert not hasattr(data, 'd')
-
-        # [1. Set] 1. Check object attrs changes without unlocking
-        msg = can_set if data._locker_set_attr else cant_set
-        for attr, prev_value in zip('acd', (1, 3, 4), strict=True):
-            raises(TypeError(msg.format(attr, 5)), setattr, data, attr, 5)
-            if attr != 'd':
-                assert getattr(data, attr) == prev_value
-            else:
-                assert not hasattr(data, attr)
-
-        # [1. Set] 2. Check object attrs changes in ignored attr and unlocked attrs
-        if data._locker_set_attr:
-            data.b = 5
-            assert data.b == 5
-
-            with data:
-                data.a = 5
-                assert data.a == 5
-
-                data.c = 5
-                assert data.c == 5
-
-                data.d = 5
-                assert data.d == 5
-        else:
-            raises(TypeError(cant_set.format('b', 5)), setattr, data, 'b', 5)
-            assert data.b == 2
-
-            with data:
-                raises(TypeError(cant_set.format('a', 5)), setattr, data, 'a', 5)
-                assert data.a == 1
-
-                raises(TypeError(cant_set.format('c', 5)), setattr, data, 'c', 5)
-                assert data.c == 3
-
-                raises(TypeError(cant_set.format('d', 5)), setattr, data, 'd', 5)
-                assert not hasattr(data, 'd')
-
-        # [1. Set] 3. Check object new attrs creation
-        with data:
-            if obj == 'All' or obj == 'Add':  # Has __dict__ and set allowed
-                data.e = 5
-                assert data.e == 5
-            elif obj == 'AllSlot' or obj == 'AddSlot':
-                raises(AttributeError(not_exists.format('e')), setattr, data, 'e', 5)
-            elif not data._locker_set_attr:
-                raises(TypeError(cant_set.format('e', 5)), setattr, data, 'e', 5)
-            else:
-                raise AssertionError(f'{obj!r} set new attrs check missing!')
-
-        # [2. Del] 1. Check object attrs deletion without unlocking
-        exists_d = 'd' if hasattr(data, 'd') else ''
-        msg = can_del if data._locker_del_attr else cant_del
-
-        for attr in 'ac' + exists_d:
-            raises(TypeError(msg.format(attr)), delattr, data, attr)
-            assert hasattr(data, attr)
-        if not exists_d:
-            raises(AttributeError(not_exists.format('d')), delattr, data, 'd')
-
-        # [2. Del] 2. Check object attrs deletion
-        if data._locker_del_attr:
-            del data.b
-            assert not hasattr(data, 'b')
-
-            with data:
-                del data.a
-                assert not hasattr(data, 'a')
-
-                del data.c
-                assert not hasattr(data, 'c')
-
-                if hasattr(data, 'd'):
-                    del data.d
-                    assert not hasattr(data, 'd')
-        else:
-            raises(TypeError(cant_del.format('b')), delattr, data, 'b')
-            assert hasattr(data, 'b')
-
-            with data:
-                raises(TypeError(cant_del.format('a')), delattr, data, 'a')
-                assert hasattr(data, 'a')
-
-                raises(TypeError(cant_del.format('c')), delattr, data, 'c')
-                assert hasattr(data, 'c')
-
-                if hasattr(data, 'd'):
-                    raises(TypeError(cant_del.format('d')), delattr, data, 'd')
-                    assert hasattr(data, 'd')
-
-        # [2. Del] 3. Check Locker attrs deletion
-        [raises(TypeError(forbid.format(attr)), delattr, data, attr) for attr in Locker.__slots__]
+from typing import Mapping, Iterable
+from itertools import product
+from functools import partial
+
+from configlayer.types import ItemError
+from configlayer.exceptions import InputError, InitError, CheckValueError, CheckTypeError
+from configlayer.utils import (
+    is_dunder, is_internal, is_hidden, is_exception, is_holder,                     # Bool checks
+    as_holder, as_holder_stated, as_dict, as_dict_stated,                           # Type casting
+    safe, with_type,                                                                # Common
+    fmt_dict, fmt_obj_errors, fmt_name, fmt_exc,                                    # Formatters
+    split,                                                                          # Split
+    join, sentence, sentences,                                                      # Joins
+    check_input, check_lengths, check_absent, check_extra, check_items, check_type, check_types,   # Data checks
+    decorate_methods, init_reraise, set_slots_defaults,                             # Decorators
+    get_cls_obj, get_cls_attr, get_attrs, GetName,                                  # Getters
+    UID, Locker)                                                                    # Uncategorized
+
+from _utilities import raises, subtest
+from _data import empty_func, increment_str, wrong_func, wrong_func_3, WrongCast
+
+
+# Bool checks
+
+
+def test_is_dunder():
+    variants = ('', '_', '__', '___')
+    data = [f'{start}name{end}' for start in variants for end in variants]
+    data.remove('__name__')
+    assert is_dunder('__name__')
+    assert not any(map(is_dunder, data))
+
+
+def test_is_internal():
+    variants = ('_', '__', '___')
+    data = [f'{start}name{end}' for start in variants for end in variants]
+    data.remove('__name__')
+    assert all(map(is_internal, data))
+    assert not is_internal('name')
+    assert not is_internal('name_')
+    assert not is_internal('name__')
+    assert not is_internal('name___')
+    assert not is_internal('__name__')
+
+
+def test_is_hidden():
+    variants = ('_', '__', '___')
+    data = [f'{start}name{end}' for start in variants for end in variants]
+    assert all(map(is_hidden, data))
+    assert not is_hidden('name')
+    assert not is_hidden('name_')
+    assert not is_hidden('name__')
+    assert not is_hidden('name___')
+    assert is_hidden('__name__')
+
+
+def test_is_exception():
+    assert is_exception(Exception)
+    assert is_exception(Exception(''))
+    assert is_exception(ValueError)
+    assert is_exception(ValueError(''))
+    assert not is_exception(Exception, ValueError)
+    assert not is_exception(Exception(''), ValueError)
+    assert not is_exception(None)
+    assert not is_exception(None, ValueError)
+
+
+def test_is_holder():
+    holder_types = tuple, list, set, dict
+    not_holder_types = bool, int, float, str, bytes, bytearray
+
+    assert is_holder(None) is None
+    assert all(is_holder(x()) for x in holder_types) is True
+    assert any(is_holder(x()) for x in not_holder_types) is False
+    assert not any(is_holder(x(), holder_types) for x in holder_types)
+
+    exc = partial(InputError, 'exclude', must_be='type or types', func_name='is_holder()')
+    raises(exc(received='5 (int)'), is_holder, 5, 5)
+    raises(exc(received='5 (int) at pos 0'), is_holder, 5, (5, int))
+    raises(exc(received="'some'='string' (str)"), is_holder, 5, {'some': 'string', 'another': str})
+
+
+# Type casting
+
+
+def test_as_holder():
+    assert as_holder(None, default=None) is None
+    assert as_holder(None, None) is None
+    assert as_holder(None, [1]) == [1]
+    assert as_holder(None) == ()
+    assert as_holder('1') == ('1',)
+    assert as_holder([]) == []
+    assert as_holder([1]) == [1]
+    assert as_holder(['1']) == ['1']
+    assert as_holder(['1'], exclude=(list,)) == (['1'],)
+
+    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
+                      received="'1' (str) at pos 1"),
+           as_holder, ['1'], exclude=(list, '1'))
+
+    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
+                      received="'1' (str) at pos 1, 2.13 (float) at pos 2"),
+           as_holder, ['1'], exclude=(list, '1', 2.13))
+
+
+def test_as_holder_stated():
+    assert as_holder_stated(None, default=None) == (None, None)
+    assert as_holder_stated(None, None) == (None, None)
+    assert as_holder_stated(None, [1]) == (None, [1])
+    assert as_holder_stated(None) == (None, ())
+    assert as_holder_stated('1') == (False, ('1',))
+    assert as_holder_stated([]) == (True, [])
+    assert as_holder_stated([1]) == (True, [1])
+    assert as_holder_stated(['1']) == (True, ['1'])
+    assert as_holder_stated(['1'], exclude=(list,)) == (False, (['1'],))
+
+    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
+                      received="'1' (str) at pos 1"),
+           as_holder_stated, ['1'], exclude=(list, '1'))
+
+    raises(InputError('exclude', func_name='is_holder()', must_be='type or types',
+                      received="'1' (str) at pos 1, 2.13 (float) at pos 2"),
+           as_holder_stated, ['1'], exclude=(list, '1', 2.13))
+
+
+def test_as_mapping():
+    def modify(x):
+        return ((str(v), v) for v in x)
+
+    raises(TypeError("'int' object is not iterable"), as_dict, 5)
+    t1 = (0, '1')
+    t2 = ('0', '1')
+    t3 = ('0',)
+    t4 = ('0', 1, 2)
+    d1 = {0: 0, 1: '1'}
+    d2 = {'0': 0, '1': '1'}
+    d3 = {'0': 0}
+    d4 = {'0': 0, 1: '1'}
+
+    # input mapping
+    assert as_dict(d1) == d1                             # -> input
+    assert as_dict(d1, modify) == d1                     # -> input
+    assert as_dict(d1, t2) == d1                         # -> input
+    assert as_dict(d1, t3) == d1                         # -> input
+    assert as_dict(d1, t4) == d1                         # -> input
+    assert as_dict(d1, t2, strict=True) == d1            # -> input
+    assert as_dict(d1, t3, strict=True) == d1            # -> input
+    assert as_dict(d1, t4, strict=True) == d1            # -> input
+
+    # input not mapping iterable
+    assert as_dict(t1) == d1                             # -> default func
+    assert as_dict(t1, modify) == d2                     # -> modify func
+    assert as_dict(t1, t2) == d2                         # -> iterable
+    assert as_dict(t1, t3) == d3                         # -> iterable less
+    assert as_dict(t1, t4) == d4                         # -> iterable more
+    assert as_dict(t1, t2, strict=True) == d2            # -> iterable strict
+    raises(ValueError, as_dict, t1, t3, strict=True)     # -> iterable strict less error
+    raises(ValueError, as_dict, t1, t4, strict=True)     # -> iterable strict more error
+
+
+def test_as_mapping_stated():
+    def modify(x):
+        return ((str(v), v) for v in x)
+
+    raises(TypeError("'int' object is not iterable"), as_dict, 5)
+    t1 = (0, '1')
+    t2 = ('0', '1')
+    t3 = ('0',)
+    t4 = ('0', 1, 2)
+    d1 = {0: 0, 1: '1'}
+    d2 = {'0': 0, '1': '1'}
+    d3 = {'0': 0}
+    d4 = {'0': 0, 1: '1'}
+
+    # input mapping
+    assert as_dict_stated(d1) == (True, d1)                      # -> input state
+    assert as_dict_stated(d1, modify) == (True, d1)              # -> input state
+    assert as_dict_stated(d1, t2) == (True, d1)                  # -> input state
+    assert as_dict_stated(d1, t3) == (True, d1)                  # -> input state
+    assert as_dict_stated(d1, t4) == (True, d1)                  # -> input state
+    assert as_dict_stated(d1, t2, strict=True) == (True, d1)     # -> input state
+    assert as_dict_stated(d1, t3, strict=True) == (True, d1)     # -> input state
+    assert as_dict_stated(d1, t4, strict=True) == (True, d1)     # -> input state
+
+    # input not mapping iterable
+    assert as_dict_stated(t1) == (False, d1)                     # -> default func state
+    assert as_dict_stated(t1, modify) == (False, d2)             # -> modify func
+    assert as_dict_stated(t1, t2) == (False, d2)                 # -> iterable
+    assert as_dict_stated(t1, t3) == (False, d3)                 # -> iterable less
+    assert as_dict_stated(t1, t4) == (False, d4)                 # -> iterable more
+    assert as_dict_stated(t1, t2, strict=True) == (False, d2)    # -> iterable strict
+    raises(ValueError, as_dict_stated, t1, t3, strict=True)      # -> iterable strict less error
+    raises(ValueError, as_dict_stated, t1, t4, strict=True)      # -> iterable strict more error
+
+
+# Common
+
+
+def test_safe():
+    assert safe(increment_str, '5') == 6
+    assert safe(wrong_func_3, 'x', y=5).args == ("Cannot change value ('x',), {'y': 5}", )
+    assert safe(increment_str, '5', _res_=increment_str) == 7
+    assert safe(increment_str, '5', _res_=55) == 55
+    assert safe(wrong_func, 'x').args == ('Wrong func!', )
+    assert safe(wrong_func, 'x', _exc_=repr) == "TypeError('Wrong func!')"
+    assert safe(wrong_func, 'x', _exc_=55) == 55
+
+
+def test_with_type():
+    assert with_type(type) == "type (type)"
+    assert with_type(5) == "5 (int)"
+    assert with_type('any') == "'any' (str)"
+
+    assert with_type(type, key1='some') == "type (type=type, key1='some')"
+    assert with_type(5, key1='some', type=0.1) == "5 (key1='some', type=int)"
+    assert with_type('any', k=0, k3=False, k2=True) == "'any' (type=str, k=0, k3=False, k2=True)"
+
+
+# Formatters
+
+
+def test_fmt_dict():
+    obj = {0: 0, 1: '1', '2': 2, 'item': 'value'}
+    fmts = (str, repr)
+    seps = ('=', ': ')
+    for i, kf, sep, vf in (st := subtest('', 8, product(fmts, seps, fmts))):
+        st.send(('', fmt_dict(obj, kf, sep, vf),
+                 tuple(f'{kf(k)}{sep}{vf(v)}' for k, v in obj.items())))
+
+
+def test_fmt_obj_errors():
+    obj = object()
+    errors = [(ItemError('1', 1, ''),), (ItemError('1', 1, ''), ItemError(2, '2', '2'))]
+    rns = ({}, {'result_name': 'some name'})
+    khs = ({}, {'key_handler': str})
+    seps = ({}, {'kv_sep': ': '})
+    bools = [False, True]
+
+    # Check all Extra - 192 cases
+    cases = product([obj], [(), *errors], [False], bools, bools, bools, rns, khs, seps)
+    for i, o, *args, rn, kh, sep in (st := subtest('All Extra', 192, cases)):
+        st.send(('', fmt_obj_errors(o, *args, **rn, **kh, **sep), (with_type(o),)))
+
+    # Check all no errors - 128 cases
+    cases = product([obj], [()], bools, bools, bools, bools, rns, khs, seps)
+    for i, o, *args, rn, kh, sep in (st := subtest('All no errors', 128, cases)):
+        st.send(('', fmt_obj_errors(o, *args, **rn, **kh, **sep), (with_type(o),)))
+
+    # Check all not holders - 64 cases
+    cases = product([obj], errors, [True], [False], bools, bools, rns, khs, seps)
+    for i, o, e, *args, r, rn, kh, sep in (st := subtest('All not holders', 64, cases)):
+        res = with_type(e[0].value, **{rn.get('result_name', 'result'): e[0].result} if r else {})
+        st.send(('', fmt_obj_errors(o, e, *args, r, **rn, **kh, **sep), (res,)))
+
+    # Check all mappings - 32 cases
+    cases = product([obj], errors, [True], [True], [True], bools, rns, khs, seps)
+    for i, o, e, *args, r, rn, kh, sep in (st := subtest('All mappings', 32, cases)):
+        h = kh.get('key_handler', repr)
+        s = sep.get('kv_sep', '=')
+        res = (f"{h(k)}{s}{with_type(v, **{rn.get('result_name', 'result'): info} if r else {})}"
+               for k, v, info in e)
+        st.send(('', fmt_obj_errors(o, e, *args, r, **rn, **kh, **sep), tuple(res)))
+
+    # Check all left (not mapping holder that has errors and exists) - 32 cases
+    cases = product([obj], errors, [True], [True], [False], bools, rns, khs, seps)
+    for i, o, e, *args, r, rn, kh, sep in (st := subtest('All left', 32, cases)):
+        res = tuple(f"{with_type(v)} at pos {i}" + (f' ({info})' if r else '') for i, v, info in e)
+        st.send(('', fmt_obj_errors(o, e, *args, r, **rn, **kh, **sep), res))
+
+
+def test_fmt_name():
+    for results, kwargs in [
+        ('items item items',        {}),
+        ('params param params',     {'item_name': 'param'}),
+        ('param item items',        {'default': 'param'}),
+        ('param(s) param params',   {'item_name': 'param', 'default': 'param(s)'})
+    ]:
+        for obj, result in zip([(), ['a'], {'b': '1', 'c': 0}], results.split(), strict=True):
+            assert fmt_name(obj, **kwargs) == result
+
+
+def test_fmt_exc():
+    msg_set = ('', 'some message')
+    exc_set = (Exception, TypeError)
+    args_set = ((), (0,), (1, 2))
+    kwargs_set = ({}, {'str': 'here'}, {'sentences': ('msg1', 'msg2'), 'dict': {'k1': 1, 'k2': 2}})
+
+    def_set = (msg_set, exc_set, args_set, kwargs_set)
+
+    name_set = ('', 'name')
+    n_args_set = ((), ('arg',), ('arg1', 'arg2'))
+    in_kw_set = ((), *((x,) for x in kwargs_set))
+    input_exc_set = [(n, *a, *k) for n, a, k in product(name_set, n_args_set, in_kw_set)]
+
+    # Check default error exception, fixed empty input_exc param
+    st = subtest('Default exception', 36, product(*def_set))
+    for i, msg, exc, args, kwargs in st:
+        recv_exc = fmt_exc((), msg, exc, *args, **kwargs)
+
+        exc_msg = InputError(msg=msg, **kwargs).args[0] if kwargs else msg
+        wait_exc = exc(exc_msg, *args) if exc_msg else exc(*args)
+
+        st.send(('', type(recv_exc), exc))
+        r_msg, *r_left = recv_exc.args or ('',)
+        w_msg, *w_left = wait_exc.args or ('',)
+        st.send(('Message or arg - args[0]', r_msg, w_msg))
+        st.send(('', r_left, w_left))
+
+    # Check input error exception
+    st = subtest('Input exception', 864, product(input_exc_set, *def_set),
+                 {'Message - args[0]': 144})
+    for i, input_exc, msg, exc, args, kwargs in st:
+        recv_exc = fmt_exc(input_exc, msg, exc, *args, **kwargs)
+
+        name, *params, in_kw = (input_exc if isinstance(input_exc[-1], dict) else (*input_exc, {}))
+        in_kw |= {k: v for k, v in kwargs.items() if k not in in_kw}
+        wait_exc = InputError(*params, msg=msg, func_name=name, args=args, **in_kw)
+
+        st.send(('', type(recv_exc), InputError))
+        r_msg, *r_left = recv_exc.args
+        w_msg, *w_left = wait_exc.args
+        st.send(('Message - args[0]', r_msg, w_msg))
+        st.send(('', r_left, w_left))
+
+
+# Split
+
+
+def test_split():
+    e_value = ValueError('3')
+    data_dict = {'0': 0, '1': 1, 'E': e_value, 'T': (1, 2), 'L': [1, -1], 'F': False, 'N': None}
+    data_list = list(data_dict.values())
+
+    # support funcs
+    def to_tuples(values: Iterable[dict]):
+        return tuple(tuple(x.values()) for x in values)
+
+    # funcs for test
+    def change(x, val=1):
+        return (not x) if isinstance(x, bool) else (x + val) if isinstance(x, int) else x
+
+    def is_int_key(k, _):
+        return isinstance(k, int)
+
+    # data values (f - fixed, s - standard, m - modified)
+    fe, fn = {'E': e_value}, {'N': None}
+    s0, s1, st, sl, sf = {'0': 0}, {'1': 1}, {'T': (1, 2)}, {'L': [1, -1]}, {'F': False}
+    m0, m1, mt, ml, mf = {'0': 1}, {'1': 2}, {'T': 3}, {'L': 0}, {'F': True}
+
+    # possible bool condition results
+    b_______ = s1 | fe | st | sl, s0 | sf | fn
+    b____s__ = s1 | st | sl, s0 | fe | sf | fn
+
+    b_c_____ = s0 | s1 | fe | st | sl | sf, fn
+    b_c___m_ = m0 | m1 | fe | st | sl | mf, fn
+    b_c__s__ = s0 | s1 | st | sl | sf, fe | fn
+    b_c__sm_ = m0 | m1 | st | sl | mf, fe | fn
+    b_c_u___ = s0 | s1 | fe | st | sf, sl | fn
+    b_c_u_m_ = m0 | m1 | fe | mt | mf, ml | fn
+    b_c_us__ = s0 | s1 | st | sf, fe | sl | fn
+    b_c_usm_ = m0 | m1 | mt | mf, fe | ml | fn
+
+    b______i = b_______[::-1]
+
+    b_c____i = b_c_____[::-1]
+    b_c___mi = b_c___m_[::-1]
+    b_c_u__i = b_c_u___[::-1]
+    b_c_u_mi = b_c_u_m_[::-1]
+
+    # possible is_exception condition results
+    i_______ = fe, s0 | s1 | st | sl | sf | fn
+    i____s__ = {}, data_dict
+
+    i_c___m_ = fe, m0 | m1 | st | sl | mf | fn
+    i_c__sm_ = {}, m0 | m1 | fe | st | sl | mf | fn
+    i_c_u_m_ = fe, m0 | m1 | mt | ml | mf | fn
+    i_c_usm_ = {}, m0 | m1 | fe | mt | ml | mf | fn
+
+    i______i = i_______[::-1]
+    i_c___mi = i_c___m_[::-1]
+    i_c_u_mi = i_c_u_m_[::-1]
+
+    # defaults test
+    assert split(data_dict) == b_______
+    assert split(data_list) == to_tuples(b_______)
+
+    # general params tests
+    conditions = (bool, is_exception)
+    funcs = (None, change)
+    bool_keys = ('unpack', 'safely', 'modify', 'cond_invert')[::-1]
+    bool_kwargs = [dict(zip(bool_keys, x)) for x in product((False, True), repeat=len(bool_keys))]
+    for i, (args, results) in enumerate(zip(product(conditions, funcs), [
+        (b_______, b_______, b____s__, b____s__, b_______, b_______, b____s__, b____s__,
+         b______i, b______i, b______i, b______i, b______i, b______i, b______i, b______i),
+        (b_c_____, b_c_u___, b_c__s__, b_c_us__, b_c___m_, b_c_u_m_, b_c__sm_, b_c_usm_,
+         b_c____i, b_c_u__i, b_c____i, b_c_u__i, b_c___mi, b_c_u_mi, b_c___mi, b_c_u_mi),
+        (i_______, i_______, i____s__, i____s__, i_______, i_______, i____s__, i____s__,
+         i______i, i______i, i______i, i______i, i______i, i______i, i______i, i______i),
+        (i_______, i_______, i____s__, i____s__, i_c___m_, i_c_u_m_, i_c__sm_, i_c_usm_,
+         i______i, i______i, i______i, i______i, i_c___mi, i_c_u_mi, i_c___mi, i_c_u_mi)
+    ], strict=True)):
+        for j, (kwargs, expected) in enumerate(zip(bool_kwargs, results, strict=True)):
+            try:
+                assert split(data_dict, *args, **kwargs) == expected
+                assert split(data_list, *args, **kwargs) == to_tuples(expected)
+                vs, ws = split(data_list, *args, as_dicts=True, **kwargs)
+                ve, we = expected
+                assert all(isinstance(x, int) for x in tuple(vs.keys()) + tuple(ws.keys()))
+                assert tuple(vs.values()) == tuple(ve.values())
+                assert tuple(ws.values()) == tuple(we.values())
+            except Exception:
+                raise Exception(f"{i=} ({args = }), {j=} ({kwargs = })")
+
+    # cond_key and cond_value params test
+    e_kv____ = InputError('cond_key', 'cond_value', must_be='at least one True or not filled',
+                          func_name='split()', received='cond_key = False, cond_value = False')
+    b__vl___ = to_tuples(b_______)
+    b_k_d___ = (data_dict, {})
+    b_k_l___ = to_tuples((s1 | fe | st | sl | sf | fn, s0))
+    for (key, value), expected in zip(product((None, False, True), repeat=2), (
+        (b_______, b__vl___),                         # None  None  -> False, True
+        (b_k_d___, b_k_l___),                         # None  False -> True, False
+        (b_______, b__vl___),                         # None  True  -> False, True
+        (b_______, b__vl___),                         # False None  -> False, True
+        e_kv____,                                     # False False -> False, False (error)
+        (b_______, b__vl___),                         # False True  -> False, True
+        (b_k_d___, b_k_l___),                         # True  None  -> True, False
+        (b_k_d___, b_k_l___),                         # True  False -> True, False
+        (({}, data_dict), (tuple(data_list), ()))     # True  True  -> True,  True  (both)
+    ), strict=True):
+        if is_exception(expected):
+            raises(expected, split, data_dict, cond_key=key, cond_value=value)
+            raises(expected, split, data_list, cond_key=key, cond_value=value)
+        else:
+            args = (is_int_key,) if key == value and key is True else ()
+            assert split(data_dict, *args, cond_key=key, cond_value=value) == expected[0]
+            assert split(data_list, *args, cond_key=key, cond_value=value) == expected[1]
+
+
+# Joins
+
+join_dataset = [(0, '', 1, False),
+                (0, 'here is a sTrAnGe STRING', 1, False),
+                ('here is', 0, 'a sTrAnGe STRING', 1, False),
+                (None, 'here is', 0, 'a', False, 'sTrAnGe STRING', 1)]
+
+
+def _join_tests(func, results_set, sep=', '):
+    for typecast in True, False:
+        for skip_false, results in zip((True, False), results_set, strict=True):
+            kwargs = {'sep': sep, 'typecast': typecast, 'skip_false': skip_false}
+            for args, result in zip(join_dataset, results, strict=True):
+                if typecast:
+                    assert func(*args, **kwargs) == sep.join(result)
+                else:
+                    raises(TypeError, func, *args, **kwargs)
+
+
+def test_join():
+    results = ([('1',),
+                ('here is a sTrAnGe STRING', '1'),
+                ('here is', 'a sTrAnGe STRING', '1'),
+                ('here is', 'a', 'sTrAnGe STRING', '1')],
+               [('0', '', '1', 'False'),
+                ('0', 'here is a sTrAnGe STRING', '1', 'False'),
+                ('here is', '0', 'a sTrAnGe STRING', '1', 'False'),
+                ('None', 'here is', '0', 'a', 'False', 'sTrAnGe STRING', '1')])
+    _join_tests(join, results)
+
+
+def test_sentence():
+    results = ([('1',),
+                ('Here is a sTrAnGe STRING', '1'),
+                ('Here is', 'a sTrAnGe STRING', '1'),
+                ('Here is', 'a', 'sTrAnGe STRING', '1')],
+               [('0', '', '1', 'False'),
+                ('0', 'here is a sTrAnGe STRING', '1', 'False'),
+                ('Here is', '0', 'a sTrAnGe STRING', '1', 'False'),
+                ('None', 'here is', '0', 'a', 'False', 'sTrAnGe STRING', '1')])
+    _join_tests(sentence, results, ' ')
+
+
+def test_sentences():
+    results = ([('1',),
+                ('Here is a sTrAnGe STRING', '1'),
+                ('Here is', 'A sTrAnGe STRING', '1'),
+                ('Here is', 'A', 'STrAnGe STRING', '1')],
+               [('0', '', '1', 'False'),
+                ('0', 'Here is a sTrAnGe STRING', '1', 'False'),
+                ('Here is', '0', 'A sTrAnGe STRING', '1', 'False'),
+                ('None', 'Here is', '0', 'A', 'False', 'STrAnGe STRING', '1')])
+    _join_tests(sentences, results, '. ')
+
+
+# Data checks
+
+
+def test_check_input():
+    exc = CheckValueError
+    raises(exc("Item is needed, but not provided"), check_input, None, 1)
+    raises(exc("Item is not needed, but provided"), check_input, 1, None)
+    raises(exc("Some is needed, but not provided"), check_input, None, 1, 'Some')
+    raises(exc("Some is not needed, but provided"), check_input, 1, None, 'Some')
+    raises(exc("Is not needed, but provided"), check_input, 1, None, '')
+    raises(exc("- not"), check_input, 1, None, template='{2}-{1}')
+    assert check_input(None, None) is False
+    assert check_input(False, False) is True
+
+    exc1 = InputError('name1', msg="Some is not needed, but provided")
+    exc2 = InputError(msg="Some is not needed, but provided", func_name='str()')
+    raises(exc1, check_input, 1, None, 'Some', input_exc=('', 'name1'))
+    raises(exc2, check_input, 1, None, 'Some', input_exc=('str()',))
+    assert check_input(1, 1, 'Some', input_exc=('str()',))
+
+
+def test_check_extra():
+    exc = CheckValueError
+    vals = (1, '2', 3), [1]
+    add = ". Must be not more than expected (1), but received: 1, '2', 3"
+    raises(exc("Extra item: 2. Must be not more than expected (1), but received: 1, 2"),
+           check_extra, (1, 2), [1])
+    raises(exc("Extra items: '2', 3" + add), check_extra, *vals)
+    raises(exc("Extra vals: '2', 3" + add), check_extra, *vals, 'val')
+    raises(exc("E\n\t'2'\n\t3" + add), check_extra, *vals, template='E\n\t', item_sep='\n\t')
+    raises(exc("E items: '2' 3" + add), check_extra, *vals, template='E {}: ', item_sep=' ')
+    raises(exc("E items('2',3)" + add), check_extra, *vals, template='E {}({})', item_sep=',')
+    raises(exc("E xs('2',3)" + add), check_extra, *vals, 'x', template='E {}({})', item_sep=',')
+    raises(exc("E x('2',3)" + add), check_extra, *vals, '', template='E x{}({})', item_sep=',')
+
+    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
+                      func_name='check_extra()'),
+           check_extra, *vals, template='{}{}{}')     # with error
+    assert check_extra([1], (1, 2), template='{}{}{}')  # without error, but more pythonic
+
+    assert check_extra(*vals, as_text=True) == "Extra items: '2', 3" + add
+    assert check_extra((1, 2), (1, 2), as_text=True) == ""
+    assert check_extra((1, 2), (1, 2)) == (1, 2)
+
+    exc_inp = InputError('name1', msg="Extra items: '2', 3" + add)
+    raises(exc_inp, check_extra, *vals, input_exc=('', 'name1'))
+    assert check_extra(*vals, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
+
+    msg = "Extra strs: 2, 3. Must be not more than expected (1), but received: 1, 2, 3"
+    raises(exc(msg), check_extra, *vals, 'str', str)
+    raises(exc(msg + ". Some x"), check_extra, *vals, 'str', str, some='x')
+
+
+def test_check_absent():
+    exc = CheckValueError
+    vals = [1], (1, '2', 3)
+    add = ". Must be not less than expected (1, '2', 3), but received: 1"
+    raises(exc("Absent item: 2. Must be not less than expected (1, 2), but received: 1"),
+           check_absent, [1], (1, 2))
+    raises(exc("Absent items: '2', 3" + add), check_absent, *vals)
+    raises(exc("Absent vals: '2', 3" + add), check_absent, *vals, 'val')
+    raises(exc("A\n\t'2'\n\t3" + add), check_absent, *vals, template='A\n\t', item_sep='\n\t')
+    raises(exc("A items: '2' 3" + add), check_absent, *vals, template='A {}: ', item_sep=' ')
+    raises(exc("A items('2',3)" + add), check_absent, *vals, template='A {}({})', item_sep=',')
+    raises(exc("A xs('2',3)" + add), check_absent, *vals, 'x', template='A {}({})', item_sep=',')
+    raises(exc("A x('2',3)" + add), check_absent, *vals, '', template='A x{}({})', item_sep=',')
+
+    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
+                      func_name='check_absent()'),
+           check_absent, *vals, template='{}{}{}')        # with error
+    assert check_absent((1, 2), [1], template='{}{}{}')     # without error, but more pythonic
+
+    assert check_absent(*vals, as_text=True) == "Absent items: '2', 3" + add
+    assert check_absent((1, 2), [1], as_text=True) == ""
+    assert check_absent((1, 2), [1]) == (1, 2)
+
+    exc_inp = InputError('name1', msg="Absent items: '2', 3" + add)
+    raises(exc_inp, check_absent, *vals, input_exc=('', 'name1'))
+    assert check_absent(*vals, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
+
+    msg = "Absent strs: 2, 3. Must be not less than expected (1, 2, 3), but received: 1"
+    raises(exc(msg), check_absent, *vals, 'str', str)
+    raises(exc(msg + ". Some x"), check_absent, *vals, 'str', str, some='x')
+
+
+def test_check_items():
+    exc = CheckValueError
+    add1 = ". Must be equal to expected (1), but received: 1, '2', 3"
+    raises(exc("Extra item: 2. Must be equal to expected (1), but received: 1, 2"),
+           check_items, (1, 2), [1])
+    raises(exc("Extra items: '2', 3" + add1), check_items, (1, '2', 3), [1])
+    raises(exc("Extra vals: '2', 3" + add1), check_items, (1, '2', 3), [1], 'val')
+
+    add2 = ". Must be equal to expected (1, '2', 3), but received: 1"
+    raises(exc("Absent item: 2. Must be equal to expected (1, 2), but received: 1"),
+           check_items, [1], (1, 2))
+    raises(exc("Absent items: '2', 3" + add2), check_items, [1], (1, '2', 3))
+    raises(exc("Absent vals: '2', 3" + add2), check_items, [1], (1, '2', 3), 'val')
+
+    msg = "Extra item: 2. Absent item: 3"
+    raises(exc(msg + ". Must be equal to expected (3), but received: 2"), check_items, [2], [3])
+    raises(exc(msg + ". Must be equal to expected (1, 3), but received: 1, 2"),
+           check_items, (1, 2), (1, 3))
+
+    eav = (1, '2', 4), (1, '3', 5)
+    add3 = ". Must be equal to expected (1, '3', 5), but received: 1, '2', 4"
+    add4 = ". Must be equal to expected (1, 3, 5), but received: 1, 2, 4"
+    msg = "Extra items: '2', 4. Absent items: '3', 5"
+    msg2 = ("Extra items: 2, 4. Absent items: 3, 5. "
+            "Must be equal to expected (3, 5), but received: 2, 4")
+    raises(exc(msg2), check_items, (2, 4), (3, 5))
+    raises(exc(msg + add3), check_items, *eav)
+
+    raises(exc("Extra vals: '2', 4. Absent vals: '3', 5" + add3), check_items, *eav, 'val')
+
+    raises(exc("Extra strs: 2, 4. Absent strs: 3, 5" + add4), check_items, *eav, 'str', str)
+    raises(exc("Extra strs: 2, 4. Absent strs: 3, 5" + add4 + ". Some x"),
+           check_items, *eav, 'str', str, some='x')
+
+    raises(exc("E:\n\t'2'\n\t4\nA:\n\t'3'\n\t5" + add3), check_items, *eav,
+           extra_template='E:\n\t', absent_template='A:\n\t', check_sep='\n', item_sep='\n\t')
+    raises(exc("E items: '2' 4 | A items: '3' 5" + add3), check_items, *eav,
+           extra_template='E {}: ', absent_template='A {}: ', check_sep=' | ', item_sep=' ')
+    raises(exc("E items('2',4) | A items('3',5)" + add3), check_items, *eav,
+           extra_template='E {}({})', absent_template='A {}({})', check_sep=' | ', item_sep=',')
+    raises(exc("E coords('2',4) | A coords('3',5)" + add3), check_items, *eav, 'coord',
+           extra_template='E {}({})', absent_template='A {}({})', check_sep=' | ', item_sep=',')
+    raises(exc("E coord('2',4) | A coord('3',5)" + add3), check_items, *eav, '',
+           extra_template='E coord{}({})', absent_template='A {}coord({})', check_sep=' | ',
+           item_sep=',')
+
+    # Template error
+    exc = partial(InputError, must_be='not more than 2 data places', received="'{}{}{}'",
+                  func_name='check_items()')
+    error = exc('extra_template')
+    raises(error, check_items, (1, 2), (1, 3), extra_template='{}{}{}')
+    raises(error, check_items, (1, 2), (1, 3), extra_template='{}{}{}', absent_template='{}{}')
+    error = exc('absent_template')
+    raises(error, check_items, (1, 2), (1, 3), absent_template='{}{}{}')
+    raises(error, check_items, (1, 2), (1, 3), extra_template='{}{}', absent_template='{}{}{}')
+
+    # Without error, but more pythonic
+    assert check_items([1], [1], extra_template='{}{}{}')
+    assert check_items([1], [1], absent_template='{}{}{}')
+    assert check_items([1], [1], extra_template='{}{}{}', absent_template='{}{}')
+    assert check_items([1], [1], extra_template='{}{}', absent_template='{}{}{}')
+    assert check_items([1], [1], extra_template='{}{}{}', absent_template='{}{}{}')
+
+    extra_msg = "Extra items: '2', 4"
+    absent_msg = "Absent items: '3', 5"
+    add_extra = ". Must be not more than expected (1, '3', 5), but received: 1, '2', 4"
+    add_absent = ". Must be not less than expected (1, '3', 5), but received: 1, '2', 4"
+    assert check_items(*eav, as_text=True) == f'{extra_msg}. {absent_msg}' + add3
+    assert check_items(*eav, as_text=True, extra=False) == absent_msg + add_absent
+    assert check_items(*eav, as_text=True, absent=False) == extra_msg + add_extra
+    assert check_items(*eav, as_text=True, extra=False, absent=False) == ""
+    assert check_items(*eav, extra=False, absent=False) == (1, '2', 4)
+    assert check_items((1, 2), (1, 2), as_text=True) == ""
+    assert check_items((1, 2), (1, 2)) == (1, 2)
+
+    exc_inp = InputError('name1', msg=f'{extra_msg}. {absent_msg}' + add3)
+    raises(exc_inp, check_items, *eav, input_exc=('', 'name1'))
+    assert check_items(*eav, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
+
+
+def test_check_lengths():
+    assert check_lengths([1], [1])
+    assert check_lengths([2], [3])
+    assert check_lengths((1, 2, 4), (1, 3, 5))
+    exc = CheckValueError
+    ev = (1, '2', 3), [1]
+    av = ev[::-1]
+
+    # Extra values length
+    add1 = ". Must be 1 value long, but received 3"
+    raises(exc("Extra value: 2. Must be 1 value long, but received 2"),
+           check_lengths, (1, 2), [1])
+    raises(exc("Extra vals: '2', 3. Must be 1 val long, but received 3"),
+           check_lengths, *ev, 'val')
+    raises(exc("Extra values: '2', 3" + add1),
+           check_lengths, *ev)
+
+    raises(exc("E\n\t'2'\n\t3" + add1),
+           check_lengths, *ev, extra_template='E\n\t', item_sep='\n\t')
+    raises(exc("E values: '2' 3" + add1),
+           check_lengths, *ev, extra_template='E {}: ', item_sep=' ')
+    raises(exc("E values('2',3)" + add1),
+           check_lengths, *ev, extra_template='E {}({})', item_sep=',')
+    raises(exc("E xs('2',3). Must be 1 x long, but received 3"),
+           check_lengths, *ev, 'x', extra_template='E {}({})', item_sep=',')
+    raises(exc("E x('2',3). Must be 1  long, but received 3"),
+           check_lengths, *ev, '', extra_template='E x{}({})', item_sep=',')
+
+    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
+                      func_name='check_lengths()'),
+           check_lengths, *ev, extra_template='{}{}{}')  # with error
+
+    assert check_lengths(*ev, as_text=True) == "Extra values: '2', 3" + add1
+    assert check_lengths([1], (1, 2), absent=False, as_text=True) == ""
+    assert check_lengths([1], (1, 2), absent=False) == [1]
+
+    exc_inp = InputError('name1', msg="Extra values: '2', 3" + add1)
+    raises(exc_inp, check_lengths, *ev, input_exc=('', 'name1'))
+    assert check_lengths(*ev, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
+
+    raises(exc("Extra strs: 2, 3. Must be 1 str long, but received 3"),
+           check_lengths, *ev, 'str', str)
+    raises(exc("Extra strs: 2, 3. Must be 1 str long, but received 3. Some x"),
+           check_lengths, *ev, 'str', str, some='x')
+
+    # Absent values length
+    add2 = ". Must be 3 values long, but received 1"
+    raises(exc("Absent value: 2. Must be 2 values long, but received 1"),
+           check_lengths, [1], (1, 2))
+    raises(exc("Absent vals: '2', 3. Must be 3 vals long, but received 1"),
+           check_lengths, *av, 'val')
+    raises(exc("Absent values: '2', 3" + add2),
+           check_lengths, *av)
+    raises(exc("A\n\t'2'\n\t3" + add2),
+           check_lengths, *av, absent_template='A\n\t', item_sep='\n\t')
+    raises(exc("A values: '2' 3" + add2),
+           check_lengths, *av, absent_template='A {}: ', item_sep=' ')
+    raises(exc("A values('2',3)" + add2),
+           check_lengths, *av, absent_template='A {}({})', item_sep=',')
+    raises(exc("A xs('2',3). Must be 3 xs long, but received 1"),
+           check_lengths, *av, 'x', absent_template='A {}({})', item_sep=',')
+    raises(exc("A x('2',3). Must be 3  long, but received 1"),
+           check_lengths, *av, '', absent_template='A x{}({})', item_sep=',')
+
+    raises(InputError('template', must_be='not more than 2 data places', received="'{}{}{}'",
+                      func_name='check_lengths()'),
+           check_lengths, *av, absent_template='{}{}{}')     # with error
+
+    assert check_lengths(*av, as_text=True) == "Absent values: '2', 3" + add2
+    assert check_lengths((1, 2), [1], extra=False,  as_text=True) == ""
+    assert check_lengths((1, 2), [1], extra=False) == (1, 2)
+
+    exc_inp = InputError('name1', msg="Absent values: '2', 3" + add2)
+    raises(exc_inp, check_lengths, *av, input_exc=('', 'name1'))
+    assert check_lengths(*av, input_exc=('', 'name1'), as_text=True) == str(exc_inp)
+
+    raises(exc("Absent strs: 2, 3. Must be 3 strs long, but received 1"),
+           check_lengths, *av, 'str', str)
+    raises(exc("Absent strs: 2, 3. Must be 3 strs long, but received 1. Some x"),
+           check_lengths, *av, 'str', str, some='x')
+
+    # Wrong template (without error, but more pythonic)
+    assert check_lengths([0], [0], extra_template='{}{}{}')
+    assert check_lengths([1], [1], absent_template='{}{}{}')
+    assert check_lengths([0], [1], extra_template='{}{}{}', absent_template='{}{}')
+    assert check_lengths([1], [0], extra_template='{}{}', absent_template='{}{}{}')
+    assert check_lengths([2], [3], extra_template='{}{}{}', absent_template='{}{}{}')
+
+
+def test_check_type():
+    # Check simple
+    assert check_type('some', str) == 'some'
+    raises(InputError('obj_t', must_be='type or types', received="'int' (str)",
+                      func_name='check_type()'),
+           check_type, 'some', 'int')
+
+    # Check with typecast if enabled
+    assert check_type('5', int, True) == check_type('5', int, typecast=True) == 5
+    assert check_type('some', (int, tuple), True) == ('s', 'o', 'm', 'e')
+
+    # Format error
+    raises(CheckTypeError("'some' (str) must be int type"), check_type, 'some', int)
+
+    assert isinstance(exc1 := safe(int, 'some'), ValueError)
+    raises(CheckTypeError(f"'some' (str) must be int type, typecast to int: {exc1!r}"),
+           check_type, 'some', int, True)
+
+    assert isinstance(exc2 := safe(dict, 'some'), ValueError)
+    msg = (f"'some' (str) must be int or dict types, typecast to int: {exc1!r}, "
+           f"typecast to dict: {exc2!r}")
+    raises(CheckTypeError(msg), check_type, 'some', (int, dict), True)
+
+    field_error = CheckTypeError('Field ' + msg)
+    raises(field_error, check_type, 'some', (int, dict), True, 'field')
+    raises(field_error, check_type, 'some', (int, dict), typecast=True, name='field')
+
+
+def test_check_types():
+    # Check mutually exclusive input parameters
+    raises(InputError('one_obj', 'pairs', must_be='not more than one True', received='both',
+                      func_name='check_types()'),
+           check_types, (), None, one_obj=True, pairs=True)
+
+    # Check input obj
+    obj_error = partial(InputError, 'obj', must_be='one or more objects without None',
+                        func_name='check_types()')
+    raises(obj_error(received="obj = None (objects = ())"), check_types, None, None)
+    raises(obj_error(received="obj = ()"), check_types, (), None)
+    raises(obj_error(received="obj = (<class 'tuple'>, None)"), check_types, (tuple, None), None)
+
+    # Check input obj_t
+    obj_t_error = partial(InputError, 'obj_t', must_be='type or types', func_name='check_types()')
+    raises(obj_t_error(received="() (tuple)"), check_types, 1, ())
+    raises(obj_t_error(received="None (NoneType)"), check_types, 1, None)
+    raises(obj_t_error(received="5 (int)"), check_types, 5, 5)
+    raises(obj_t_error(received="5 (int) at pos 0"), check_types, 5, (5, int))
+    raises(obj_t_error(received="5 (int) at pos 1"), check_types, 5, (int, 5))
+    raises(obj_t_error(received="5 (int) at pos 0, True (bool) at pos 3"),
+           check_types, 5, (5, int, str, True))
+
+    # Check typecast specific
+    msg = ("5 (int) must be WrongCast or tuple types, "
+           "typecast to WrongCast: 5 (int), "
+           "typecast to tuple: TypeError(\"'int' object is not iterable\")")
+    raises(CheckTypeError(msg), check_types, 5, (WrongCast, tuple), True)
+
+    # Check dicts specific
+    msg = "Extra key (without type): '2'. Absent keys (type provided): '3', '4'"
+    raises(InputError('obj', msg=msg, func_name='check_types()'),
+           check_types, {'1': 1, '2': 2}, {'1': int, '3': str, '4': str})
+
+    # Check pairs specific
+    msg = "Extra value (without type): '13'. Must be 1 value long, but received 2"
+    raises(InputError('obj', msg=msg, func_name='check_types()'),
+           check_types, (5, '13'), str, pairs=True)
+
+    # Check error in single objects
+    raises(CheckTypeError("5 (int) must be str type"), check_types, 5, str)
+    raises(CheckTypeError("5 (int) must be str or bool types"), check_types, 5, (str, bool))
+    raises(CheckTypeError("5 (int) at pos 0 must be str type"), check_types, (5, 'x'), str)
+    raises(CheckTypeError("5 (int) at pos 0 must be str or bool types"),
+           check_types, (5, 'x'), (str, bool))
+
+    # Check errors in multiple positional objects
+    msg = "Several objects are not bool type: 5 (int) at pos 0, 'x' (str) at pos 1"
+    raises(CheckTypeError(msg), check_types, (5, 'x'), bool)
+
+    msg = "Several objects are not bool or float types: 5 (int) at pos 0, 'x' (str) at pos 1"
+    raises(CheckTypeError(msg), check_types, (5, 'x'), (bool, float))
+
+    msg = ("Several objects has a wrong type:\n"
+           "\t5 (int) at pos 0 must be bool type\n"
+           "\t'x' (str) at pos 1 must be float type")
+    raises(CheckTypeError(msg), check_types, (5, 'x'), (bool, float), pairs=True)
+
+    msg = ("Several objects has a wrong type:\n"
+           "\t5 (int) at pos 0 must be bool type\n"
+           "\t'x' (str) at pos 1 must be float type")
+    raises(CheckTypeError(msg), check_types, (5, 'x'), {1: bool, 2: float}, pairs=True)
+
+    # Check errors in multiple named objects
+    dict_item, dict_items = {'name1': 5}, {'name1': 5, 2: '3'}
+    raises(CheckTypeError("'name1'=5 (int) must be str type"), check_types, dict_item, str)
+
+    msg = ("'name1'=5 (int) must be WrongCast or tuple types, "
+           "typecast to WrongCast: 5 (int), "
+           "typecast to tuple: TypeError(\"'int' object is not iterable\")")
+    raises(CheckTypeError(msg), check_types, dict_item, (WrongCast, tuple), True)
+
+    msg = "Several objects are not bool type: 'name1'=5 (int), 2='3' (str)"
+    raises(CheckTypeError(msg), check_types, dict_items, bool)
+
+    msg = ("Several objects has a wrong type:\n"
+           "\tname1: 5 (int) must be bool type\n"
+           "\t2: '3' (str) must be float type")
+    raises(CheckTypeError(msg), check_types, dict_items, (bool, float), pairs=True)
+
+    msg = ("Several objects has a wrong type:\n"
+           "\tname1: 5 (int) must be bool type\n"
+           "\t2: '3' (str) must be float type")
+    raises(CheckTypeError(msg), check_types, dict_items, {2: float, 'name1': bool})
+
+    # Check named params
+    name = 'item'
+    raises(CheckTypeError("Item 'name1'=5 (int) must be str type"),
+           check_types, dict_item, str, item_name=name)
+
+    msg = ("Item 'name1'=5 (int) must be WrongCast or tuple types, "
+           "typecast to WrongCast: 5 (int), "
+           "typecast to tuple: TypeError(\"'int' object is not iterable\")")
+    raises(CheckTypeError(msg), check_types, dict_item, (WrongCast, tuple), True, item_name=name)
+
+    msg = ("Several items has a wrong type:\n"
+           "\tItem name1: 5 (int) must be bool type\n"
+           "\tItem 2: '3' (str) must be float type")
+    raises(CheckTypeError(msg), check_types, dict_items, (bool, float), pairs=True, item_name=name)
+
+    msg = "Several items are not bool type: 5 (int) at pos 0, '3' (str) at pos 1"
+    raises(CheckTypeError(msg), check_types, (5, '3'), bool, item_name=name)
+
+    msg = "Several items are not bool type: 'name1'=5 (int), 2='3' (str)"
+    raises(CheckTypeError(msg), check_types, dict_items, bool, item_name=name)
+
+    # Positive check input obj
+    assert check_types((), tuple, one_obj=True) == ()
+    assert check_types((5,), int) == (5,)
+    assert check_types((5,), tuple, one_obj=True) == (5,)
+
+    # Positive check single objects
+    assert check_types(5, (str, bool, int)) == 5
+    assert check_types(5, (str, bool, int), True) == 5
+    assert check_types('5', int, True) == 5
+
+    # Positive check multiple objects
+    test_obj = (5, 'x', False)
+    assert check_types(test_obj, str, True) == ('5', 'x', 'False')
+    assert check_types(test_obj, (str, bool, int)) == test_obj
+    assert check_types(test_obj, (str, bool, int), True, pairs=True) == ('5', True, 0)
+    assert check_types(dict_items, (str, int)) == dict_items
+    assert check_types(dict_items, (str, int), True, pairs=True) == {'name1': '5', 2: 3}
+    assert check_types(dict_items, {2: int, 'name1': str}, True) == {'name1': '5', 2: 3}  # noqa
+
+    # Positive check mutually exclusive input parameters
+    assert check_types(test_obj, (tuple,), one_obj=True, pairs=False) == test_obj
+    assert check_types(test_obj, (int, str, bool), one_obj=False, pairs=True) == test_obj
+    assert check_types(test_obj, (int, str), one_obj=False, pairs=False) == test_obj
+
+
+# Decorators
+
+
+def test_decorate_methods():    # noqa C901
+    class Fixed(str):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    def decorator(func):  # noqa
+        return 'Processed'
+
+    @decorate_methods(decorator)
+    class Empty(Fixed):
+        attr = 1
+
+    @decorate_methods(decorator)
+    class Visible(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude=is_hidden)
+    class Hidden1(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude=('_intern', '__dnd__'))
+    class Hidden2(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude=is_internal)
+    class Internal1(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude='_intern')
+    class Internal2(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude=is_dunder)
+    class Dunder1(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude='__dnd__')
+    class Dunder2(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude=lambda x: x)
+    class NoOne(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    @decorate_methods(decorator, exclude=lambda x: '')
+    class All(Fixed):
+        attr = 1
+        def visible(self): pass
+        def _intern(self): pass
+        def __dnd__(self): pass
+
+    for cls, v_state, h_state, d_state in [(Fixed, False, False, False),
+                                           (Empty, False, False, False),
+                                           (Visible, True, False, False),
+                                           (Hidden1, True, False, False),
+                                           (Hidden2, True, False, False),
+                                           (Internal1, True, False, True),
+                                           (Internal2, True, False, True),
+                                           (Dunder1, True, True, False),
+                                           (Dunder2, True, True, False),
+                                           (NoOne, False, False, False),
+                                           (All, True, True, True)]:
+        assert cls.attr == 1
+        assert (cls.visible == 'Processed') == v_state
+        assert (cls._intern == 'Processed') == h_state
+        assert (cls.__dnd__ == 'Processed') == d_state
+
+
+def test_init_reraise():
+    class Some1:
+        @init_reraise
+        def __init__(self, *args, **kwargs):  # noqa
+            if kwargs.get('no_exception'):
+                return
+            raise ValueError('Bad')
+
+    class Some2:
+        @init_reraise
+        def __init__(self):
+            raise ValueError('Bad')
+
+    class Cat:
+        @init_reraise('animal')
+        def __init__(self):
+            raise ValueError('Bad')
+
+    class Dog:
+        """Kristy, the dog"""
+        @init_reraise('animal', doc=True)
+        def __init__(self):
+            raise ValueError('Bad')
+
+    def error(view='', *, cn='Some1', tn='class'):
+        return InitError(f"Cannot init {tn} {cn!r} (self.__init__({view}))"), ValueError('Bad')
+
+    Some1(no_exception=True)
+    raises(error(), Some1)
+    raises(error(cn='Some2'), Some2)
+    raises(error(cn='Cat', tn='animal'), Cat)
+    raises(error(cn='Kristy, the dog', tn='animal'), Dog)
+
+    for kwv, _kwargs in (('', {}), ('x=3', {'x': 3}), ('x=3, y=4', {'x': 3, 'y': 4})):
+        for v, _args in (('', ()), ('1', (1,)), ('1, 2', (1, 2))):
+            raises(error(f'{v}, {kwv}' if v and kwv else v or kwv), Some1, *_args, **_kwargs)
+
+
+def test_set_slots_defaults():
+    def deco(*args, **kwargs):
+        @set_slots_defaults(*args, **kwargs)
+        class Deco:  # noqa
+            f1 = 1
+            f2 = '2'
+        return Deco
+
+    def error(params, msg, func_name):
+        return InputError(*as_holder(params), func_name=func_name, msg=msg)
+
+    def deco_error(params, msg):
+        return error(params, msg, '@set_slots_defaults()')
+
+    def init_error(params, msg):
+        return error(params, msg, 'Deco()')
+
+    # Decorator input params error
+    raises(deco_error('field_names', '5 (int) must be str type'), deco, 5)
+    raises(deco_error('field_names', '5 (int) at pos 2 must be str type'), deco, ('x', 'y', 5))
+    raises(deco_error('field_func', '5 (int) must be Callable type'), deco, 'x', 5)
+    raises(deco_error('fields_t', '5 (int) must be type type'), deco, 'x', lambda: True, 5)
+
+    # Decorator equality with different ways of fields declaring
+    @set_slots_defaults
+    class Deco:
+        f1 = 1
+        f2 = '2'
+        f3 = empty_func
+    assert Deco() == deco()() == deco('f1')() == deco(('f1', 'f2'), lambda k, v: False)()
+
+    # Decorator repr validity
+    assert Deco() == eval(repr(Deco()))
+
+    # Decorated class init error
+    raises(init_error('*args', "Extra value: 'x3'. Must be 2 values long, but received 3"),
+           Deco, 'x1', 'x2', 'x3')
+    err_msg = ". Must be not more than expected ('f1', 'f2'), but received: 'f1', 'f2', 'f3'"
+    raises(init_error('**kwargs', "Extra item: 'f3'" + err_msg), Deco, f1='x1', f2='x2', f3='x3')
+
+    err_msg = 'Already provided item in args: '
+    raises(init_error(('*args', '**kwargs'), err_msg + 'f2'), Deco, 'x1', 'x2', f2='x2')
+    raises(init_error(('*args', '**kwargs'), err_msg + 'f1'), Deco, 'x1', f1='x1')
+
+    raises(init_error('*args', "'x1' (str) at pos 0 must be int type"), deco(fields_t=int), 'x1')
+    raises(init_error('**kwargs', "'f1'='x1' (str) must be int type"), deco(fields_t=int), f1='x1')
+
+
+# Getters
+
+
+def test_get_cls_obj():
+    assert get_cls_obj(None) == (None, None)
+    assert get_cls_obj(int) == (int, None)
+    assert (x := get_cls_obj(5)) == (int, 5) == (x.cls, x.obj)
+
+
+def test_get_cls_attr():
+    class Something:
+        pass
+
+    assert get_cls_attr(None, '__qualname__') is None
+    assert get_cls_attr(Something, '__qualname__') == Something.__qualname__
+    assert get_cls_attr(Something(), '__qualname__') == Something.__qualname__
+    raises(AttributeError("type object 'Something' has no attribute 'asd'"),
+           get_cls_attr, Something, 'asd')
+
+
+def test_get_attrs():
+    # Checked classes
+    class C1:
+        """Class 1 (base)"""
+        x1: int                                                                      # type: ignore
+        x2: int = 12                                                                 # type: ignore
+        x3 = 13
+        x6: int                                                                      # type: ignore
+        _x7: int                                                                     # type: ignore
+        _x8 = 18
+
+    class C1S:
+        """Class 1 (base, slots)"""
+        __slots__ = ('x6', '_x7')
+        x1: int                                                                      # type: ignore
+        x2: int = 12                                                                 # type: ignore
+        x3 = 13
+        x6: int                                                                      # type: ignore
+        _x7: int                                                                     # type: ignore
+        _x8 = 18
+
+    class C2(C1):
+        """Class 2 (inherited)"""
+        x1 = 21
+        x2 = 22
+        x4 = 24
+        x5: int = 25                                                                 # type: ignore
+
+        def __init__(self, x6=36, x7=37, x9=39):
+            self.x6 = x6
+            self._x7 = x7
+            self.x9 = x9
+
+    class C2S(C1S):
+        """Class 2 (inherited, slots)"""
+        __slots__ = ('x9',)
+        x1 = 21
+        x2 = 22
+        x4 = 24
+        x5: int = 25                                                                 # type: ignore
+
+        def __init__(self, x6=36, x7=37, x9=39):
+            self.x6 = x6
+            self._x7 = x7
+            self.x9 = x9
+
+    # Skip args check
+    def skip_recv(total: int, parent: int, child: int):
+        return {'must_be': f'less than {total} skipped in total',
+                'skipped': f': {total} (skip_parent = {parent}, skip_child = {child})'}
+
+    exc = partial(InputError, 'skip_parent', 'skip_child', func_name='get_attrs()')
+    raises(exc(**skip_recv(2, 2, 0)), get_attrs, C2, 2)
+    raises(exc(**skip_recv(2, 1, 1)), get_attrs, C2, 1, 1)
+    raises(exc(**skip_recv(3, 3, 0)), get_attrs, C2, 3, ignored=())
+    raises(exc(**skip_recv(3, 2, 1)), get_attrs, C2, 2, 1, ignored=())
+
+    exc2 = InputError('ignored', func_name='get_attrs()', msg="1 (int) at pos 0 must be type type")
+    raises(exc2, get_attrs, C2, ignored=(1,))
+
+    # Helper functions
+    def merge_common(x, y, attrs=('__annotations__', '__slots__')) -> dict:
+        return {attr: (xa | ya if isinstance(xa or ya, Mapping) else (*xa, *ya)) for attr in attrs
+                if (xa := getattr(x, attr, {}), ya := getattr(y, attr, {})) and xa or ya}
+
+    def dict_build(obj) -> dict:
+        return {k: getattr(obj, k, None) for k in obj.__dir__()}
+
+    # Helper base objects
+    co = object                 # class <object>
+    cod = co.__dict__           # class <object> dict
+
+    ct = type                   # class <type>
+    ctd = cod | type.__dict__   # class <type> dict (type is inherited from object!)
+    cta = {'mro': type.mro}     # class <type> attributes
+
+    oo = co()                   # object <object>
+    ood = dict_build(oo)        # object <object> dict
+
+    # Helper exceptions
+    __e = partial(InputError, 'obj', must_be='not ignored type', func_name='get_attrs()',
+                  ignored_types=': type, object')
+    cte = __e(received="type (type)")
+    coe = __e(received="object (type)")
+    ooe = __e(received=f"{oo!r} (object)")
+
+    # Helper class 1 objects
+    c1_____ = {'x2': 12, 'x3': 13}      # class 1 attributes
+    c1__h__ = c1_____ | {'_x8': 18}     # class 1 internal
+    c1__hd_ = C1.__dict__               # class 1 hidden
+    c1___d_ = c1__hd_.copy()            # class 1 dunder
+    c1___d_.pop('_x8')                  # [-] remove internal
+    c1___di = cod | c1___d_             # class 1 dunder no_ignored
+    c1__hdi = cod | c1__hd_             # class 1 hidden no_ignored
+
+    o1 = C1()                           # object 1
+
+    # Helper class 1 slots objects
+    c1s____ = c1_____ | {'x6': C1S.x6}              # class 1 slots attributes
+    c1s_h__ = c1__h__ | c1s____ | {'_x7': C1S._x7}  # class 1 slots internal
+    c1s_hd_ = C1S.__dict__                          # class 1 slots hidden
+    c1s__d_ = c1s_hd_.copy()                        # class 1 slots dunder
+    c1s__d_.pop('_x7')                              # [-] remove internal
+    c1s__d_.pop('_x8')                              # [-] remove internal
+    c1s__di = cod | c1s__d_                         # class 1 slots dunder no_ignored
+    c1s_hdi = cod | c1s_hd_                         # class 1 slots hidden no_ignored
+
+    o1s = C1S()                                     # object 1 slots
+    o1s_hd_ = dict_build(o1s) | c1s_hd_             # object 1 slots hidden
+    o1s__d_ = o1s_hd_.copy()                        # object 1 slots dunder
+    o1s__d_.pop('_x7')                              # [-] remove internal
+    o1s__d_.pop('_x8')                              # [-] remove internal
+    o1s__di = cod | o1s__d_                         # object 1 slots dunder no_ignored
+    o1s_hdi = cod | o1s_hd_                         # object 1 slots hidden no_ignored
+
+    # Helper class 2 objects
+    c2_____ = c1_____ | {'x1': 21, 'x2': 22, 'x4': 24, 'x5': 25}    # class 2 attributes
+    c2__h__ = c1__h__ | c2_____                                     # class 2 internal
+    c2__hd_ = c1__hd_ | C2.__dict__ | merge_common(C1, C2)          # class 2 hidden
+    c2___d_ = c2__hd_.copy()                                        # class 2 dunder
+    c2___d_.pop('_x8')                                              # [-] remove internal
+    c2___di = cod | c2___d_                                         # class 2 dunder no_ignored
+    c2__hdi = cod | c2__hd_                                         # class 2 hidden no_ignored
+
+    o2 = C2()                                                       # object 2
+    o2_____ = c2_____ | {'x6': 36, 'x9': 39}                        # object 2 attributes
+    o2__h__ = c1__h__ | o2_____ | {'_x7': 37}                       # object 2 internal
+    o2___d_ = c1___d_ | c2___d_ | o2_____                           # object 2 dunder
+    o2__hd_ = o2__h__ | o2___d_                                     # object 2 hidden
+    o2___di = cod | o2___d_                                         # object 2 dunder no_ignored
+    o2__hdi = cod | o2__hd_                                         # object 2 hidden no_ignored
+
+    # Helper class 2 slots objects
+    c2s____ = c1s____ | c2_____ | {'x9': C2S.x9}                # class 2 slots attributes
+    c2s_h__ = c1s_h__ | c2s____                                 # class 2 slots internal
+    c2s_hd_ = c1s_hd_ | C2S.__dict__ | merge_common(C1S, C2S)   # class 2 slots hidden
+    c2s__d_ = c2s_hd_.copy()                                    # class 2 slots dunder
+    c2s__d_.pop('_x7')                                          # [-] remove internal
+    c2s__d_.pop('_x8')                                          # [-] remove internal
+    c2s__di = cod | c2s__d_                                     # class 2 dunder no_ignored
+    c2s_hdi = cod | c2s_hd_                                     # class 2 hidden no_ignored
+
+    o2s = C2S()
+    o2s_hd_ = dict_build(o2s) | merge_common(C1S, C2S)          # object 2 slots hidden
+    o2s__d_ = o2s_hd_.copy()                                    # object 2 slots dunder
+    o2s__d_.pop('_x7')                                          # [-] remove internal
+    o2s__d_.pop('_x8')                                          # [-] remove internal
+    o2s__di = cod | o2s__d_                                     # object 2 slots dunder no_ignored
+    o2s_hdi = cod | o2s_hd_                                     # object 2 slots hidden no_ignored
+
+    # Helper func kwargs
+    h__ = {'internal': True}
+    _d_ = {'dunder': True}
+    __i = {'ignored': ()}
+    hd_ = h__ | _d_
+    h_i = h__ | __i
+    _di = _d_ | __i
+    hdi = hd_ | __i
+
+    # All others checks, values: 0:empty, 1:internal, 2:dunder, 3:internal|dunder,
+    # 4:no_ignored, 5:no_ignored|internal, 6:no_ignored|dunder, 7:no_ignored|internal|dunder
+    for func, results in (
+            (None,  [InputError('obj', must_be='not None', received='None',
+                                func_name='get_attrs()')] * 8),
+            (ct,    [cte, cte, cte, cte, cta, cta, ctd, ctd]),
+            (co,    [coe, coe, coe, coe, {},  {},  cod, cod]),
+            (oo,    [ooe, ooe, ooe, ooe, {},  {},  ood, ood]),
+            (C1,    [c1_____, c1__h__, c1___d_, c1__hd_, c1_____, c1__h__, c1___di, c1__hdi]),
+            (o1,    [c1_____, c1__h__, c1___d_, c1__hd_, c1_____, c1__h__, c1___di, c1__hdi]),
+            (C1S,   [c1s____, c1s_h__, c1s__d_, c1s_hd_, c1s____, c1s_h__, c1s__di, c1s_hdi]),
+            (o1s,   [c1s____, c1s_h__, o1s__d_, o1s_hd_, c1s____, c1s_h__, o1s__di, o1s_hdi]),
+            (C2,    [c2_____, c2__h__, c2___d_, c2__hd_, c2_____, c2__h__, c2___di, c2__hdi]),
+            (o2,    [o2_____, o2__h__, o2___d_, o2__hd_, o2_____, o2__h__, o2___di, o2__hdi]),
+            (C2S,   [c2s____, c2s_h__, c2s__d_, c2s_hd_, c2s____, c2s_h__, c2s__di, c2s_hdi]),
+            (o2s,   [o2_____, o2__h__, o2s__d_, o2s_hd_, o2_____, o2__h__, o2s__di, o2s_hdi])):
+        for kwargs, result in zip(({}, h__, _d_, hd_, __i, h_i, _di, hdi), results, strict=True):
+            if isinstance(result, Exception) or result == InputError:
+                raises(result, get_attrs, func, **kwargs)
+            else:
+                assert get_attrs(func, **kwargs) == result
+
+
+def test_get_name():    # noqa C901
+    test_funcs = (GetName, partial(GetName, full=True))
+
+    # Check wrong input
+    wrong_names = ("attr", "attr_cls", "attrs_", "attrs_cos")
+    order = ('some_obj', 'code_obj', 'not_exists')
+    possible_parameters = ("Possible parameters: doc_obj, code_obj, attrs_obj, doc_cls, "
+                           "attrs_cls, str_obj, str_cls, repr_cls, repr_obj")
+    details = f"Received: 'some_obj', 'code_obj', 'not_exists'. {possible_parameters}"
+    for kwargs, exc_kwargs in [
+        ({'doc': ()}, {"msg": "() (tuple) must be bool type"}),
+        ({'doc_cls': ()}, {"msg": "() (tuple) must be bool type"}),
+        ({'attrs': []}, {"msg": "[] (list) must be bool or tuple types"}),
+        ({'attrs_obj': []}, {"msg": "[] (list) must be bool or tuple types"}),
+        ({'order': order}, {"msg": f"Not exists methods: 'some_obj', 'not_exists'. {details}"}),
+        ({}.fromkeys(wrong_names), {"msg": possible_parameters})
+    ]:
+        for func in test_funcs:
+            raises(InputError(*kwargs, **exc_kwargs, func_name='GetName()'), func, '', **kwargs)
+
+    # Check method wrong input
+    msg = ("Provided wrong parameter to GetName.attrs(): attrs. Must be 1 (same for both) "
+           "or 2 (separately) provided for cls and obj, but received 3: 'some', 1, 2")
+    raises(InputError(msg=msg), GetName.attrs, 'obj', 'some', 1, 2)
+    msg = ("Provided wrong parameter(s) to GetName.doc(). "
+           "Must be no arguments, but received 1: 'some'")
+    raises(InputError(msg=msg), GetName.doc, 'obj', 'some')
+
+    # Check for None target
+    for func in test_funcs:
+        assert func(None, none=None) is None
+        assert (name_obj := func(None)) == ""
+        assert isinstance(name_obj, GetName)
+
+    # Check for unknown target
+    for func in test_funcs:
+        assert func('', unknown=None, attrs=False, repr=False) is None
+        assert (name_obj := func('', attrs=False, repr=False)) == ""
+        assert isinstance(name_obj, GetName)
+
+    # Prepare data for positive full=True check
+    def code_obj():
+        pass
+
+    class Non:
+        pass
+
+    class Cls:
+        """doc_cls"""
+        name = 'attrs_cls'
+        custom_name = 'attrs_custom_cls'
+
+        @classmethod
+        def __repr__(cls):
+            return 'repr_cls'
+
+        @classmethod
+        def __str__(cls):
+            return 'str_cls'
+
+    class Obj:
+        def __init__(self):
+            self.__doc__ = 'doc_obj'
+            self.__code__ = code_obj.__code__
+            self.name = 'attrs_obj'
+            self.__name__ = 'attrs_dunder_obj'
+            self.custom_name = 'attrs_custom_obj'
+            self.__repr__ = lambda: 'repr_obj'
+            self.__str__ = lambda: 'str_obj'
+
+    class COb(Cls, Obj):
+        pass
+
+    class All:
+        """doc_cls"""
+        name = 'attrs_cls'
+        custom_name = 'attrs_custom_cls'
+
+        @classmethod
+        def __repr__(cls):
+            return 'repr_cls'
+
+        @classmethod
+        def __str__(cls):
+            return 'str_cls'
+
+        def __init__(self):
+            self.__doc__ = 'doc_obj'
+            self.__code__ = code_obj.__code__
+            self.name = 'attrs_obj'
+            self.__name__ = 'attrs_dunder_obj'
+            self.custom_name = 'attrs_custom_obj'
+            self.__repr__ = lambda: 'repr_obj'
+            self.__str__ = lambda: 'str_obj'
+
+    def prepare_name(*prefixes):
+        def make_name(root=None):
+            if callable(root):  # set prefixes as fixed name if func provided
+                return root()
+            return join(*prefixes, root, sep='_') if root != '' else ''
+        return make_name
+
+    empty = ''
+    cls_s = 'cls'
+    obj_s = 'obj'
+    non_f = prepare_name('Non')         # fixed Non.__name__
+    cls_f = prepare_name('Cls')         # fixed Cls.__name__
+    obj_f = prepare_name('Obj')         # fixed Obj.__name__
+    cob_f = prepare_name('COb')         # fixed COb.__name__
+    all_f = prepare_name('All')         # fixed All.__name__
+
+    extension = (
+        ['default', '', ()],
+        ['empty', '', ([],)],
+        ['simple', '', (['name'],)],
+        ['dunder', 'dunder', (['__name__'],)],
+        ['custom', 'custom', (['custom_name'],)]
+    )
+
+    # [(attrs_default), (attrs_empty), (attrs_simple), (attrs_dunder), (attrs_custom)],
+    # [(doc)], [(code)], [(str)], [(repr)]
+    data = [
+        ([(non_f, empty), (empty, empty), (empty, empty), (non_f, empty), (empty, empty)],  # Non
+         [(empty, empty)], [(empty, empty)], [(empty, empty)], [(empty, empty)]),
+        ([(cls_s, cls_s), (empty, empty), (cls_s, cls_s), (cls_f, empty), (cls_s, cls_s)],  # Cls
+         [(cls_s, cls_s)], [(empty, empty)], [(cls_s, cls_s)], [(cls_s, cls_s)]),
+        ([(obj_f, obj_s), (empty, empty), (empty, obj_s), (obj_f, obj_s), (empty, obj_s)],  # Obj
+         [(empty, obj_s)], [(empty, obj_s)], [(empty, obj_s)], [(empty, obj_s)]),
+        ([(cls_s, obj_s), (empty, empty), (cls_s, obj_s), (cob_f, obj_s), (cls_s, obj_s)],  # COb
+         [(empty, obj_s)], [(empty, obj_s)], [(cls_s, obj_s)], [(cls_s, obj_s)]),
+        ([(cls_s, obj_s), (empty, empty), (cls_s, obj_s), (all_f, obj_s), (cls_s, obj_s)],  # All
+         [(cls_s, obj_s)], [(empty, obj_s)], [(cls_s, obj_s)], [(cls_s, obj_s)])
+    ]
+
+    # GetName.method(target, *args) + GetName(target, *args, full=True).method tests
+    errors = []
+    calls = ('GetName.{0}({1}{2}, {3})', 'GetName({1}{2}, full=True, {3}).{0}')
+    postfix = ('', '.cls', '.obj')
+    for cls, results in zip((Non, Cls, Obj, COb, All), data, strict=True):
+        for method, result in zip('attrs doc code str repr'.split(), results, strict=True):
+            cm = getattr(GetName, method)
+            args_str = ' || args set: ' if len(result) == len(extension) else ''
+            for (args_name, suffix, args), (val_cls, val_obj) in zip(extension, result):
+
+                # Must be
+                name = prepare_name(method, suffix)
+                name_cls, name_obj = name(val_cls), name(val_obj)
+                name_first = (name_obj or name_cls)
+                must_be_data = ((name_cls, name_cls, empty), (name_first, name_cls, name_obj))
+
+                # Received
+                kwargs = {method: args} if args else {method: True}
+                received_data = tuple((x, x.cls, x.obj) for x in (
+                    cm(cls, *args),
+                    cm(cls(), *args),
+                    getattr(GetName(cls, full=True, **kwargs), method),
+                    getattr(GetName(cls(), full=True, **kwargs), method)))
+
+                # Compare
+                if must_be_data * 2 != received_data:
+                    for i, (r, m) in enumerate(zip(received_data, must_be_data, strict=True)):
+                        for received, must_be, p in zip(r, m, postfix, strict=True):
+                            if received != must_be:
+                                obj_str = '()' if i % 2 else ''
+                                kw_str = ', '.join(fmt_dict(kwargs))
+                                sig = calls[i // 2].format(method, cls.__name__, obj_str, kw_str)
+                                add = args_str + args_name if args_str else ''
+                                msg = f'{sig}{p} == {received!r} || must be: {must_be!r}{add}'
+                                errors.append(msg)
+    if errors:
+        raise ValueError('\n\t'.join(('Test failed, errors:', *errors)))
+
+
+# Uncategorized
+
+
+def test_uid():
+    id1 = UID('1')
+    id2 = UID('2')
+    raises(TypeError, UID)
+    raises(ValueError("'1' unique ID cannot be created, it already exists"), UID, 1)
+    assert repr(id1) == "UID('1')"
+    assert str(id1) == "1 ID"
+    assert id1 == id1
+    assert id1 != id2
+
+
+def test_locker():  # noqa C901
+    class All(Locker):
+        def __init__(self):
+            self.a = 1
+            super().__init__('b')
+            self.b = 2
+            with self:
+                self.c = 3
+
+    class Add(Locker):
+        def __init__(self):
+            self.a = 1
+            super().__init__('b', del_attr=False)
+            self.b = 2
+            with self:
+                self.c = 3
+
+    class Del(Locker):
+        def __init__(self):
+            self.a = 1
+            super().__init__('b', set_attr=False)
+            exceptions = ''
+            try:
+                self.b = 2
+            except TypeError:
+                exceptions += 'b'
+            try:
+                with self:
+                    self.c = 3
+            except TypeError:
+                exceptions += 'c'
+
+            assert exceptions == 'bc'
+            object.__setattr__(self, 'b', 2)
+            object.__setattr__(self, 'c', 3)
+
+    class Non(Locker):
+        def __init__(self):
+            self.a = 1
+            super().__init__('b', set_attr=False, del_attr=False)
+            exceptions = ''
+            try:
+                self.b = 2
+            except TypeError:
+                exceptions += 'b'
+            try:
+                with self:
+                    self.c = 3
+            except TypeError:
+                exceptions += 'c'
+
+            assert exceptions == 'bc'
+            object.__setattr__(self, 'b', 2)
+            object.__setattr__(self, 'c', 3)
+
+    class AllSlot(Locker):
+        __slots__ = tuple('abcd')
+
+        def __init__(self):
+            self.a = 1
+            super().__init__('b')
+            self.b = 2
+            with self:
+                self.c = 3
+
+    class AddSlot(Locker):
+        __slots__ = tuple('abcd')
+
+        def __init__(self):
+            self.a = 1
+            super().__init__('b', del_attr=False)
+            self.b = 2
+            with self:
+                self.c = 3
+
+    class DelSlot(Locker):
+        __slots__ = tuple('abcd')
+
+        def __init__(self):
+            self.a = 1
+            super().__init__('b', set_attr=False)
+            exceptions = ''
+            try:
+                self.b = 2
+            except TypeError:
+                exceptions += 'b'
+            try:
+                with self:
+                    self.c = 3
+            except TypeError:
+                exceptions += 'c'
+
+            assert exceptions == 'bc'
+            object.__setattr__(self, 'b', 2)
+            object.__setattr__(self, 'c', 3)
+
+    class NonSlot(Locker):
+        __slots__ = tuple('abcd')
+
+        def __init__(self):
+            self.a = 1
+            super().__init__('b', set_attr=False, del_attr=False)
+            exceptions = ''
+            try:
+                self.b = 2
+            except TypeError:
+                exceptions += 'b'
+            try:
+                with self:
+                    self.c = 3
+            except TypeError:
+                exceptions += 'c'
+
+            assert exceptions == 'bc'
+            object.__setattr__(self, 'b', 2)
+            object.__setattr__(self, 'c', 3)
+
+    for data in (All, Add, Del, Non, AllSlot, AddSlot, DelSlot, NonSlot):
+        # Prepare message templates for set and del parts test
+        data = data()
+        obj = GetName(data)
+        name = f'{obj!r} object'
+        can_set = name + " is locked for changes (self.__setattr__('{}', {}))"
+        can_del = name + " is locked for changes (self.__delattr__('{}'))"
+        cant_set = name + " does not support setting attributes (self.__setattr__('{}', {}))"
+        cant_del = name + " does not support deleting attributes (self.__delattr__('{}'))"
+        not_exists = name + " has no attribute '{}'"
+        forbid = name + " Locker attrs deletion is forbidden (self.__delattr__('{}'))"
+
+        # [0. Init] Check locked object condition after init
+        assert data._locker_state is True
+        assert data._locker_ignored == ('b',)
+        assert data.a == 1
+        assert data.b == 2
+        assert data.c == 3
+        assert not hasattr(data, 'd')
+
+        # [1. Set] 1. Check object attrs changes without unlocking
+        msg = can_set if data._locker_set_attr else cant_set
+        for attr, prev_value in zip('acd', (1, 3, 4), strict=True):
+            raises(TypeError(msg.format(attr, 5)), setattr, data, attr, 5)
+            if attr != 'd':
+                assert getattr(data, attr) == prev_value
+            else:
+                assert not hasattr(data, attr)
+
+        # [1. Set] 2. Check object attrs changes in ignored attr and unlocked attrs
+        if data._locker_set_attr:
+            data.b = 5
+            assert data.b == 5
+
+            with data:
+                data.a = 5
+                assert data.a == 5
+
+                data.c = 5
+                assert data.c == 5
+
+                data.d = 5
+                assert data.d == 5
+        else:
+            raises(TypeError(cant_set.format('b', 5)), setattr, data, 'b', 5)
+            assert data.b == 2
+
+            with data:
+                raises(TypeError(cant_set.format('a', 5)), setattr, data, 'a', 5)
+                assert data.a == 1
+
+                raises(TypeError(cant_set.format('c', 5)), setattr, data, 'c', 5)
+                assert data.c == 3
+
+                raises(TypeError(cant_set.format('d', 5)), setattr, data, 'd', 5)
+                assert not hasattr(data, 'd')
+
+        # [1. Set] 3. Check object new attrs creation
+        with data:
+            if obj == 'All' or obj == 'Add':  # Has __dict__ and set allowed
+                data.e = 5
+                assert data.e == 5
+            elif obj == 'AllSlot' or obj == 'AddSlot':
+                raises(AttributeError(not_exists.format('e')), setattr, data, 'e', 5)
+            elif not data._locker_set_attr:
+                raises(TypeError(cant_set.format('e', 5)), setattr, data, 'e', 5)
+            else:
+                raise AssertionError(f'{obj!r} set new attrs check missing!')
+
+        # [2. Del] 1. Check object attrs deletion without unlocking
+        exists_d = 'd' if hasattr(data, 'd') else ''
+        msg = can_del if data._locker_del_attr else cant_del
+
+        for attr in 'ac' + exists_d:
+            raises(TypeError(msg.format(attr)), delattr, data, attr)
+            assert hasattr(data, attr)
+        if not exists_d:
+            raises(AttributeError(not_exists.format('d')), delattr, data, 'd')
+
+        # [2. Del] 2. Check object attrs deletion
+        if data._locker_del_attr:
+            del data.b
+            assert not hasattr(data, 'b')
+
+            with data:
+                del data.a
+                assert not hasattr(data, 'a')
+
+                del data.c
+                assert not hasattr(data, 'c')
+
+                if hasattr(data, 'd'):
+                    del data.d
+                    assert not hasattr(data, 'd')
+        else:
+            raises(TypeError(cant_del.format('b')), delattr, data, 'b')
+            assert hasattr(data, 'b')
+
+            with data:
+                raises(TypeError(cant_del.format('a')), delattr, data, 'a')
+                assert hasattr(data, 'a')
+
+                raises(TypeError(cant_del.format('c')), delattr, data, 'c')
+                assert hasattr(data, 'c')
+
+                if hasattr(data, 'd'):
+                    raises(TypeError(cant_del.format('d')), delattr, data, 'd')
+                    assert hasattr(data, 'd')
+
+        # [2. Del] 3. Check Locker attrs deletion
+        [raises(TypeError(forbid.format(attr)), delattr, data, attr) for attr in Locker.__slots__]
```

### Comparing `configlayer-0.1/tests/test_3_main.py` & `configlayer-0.1.1/tests/test_3_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-from configlayer.exceptions import InputError, CheckTypeError, FieldError
-from configlayer.types import mb_holder_t
-
-from _utilities import raises_init, raises, init
-from _data import ConfigBase, CfgInConfig, DunderInConfig, EmptyConfig, NoType, NoDefaults, NoBoth
-from _data import LanguageBase, ProvidedType, Lang1
-from _data import Config1, Config1Alias, Config2, Config3, Config4, OwnInt
-from _data import WrongType1, WrongType2, WrongType3, WrongType4, WrongTypeLang
-
-
-def raises_init_lang(exceptions: mb_holder_t[Exception], func, *args, **kwargs):
-    raises(init('language', exceptions, func, *args, **kwargs), func, *args, **kwargs)
-
-
-def raises_init_lang_config(exceptions: mb_holder_t[Exception], func, *args, **kwargs):
-    config_exception = init('config', exceptions, func, *args,
-                            group='Language', type_name='language', **kwargs)
-    lang_exception = init('language', config_exception, func, *args, **kwargs)
-    raises(lang_exception, func, *args, **kwargs)
-
-
-def test_config_init():
-    # Check for call without config and options correctness
-    raises_init(InputError(must_be="inherited"), ConfigBase)
-    raises_init(InputError("options", must_be="Options type", received="(True, True) (tuple)"),
-                Config1, options=(True, True))
-
-    # Check bound settings
-    raises_init(InputError("profiles", must_be="True or unfilled when group='group1' provided"),
-                Config1, group='group1', profiles=False)
-    raises_init(InputError("io", must_be="True or unfilled when path='some path' provided"),
-                Config1, 'some path', io=False)
-
-    # Check for empty config, reserved field name and that all values and types was provided
-    msg = "Must be at least one field, but received empty config"
-    raises_init(InputError(msg=msg), EmptyConfig)
-    msg = "Provided wrong field: cfg. Reserved for ConfigSupport structure, use another field name"
-    raises_init(InputError(msg=msg), CfgInConfig)
-    msg = "Provided wrong field: __dunder__. Dunder names are forbidden"
-    raises_init(InputError(msg=msg), DunderInConfig)
-    msg = "Field without type: test. Fields: {'test': None}. Types: {}"
-    raises_init(InputError(msg=msg), NoType)
-    msg = "Field without factory default: test. Fields: {}. Types: {'test': <class 'str'>}"
-    raises_init(InputError(msg=msg), NoDefaults)
-    msg = ("Field without type: test_no_t. Field without factory default: test_no_d. "
-           "Fields: {'test_no_t': None, 'test_ok': None}. "
-           "Types: {'test_no_d': <class 'str'>, 'test_ok': <class 'str'>}")
-    raises_init(InputError(msg=msg), NoBoth)
-
-    # Prepare and check data
-    msg = "Field 'str' type 'text' (str) - is not a type, and is equal to a value. "
-    msg_shadow = "If shadowing - regular scoping rules applied (cpython issue #98876)"
-    raises_init(InputError(msg=msg + msg_shadow), WrongType1)
-    raises_init(InputError(msg="Field 'str' type 'attr' (str) - is not a type"), WrongType2)
-    raises_init(InputError(msg="Field 'some'=b'1' (bytes) must be int type"), WrongType3)
-    raises_init(InputError(msg="Field 'test'=b'1' (bytes) must be int type"), WrongType4)
-    raises_init_lang_config(InputError(msg="Field 'wrong_attr'=1 (int) must be str type"),
-                            WrongTypeLang)
-
-
-def test_config_repr_str():
-    def fmt(name: str, *add_fields: str):
-        fields = ("v_bool: bool = False",
-                  "v_str: str = 'Some string'",
-                  "v_int: int = 65535",
-                  "v_float: float = 3.1415",
-                  "v_bytes: bytes = b'Some bytes'",
-                  "v_tuple: tuple = (1, 2, 3, None)",
-                  "v_list: list = [-1, 0, 1, 'repeat']",
-                  "v_set: set = {'first'}",
-                  "v_dict: dict = {1: 'one', 2: 'two'}",
-                  "v_cust1: OwnInt = 5",
-                  "v_cust2: str = 'something'",
-                  "v_cust3: int = 2",
-                  "_internal: int = 8")
-        return '\n\t'.join((f'{name!r} config:', *fields, *add_fields))
-
-    for cls, str1, str2 in (
-            [Config1, "Config1", fmt('Config1')],
-            [Config2, "Config2", fmt('Valid fields', "c2: str = 'c2'")],
-            [Config3, "Config3", fmt('Gotcha', "c2: str = 'c2'", "c3: str = 'c3'")],
-            [Config4, "Config4", fmt('IO', "C4: int = 4")]):
-        obj = cls()
-        assert repr(obj) == str1
-        assert str(obj) == str2
-
-
-def test_config_data():
-    data = Config1()
-    temp = ('v_bool', 'v_str', 'v_int', 'v_float', 'v_bytes', 'v_tuple', 'v_list', 'v_set',
-            'v_dict', 'v_cust1', 'v_cust2', 'v_cust3', '_internal')
-    assert tuple(data.cfg.get_fields) == temp
-    assert data.v_bool is False
-    assert data.v_str == 'Some string'
-    assert data.v_int == 65535
-    assert data.v_float == 3.1415
-    assert data.v_bytes == b'Some bytes'
-    assert data.v_tuple == (1, 2, 3, None)
-    assert data.v_list == [-1, 0, 1, 'repeat']
-    assert data.v_set == {'first'}
-    assert data.v_dict == {1: 'one', 2: 'two'}
-    assert data.v_cust1 == OwnInt(5)
-    assert data.v_cust2 == 'something'
-    assert data.v_cust3 == 2
-    assert data._internal == 8
-
-
-def test_config_eq():
-    config1 = Config1()
-    config1a = Config1Alias()
-    assert config1 == config1a
-    config1a.v_int = 2
-    assert config1 != config1a
-
-
-def test_config_field():
-    data = Config1()
-
-    # Set field
-    reason = ("it is not field. Available: v_bool, v_str, v_int, v_float, v_bytes, "
-              "v_tuple, v_list, v_set, v_dict, v_cust1, v_cust2, v_cust3, _internal")
-    raises(FieldError('Set', 'Config1', 'cfg', 1, reason=reason), setattr, data, 'cfg', 1)
-    raises(FieldError('Set', 'Config1', 'x', 2, reason=reason), setattr, data, 'x', 2)
-
-    data.v_str = 2
-
-    data.cfg.options.typecast = False
-    raises(CheckTypeError("2 (int) must be str type"), setattr, data, 'v_str', 2)
-
-    data.cfg.options.typecheck = False
-    data.v_str = 2
-    assert data.v_str == 2
-
-    # Delete field
-    del data.v_str
-    assert data.v_str == data.cfg.get_defaults['v_str']
-
-    assert not data.v_bool
-    data.v_bool = True
-    assert data.v_bool
-
-    raises(FieldError('Delete', 'Config1', 'x',
-                      reason="it is not field. Attributes cannot be deleted"),
-           delattr, data, 'x')
-
-    # Profiles part in set
-    data = Config1(profiles=True)
-    cfg = data.cfg
-    profiles = cfg.profiles
-
-    # Set defaults too if default profile active
-    def_v_str = data.v_str
-    new_v_str = 'new_str'
-    assert cfg.get_defaults['v_str'] == def_v_str
-
-    data.v_str = new_v_str
-    assert data.v_str == new_v_str
-    assert cfg.get_defaults['v_str'] == new_v_str
-
-    # Set in profile with fixed fields
-    profiles.set('1', {'v_str': def_v_str, 'v_bool': True}, defaults=False)
-    profiles.switch('1')
-    assert data.v_str == def_v_str
-
-    data.v_str = new_v_str
-    assert data.v_str == new_v_str
-
-    raises(FieldError('Set', 'Config1', 'v_int', 5, 65535,
-                      reason="it is fixed by '1' profile. Available fields: v_str, v_bool"),
-           setattr, data, 'v_int', 5)
-
-
-def test_language_init():
-    raises_init_lang(InputError(must_be='inherited'), LanguageBase)
-
-    msg = 'No need to annotate language fields, only str type allowed'
-    raises_init_lang(InputError('some', item_name='field', msg=msg), ProvidedType)
-
-    msg = "Reserved for LanguageBase ('SomeGroup' will be 'Language')"
-    raises_init_lang(InputError('group', msg=msg), Lang1, group='SomeGroup')
-
-
-def test_language_repr_str():
-    assert repr(Lang1()) == 'Lang1'
-    assert str(Lang1()) == '\n\t'.join(("'Random' language:", "some1: 'First some'",
-                                        "some2: 'Second some'", "another_one: 'Another'"))
-
-    Lang1().cfg.profiles.del_group('Language')
-
-
-def test_language_data():
-    text = Lang1()
-    assert text.some1 == 'First some'
-    assert text.some2 == 'Second some'
-    assert text.another_one == 'Another'
-    text.cfg.profiles._groups.clear()
+from configlayer.exceptions import InputError, CheckTypeError, FieldError
+from configlayer.types import mb_holder_t
+
+from _utilities import raises_init, raises, init
+from _data import ConfigBase, CfgInConfig, DunderInConfig, EmptyConfig, NoType, NoDefaults, NoBoth
+from _data import LanguageBase, ProvidedType, Lang1
+from _data import Config1, Config1Alias, Config2, Config3, Config4, OwnInt
+from _data import WrongType1, WrongType2, WrongType3, WrongType4, WrongTypeLang
+
+
+def raises_init_lang(exceptions: mb_holder_t[Exception], func, *args, **kwargs):
+    raises(init('language', exceptions, func, *args, **kwargs), func, *args, **kwargs)
+
+
+def raises_init_lang_config(exceptions: mb_holder_t[Exception], func, *args, **kwargs):
+    config_exception = init('config', exceptions, func, *args,
+                            group='Language', type_name='language', **kwargs)
+    lang_exception = init('language', config_exception, func, *args, **kwargs)
+    raises(lang_exception, func, *args, **kwargs)
+
+
+def test_config_init():
+    # Check for call without config and options correctness
+    raises_init(InputError(must_be="inherited"), ConfigBase)
+    raises_init(InputError("options", must_be="Options type", received="(True, True) (tuple)"),
+                Config1, options=(True, True))
+
+    # Check bound settings
+    raises_init(InputError("profiles", must_be="True or unfilled when group='group1' provided"),
+                Config1, group='group1', profiles=False)
+    raises_init(InputError("io", must_be="True or unfilled when path='some path' provided"),
+                Config1, 'some path', io=False)
+
+    # Check for empty config, reserved field name and that all values and types was provided
+    msg = "Must be at least one field, but received empty config"
+    raises_init(InputError(msg=msg), EmptyConfig)
+    msg = "Provided wrong field: cfg. Reserved for ConfigSupport structure, use another field name"
+    raises_init(InputError(msg=msg), CfgInConfig)
+    msg = "Provided wrong field: __dunder__. Dunder names are forbidden"
+    raises_init(InputError(msg=msg), DunderInConfig)
+    msg = "Field without type: test. Fields: {'test': None}. Types: {}"
+    raises_init(InputError(msg=msg), NoType)
+    msg = "Field without factory default: test. Fields: {}. Types: {'test': <class 'str'>}"
+    raises_init(InputError(msg=msg), NoDefaults)
+    msg = ("Field without type: test_no_t. Field without factory default: test_no_d. "
+           "Fields: {'test_no_t': None, 'test_ok': None}. "
+           "Types: {'test_no_d': <class 'str'>, 'test_ok': <class 'str'>}")
+    raises_init(InputError(msg=msg), NoBoth)
+
+    # Prepare and check data
+    msg = "Field 'str' type 'text' (str) - is not a type, and is equal to a value. "
+    msg_shadow = "If shadowing - regular scoping rules applied (cpython issue #98876)"
+    raises_init(InputError(msg=msg + msg_shadow), WrongType1)
+    raises_init(InputError(msg="Field 'str' type 'str' (str) - is not a type"), WrongType2)
+    raises_init(InputError(msg="Field 'some'=b'1' (bytes) must be int type"), WrongType3)
+    raises_init(InputError(msg="Field 'test'=b'1' (bytes) must be int type"), WrongType4)
+    raises_init_lang_config(InputError(msg="Field 'wrong_attr'=1 (int) must be str type"),
+                            WrongTypeLang)
+
+
+def test_config_repr_str():
+    def fmt(name: str, *add_fields: str):
+        fields = ("v_bool: bool = False",
+                  "v_str: str = 'Some string'",
+                  "v_int: int = 65535",
+                  "v_float: float = 3.1415",
+                  "v_bytes: bytes = b'Some bytes'",
+                  "v_tuple: tuple = (1, 2, 3, None)",
+                  "v_list: list = [-1, 0, 1, 'repeat']",
+                  "v_set: set = {'first'}",
+                  "v_dict: dict = {1: 'one', 2: 'two'}",
+                  "v_cust1: OwnInt = 5",
+                  "v_cust2: str = 'something'",
+                  "v_cust3: int = 2",
+                  "_internal: int = 8")
+        return '\n\t'.join((f'{name!r} config:', *fields, *add_fields))
+
+    for cls, str1, str2 in (
+            [Config1, "Config1", fmt('Config1')],
+            [Config2, "Config2", fmt('Valid fields', "c2: str = 'c2'")],
+            [Config3, "Config3", fmt('Gotcha', "c2: str = 'c2'", "c3: str = 'c3'")],
+            [Config4, "Config4", fmt('IO', "C4: int = 4")]):
+        obj = cls()
+        assert repr(obj) == str1
+        assert str(obj) == str2
+
+
+def test_config_data():
+    data = Config1()
+    temp = ('v_bool', 'v_str', 'v_int', 'v_float', 'v_bytes', 'v_tuple', 'v_list', 'v_set',
+            'v_dict', 'v_cust1', 'v_cust2', 'v_cust3', '_internal')
+    assert tuple(data.cfg.get_fields) == temp
+    assert data.v_bool is False
+    assert data.v_str == 'Some string'
+    assert data.v_int == 65535
+    assert data.v_float == 3.1415
+    assert data.v_bytes == b'Some bytes'
+    assert data.v_tuple == (1, 2, 3, None)
+    assert data.v_list == [-1, 0, 1, 'repeat']
+    assert data.v_set == {'first'}
+    assert data.v_dict == {1: 'one', 2: 'two'}
+    assert data.v_cust1 == OwnInt(5)
+    assert data.v_cust2 == 'something'
+    assert data.v_cust3 == 2
+    assert data._internal == 8
+
+
+def test_config_eq():
+    config1 = Config1()
+    config1a = Config1Alias()
+    assert config1 == config1a
+    config1a.v_int = 2
+    assert config1 != config1a
+
+
+def test_config_field():
+    data = Config1()
+
+    # Set field
+    reason = ("it is not field. Available: v_bool, v_str, v_int, v_float, v_bytes, "
+              "v_tuple, v_list, v_set, v_dict, v_cust1, v_cust2, v_cust3, _internal")
+    raises(FieldError('Set', 'Config1', 'cfg', 1, reason=reason), setattr, data, 'cfg', 1)
+    raises(FieldError('Set', 'Config1', 'x', 2, reason=reason), setattr, data, 'x', 2)
+
+    data.v_str = 2
+
+    data.cfg.options.typecast = False
+    raises(CheckTypeError("2 (int) must be str type"), setattr, data, 'v_str', 2)
+
+    data.cfg.options.typecheck = False
+    data.v_str = 2
+    assert data.v_str == 2
+
+    # Delete field
+    del data.v_str
+    assert data.v_str == data.cfg.get_defaults['v_str']
+
+    assert not data.v_bool
+    data.v_bool = True
+    assert data.v_bool
+
+    raises(FieldError('Delete', 'Config1', 'x',
+                      reason="it is not field. Attributes cannot be deleted"),
+           delattr, data, 'x')
+
+    # Profiles part in set
+    data = Config1(profiles=True)
+    cfg = data.cfg
+    profiles = cfg.profiles
+
+    # Set defaults too if default profile active
+    def_v_str = data.v_str
+    new_v_str = 'new_str'
+    assert cfg.get_defaults['v_str'] == def_v_str
+
+    data.v_str = new_v_str
+    assert data.v_str == new_v_str
+    assert cfg.get_defaults['v_str'] == new_v_str
+
+    # Set in profile with fixed fields
+    profiles.set('1', {'v_str': def_v_str, 'v_bool': True}, defaults=False)
+    profiles.switch('1')
+    assert data.v_str == def_v_str
+
+    data.v_str = new_v_str
+    assert data.v_str == new_v_str
+
+    raises(FieldError('Set', 'Config1', 'v_int', 5, 65535,
+                      reason="it is fixed by '1' profile. Available fields: v_str, v_bool"),
+           setattr, data, 'v_int', 5)
+
+
+def test_language_init():
+    raises_init_lang(InputError(must_be='inherited'), LanguageBase)
+
+    msg = 'No need to annotate language fields, only str type allowed'
+    raises_init_lang(InputError('some', item_name='field', msg=msg), ProvidedType)
+
+    msg = "Reserved for LanguageBase ('SomeGroup' will be 'Language')"
+    raises_init_lang(InputError('group', msg=msg), Lang1, group='SomeGroup')
+
+
+def test_language_repr_str():
+    assert repr(Lang1()) == 'Lang1'
+    assert str(Lang1()) == '\n\t'.join(("'Random' language:", "some1: 'First some'",
+                                        "some2: 'Second some'", "another_one: 'Another'"))
+
+    Lang1().cfg.profiles.del_group('Language')
+
+
+def test_language_data():
+    text = Lang1()
+    assert text.some1 == 'First some'
+    assert text.some2 == 'Second some'
+    assert text.another_one == 'Another'
+    text.cfg.profiles._groups.clear()
```

### Comparing `configlayer-0.1/tests/test_4_config.py` & `configlayer-0.1.1/tests/test_4_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,304 +1,302 @@
-from typing import Iterable
-from pathlib import Path
-from functools import partial
-from itertools import product
-
-from configlayer import Field, Options
-from configlayer.exceptions import CheckTypeError, OptionsCheckError, FieldError, InputError
-
-from _utilities import raises, init
-from _data import (Config1, Config2, Config3, Config4, Lang1,
-                   wrong_func, wrong_func_2, wrong_func_3, exp_strict, imp_strict)
-
-
-def raises_init_lang(exceptions: Exception | Iterable[Exception], func, *args, **kwargs):
-    raises((*init('language', (), func, *args, **kwargs),
-            *init('config', exceptions, func, *args, **kwargs, group='Language')),
-           func, *args, **kwargs)
-
-
-def test_init():
-    cust_opt = Options(revert_fails=True)
-    path = '_file_data\\temp_config.ini'
-    Path(path).unlink(missing_ok=True)
-    for data, field_keys, name, type_name, def_sect, opt, profiles, io, file in [
-        (Config3(default_section='x', options=cust_opt), (*exp_strict, 'c2', 'c3'),
-         'Gotcha', 'config', 'x', cust_opt, False, False, False),
-        (Lang1(path, profiles=True), ('some1', 'some2', 'another_one'),
-         'Random', 'language', 'DEFAULT', Options(), True, True, True)
-    ]:
-        cfg = data.cfg
-        assert cfg._data == data
-        assert tuple(cfg._fields) == field_keys
-        assert all(isinstance(x, Field) for x in cfg._fields.values())
-        assert cfg._on_set == {}
-        assert cfg.name == name
-        assert cfg.type_name == type_name
-        assert cfg.def_sect == def_sect
-        assert cfg.options == opt
-        assert cfg.version is None
-        assert bool(cfg.profiles) == profiles
-        assert bool(cfg.io) == io
-        assert bool(cfg.file) == file
-
-
-def test_repr_str():
-    for cls, str1, str2 in (
-            [Config1, "Config1.cfg", "'Config1' config support structure"],
-            [Config2, "Config2.cfg", "'Valid fields' config support structure"],
-            [Config3, "Config3.cfg", "'Gotcha' config support structure"],
-            [Config4, "Config4.cfg", "'IO' config support structure"],
-            [Lang1, "Lang1.cfg", "'Random' language support structure"]):
-        obj = cls().cfg
-        assert repr(obj) == str1
-        assert str(obj) == str2
-
-    Lang1().cfg.profiles.del_group('Language')
-
-
-def test_change_attr():
-    cfg = Config1().cfg
-    obj_name = "'Config1' config support structure"
-    raises(TypeError(f"{obj_name} is locked for changes (self.__setattr__('x', 1))"),
-           setattr, cfg, 'x', 1)
-    raises(TypeError(f"{obj_name} is locked for changes (self.__setattr__('fields', 2))"),
-           setattr, cfg, 'fields', 2)
-
-    assert cfg._locker_state
-    with cfg:
-        cfg.file = None
-        raises(AttributeError("'ConfigSupport' object has no attribute 'some'"),
-               setattr, cfg, 'some', 5)
-    assert cfg._locker_state
-    cfg._locker_state = False
-    cfg.file = None
-    with cfg:
-        cfg.file = None
-    assert not cfg._locker_state
-
-    raises(AttributeError(f"{obj_name} has no attribute 'x'"), delattr, cfg, 'x')
-
-    msg = f"{obj_name} does not support deleting attributes (self.__delattr__('_fields'))"
-    raises(TypeError(msg), delattr, cfg, '_fields')
-
-    msg = f"{obj_name} Locker attrs deletion is forbidden (self.__delattr__('_locker_state'))"
-    raises(TypeError(msg), delattr, cfg, '_locker_state')
-
-
-def test_on_set():
-    result = []
-
-    def log_arg(event, param, prev_value, curr_value):
-        result.append(f'{event} {param}: {prev_value!r} -> {curr_value!r}')
-
-    def log_kwarg(param, prev_value, curr_value, event=None):
-        event = '' if event is None else str(event) + ' '
-        result.append(f'{event}{param}: {prev_value!r} -> {curr_value!r}')
-
-    data = Config1()
-    data.cfg.add_on_set('1', None, True, log_arg, 'Global1')
-    data.cfg.add_on_set('2', 'v_bool', True, log_arg, 'Single')
-    data.cfg.add_on_set('3', 'v_str', True, log_kwarg)
-    data.cfg.add_on_set('4', None, True, log_kwarg, event='Global2')
-    data.cfg.add_on_set('5', 'v_bool', False, log_kwarg)
-    data.cfg.add_on_set('6', 'v_str', False, log_kwarg, event='Single')
-
-    data.v_int = 5
-    assert result == ['Global1 v_int: 65535 -> 5', 'Global2 v_int: 65535 -> 5']
-
-    result.clear()
-    data.v_bool = True
-    assert result == ['Global1 v_bool: False -> True', 'Single v_bool: False -> True',
-                      'Global2 v_bool: False -> True', 'v_bool: False -> True']
-
-    result.clear()
-    data.v_str = '123'
-    assert result == ['Global1 v_str: \'Some string\' -> \'123\'',
-                      'v_str: \'Some string\' -> \'123\'',
-                      'Global2 v_str: \'Some string\' -> \'123\'',
-                      'Single v_str: \'Some string\' -> \'123\'']
-
-    result.clear()
-    data.v_int = 5
-    assert result == ['Global1 v_int: 5 -> 5', 'Global2 v_int: 5 -> 5']
-
-    result.clear()
-    data.v_bool = True
-    assert result == ['Global1 v_bool: True -> True', 'Single v_bool: True -> True',
-                      'Global2 v_bool: True -> True']
-
-    result.clear()
-    data.v_str = '123'
-    assert result == ['Global1 v_str: \'123\' -> \'123\'',
-                      'v_str: \'123\' -> \'123\'',
-                      'Global2 v_str: \'123\' -> \'123\'']
-
-    msg = ("Provided wrong parameter to Config1.cfg.add_on_set(): field_name. "
-           "Cannot add '7' handler, not exists field_name = 'not_exists'")
-    raises(InputError(msg=msg), data.cfg.add_on_set, '7', 'not_exists', True, log_kwarg)
-
-    msg = ("Provided wrong parameter to Config1.cfg.add_on_set(): name. "
-           "Cannot add '6' handler, it already exists")
-    raises(InputError(msg=msg), data.cfg.add_on_set, '6', None, True, log_kwarg)
-
-    data.cfg.add_on_set('7', 'v_int', True, wrong_func)
-    r_msg = "\nRevert option is disabled - field value is left changed"
-    msg = ("on_set handlers errors:\n"
-           "\t'7' handler (wrong_func): wrong_func() takes 1 positional argument but 3 were given")
-    raises(FieldError('Set', 'Config1', 'v_int', 3, 5, reason=msg + r_msg, failed=False),
-           setattr, data, 'v_int', 3)
-
-    data.cfg.add_on_set('8', None, True, wrong_func_2)
-    msg = ("on_set handlers errors:\n"
-           "\t'7' handler (wrong_func): wrong_func() takes 1 positional argument but 3 were given"
-           "\n\t'8' handler (wrong_func_2): Wrong func 2! ('v_int', 3, 5)")
-    raises(FieldError('Set', 'Config1', 'v_int', 5, 3, reason=msg + r_msg, failed=False),
-           setattr, data, 'v_int', 5)
-
-    msg = ("on_set handlers errors:\n"
-           "\t'8' handler (wrong_func_2): Wrong func 2! ('v_float', 3.1415, 0.0)")
-    raises(FieldError('Set', 'Config1', 'v_float', 0.0, 3.1415, reason=msg + r_msg, failed=False),
-           setattr, data, 'v_float', 0.0)
-
-    raises(KeyError('9'), data.cfg.del_on_set, '9')
-
-    assert tuple(data.cfg.get_on_set) == tuple('12345678')
-
-    data.cfg.del_on_set('8')
-    data.v_float = 3.1415
-
-    data.cfg.del_on_set('7')
-    data.v_int = 6
-
-    [data.cfg.del_on_set(repr(i)) for i in range(6, 0, -1)]
-    assert not data.cfg.get_on_set
-
-
-def test_get_set():
-    default_data = imp_strict | {'c2': 'c2', 'c3': 'c3'}
-    data_s, data_p = Config3(), Config3(profiles=True)
-    cfg_s, cfg_p = data_s.cfg, data_p.cfg
-
-    def check(cfg, current, default, changed):
-        assert cfg.get_data == default_data | current
-        assert cfg.get_defaults == default_data | default
-        assert cfg.get_factory_defaults == default_data
-
-        assert {k: v.default for k, v in cfg.get_fields.items()} == default_data | default
-        assert [k for k, v in cfg.get_changed.items() if v] == changed
-        assert cfg.get_types == {k: type(v) for k, v in cfg.get_data.items()}
-
-    data_s.v_int = data_p.v_int = 255
-    cfg_s.get_fields['v_int'].default = cfg_p.get_fields['v_int'].default = 32767
-    check(cfg_s, {'v_int': 255}, {'v_int': 32767}, ['v_int'])
-    check(cfg_p, {'v_int': 255}, {'v_int': 32767}, ['v_int'])
-
-    data_s.v_int = data_p.v_int = 1024
-    check(cfg_s, {'v_int': 1024}, {'v_int': 32767}, ['v_int'])
-    check(cfg_p, {'v_int': 1024}, {'v_int': 1024}, [])
-
-    cfg_s.set_fields({'v_int': 512, 'v_str': 's1'})
-    cfg_p.set_fields({'v_int': 512, 'v_str': 's1'})
-    cfg_s.set_defaults({'v_int': 127, 'v_str': 's2'})
-    cfg_p.set_defaults({'v_int': 127, 'v_str': 's2'})
-    check(cfg_s, {'v_int': 512, 'v_str': 's1'}, {'v_int': 127, 'v_str': 's2'}, ['v_str', 'v_int'])
-    check(cfg_p, {'v_int': 127, 'v_str': 's2'}, {'v_int': 127, 'v_str': 's2'}, [])
-
-    cfg_p.profiles.set('p1', {'v_bool': True})
-    cfg_p.profiles.switch('p1')
-
-    data_p.v_str = 'Some string'
-    data_p.v_int = 8
-    cfg_p.get_fields['v_int'].default = 65535
-    check(cfg_p, {'v_bool': True, 'v_int': 8}, {'v_str': 's2'}, ['v_bool', 'v_str', 'v_int'])
-
-    cfg_p.set_fields({'v_int': 32})
-    cfg_p.set_defaults({'v_int': 64, 'v_str': 'Some string'})
-    check(cfg_p, {'v_bool': True, 'v_int': 32}, {'v_int': 64}, ['v_bool', 'v_int'])
-
-    exc_part = partial(InputError, 'fields', msg='Empty fields provided')
-    raises(exc_part(func_name="Config3.cfg.set_fields()"), cfg_p.set_fields, {})
-    raises(exc_part(func_name="Config3.cfg.set_defaults()"), cfg_p.set_defaults, {})
-
-
-def test_options():
-    options1 = Options()
-    options2 = Options(True, typecast=True)
-    options3 = Options(typecast=True, typecheck=True)
-    assert options1 == options2 == options3
-
-    msg_cast = "Type checking is disabled, type casting cannot be enabled"
-
-    for args in product((True, False), repeat=3):
-        check, cast, *_ = args
-
-        errors = []
-        if cast and not check:
-            errors.append(msg_cast)
-
-        if errors:
-            raises(OptionsCheckError('. '.join(errors)), Options, *args)
-        else:
-            Config1(options=Options(*args))
-
-    option = 'typecheck'
-    msg = f"Set option {option!r} to False failed: {msg_cast}. Reverted to True successfully"
-    raises(OptionsCheckError(msg), setattr, options1, option, False)
-    assert options1.typecheck is True
-
-    object.__setattr__(options1, option, False)
-    option = 'revert_fails'
-    msg2 = f"Some options changed in wrong way, check failed: {msg_cast}"
-    msg = f"Set option {option!r} to True failed: {msg_cast}. Revert to False also failed: {msg2}"
-    raises(OptionsCheckError(msg), setattr, options1, option, True)
-
-    msg = 'Options accepting only booleans'
-    raises(OptionsCheckError(msg), setattr, options1, option, 1)
-
-    # No type check and cast
-    config = Config1(options=Options(False, False))
-    config.v_int = '5'
-    assert config.v_int == '5'
-
-    # Type check
-    config = Config1(options=Options(True, False))
-    raises(CheckTypeError("'5' (str) must be int type"), setattr, config, 'v_int', '5')
-
-    # Type check and cast
-    config = Config1()
-    config.v_int = '5'
-    assert config.v_int == 5
-
-    # Clear at default
-    config = Config1()
-    config.v_int = 32767
-    assert config.v_int == 32767
-    assert [k for k, v in config.cfg.get_changed.items() if v] == ['v_int']
-    config.v_int = 65535
-    assert config.v_int == 65535
-    assert [k for k, v in config.cfg.get_changed.items() if v] == []
-
-    # Revert at on_set error and not
-    revert_disabled = "\nRevert option is disabled - field value is left changed"
-    revert_details = ("\nRevert completed, but on_set handlers errors:\n"
-                      "\t'2' handler (wrong_func_2): Wrong func 2! ('v_int', 32767, 65535)")
-    for state, result1, result2 in (True, 65535, 'Some string'), (False, 32767, 'other'):
-        config = Config1(options=Options(revert_fails=state))
-        config.cfg.add_on_set('2', 'v_int', True, wrong_func_2)
-        config.cfg.add_on_set('3', 'v_str', True, wrong_func_3)
-
-        msg = ("on_set handlers errors:\n"
-               "\t'2' handler (wrong_func_2): Wrong func 2! ('v_int', 65535, 32767)")
-        msg += revert_details if state else revert_disabled
-        raises(FieldError('Set', 'Config1', 'v_int', 32767, 65535, reason=msg, failed=False),
-               setattr, config, 'v_int', 32767)
-        assert config.v_int == result1
-
-        msg = ("on_set handlers errors:\n"
-               "\t'3' handler (wrong_func_3): Cannot change value ('v_str', 'Some string', "
-               "'other')")
-        msg += "\nRevert completed" if state else revert_disabled
-        raises(FieldError('Set', 'Config1', 'v_str', 'other', 'Some string', reason=msg,
-                          failed=False),
-               setattr, config, 'v_str', 'other')
-        assert config.v_str == result2
+from typing import Iterable
+from functools import partial
+from itertools import product
+
+from configlayer import Field, Options
+from configlayer.exceptions import CheckTypeError, OptionsCheckError, FieldError, InputError
+
+from _utilities import raises, init
+from _data import (TEMP_PATH, Config1, Config2, Config3, Config4, Lang1,
+                   wrong_func, wrong_func_2, wrong_func_3, exp_strict, imp_strict)
+
+
+def raises_init_lang(exceptions: Exception | Iterable[Exception], func, *args, **kwargs):
+    raises((*init('language', (), func, *args, **kwargs),
+            *init('config', exceptions, func, *args, **kwargs, group='Language')),
+           func, *args, **kwargs)
+
+
+def test_init():
+    cust_opt = Options(revert_fails=True)
+    TEMP_PATH.unlink(missing_ok=True)
+    for data, field_keys, name, type_name, def_sect, opt, profiles, io, file in [
+        (Config3(default_section='x', options=cust_opt), (*exp_strict, 'c2', 'c3'),
+         'Gotcha', 'config', 'x', cust_opt, False, False, False),
+        (Lang1(TEMP_PATH, profiles=True), ('some1', 'some2', 'another_one'),
+         'Random', 'language', 'DEFAULT', Options(), True, True, True)
+    ]:
+        cfg = data.cfg
+        assert cfg._data == data
+        assert tuple(cfg._fields) == field_keys
+        assert all(isinstance(x, Field) for x in cfg._fields.values())
+        assert cfg._on_set == {}
+        assert cfg.name == name
+        assert cfg.type_name == type_name
+        assert cfg.def_sect == def_sect
+        assert cfg.options == opt
+        assert cfg.version is None
+        assert bool(cfg.profiles) == profiles
+        assert bool(cfg.io) == io
+        assert bool(cfg.file) == file
+
+
+def test_repr_str():
+    for cls, str1, str2 in (
+            [Config1, "Config1.cfg", "'Config1' config support structure"],
+            [Config2, "Config2.cfg", "'Valid fields' config support structure"],
+            [Config3, "Config3.cfg", "'Gotcha' config support structure"],
+            [Config4, "Config4.cfg", "'IO' config support structure"],
+            [Lang1, "Lang1.cfg", "'Random' language support structure"]):
+        obj = cls().cfg
+        assert repr(obj) == str1
+        assert str(obj) == str2
+
+    Lang1().cfg.profiles.del_group('Language')
+
+
+def test_change_attr():
+    cfg = Config1().cfg
+    obj_name = "'Config1' config support structure"
+    raises(TypeError(f"{obj_name} is locked for changes (self.__setattr__('x', 1))"),
+           setattr, cfg, 'x', 1)
+    raises(TypeError(f"{obj_name} is locked for changes (self.__setattr__('fields', 2))"),
+           setattr, cfg, 'fields', 2)
+
+    assert cfg._locker_state
+    with cfg:
+        cfg.file = None
+        raises(AttributeError("'ConfigSupport' object has no attribute 'some'"),
+               setattr, cfg, 'some', 5)
+    assert cfg._locker_state
+    cfg._locker_state = False
+    cfg.file = None
+    with cfg:
+        cfg.file = None
+    assert not cfg._locker_state
+
+    raises(AttributeError(f"{obj_name} has no attribute 'x'"), delattr, cfg, 'x')
+
+    msg = f"{obj_name} does not support deleting attributes (self.__delattr__('_fields'))"
+    raises(TypeError(msg), delattr, cfg, '_fields')
+
+    msg = f"{obj_name} Locker attrs deletion is forbidden (self.__delattr__('_locker_state'))"
+    raises(TypeError(msg), delattr, cfg, '_locker_state')
+
+
+def test_on_set():
+    result = []
+
+    def log_arg(event, param, prev_value, curr_value):
+        result.append(f'{event} {param}: {prev_value!r} -> {curr_value!r}')
+
+    def log_kwarg(param, prev_value, curr_value, event=None):
+        event = '' if event is None else str(event) + ' '
+        result.append(f'{event}{param}: {prev_value!r} -> {curr_value!r}')
+
+    data = Config1()
+    data.cfg.add_on_set('1', None, True, log_arg, 'Global1')
+    data.cfg.add_on_set('2', 'v_bool', True, log_arg, 'Single')
+    data.cfg.add_on_set('3', 'v_str', True, log_kwarg)
+    data.cfg.add_on_set('4', None, True, log_kwarg, event='Global2')
+    data.cfg.add_on_set('5', 'v_bool', False, log_kwarg)
+    data.cfg.add_on_set('6', 'v_str', False, log_kwarg, event='Single')
+
+    data.v_int = 5
+    assert result == ['Global1 v_int: 65535 -> 5', 'Global2 v_int: 65535 -> 5']
+
+    result.clear()
+    data.v_bool = True
+    assert result == ['Global1 v_bool: False -> True', 'Single v_bool: False -> True',
+                      'Global2 v_bool: False -> True', 'v_bool: False -> True']
+
+    result.clear()
+    data.v_str = '123'
+    assert result == ['Global1 v_str: \'Some string\' -> \'123\'',
+                      'v_str: \'Some string\' -> \'123\'',
+                      'Global2 v_str: \'Some string\' -> \'123\'',
+                      'Single v_str: \'Some string\' -> \'123\'']
+
+    result.clear()
+    data.v_int = 5
+    assert result == ['Global1 v_int: 5 -> 5', 'Global2 v_int: 5 -> 5']
+
+    result.clear()
+    data.v_bool = True
+    assert result == ['Global1 v_bool: True -> True', 'Single v_bool: True -> True',
+                      'Global2 v_bool: True -> True']
+
+    result.clear()
+    data.v_str = '123'
+    assert result == ['Global1 v_str: \'123\' -> \'123\'',
+                      'v_str: \'123\' -> \'123\'',
+                      'Global2 v_str: \'123\' -> \'123\'']
+
+    msg = ("Provided wrong parameter to Config1.cfg.add_on_set(): field_name. "
+           "Cannot add '7' handler, not exists field_name = 'not_exists'")
+    raises(InputError(msg=msg), data.cfg.add_on_set, '7', 'not_exists', True, log_kwarg)
+
+    msg = ("Provided wrong parameter to Config1.cfg.add_on_set(): name. "
+           "Cannot add '6' handler, it already exists")
+    raises(InputError(msg=msg), data.cfg.add_on_set, '6', None, True, log_kwarg)
+
+    data.cfg.add_on_set('7', 'v_int', True, wrong_func)
+    r_msg = "\nRevert option is disabled - field value is left changed"
+    msg = ("on_set handlers errors:\n"
+           "\t'7' handler (wrong_func): wrong_func() takes 1 positional argument but 3 were given")
+    raises(FieldError('Set', 'Config1', 'v_int', 3, 5, reason=msg + r_msg, failed=False),
+           setattr, data, 'v_int', 3)
+
+    data.cfg.add_on_set('8', None, True, wrong_func_2)
+    msg = ("on_set handlers errors:\n"
+           "\t'7' handler (wrong_func): wrong_func() takes 1 positional argument but 3 were given"
+           "\n\t'8' handler (wrong_func_2): Wrong func 2! ('v_int', 3, 5)")
+    raises(FieldError('Set', 'Config1', 'v_int', 5, 3, reason=msg + r_msg, failed=False),
+           setattr, data, 'v_int', 5)
+
+    msg = ("on_set handlers errors:\n"
+           "\t'8' handler (wrong_func_2): Wrong func 2! ('v_float', 3.1415, 0.0)")
+    raises(FieldError('Set', 'Config1', 'v_float', 0.0, 3.1415, reason=msg + r_msg, failed=False),
+           setattr, data, 'v_float', 0.0)
+
+    raises(KeyError('9'), data.cfg.del_on_set, '9')
+
+    assert tuple(data.cfg.get_on_set) == tuple('12345678')
+
+    data.cfg.del_on_set('8')
+    data.v_float = 3.1415
+
+    data.cfg.del_on_set('7')
+    data.v_int = 6
+
+    [data.cfg.del_on_set(repr(i)) for i in range(6, 0, -1)]
+    assert not data.cfg.get_on_set
+
+
+def test_get_set():
+    default_data = imp_strict | {'c2': 'c2', 'c3': 'c3'}
+    data_s, data_p = Config3(), Config3(profiles=True)
+    cfg_s, cfg_p = data_s.cfg, data_p.cfg
+
+    def check(cfg, current, default, changed):
+        assert cfg.get_data == default_data | current
+        assert cfg.get_defaults == default_data | default
+        assert cfg.get_factory_defaults == default_data
+
+        assert {k: v.default for k, v in cfg.get_fields.items()} == default_data | default
+        assert [k for k, v in cfg.get_changed.items() if v] == changed
+        assert cfg.get_types == {k: type(v) for k, v in cfg.get_data.items()}
+
+    data_s.v_int = data_p.v_int = 255
+    cfg_s.get_fields['v_int'].default = cfg_p.get_fields['v_int'].default = 32767
+    check(cfg_s, {'v_int': 255}, {'v_int': 32767}, ['v_int'])
+    check(cfg_p, {'v_int': 255}, {'v_int': 32767}, ['v_int'])
+
+    data_s.v_int = data_p.v_int = 1024
+    check(cfg_s, {'v_int': 1024}, {'v_int': 32767}, ['v_int'])
+    check(cfg_p, {'v_int': 1024}, {'v_int': 1024}, [])
+
+    cfg_s.set_fields({'v_int': 512, 'v_str': 's1'})
+    cfg_p.set_fields({'v_int': 512, 'v_str': 's1'})
+    cfg_s.set_defaults({'v_int': 127, 'v_str': 's2'})
+    cfg_p.set_defaults({'v_int': 127, 'v_str': 's2'})
+    check(cfg_s, {'v_int': 512, 'v_str': 's1'}, {'v_int': 127, 'v_str': 's2'}, ['v_str', 'v_int'])
+    check(cfg_p, {'v_int': 127, 'v_str': 's2'}, {'v_int': 127, 'v_str': 's2'}, [])
+
+    cfg_p.profiles.set('p1', {'v_bool': True})
+    cfg_p.profiles.switch('p1')
+
+    data_p.v_str = 'Some string'
+    data_p.v_int = 8
+    cfg_p.get_fields['v_int'].default = 65535
+    check(cfg_p, {'v_bool': True, 'v_int': 8}, {'v_str': 's2'}, ['v_bool', 'v_str', 'v_int'])
+
+    cfg_p.set_fields({'v_int': 32})
+    cfg_p.set_defaults({'v_int': 64, 'v_str': 'Some string'})
+    check(cfg_p, {'v_bool': True, 'v_int': 32}, {'v_int': 64}, ['v_bool', 'v_int'])
+
+    exc_part = partial(InputError, 'fields', msg='Empty fields provided')
+    raises(exc_part(func_name="Config3.cfg.set_fields()"), cfg_p.set_fields, {})
+    raises(exc_part(func_name="Config3.cfg.set_defaults()"), cfg_p.set_defaults, {})
+
+
+def test_options():
+    options1 = Options()
+    options2 = Options(True, typecast=True)
+    options3 = Options(typecast=True, typecheck=True)
+    assert options1 == options2 == options3
+
+    msg_cast = "Type checking is disabled, type casting cannot be enabled"
+
+    for args in product((True, False), repeat=3):
+        check, cast, *_ = args
+
+        errors = []
+        if cast and not check:
+            errors.append(msg_cast)
+
+        if errors:
+            raises(OptionsCheckError('. '.join(errors)), Options, *args)
+        else:
+            Config1(options=Options(*args))
+
+    option = 'typecheck'
+    msg = f"Set option {option!r} to False failed: {msg_cast}. Reverted to True successfully"
+    raises(OptionsCheckError(msg), setattr, options1, option, False)
+    assert options1.typecheck is True
+
+    object.__setattr__(options1, option, False)
+    option = 'revert_fails'
+    msg2 = f"Some options changed in wrong way, check failed: {msg_cast}"
+    msg = f"Set option {option!r} to True failed: {msg_cast}. Revert to False also failed: {msg2}"
+    raises(OptionsCheckError(msg), setattr, options1, option, True)
+
+    msg = 'Options accepting only booleans'
+    raises(OptionsCheckError(msg), setattr, options1, option, 1)
+
+    # No type check and cast
+    config = Config1(options=Options(False, False))
+    config.v_int = '5'
+    assert config.v_int == '5'
+
+    # Type check
+    config = Config1(options=Options(True, False))
+    raises(CheckTypeError("'5' (str) must be int type"), setattr, config, 'v_int', '5')
+
+    # Type check and cast
+    config = Config1()
+    config.v_int = '5'
+    assert config.v_int == 5
+
+    # Clear at default
+    config = Config1()
+    config.v_int = 32767
+    assert config.v_int == 32767
+    assert [k for k, v in config.cfg.get_changed.items() if v] == ['v_int']
+    config.v_int = 65535
+    assert config.v_int == 65535
+    assert [k for k, v in config.cfg.get_changed.items() if v] == []
+
+    # Revert at on_set error and not
+    revert_disabled = "\nRevert option is disabled - field value is left changed"
+    revert_details = ("\nRevert completed, but on_set handlers errors:\n"
+                      "\t'2' handler (wrong_func_2): Wrong func 2! ('v_int', 32767, 65535)")
+    for state, result1, result2 in (True, 65535, 'Some string'), (False, 32767, 'other'):
+        config = Config1(options=Options(revert_fails=state))
+        config.cfg.add_on_set('2', 'v_int', True, wrong_func_2)
+        config.cfg.add_on_set('3', 'v_str', True, wrong_func_3)
+
+        msg = ("on_set handlers errors:\n"
+               "\t'2' handler (wrong_func_2): Wrong func 2! ('v_int', 65535, 32767)")
+        msg += revert_details if state else revert_disabled
+        raises(FieldError('Set', 'Config1', 'v_int', 32767, 65535, reason=msg, failed=False),
+               setattr, config, 'v_int', 32767)
+        assert config.v_int == result1
+
+        msg = ("on_set handlers errors:\n"
+               "\t'3' handler (wrong_func_3): Cannot change value ('v_str', 'Some string', "
+               "'other')")
+        msg += "\nRevert completed" if state else revert_disabled
+        raises(FieldError('Set', 'Config1', 'v_str', 'other', 'Some string', reason=msg,
+                          failed=False),
+               setattr, config, 'v_str', 'other')
+        assert config.v_str == result2
```

### Comparing `configlayer-0.1/tests/test_6_io.py` & `configlayer-0.1.1/tests/test_6_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,693 +1,692 @@
-from functools import partial
-from itertools import product
-
-from configlayer.exceptions import (InputError, CheckValueError, CheckTypeError,
-                                    FieldError, IOExportError, IOImportError)
-from configlayer.utils import safe, as_holder, is_exception
-
-from _utilities import raises_init, raises, subtest
-from _data import (WrongExportRepr, WrongExportFunc, WrongExportType, WrongImportEval,
-                   WrongImportFunc, WrongImportResult, WrongReprType, ExportSensitive,
-                   Config1, Config2, Config3, Config4, Lang1, exp_strict, imp_strict, OwnInt)
-
-
-def test_init():
-    # Correct
-    assert Config1(io=True)
-
-    # Error at export fields check
-    exc1e = TypeError("Wrong repr!")
-    exc1ef = FieldError('Export', 'WrongExportRepr', 'test', from_value=exc1e, by_func='repr',
-                        reason=repr(exc1e))
-    raises_init((exc1ef, exc1e), WrongExportRepr, io=True)
-
-    exc2e = TypeError("Wrong func!")
-    exc2ef = FieldError('Export', 'WrongExportFunc', 'test', from_value=5, by_func='wrong_func',
-                        reason=repr(exc2e))
-    raises_init((exc2ef, exc2e), WrongExportFunc, io=True)
-
-    exc3e = TypeError("__repr__ returned non-string (type WrongReprType)")
-    exc3ef = FieldError('Export', 'WrongExportType', 'test', from_value=exc3e, by_func='repr',
-                        reason=repr(exc3e))
-    raises_init((exc3ef, exc3e), WrongExportType, io=True)
-
-    # Error at import fields check
-    exc1i = SyntaxError('invalid syntax', ('<unknown>', 1, 6, 'Eval it!', 1, 8))
-    exc1if = FieldError('Import', 'WrongImportEval', 'test', from_value='Eval it!',
-                        by_func='literal_eval', reason=repr(exc1i))
-    raises_init((exc1if, exc1i), WrongImportEval, io=True)
-
-    exc2i = TypeError("Wrong func!")
-    exc2if = FieldError('Import', 'WrongImportFunc', 'test', from_value='5', by_func='wrong_func',
-                        reason=repr(exc2i))
-    raises_init((exc2if, exc2i), WrongImportFunc, io=True)
-
-    # Error at compare default fields with imported during check
-    msg = ("'WrongImportResult' config IO check failed:\n\tField test=5 (int) must be equal "
-           "imported=6 (int): export_func = 'repr', exported = '5', import_func = 'increment_str'")
-    raises_init(CheckValueError(msg), WrongImportResult, io=True)
-
-
-def test_repr_str():
-    for cls, str1, str2 in (
-            [Config1, "Config1.cfg.io", "'Config1' config I/O support structure"],
-            [Config2, "Config2.cfg.io", "'Valid fields' config I/O support structure"],
-            [Config3, "Config3.cfg.io", "'Gotcha' config I/O support structure"],
-            [Config4, "Config4.cfg.io", "'IO' config I/O support structure"],
-            [Lang1, "Lang1.cfg.io", "'Random' language I/O support structure"]):
-        obj = cls(io=True).cfg.io
-        assert repr(obj) == str1
-        assert str(obj) == str2
-
-    Lang1().cfg.profiles.del_group('Language')
-
-
-def test_export_field():
-    wfn = 'v_not_exists'                # Wrong field name
-    wrv = WrongReprType()               # Wrong repr value
-    cfn = 'v_list'                      # Correct field name
-    ccv = [{'s': 4}, 1, 0.7, 'data']    # Correct custom value
-    ccr = "[{'s': 4}, 1, 0.7, 'data']"  # Correct custom result
-
-    # Correct
-    cfg = Config1(io=True).cfg
-    export_field = cfg.io.export_field
-    assert export_field(cfn) == "[-1, 0, 1, 'repeat']"
-    assert export_field(cfn, ccv) == ccr
-    assert export_field(cfn, ccv, True) == ccr
-    assert export_field(cfn, ccv, False) == ccr
-
-    exp_fields = ['False', "'Some string'", '65535', '3.1415', "b'Some bytes'",  '(1, 2, 3, None)',
-                  "[-1, 0, 1, 'repeat']", "{'first'}", "{1: 'one', 2: 'two'}", '5', "'something'",
-                  '2custom', '8']
-    assert [export_field(k) for k in cfg.get_fields] == exp_fields
-    assert [export_field(k, v.default) for k, v in cfg.get_fields.items()] == exp_fields
-    assert [export_field(k, v.default, True) for k, v in cfg.get_fields.items()] == exp_fields
-    assert [export_field(k, v.default, False) for k, v in cfg.get_fields.items()] == exp_fields
-
-    # Errors
-    exc = partial(FieldError, 'Export', cfg.name)
-
-    exc_key = KeyError(wfn)
-    raises((exc(wfn, reason=repr(exc_key)), exc_key), export_field, wfn)
-    raises((exc(wfn, reason=repr(exc_key), from_value=ccv), exc_key), export_field, wfn, ccv)
-
-    exc_type = TypeError("__repr__ returned non-string (type WrongReprType)")
-    raises((exc(cfn, reason=repr(exc_type), from_value=exc_type, by_func='repr'), exc_type),
-           export_field, cfn, wrv)
-
-
-def test_export_section():
-    name1, name2 = 'name1', 'name2'
-    i1_, i1m = {'v_bool': False}, {'v_bool': True}
-    o1_, o1m = {'v_bool': 'False'}, {'v_bool': 'True'}
-    i2_, i2m = {'v_int': 65535}, {'v_int': 32767}
-    o2_, o2m = {'v_int': '65535'}, {'v_int': '32767'}
-    exp = exp_strict
-    imp = imp_strict
-
-    # Init single and profile configs related data
-    data_s = Config1(io=True)
-    data_p = Config1(io=True, profiles=True)
-    cfg_s = data_s.cfg
-    cfg_p = data_p.cfg
-    profiles = cfg_p.profiles
-    key_section = cfg_s.io._key_section
-    def_section = cfg_s.def_sect
-    ess = cfg_s.io.export_section
-    esp = cfg_p.io.export_section
-
-    # Export provided section (single and profile)
-    assert ess({}) == esp({}) == ess(i1_) == ess(i1_) == {}
-    assert (ess({}, strict=True) == esp({}, strict=True) == ess(i1_, strict=True)
-            == esp(i1_, strict=True) == exp)
-    assert ess(i1m) == esp(i1m) == o1m
-    assert ess(i1m, strict=True) == esp(i1m, strict=True) == exp | o1m
-
-    cfg_s.set_defaults(i1m)
-    cfg_p.set_defaults(i1m)
-    assert ess({}) == esp({}) == ess(i1m) == ess(i1m) == {}
-    assert (ess({}, strict=True) == esp({}, strict=True) == ess(i1m, strict=True)
-            == esp(i1m, strict=True) == exp | o1m)
-    assert ess(i1_) == esp(i1_) == o1_
-    assert ess(i1_, strict=True) == esp(i1_, strict=True) == exp
-    cfg_s.set_defaults(i1_)
-    cfg_p.set_defaults(i1_)
-
-    # Export internal section (single and profile)
-    assert ess(key_section) == ess(key_section, strict=True) == {}
-    assert esp(key_section) == esp(key_section, strict=True) == {'profile': repr(def_section)}
-    profiles.switch(name1, True)
-    assert esp(key_section) == esp(key_section, strict=True) == {'profile': repr(name1)}
-    profiles.set(name2, {'v_bool': False, 'v_int': 5}, defaults=False)
-    assert (esp(key_section) == esp(key_section, strict=True)
-            == {'profile': repr(name1), 'fields': "{'name2': ('v_bool', 'v_int')}"})
-
-    # Export default section (single and profile)
-    assert ess(def_section) == esp(def_section) == {}
-    assert ess(def_section, strict=True) == esp(def_section, strict=True) == exp
-
-    profiles.switch(def_section)
-    cfg_s.set_defaults(i1m)
-    cfg_p.set_defaults(i1m)
-    assert ess(def_section) == esp() == esp(def_section) == o1m
-
-    # Export section (single)
-    assert ess() == ess(cfg_s.name) == o1_
-    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp
-
-    data_s.v_bool = True
-    assert ess() == ess(cfg_s.name) == {}
-    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp | o1m
-
-    cfg_s.set_defaults(i1_)
-    assert ess() == ess(cfg_s.name) == o1m
-    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp | o1m
-
-    data_s.v_bool = False
-    assert ess() == ess(cfg_s.name) == {}
-    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp
-
-    # Export section (profile)
-    msg = 'Defaults v_bool state | Profile name {key: value} | short or strict export'
-    st = subtest(msg, 8, product([(False, False, i1_, i1m, o1_, o1m),
-                                  (False, True,  i2_, i2m, o2_, o2m),
-                                  (True,  False, imp | i1_, imp | i1m, exp | o1_, exp | o1m),
-                                  (True,  True,  imp | i2_, imp | i2m, exp | o2_, exp | o2m)],
-                                 [False, True]))
-    for i, (strict, crossing, i_def, i_mod, o_def, o_mod), defaults in st:
-        full = strict or defaults
-        cfg_p.set_defaults(i1_)
-        profiles.set(name1, i_def, defaults=defaults)
-        profiles.set(name2, i_mod, defaults=defaults)
-        for def_i1m in (False, True):
-            if def_i1m:
-                cfg_p.set_defaults(i1m)
-
-            # result name1 (default, short)
-            rn1d = {} if not def_i1m or crossing and not full else o1_
-
-            # result name2 (modified, short)
-            if crossing:
-                rn2m = (o1_ | o2m) if def_i1m and full else o2m
-            else:
-                rn2m = {} if def_i1m else o1m
-
-            # results strict name1 and name2 (default and modified)
-            rn1ds, rn2ms = (exp, exp | o_mod) if full else (o_def, o_mod)
-
-            # check
-            for name, res, res_strict in ((name1, rn1d, rn1ds), (name2, rn2m, rn2ms)):
-                profiles.switch(name)
-
-                val = i_def if name == name1 else i_mod
-                if strict:
-                    val = (repr({k: v for k, v in val.items() if k in ('v_bool', 'v_int')})[:-1]
-                           + ', ...}')
-                msg = f'{str(def_i1m):>5} | {name} {str(val):<17} | '
-
-                st.send((msg + ' short', esp(), esp(name), res))
-                st.send((msg + 'strict', esp(strict=True), esp(name, strict=True), res_strict))
-
-    # Errors
-    def names(target):
-        return repr(tuple(target))[1:-1]
-
-    cfg_e = ExportSensitive(io=True).cfg
-    exp_sens = cfg_e.io.export_section
-    if1 = {'wrong_name': 'wrong_data'}
-    if2 = {'some_name': 'some_data'}
-    if3 = {'f1': [1]}
-    if4 = {'f2': 2}
-
-    ie = "Provided wrong parameter to {}.cfg.io.export_section(): section. "
-    add = f"Must be not more than expected ({names(cfg_s.get_fields)}), but received"
-    add2 = f"Must be not more than expected ({names(cfg_e.get_fields)}), but received"
-    ie1 = "[[]] (list) must be Mapping type"
-    ie2 = f"Extra field: 'wrong_name'. {add}: {names(imp | if1)}"
-    ie3 = f"Extra fields: 'wrong_name', 'some_name'. {add}: {names(imp | if1 | if2)}"
-    ie4 = f"Extra fields: 'wrong_name', 'some_name'. {add2}: {names(if1 | if2 | if3 | if4)}"
-    ie5 = "Profile is not exists, there is no profiles"
-    ie6 = "Profile is not exists, available profiles: 'name1', 'name2'"
-    ie7 = "Must be 'Config1', but received 'nes'"
-    raises(InputError(msg=ie.format('Config1') + ie1), esp, [[]])
-    raises(InputError(msg=ie.format('Config1') + ie2), esp, imp | if1)
-    raises(InputError(msg=ie.format('Config1') + ie3), esp, imp | if1 | if2)
-    raises(InputError(msg=ie.format('ExportSensitive') + ie4), exp_sens, if1 | if2 | if3 | if4)
-    raises(InputError(msg=ie.format('Config1') + ie5),
-           Config1(io=True, profiles=True).cfg.io.export_section, 'nes')
-    raises(InputError(msg=ie.format('Config1') + ie6), esp, 'nes')
-    raises(InputError(msg=ie.format('Config1') + ie7), ess, 'nes')
-
-    msg = "Cannot export 'ExportSensitive' config section. Errors:"
-    f1 = "Field f1=[1] (list) by <lambda>: CheckTypeError('Field [1] (list) must be str type')"
-    f2 = "Field f2=2 (int) by <lambda>: CheckTypeError('Field 2 (int) must be str type')"
-    raises(IOExportError(msg + f"\n\t{f1}"), exp_sens, if3, typecast=False)
-    raises(IOExportError(msg + f"\n\t{f1}\n\t{f2}"), exp_sens, if3 | if4, typecast=False)
-
-
-def test_export_configs():
-    # Prepare simple config data
-    data_s = Config4(io=True)
-    data_s.C4 = 10
-    ecs = data_s.cfg.io.export_config
-
-    # Section names
-    sec_internal = data_s.cfg.io._key_section
-    sec_default = data_s.cfg.def_sect
-    sec_simple = 'IO'
-    sec_profile1 = 'profile1'
-    sec_profile2 = 'Profile 2'
-
-    # Section values
-    val_internal = {'profile': repr(sec_default)} | {'fields': "{'profile1': ('C4',)}"}
-    val_default = {'C4': '4'}
-    val_modified = {'C4': '10'}
-
-    # Prepare profiles config data
-    data_p = Config4(io=True, profiles=True)
-    data_p.C4 = 10
-    data_p.cfg.profiles.set(sec_profile1, val_default, typecast=True, defaults=False)
-    data_p.cfg.profiles.set(sec_profile2)
-    ecp = data_p.cfg.io.export_config
-
-    # Internal section completed
-    ip_ = {sec_internal: val_internal}
-
-    # Default sections completed
-    ds_ = {sec_default: {}}
-    dp_ = {sec_default: val_modified}
-    dss = {sec_default: exp_strict | val_default}
-    dps = {sec_default: exp_strict | val_modified}
-
-    # Simple config section completed
-    vs_ = {sec_simple: val_modified}
-    vss = {sec_simple: exp_strict | val_modified}
-
-    # Profiles config section completed
-    vp_1 = {sec_profile1: val_default}
-    vp_2 = {sec_profile2: {}}
-    vps2 = {sec_profile2: exp_strict | val_modified}
-
-    # Exceptions
-    exc_ie = partial(InputError, 'profiles', func_name='Config4.cfg.io.export_config()')
-    msg_disabled = "Profiles disabled, but provided"
-    msg_extra = ("Extra profile: ''. "
-                 "Must be not more than expected ('profile1', 'Profile 2'), but received: ''")
-
-    def fmt_cte(section, value):
-        inner_exc = CheckTypeError(f'Field {value} (int) must be str type')
-        return IOExportError(f"Cannot export 'IO' config section {section!r}. Errors:\n"
-                             f"\tField C4={value} (int) by <lambda>: {inner_exc!r}")
-
-    # Build subtest dataset
-    profiles_set = [None, '', sec_profile1, [sec_profile1], [sec_profile1, sec_profile2]]
-    cases = product(profiles_set, *((False, True),) * 3)
-    names = ('profiles', 'strict_defaults', 'strict_data', 'typecast')
-
-    # Run subtest
-    for i, profiles, s_def, s_data, typecast in (st := subtest('', 40, cases, names=names)):
-        kwargs = dict(zip(names[1:], (s_def, s_data, typecast), strict=True))
-
-        # Prepare simple result
-        if profiles is None:
-            if typecast:
-                rs = (dss if s_def else ds_) | (vss if s_data else vs_)
-            else:
-                rs = fmt_cte(sec_default, 4) if s_def else fmt_cte(sec_simple, 10)
-        else:
-            rs = exc_ie(msg=f'{msg_disabled}: {profiles!r}')
-
-        # Prepare profiles result
-        if not typecast:
-            rp = fmt_cte(sec_default, 10)
-        elif profiles == '':
-            rp = exc_ie(msg=msg_extra)
-        else:
-            rp = ip_ | (dps if s_def else dp_)
-            if profiles is None or sec_profile1 in profiles:
-                rp |= vp_1
-            if profiles is None or sec_profile2 in profiles:
-                rp |= (vps2 if s_data else vp_2)
-
-        # Test both
-        for name, target, result in (('simple', ecs, rs), ('profiles', ecp, rp)):
-            if any(map(is_exception, results := as_holder(result))):
-                try:
-                    raises(result, target, profiles, **kwargs)
-                except Exception as e:
-                    st.send(('', type(e).__name__, results[0]))
-                else:
-                    st.send((f'Exception {name}', results[0], results[0]))
-            else:
-                st.send((f'Result {name}', safe(target, profiles, **kwargs), result))
-
-
-def test_import_field():
-    wfn = 'v_not_exists'                # Wrong field name
-    wev = 'wrong value'                 # Wrong eval value
-    wrv = WrongReprType()               # Wrong repr value
-    wcv = "'wrong value'"               # Wrong custom value
-    cfn = 'v_list'                      # Correct field name
-    ccv = "[{'s': 4}, 1, 0.7, 'data']"  # Correct custom value
-    ccr = [{'s': 4}, 1, 0.7, 'data']    # Correct custom result
-
-    # Correct
-    cfg = Config1(io=True).cfg
-    import_field = cfg.io.import_field
-    assert import_field(cfn, ccv) == ccr
-    assert import_field(cfn, ccv, True) == ccr
-    assert import_field(cfn, ccv, False) == ccr
-
-    exp_f_std = ['False', "'Some string'", '65535', '3.1415', "b'Some bytes'", '(1, 2, 3, None)',
-                 "[-1, 0, 1, 'repeat']", "{'first'}", "{1: 'one', 2: 'two'}"]
-    exp_f_safe = ["'something'", '2custom', '8']
-
-    imp_f_std = [False, 'Some string', 65535, 3.1415, b'Some bytes',  (1, 2, 3, None),
-                 [-1, 0, 1, 'repeat'], {'first'}, {1: 'one', 2: 'two'}]
-    imp_f_safe = ['something', 2, 8]
-
-    names_safe = ['v_cust2', 'v_cust3', '_internal']
-
-    exp_dict = dict(zip(cfg.get_fields, exp_f_std + ['5'] + exp_f_safe))
-    imp_list = imp_f_std + [OwnInt(5)] + imp_f_safe
-
-    exp_dict_safe = dict(zip(cfg.get_fields, exp_f_std)) | dict(zip(names_safe, exp_f_safe))
-    imp_list_safe = imp_f_std + imp_f_safe
-
-    assert [import_field(k, v) for k, v in exp_dict.items()] == imp_list
-    assert [import_field(k, v, True) for k, v in exp_dict.items()] == imp_list
-    assert [import_field(k, v, False) for k, v in exp_dict_safe.items()] == imp_list_safe
-
-    # Errors
-    exc_field = partial(FieldError, 'Import', cfg.name)
-
-    exc1 = CheckTypeError('Field 5 (int) must be OwnInt type')
-    exc1f = exc_field('v_cust1', from_value='5', by_func='literal_eval', reason=repr(exc1))
-    raises((exc1f, exc1), import_field, 'v_cust1', '5', False)
-
-    exc2 = KeyError(wfn)
-    exc2f = exc_field(wfn, from_value=ccv, reason=repr(exc2))
-    raises((exc2f, exc2), import_field, wfn, ccv)
-
-    exc3 = SyntaxError('invalid syntax', ('<unknown>', 1, 7, wev, 1, 12))
-    exc3f = exc_field(cfn, from_value=wev, by_func='literal_eval', reason=repr(exc3))
-    raises((exc3f, exc3), import_field, cfn, wev)
-
-    exc4 = TypeError("__repr__ returned non-string (type WrongReprType)")
-    exc4f = exc_field(cfn, from_value=wrv, by_func='literal_eval', reason=repr(exc4))
-    raises((exc4f, exc4), import_field, cfn, wrv)
-
-    exc5 = CheckTypeError("Field 'wrong value' (str) must be list type")
-    exc5f = exc_field(cfn, from_value=wcv, by_func='literal_eval', reason=repr(exc5))
-    raises((exc5f, exc5), import_field, cfn, wcv, typecast=False)
-
-
-def test_import_section():
-    exp = exp_strict
-    exp2 = exp.copy()
-    exp2['v_bool'] = 'True'
-
-    # i1_, i1m = {'v_bool': 'False'}, {'v_bool': 'True'}
-    # o1_, o1m = {'v_bool': False}, {'v_bool': True}
-    i2_, i2m = {'v_int': '65535'}, {'v_int': '32767'}
-    o2_, o2m = {'v_int': 65535}, {'v_int': 32767}
-
-    imp = imp_strict
-    imp2 = imp.copy()
-    imp2['v_bool'] = True
-
-    cfg_s = Config1(io=True).cfg
-    cfg_p = Config1(io=True, profiles=True).cfg
-    iss = cfg_s.io.import_section
-    isp = cfg_p.io.import_section
-
-    # Not change data in configs (single and profile)
-    assert iss(i2m) == isp(i2m) == o2m
-    assert cfg_s.get_data == cfg_p.get_data == cfg_s.get_defaults == cfg_p.get_defaults == imp
-
-    assert iss(exp) == isp(exp) == imp
-    assert cfg_s.get_data == cfg_p.get_data == cfg_s.get_defaults == cfg_p.get_defaults == imp
-
-    assert iss(exp2) == isp(exp2) == imp2
-    assert cfg_s.get_data == cfg_p.get_data == cfg_s.get_defaults == cfg_p.get_defaults == imp
-
-    # Change data in configs (single)
-    pass  # Not implemented
-
-    # Change data in configs (profile)
-    pass  # Not implemented
-
-    # Errors
-    def names(target):
-        return repr(tuple(target))[1:-1]
-
-    add = f"Must be not more than expected ({names(cfg_s.get_fields)}), but received"
-
-    ef1 = {'wrong_name': 'wrong_data'}
-    ef2 = {'some_name': 'some_data'}
-    ef3 = {'v_int': 13}
-    ef4 = {'v_dict': 1}
-
-    ie = "Provided wrong parameter to Config1.cfg.io.import_section(): raw_section. "
-    ie1 = "[[]] (list) must be Mapping type"
-    ie2 = f"Extra field: 'wrong_name'. {add}: {names(exp | ef1)}"
-    ie3 = f"Extra fields: 'wrong_name', 'some_name'. {add}: {names(exp | ef1 | ef2)}"
-    ie4 = f"Extra fields: 'wrong_name', 'some_name'. {add}: {names(exp | ef1 | ef2 | ef3 | ef4)}"
-    raises(InputError(msg=ie + ie1), iss, [[]])
-    raises(InputError(msg=ie + ie1), isp, [[]])
-    raises(InputError(msg=ie + ie2), iss, exp | ef1)
-    raises(InputError(msg=ie + ie2), isp, exp | ef1)
-    raises(InputError(msg=ie + ie3), iss, exp | ef1 | ef2)
-    raises(InputError(msg=ie + ie3), isp, exp | ef1 | ef2)
-    raises(InputError(msg=ie + ie4), iss, exp | ef1 | ef2 | ef3 | ef4)
-    raises(InputError(msg=ie + ie4), isp, exp | ef1 | ef2 | ef3 | ef4)
-
-    msg = "Cannot import 'Config1' config section"
-    p1 = "Field v_int=13 (int) by literal_eval: ValueError('malformed node or string: 13')"
-    p2 = "Field v_dict=1 (int) by literal_eval: ValueError('malformed node or string: 1')"
-    raises(IOImportError(msg + f". Errors:\n\t{p1}"), iss, exp | ef3)
-    raises(IOImportError(msg + f". Errors:\n\t{p1}"), isp, exp | ef3)
-    raises(IOImportError(msg + f". Errors:\n\t{p1}\n\t{p2}"), iss, exp | ef3 | ef4)
-    raises(IOImportError(msg + f". Errors:\n\t{p1}\n\t{p2}"), isp, exp | ef3 | ef4)
-
-
-def test_import_config():
-    # Prepare simple and profiles configs
-    data_s = Config4(io=True)
-    data_p = Config4(io=True, profiles=True)
-    ics = data_s.cfg.io.import_config
-    icp = data_p.cfg.io.import_config
-    df = exp_strict | {'C4': '4'}                       # default fields
-
-    # Internal section keys
-    kiv = data_s.cfg.io._key_version
-    kip = data_s.cfg.io._key_profile
-    kif = data_s.cfg.io._key_fields
-
-    # Values
-    e1_, e1m = {'v_bool': 'False'}, {'v_bool': 'True'}
-    i1_, i1m = {'v_bool': False}, {'v_bool': True}
-    e2_, e2m = {'v_int': '65535'}, {'v_int': '32767'}
-    i2_, i2m = {'v_int': 65535}, {'v_int': 32767}
-
-    # Sections names
-    internal = data_s.cfg.io._key_section
-    default_ = data_s.cfg.def_sect
-    simple__ = 'IO'
-    profile_ = 'p1'
-
-    # Exported values
-    ev_d_ = e2m                                                 # default
-    ev_s_ = e1m | e2_                                           # simple
-    ev_p_ = ev_s_ | ev_d_                                       # profile
-    ev_f_ = e1m                                                 # fields active
-    ev_id = {kip: repr(default_)}                               # internal default
-    ev_ip = {kip: repr(profile_)}                               # internal profile
-    ev_if = {kip: repr(profile_), kif: "{'p1': ('v_bool',)}"}   # internal fields (profiles active)
-
-    # 1. Exported Simple
-    s___ed_ = {default_: {} | ev_d_}                            # default
-    s___eds = {default_: df | ev_d_}                            # default strict
-    s___es_ = {simple__: {} | ev_s_}                            # section
-    s___ess = {simple__: df | ev_s_}                            # section strict
-
-    # 2. Exported Profiles: default
-    pd__ed_ = {internal: ev_id, default_: {} | ev_p_}           # default
-    pd__eds = {internal: ev_id, default_: df | ev_p_}           # default strict
-    pd__es_ = {}                                                # section
-    pd__ess = {}                                                # section strict
-
-    # 3. Exported Profiles: default, active fields
-    # The same as 2, because default profile always have all fields active
-
-    # 4. Exported Profiles: profile
-    pp__ed_ = {internal: ev_ip, default_: {} | ev_d_}           # default
-    pp__eds = {internal: ev_ip, default_: df | ev_d_}           # default strict
-    pp__es_ = {profile_: {} | ev_s_}                            # section
-    pp__ess = {profile_: df | ev_s_}                            # section strict
-
-    # 5. Profiles: profile, active fields
-    ppa_ed_ = {internal: ev_if, default_: {} | ev_d_}           # default
-    ppa_eds = {internal: ev_if, default_: df | ev_d_}           # default strict
-    ppa_es_ = {profile_: {} | ev_f_}                            # section
-
-    # Typecast error
-    e1 = CheckTypeError('Field 5 (int) must be OwnInt type')
-    e2 = CheckTypeError("Field '4' (str) must be int type")
-    msg = ("Cannot import 'IO' config section {!r}. Errors:\n"
-           f"\tField v_cust1='5' (str) by literal_eval: {e1!r}\n"
-           f"\tField C4='4' (str) by <lambda>: {e2!r}")
-
-    def import_and_compare_configs(**kwargs):
-        nonlocal k
-        k += 1
-        i_data = Config4(io=True, profiles=profiles)
-        i_data.cfg.io.import_config(data, **kwargs)
-        assert e_data.cfg.get_data == i_data.cfg.get_data
-        assert e_data.cfg.get_defaults == i_data.cfg.get_defaults
-        if profiles:
-            assert e_data.cfg.profiles.get == i_data.cfg.profiles.get
-            assert e_data.cfg.profiles.active == i_data.cfg.profiles.active
-            assert e_data.cfg.profiles.active_fields == i_data.cfg.profiles.active_fields
-        assert data == i_data.cfg.io.export_config(strict_defaults=bd, strict_data=bv)
-
-    # Correct
-    i = j = k = 0
-    section = defaults = bd = bv = data = None
-    try:
-        for i, (section, defaults, d_, ds, s_, ss) in enumerate([
-            (simple__, None,  s___ed_, s___eds, s___es_, s___ess),
-            (default_, True,  pd__ed_, pd__eds, pd__es_, pd__ess),
-            (default_, False, pd__ed_, pd__eds, pd__es_, pd__ess),
-            (profile_, True,  pp__ed_, pp__eds, pp__es_, pp__ess),
-            (profile_, False, ppa_ed_, ppa_eds, ppa_es_, ppa_es_)
-        ], 1):
-            # Prepare source config
-            if profiles := section != simple__:
-                e_data = Config4(io=True, profiles=True)
-                e_data.cfg.profiles.set(section, i1m, defaults=defaults)
-                e_data.cfg.profiles.set(default_, i2m)
-                e_data.cfg.profiles.switch(section)
-            else:
-                e_data = Config4(io=True)
-                e_data.cfg.set_fields(i1m)
-                e_data.cfg.set_defaults(i2m)
-
-            # Check source config and target configs for equality
-            tests = product([(False, d_), (True, ds)], [(False, s_), (True, ss)])
-            for j, ((bd, sd), (bv, sv)) in enumerate(tests, 1):
-                # Export
-                k, data = 0, sd | sv
-                assert data == e_data.cfg.io.export_config(strict_defaults=bd, strict_data=bv)
-
-                # Import
-                dd, dv = data.get(default_, ()), data.get(section, {})
-                if (dd := 'C4' in dd) or 'C4' in dv:
-                    k = 1
-                    i1 = Config4(io=True, profiles=profiles)
-                    raises(IOImportError(msg.format(default_ if dd else section)),
-                           i1.cfg.io.import_config, data, typecast=False)
-                else:
-                    import_and_compare_configs(typecast=False)
-                import_and_compare_configs(typecast=True)
-                import_and_compare_configs(sections=(default_, section))
-
-    except Exception as e:
-        raise AssertionError(f"Correct import test failed at {i}.{j}.{k}: "
-                             f"{section=}, {defaults=}, {bd=}, {bv=}, \n{data=}") from e
-
-    # Errors
-
-    # For version errors only
-    with (cfg_v := Config4(io=True).cfg):
-        cfg_v.version = '0.1'
-    icv = cfg_v.io.import_config
-
-    # Valid params
-    vpp = {kip: repr(default_)}
-    vpf = {kif: "{'p1': ('v_str', 'v_int')}"}
-
-    # Valid sections
-    vs_is = {internal: vpp}
-    vs_ip = {internal: vpp | vpf}
-    vsd = {default_: {}}
-    vsp = {'p1': {'v_str': '123', 'v_int': '5'}}
-
-    def names(target):
-        return repr(tuple(target))[1:-1]
-
-    # Input errors
-    ie = "Provided wrong parameter to Config4.cfg.io.import_config()"
-    add = "Must be not more than expected ({}), but received: {}"
-    add2 = add.format("'DEFAULT'", "'Some'")
-    add3 = add.format(names(cfg_v.get_fields), "'wrong'")
-    add4 = add.format(names(cfg_v.get_fields), "'v_bool', 'wrong'")
-
-    exc1 = TypeError("'int' object is not iterable")
-    exc2 = SyntaxError('invalid syntax', ('<unknown>', 0, 0, '', 0, 0))
-    exc3 = TypeError('cannot convert dictionary update sequence element #0 to a sequence')
-
-    ies = f"{ie}: sections. Extra section: 'Some'. {add}"      # sections
-    ie_s1 = InputError(msg=ies.format("'IO'", "'Some'"))
-    ie_s2 = InputError(msg=ies.format("'IO'", "'IO', 'Some'"))
-    ie_s3 = InputError(msg=ies.format("'p1'", "'Some'"))
-    ie_s4 = InputError(msg=ies.format("'p1', '1', '2'", "'Some'"))
-
-    ci_p = "is not needed, but provided"                        # check_input provided error
-    ci_n = "is needed, but not provided"                        # check_input needed error
-    af_p = "Active fields dict is not parsed"                   # active_fields parsing
-    af_e = f"Extra active fields profile: 'Some'. {add2}"       # active_fields extra
-    afke = f"Extra 'p1' profile active field: 'wrong'. {add3}"  # active_fields extra
-    df_e = f"Extra default field: 'wrong'. {add4}"              # default field extra
-
-    ier = f"{ie}: raw_config."                                  # raw_config
-    msg_r14 = (f"{ier} Extra 'p1' profile field: 'v_bool'. Absent 'p1' profile field: 'v_str'. "
-               "Must be equal to expected ('v_str', 'v_int'), but received: 'v_bool', 'v_int'")
-    ie_r01 = InputError(msg=f"{ier} {internal!r} section {ci_p}")
-    ie_r02 = InputError(msg=f"{ier} {internal!r} section {ci_n}")
-    ie_r03 = InputError(msg=f"{ier} {kiv.capitalize()} {ci_p}")
-    ie_r04 = InputError(msg=f"{ier} {kiv.capitalize()} {ci_n}")
-    # ie_r05 = InputError(msg=f"{ier} {kip.capitalize()} {ci_p}")                 waits for version
-    ie_r06 = InputError(msg=f"{ier} {kip.capitalize()} {ci_n}")
-    ie_r07 = InputError(msg=f"{ier} Active profile is not provided: 'Some'")
-    ie_r08 = (InputError(msg=f"{ier} {af_p}: '1'"), exc1)
-    ie_r09 = (InputError(msg=f"{ier} {af_p}: ''"), exc2)
-    ie_r10 = (InputError(msg=f"{ier} {af_p}: '[1]'"), exc3)
-    ie_r11 = InputError(msg=f"{ier} {af_e}")
-    ie_r12 = InputError(msg=f"{ier} {afke}")
-    ie_r13 = InputError(msg=f"{ier} {df_e}")
-    ie_r14 = InputError(msg=msg_r14)
-
-    raises(ie_s1, ics, {}, 'Some')
-    raises(ie_s2, ics, {}, ('IO', 'Some'))
-    raises(ie_s3, icp, vs_ip | vsp, 'Some')
-    raises(ie_s4, icp, vs_ip | vsp | {'1': {}, '2': {}}, 'Some')
-
-    raises(ie_r01, ics, {internal: {}})
-    raises(ie_r02, icp, {})
-    raises(ie_r03, icp, {internal: {kiv: ''}})
-    raises(ie_r04, icv, {internal: {}})
-    # raises(ie_r05, icv, {internal: {kiv: '', kip: ''}})                         waits for version
-    raises(ie_r06, icp, {internal: {}})
-    raises(ie_r07, icp, {internal: {kip: "'Some'"}})
-    raises(ie_r08, icp, {internal: vpp | {kif: '1'}} | vsd)
-    raises(ie_r09, icp, {internal: vpp | {kif: ''}} | vsd)
-    raises(ie_r10, icp, {internal: vpp | {kif: '[1]'}} | vsd)
-    raises(ie_r11, icp, {internal: vpp | {kif: "{'Some': ('v_str',)}"}} | vsd)
-    raises(ie_r12, icp, {internal: vpp | {kif: "{'p1': ('wrong',)}"}} | vsd | vsp)
-    raises(ie_r13, ics, {default_: {'v_bool': True, 'wrong': True}})
-    raises(ie_r13, icp, {default_: {'v_bool': True, 'wrong': True}} | vs_is)
-    raises(ie_r14, icp, vs_ip | vsd | {'p1': {'v_bool': 'True', 'v_int': '1'}})
-
-    # IOImport Errors
-    msg = "Cannot import 'IO' config. "
-    exc4 = NotImplementedError('Version import is not available yet')
-    tmpl = ("Cannot import 'IO' config section {!r}. Errors:\n\tField v_bool=True (bool)"
-            " by literal_eval: ValueError('malformed node or string: True')")
-
-    raises((IOImportError(msg + repr(exc4)), exc4), icv, {internal: {kiv: ''}})
-    raises(IOImportError(tmpl.format(default_)), ics, {default_: {'v_bool': True}})
-    raises(IOImportError(tmpl.format(default_)), icp, {default_: {'v_bool': True}} | vs_is)
-    raises(IOImportError(tmpl.format(simple__)), ics, {simple__: {'v_bool': True}})
-    raises(IOImportError(tmpl.format('Some1')), icp, {'Some1': {'v_bool': True}} | vs_is | vsd)
+from functools import partial
+from itertools import product
+
+from configlayer.exceptions import (InputError, CheckValueError, CheckTypeError,
+                                    FieldError, IOExportError, IOImportError)
+from configlayer.utils import safe, as_holder, is_exception
+
+from _utilities import raises_init, raises, subtest
+from _data import (WrongExportRepr, WrongExportFunc, WrongExportType, WrongImportEval,
+                   WrongImportFunc, WrongImportResult, WrongReprType, ExportSensitive,
+                   Config1, Config2, Config3, Config4, Lang1, exp_strict, imp_strict, OwnInt)
+
+
+def test_init():
+    # Correct
+    assert Config1(io=True)
+
+    # Error at export fields check
+    exc1e = TypeError("Wrong repr!")
+    exc1ef = FieldError('Export', 'WrongExportRepr', 'test', from_value=exc1e, by_func='repr',
+                        reason=repr(exc1e))
+    raises_init((exc1ef, exc1e), WrongExportRepr, io=True)
+
+    exc2e = TypeError("Wrong func!")
+    exc2ef = FieldError('Export', 'WrongExportFunc', 'test', from_value=5, by_func='wrong_func',
+                        reason=repr(exc2e))
+    raises_init((exc2ef, exc2e), WrongExportFunc, io=True)
+
+    exc3e = TypeError("__repr__ returned non-string (type WrongReprType)")
+    exc3ef = FieldError('Export', 'WrongExportType', 'test', from_value=exc3e, by_func='repr',
+                        reason=repr(exc3e))
+    raises_init((exc3ef, exc3e), WrongExportType, io=True)
+
+    # Error at import fields check
+    exc1i = SyntaxError('invalid syntax', ('<unknown>', 1, 6, 'Eval it!', 1, 8))
+    exc1if = FieldError('Import', 'WrongImportEval', 'test', from_value='Eval it!',
+                        by_func='literal_eval', reason=repr(exc1i))
+    raises_init((exc1if, exc1i), WrongImportEval, io=True)
+
+    exc2i = TypeError("Wrong func!")
+    exc2if = FieldError('Import', 'WrongImportFunc', 'test', from_value='5', by_func='wrong_func',
+                        reason=repr(exc2i))
+    raises_init((exc2if, exc2i), WrongImportFunc, io=True)
+
+    # Error at compare default fields with imported during check
+    msg = ("'WrongImportResult' config IO check failed:\n\tField test=5 (int) must be equal "
+           "imported=6 (int): export_func = 'repr', exported = '5', import_func = 'increment_str'")
+    raises_init(CheckValueError(msg), WrongImportResult, io=True)
+
+
+def test_repr_str():
+    for cls, str1, str2 in (
+            [Config1, "Config1.cfg.io", "'Config1' config I/O support structure"],
+            [Config2, "Config2.cfg.io", "'Valid fields' config I/O support structure"],
+            [Config3, "Config3.cfg.io", "'Gotcha' config I/O support structure"],
+            [Config4, "Config4.cfg.io", "'IO' config I/O support structure"],
+            [Lang1, "Lang1.cfg.io", "'Random' language I/O support structure"]):
+        obj = cls(io=True).cfg.io
+        assert repr(obj) == str1
+        assert str(obj) == str2
+
+    Lang1().cfg.profiles.del_group('Language')
+
+
+def test_export_field():
+    wfn = 'v_not_exists'                # Wrong field name
+    wrv = WrongReprType()               # Wrong repr value
+    cfn = 'v_list'                      # Correct field name
+    ccv = [{'s': 4}, 1, 0.7, 'data']    # Correct custom value
+    ccr = "[{'s': 4}, 1, 0.7, 'data']"  # Correct custom result
+
+    # Correct
+    cfg = Config1(io=True).cfg
+    export_field = cfg.io.export_field
+    assert export_field(cfn) == "[-1, 0, 1, 'repeat']"
+    assert export_field(cfn, ccv) == ccr
+    assert export_field(cfn, ccv, True) == ccr
+    assert export_field(cfn, ccv, False) == ccr
+
+    exp_fields = ['False', "'Some string'", '65535', '3.1415', "b'Some bytes'",  '(1, 2, 3, None)',
+                  "[-1, 0, 1, 'repeat']", "{'first'}", "{1: 'one', 2: 'two'}", '5', "'something'",
+                  '2custom', '8']
+    assert [export_field(k) for k in cfg.get_fields] == exp_fields
+    assert [export_field(k, v.default) for k, v in cfg.get_fields.items()] == exp_fields
+    assert [export_field(k, v.default, True) for k, v in cfg.get_fields.items()] == exp_fields
+    assert [export_field(k, v.default, False) for k, v in cfg.get_fields.items()] == exp_fields
+
+    # Errors
+    exc = partial(FieldError, 'Export', cfg.name)
+
+    exc_key = KeyError(wfn)
+    raises((exc(wfn, reason=repr(exc_key)), exc_key), export_field, wfn)
+    raises((exc(wfn, reason=repr(exc_key), from_value=ccv), exc_key), export_field, wfn, ccv)
+
+    exc_type = TypeError("__repr__ returned non-string (type WrongReprType)")
+    raises((exc(cfn, reason=repr(exc_type), from_value=exc_type, by_func='repr'), exc_type),
+           export_field, cfn, wrv)
+
+
+def test_export_section():
+    name1, name2 = 'name1', 'name2'
+    i1_, i1m = {'v_bool': False}, {'v_bool': True}
+    o1_, o1m = {'v_bool': 'False'}, {'v_bool': 'True'}
+    i2_, i2m = {'v_int': 65535}, {'v_int': 32767}
+    o2_, o2m = {'v_int': '65535'}, {'v_int': '32767'}
+    exp = exp_strict
+    imp = imp_strict
+
+    # Init single and profile configs related data
+    data_s = Config1(io=True)
+    data_p = Config1(io=True, profiles=True)
+    cfg_s = data_s.cfg
+    cfg_p = data_p.cfg
+    profiles = cfg_p.profiles
+    key_section = cfg_s.io._key_section
+    def_section = cfg_s.def_sect
+    ess = cfg_s.io.export_section
+    esp = cfg_p.io.export_section
+
+    # Export provided section (single and profile)
+    assert ess({}) == esp({}) == ess(i1_) == ess(i1_) == {}
+    assert (ess({}, strict=True) == esp({}, strict=True) == ess(i1_, strict=True)
+            == esp(i1_, strict=True) == exp)
+    assert ess(i1m) == esp(i1m) == o1m
+    assert ess(i1m, strict=True) == esp(i1m, strict=True) == exp | o1m
+
+    cfg_s.set_defaults(i1m)
+    cfg_p.set_defaults(i1m)
+    assert ess({}) == esp({}) == ess(i1m) == ess(i1m) == {}
+    assert (ess({}, strict=True) == esp({}, strict=True) == ess(i1m, strict=True)
+            == esp(i1m, strict=True) == exp | o1m)
+    assert ess(i1_) == esp(i1_) == o1_
+    assert ess(i1_, strict=True) == esp(i1_, strict=True) == exp
+    cfg_s.set_defaults(i1_)
+    cfg_p.set_defaults(i1_)
+
+    # Export internal section (single and profile)
+    assert ess(key_section) == ess(key_section, strict=True) == {}
+    assert esp(key_section) == esp(key_section, strict=True) == {'profile': repr(def_section)}
+    profiles.switch(name1, True)
+    assert esp(key_section) == esp(key_section, strict=True) == {'profile': repr(name1)}
+    profiles.set(name2, {'v_bool': False, 'v_int': 5}, defaults=False)
+    assert (esp(key_section) == esp(key_section, strict=True)
+            == {'profile': repr(name1), 'fields': "{'name2': ('v_bool', 'v_int')}"})
+
+    # Export default section (single and profile)
+    assert ess(def_section) == esp(def_section) == {}
+    assert ess(def_section, strict=True) == esp(def_section, strict=True) == exp
+
+    profiles.switch(def_section)
+    cfg_s.set_defaults(i1m)
+    cfg_p.set_defaults(i1m)
+    assert ess(def_section) == esp() == esp(def_section) == o1m
+
+    # Export section (single)
+    assert ess() == ess(cfg_s.name) == o1_
+    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp
+
+    data_s.v_bool = True
+    assert ess() == ess(cfg_s.name) == {}
+    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp | o1m
+
+    cfg_s.set_defaults(i1_)
+    assert ess() == ess(cfg_s.name) == o1m
+    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp | o1m
+
+    data_s.v_bool = False
+    assert ess() == ess(cfg_s.name) == {}
+    assert ess(strict=True) == ess(cfg_s.name, strict=True) == exp
+
+    # Export section (profile)
+    msg = 'Defaults v_bool state | Profile name {key: value} | short or strict export'
+    st = subtest(msg, 8, product([(False, False, i1_, i1m, o1_, o1m),
+                                  (False, True,  i2_, i2m, o2_, o2m),
+                                  (True,  False, imp | i1_, imp | i1m, exp | o1_, exp | o1m),
+                                  (True,  True,  imp | i2_, imp | i2m, exp | o2_, exp | o2m)],
+                                 [False, True]))
+    for i, (strict, crossing, i_def, i_mod, o_def, o_mod), defaults in st:
+        full = strict or defaults
+        cfg_p.set_defaults(i1_)
+        profiles.set(name1, i_def, defaults=defaults)
+        profiles.set(name2, i_mod, defaults=defaults)
+        for def_i1m in (False, True):
+            if def_i1m:
+                cfg_p.set_defaults(i1m)
+
+            # result name1 (default, short)
+            rn1d = {} if not def_i1m or crossing and not full else o1_
+
+            # result name2 (modified, short)
+            if crossing:
+                rn2m = (o1_ | o2m) if def_i1m and full else o2m
+            else:
+                rn2m = {} if def_i1m else o1m
+
+            # results strict name1 and name2 (default and modified)
+            rn1ds, rn2ms = (exp, exp | o_mod) if full else (o_def, o_mod)
+
+            # check
+            for name, res, res_strict in ((name1, rn1d, rn1ds), (name2, rn2m, rn2ms)):
+                profiles.switch(name)
+
+                val = i_def if name == name1 else i_mod
+                if strict:
+                    val = (repr({k: v for k, v in val.items() if k in ('v_bool', 'v_int')})[:-1]
+                           + ', ...}')
+                msg = f'{str(def_i1m):>5} | {name} {str(val):<17} | '
+
+                st.send((msg + ' short', esp(), esp(name), res))
+                st.send((msg + 'strict', esp(strict=True), esp(name, strict=True), res_strict))
+
+    # Errors
+    def names(target):
+        return repr(tuple(target))[1:-1]
+
+    cfg_e = ExportSensitive(io=True).cfg
+    exp_sens = cfg_e.io.export_section
+    if1 = {'wrong_name': 'wrong_data'}
+    if2 = {'some_name': 'some_data'}
+    if3 = {'f1': [1]}
+    if4 = {'f2': 2}
+
+    ie = "Provided wrong parameter to {}.cfg.io.export_section(): section. "
+    add = f"Must be not more than expected ({names(cfg_s.get_fields)}), but received"
+    add2 = f"Must be not more than expected ({names(cfg_e.get_fields)}), but received"
+    ie1 = "[[]] (list) must be Mapping type"
+    ie2 = f"Extra field: 'wrong_name'. {add}: {names(imp | if1)}"
+    ie3 = f"Extra fields: 'wrong_name', 'some_name'. {add}: {names(imp | if1 | if2)}"
+    ie4 = f"Extra fields: 'wrong_name', 'some_name'. {add2}: {names(if1 | if2 | if3 | if4)}"
+    ie5 = "Profile is not exists, there is no profiles"
+    ie6 = "Profile is not exists, available profiles: 'name1', 'name2'"
+    ie7 = "Must be 'Config1', but received 'nes'"
+    raises(InputError(msg=ie.format('Config1') + ie1), esp, [[]])
+    raises(InputError(msg=ie.format('Config1') + ie2), esp, imp | if1)
+    raises(InputError(msg=ie.format('Config1') + ie3), esp, imp | if1 | if2)
+    raises(InputError(msg=ie.format('ExportSensitive') + ie4), exp_sens, if1 | if2 | if3 | if4)
+    raises(InputError(msg=ie.format('Config1') + ie5),
+           Config1(io=True, profiles=True).cfg.io.export_section, 'nes')
+    raises(InputError(msg=ie.format('Config1') + ie6), esp, 'nes')
+    raises(InputError(msg=ie.format('Config1') + ie7), ess, 'nes')
+
+    msg = "Cannot export 'ExportSensitive' config section. Errors:"
+    f1 = "Field f1=[1] (list) by <lambda>: CheckTypeError('Field [1] (list) must be str type')"
+    f2 = "Field f2=2 (int) by <lambda>: CheckTypeError('Field 2 (int) must be str type')"
+    raises(IOExportError(msg + f"\n\t{f1}"), exp_sens, if3, typecast=False)
+    raises(IOExportError(msg + f"\n\t{f1}\n\t{f2}"), exp_sens, if3 | if4, typecast=False)
+
+
+def test_export_configs():
+    # Prepare simple config data
+    data_s = Config4(io=True)
+    data_s.C4 = 10
+    ecs = data_s.cfg.io.export_config
+
+    # Section names
+    sec_internal = data_s.cfg.io._key_section
+    sec_default = data_s.cfg.def_sect
+    sec_simple = 'IO'
+    sec_profile1 = 'profile1'
+    sec_profile2 = 'Profile 2'
+
+    # Section values
+    val_internal = {'profile': repr(sec_default)} | {'fields': "{'profile1': ('C4',)}"}
+    val_default = {'C4': '4'}
+    val_modified = {'C4': '10'}
+
+    # Prepare profiles config data
+    data_p = Config4(io=True, profiles=True)
+    data_p.C4 = 10
+    data_p.cfg.profiles.set(sec_profile1, val_default, typecast=True, defaults=False)
+    data_p.cfg.profiles.set(sec_profile2)
+    ecp = data_p.cfg.io.export_config
+
+    # Internal section completed
+    ip_ = {sec_internal: val_internal}
+
+    # Default sections completed
+    ds_ = {sec_default: {}}
+    dp_ = {sec_default: val_modified}
+    dss = {sec_default: exp_strict | val_default}
+    dps = {sec_default: exp_strict | val_modified}
+
+    # Simple config section completed
+    vs_ = {sec_simple: val_modified}
+    vss = {sec_simple: exp_strict | val_modified}
+
+    # Profiles config section completed
+    vp_1 = {sec_profile1: val_default}
+    vp_2 = {sec_profile2: {}}
+    vps2 = {sec_profile2: exp_strict | val_modified}
+
+    # Exceptions
+    exc_ie = partial(InputError, 'profiles', func_name='Config4.cfg.io.export_config()')
+    msg_disabled = "Profiles disabled, but provided"
+    msg_extra = ("Extra profile: ''. "
+                 "Must be not more than expected ('profile1', 'Profile 2'), but received: ''")
+
+    def fmt_cte(section, value):
+        inner_exc = CheckTypeError(f'Field {value} (int) must be str type')
+        return IOExportError(f"Cannot export 'IO' config section {section!r}. Errors:\n"
+                             f"\tField C4={value} (int) by <lambda>: {inner_exc!r}")
+
+    # Build subtest dataset
+    profiles_set = [None, '', sec_profile1, [sec_profile1], [sec_profile1, sec_profile2]]
+    cases = product(profiles_set, *((False, True),) * 3)
+    names = ('profiles', 'strict_defaults', 'strict_data', 'typecast')
+
+    # Run subtest
+    for i, profiles, s_def, s_data, typecast in (st := subtest('', 40, cases, names=names)):
+        kwargs = dict(zip(names[1:], (s_def, s_data, typecast), strict=True))
+
+        # Prepare simple result
+        if profiles is None:
+            if typecast:
+                rs = (dss if s_def else ds_) | (vss if s_data else vs_)
+            else:
+                rs = fmt_cte(sec_default, 4) if s_def else fmt_cte(sec_simple, 10)
+        else:
+            rs = exc_ie(msg=f'{msg_disabled}: {profiles!r}')
+
+        # Prepare profiles result
+        if not typecast:
+            rp = fmt_cte(sec_default, 10)
+        elif profiles == '':
+            rp = exc_ie(msg=msg_extra)
+        else:
+            rp = ip_ | (dps if s_def else dp_)
+            if profiles is None or sec_profile1 in profiles:
+                rp |= vp_1
+            if profiles is None or sec_profile2 in profiles:
+                rp |= (vps2 if s_data else vp_2)
+
+        # Test both
+        for name, target, result in (('simple', ecs, rs), ('profiles', ecp, rp)):
+            if any(map(is_exception, results := as_holder(result))):
+                try:
+                    raises(result, target, profiles, **kwargs)
+                except Exception as e:
+                    st.send(('', type(e).__name__, results[0]))
+                else:
+                    st.send((f'Exception {name}', results[0], results[0]))
+            else:
+                st.send((f'Result {name}', safe(target, profiles, **kwargs), result))
+
+
+def test_import_field():
+    wfn = 'v_not_exists'                # Wrong field name
+    wev = 'wrong value'                 # Wrong eval value
+    wrv = WrongReprType()               # Wrong repr value
+    wcv = "'wrong value'"               # Wrong custom value
+    cfn = 'v_list'                      # Correct field name
+    ccv = "[{'s': 4}, 1, 0.7, 'data']"  # Correct custom value
+    ccr = [{'s': 4}, 1, 0.7, 'data']    # Correct custom result
+
+    # Correct
+    cfg = Config1(io=True).cfg
+    import_field = cfg.io.import_field
+    assert import_field(cfn, ccv) == ccr
+    assert import_field(cfn, ccv, True) == ccr
+    assert import_field(cfn, ccv, False) == ccr
+
+    exp_f_std = ['False', "'Some string'", '65535', '3.1415', "b'Some bytes'", '(1, 2, 3, None)',
+                 "[-1, 0, 1, 'repeat']", "{'first'}", "{1: 'one', 2: 'two'}"]
+    exp_f_safe = ["'something'", '2custom', '8']
+
+    imp_f_std = [False, 'Some string', 65535, 3.1415, b'Some bytes',  (1, 2, 3, None),
+                 [-1, 0, 1, 'repeat'], {'first'}, {1: 'one', 2: 'two'}]
+    imp_f_safe = ['something', 2, 8]
+
+    names_safe = ['v_cust2', 'v_cust3', '_internal']
+
+    exp_dict = dict(zip(cfg.get_fields, exp_f_std + ['5'] + exp_f_safe))
+    imp_list = imp_f_std + [OwnInt(5)] + imp_f_safe
+
+    exp_dict_safe = dict(zip(cfg.get_fields, exp_f_std)) | dict(zip(names_safe, exp_f_safe))
+    imp_list_safe = imp_f_std + imp_f_safe
+
+    assert [import_field(k, v) for k, v in exp_dict.items()] == imp_list
+    assert [import_field(k, v, True) for k, v in exp_dict.items()] == imp_list
+    assert [import_field(k, v, False) for k, v in exp_dict_safe.items()] == imp_list_safe
+
+    # Errors
+    exc_field = partial(FieldError, 'Import', cfg.name)
+
+    exc1 = CheckTypeError('Field 5 (int) must be OwnInt type')
+    exc1f = exc_field('v_cust1', from_value='5', by_func='literal_eval', reason=repr(exc1))
+    raises((exc1f, exc1), import_field, 'v_cust1', '5', False)
+
+    exc2 = KeyError(wfn)
+    exc2f = exc_field(wfn, from_value=ccv, reason=repr(exc2))
+    raises((exc2f, exc2), import_field, wfn, ccv)
+
+    exc3 = SyntaxError('invalid syntax', ('<unknown>', 1, 7, wev, 1, 12))
+    exc3f = exc_field(cfn, from_value=wev, by_func='literal_eval', reason=repr(exc3))
+    raises((exc3f, exc3), import_field, cfn, wev)
+
+    exc4 = TypeError("__repr__ returned non-string (type WrongReprType)")
+    exc4f = exc_field(cfn, from_value=wrv, by_func='literal_eval', reason=repr(exc4))
+    raises((exc4f, exc4), import_field, cfn, wrv)
+
+    exc5 = CheckTypeError("Field 'wrong value' (str) must be list type")
+    exc5f = exc_field(cfn, from_value=wcv, by_func='literal_eval', reason=repr(exc5))
+    raises((exc5f, exc5), import_field, cfn, wcv, typecast=False)
+
+
+def test_import_section():
+    exp = exp_strict
+    exp2 = exp.copy()
+    exp2['v_bool'] = 'True'
+
+    # i1_, i1m = {'v_bool': 'False'}, {'v_bool': 'True'}
+    # o1_, o1m = {'v_bool': False}, {'v_bool': True}
+    i2m = {'v_int': '32767'}
+    o2m = {'v_int': 32767}
+
+    imp = imp_strict
+    imp2 = imp.copy()
+    imp2['v_bool'] = True
+
+    cfg_s = Config1(io=True).cfg
+    cfg_p = Config1(io=True, profiles=True).cfg
+    iss = cfg_s.io.import_section
+    isp = cfg_p.io.import_section
+
+    # Not change data in configs (single and profile)
+    assert iss(i2m) == isp(i2m) == o2m
+    assert cfg_s.get_data == cfg_p.get_data == cfg_s.get_defaults == cfg_p.get_defaults == imp
+
+    assert iss(exp) == isp(exp) == imp
+    assert cfg_s.get_data == cfg_p.get_data == cfg_s.get_defaults == cfg_p.get_defaults == imp
+
+    assert iss(exp2) == isp(exp2) == imp2
+    assert cfg_s.get_data == cfg_p.get_data == cfg_s.get_defaults == cfg_p.get_defaults == imp
+
+    # Change data in configs (single)
+    pass  # Not implemented
+
+    # Change data in configs (profile)
+    pass  # Not implemented
+
+    # Errors
+    def names(target):
+        return repr(tuple(target))[1:-1]
+
+    add = f"Must be not more than expected ({names(cfg_s.get_fields)}), but received"
+
+    ef1 = {'wrong_name': 'wrong_data'}
+    ef2 = {'some_name': 'some_data'}
+    ef3 = {'v_int': 13}
+    ef4 = {'v_dict': 1}
+
+    ie = "Provided wrong parameter to Config1.cfg.io.import_section(): raw_section. "
+    ie1 = "[[]] (list) must be Mapping type"
+    ie2 = f"Extra field: 'wrong_name'. {add}: {names(exp | ef1)}"
+    ie3 = f"Extra fields: 'wrong_name', 'some_name'. {add}: {names(exp | ef1 | ef2)}"
+    ie4 = f"Extra fields: 'wrong_name', 'some_name'. {add}: {names(exp | ef1 | ef2 | ef3 | ef4)}"
+    raises(InputError(msg=ie + ie1), iss, [[]])
+    raises(InputError(msg=ie + ie1), isp, [[]])
+    raises(InputError(msg=ie + ie2), iss, exp | ef1)
+    raises(InputError(msg=ie + ie2), isp, exp | ef1)
+    raises(InputError(msg=ie + ie3), iss, exp | ef1 | ef2)
+    raises(InputError(msg=ie + ie3), isp, exp | ef1 | ef2)
+    raises(InputError(msg=ie + ie4), iss, exp | ef1 | ef2 | ef3 | ef4)
+    raises(InputError(msg=ie + ie4), isp, exp | ef1 | ef2 | ef3 | ef4)
+
+    msg = "Cannot import 'Config1' config section"
+    p1 = "Field v_int=13 (int) by literal_eval: ValueError('malformed node or string: 13')"
+    p2 = "Field v_dict=1 (int) by literal_eval: ValueError('malformed node or string: 1')"
+    raises(IOImportError(msg + f". Errors:\n\t{p1}"), iss, exp | ef3)
+    raises(IOImportError(msg + f". Errors:\n\t{p1}"), isp, exp | ef3)
+    raises(IOImportError(msg + f". Errors:\n\t{p1}\n\t{p2}"), iss, exp | ef3 | ef4)
+    raises(IOImportError(msg + f". Errors:\n\t{p1}\n\t{p2}"), isp, exp | ef3 | ef4)
+
+
+def test_import_config():
+    # Prepare simple and profiles configs
+    data_s = Config4(io=True)
+    data_p = Config4(io=True, profiles=True)
+    ics = data_s.cfg.io.import_config
+    icp = data_p.cfg.io.import_config
+    df = exp_strict | {'C4': '4'}                       # default fields
+
+    # Internal section keys
+    kiv = data_s.cfg.io._key_version
+    kip = data_s.cfg.io._key_profile
+    kif = data_s.cfg.io._key_fields
+
+    # Values
+    e1m, i1m = {'v_bool': 'True'}, {'v_bool': True}
+    e2_ = {'v_int': '65535'}
+    e2m, i2m = {'v_int': '32767'}, {'v_int': 32767}
+
+    # Sections names
+    internal = data_s.cfg.io._key_section
+    default_ = data_s.cfg.def_sect
+    simple__ = 'IO'
+    profile_ = 'p1'
+
+    # Exported values
+    ev_d_ = e2m                                                 # default
+    ev_s_ = e1m | e2_                                           # simple
+    ev_p_ = ev_s_ | ev_d_                                       # profile
+    ev_f_ = e1m                                                 # fields active
+    ev_id = {kip: repr(default_)}                               # internal default
+    ev_ip = {kip: repr(profile_)}                               # internal profile
+    ev_if = {kip: repr(profile_), kif: "{'p1': ('v_bool',)}"}   # internal fields (profiles active)
+
+    # 1. Exported Simple
+    s___ed_ = {default_: {} | ev_d_}                            # default
+    s___eds = {default_: df | ev_d_}                            # default strict
+    s___es_ = {simple__: {} | ev_s_}                            # section
+    s___ess = {simple__: df | ev_s_}                            # section strict
+
+    # 2. Exported Profiles: default
+    pd__ed_ = {internal: ev_id, default_: {} | ev_p_}           # default
+    pd__eds = {internal: ev_id, default_: df | ev_p_}           # default strict
+    pd__es_ = {}                                                # section
+    pd__ess = {}                                                # section strict
+
+    # 3. Exported Profiles: default, active fields
+    # The same as 2, because default profile always have all fields active
+
+    # 4. Exported Profiles: profile
+    pp__ed_ = {internal: ev_ip, default_: {} | ev_d_}           # default
+    pp__eds = {internal: ev_ip, default_: df | ev_d_}           # default strict
+    pp__es_ = {profile_: {} | ev_s_}                            # section
+    pp__ess = {profile_: df | ev_s_}                            # section strict
+
+    # 5. Profiles: profile, active fields
+    ppa_ed_ = {internal: ev_if, default_: {} | ev_d_}           # default
+    ppa_eds = {internal: ev_if, default_: df | ev_d_}           # default strict
+    ppa_es_ = {profile_: {} | ev_f_}                            # section
+
+    # Typecast error
+    e1 = CheckTypeError('Field 5 (int) must be OwnInt type')
+    e2 = CheckTypeError("Field '4' (str) must be int type")
+    msg = ("Cannot import 'IO' config section {!r}. Errors:\n"
+           f"\tField v_cust1='5' (str) by literal_eval: {e1!r}\n"
+           f"\tField C4='4' (str) by <lambda>: {e2!r}")
+
+    def import_and_compare_configs(**kwargs):
+        nonlocal k
+        k += 1
+        i_data = Config4(io=True, profiles=profiles)
+        i_data.cfg.io.import_config(data, **kwargs)
+        assert e_data.cfg.get_data == i_data.cfg.get_data
+        assert e_data.cfg.get_defaults == i_data.cfg.get_defaults
+        if profiles:
+            assert e_data.cfg.profiles.get == i_data.cfg.profiles.get
+            assert e_data.cfg.profiles.active == i_data.cfg.profiles.active
+            assert e_data.cfg.profiles.active_fields == i_data.cfg.profiles.active_fields
+        assert data == i_data.cfg.io.export_config(strict_defaults=bd, strict_data=bv)
+
+    # Correct
+    i = j = k = 0
+    section = defaults = bd = bv = data = None
+    try:
+        for i, (section, defaults, d_, ds, s_, ss) in enumerate([
+            (simple__, None,  s___ed_, s___eds, s___es_, s___ess),
+            (default_, True,  pd__ed_, pd__eds, pd__es_, pd__ess),
+            (default_, False, pd__ed_, pd__eds, pd__es_, pd__ess),
+            (profile_, True,  pp__ed_, pp__eds, pp__es_, pp__ess),
+            (profile_, False, ppa_ed_, ppa_eds, ppa_es_, ppa_es_)
+        ], 1):
+            # Prepare source config
+            if profiles := section != simple__:
+                e_data = Config4(io=True, profiles=True)
+                e_data.cfg.profiles.set(section, i1m, defaults=defaults)
+                e_data.cfg.profiles.set(default_, i2m)
+                e_data.cfg.profiles.switch(section)
+            else:
+                e_data = Config4(io=True)
+                e_data.cfg.set_fields(i1m)
+                e_data.cfg.set_defaults(i2m)
+
+            # Check source config and target configs for equality
+            tests = product([(False, d_), (True, ds)], [(False, s_), (True, ss)])
+            for j, ((bd, sd), (bv, sv)) in enumerate(tests, 1):
+                # Export
+                k, data = 0, sd | sv
+                assert data == e_data.cfg.io.export_config(strict_defaults=bd, strict_data=bv)
+
+                # Import
+                dd, dv = data.get(default_, ()), data.get(section, {})
+                if (dd := 'C4' in dd) or 'C4' in dv:
+                    k = 1
+                    i1 = Config4(io=True, profiles=profiles)
+                    raises(IOImportError(msg.format(default_ if dd else section)),
+                           i1.cfg.io.import_config, data, typecast=False)
+                else:
+                    import_and_compare_configs(typecast=False)
+                import_and_compare_configs(typecast=True)
+                import_and_compare_configs(sections=(default_, section))
+
+    except Exception as e:
+        raise AssertionError(f"Correct import test failed at {i}.{j}.{k}: "
+                             f"{section=}, {defaults=}, {bd=}, {bv=}, \n{data=}") from e
+
+    # Errors
+
+    # For version errors only
+    with (cfg_v := Config4(io=True).cfg):
+        cfg_v.version = '0.1'
+    icv = cfg_v.io.import_config
+
+    # Valid params
+    vpp = {kip: repr(default_)}
+    vpf = {kif: "{'p1': ('v_str', 'v_int')}"}
+
+    # Valid sections
+    vs_is = {internal: vpp}
+    vs_ip = {internal: vpp | vpf}
+    vsd = {default_: {}}
+    vsp = {'p1': {'v_str': '123', 'v_int': '5'}}
+
+    def names(target):
+        return repr(tuple(target))[1:-1]
+
+    # Input errors
+    ie = "Provided wrong parameter to Config4.cfg.io.import_config()"
+    add = "Must be not more than expected ({}), but received: {}"
+    add2 = add.format("'DEFAULT'", "'Some'")
+    add3 = add.format(names(cfg_v.get_fields), "'wrong'")
+    add4 = add.format(names(cfg_v.get_fields), "'v_bool', 'wrong'")
+
+    exc1 = TypeError("'int' object is not iterable")
+    exc2 = SyntaxError('invalid syntax', ('<unknown>', 0, 0, '', 0, 0))
+    exc3 = TypeError('cannot convert dictionary update sequence element #0 to a sequence')
+
+    ies = f"{ie}: sections. Extra section: 'Some'. {add}"      # sections
+    ie_s1 = InputError(msg=ies.format("'IO'", "'Some'"))
+    ie_s2 = InputError(msg=ies.format("'IO'", "'IO', 'Some'"))
+    ie_s3 = InputError(msg=ies.format("'p1'", "'Some'"))
+    ie_s4 = InputError(msg=ies.format("'p1', '1', '2'", "'Some'"))
+
+    ci_p = "is not needed, but provided"                        # check_input provided error
+    ci_n = "is needed, but not provided"                        # check_input needed error
+    af_p = "Active fields dict is not parsed"                   # active_fields parsing
+    af_e = f"Extra active fields profile: 'Some'. {add2}"       # active_fields extra
+    afke = f"Extra 'p1' profile active field: 'wrong'. {add3}"  # active_fields extra
+    df_e = f"Extra default field: 'wrong'. {add4}"              # default field extra
+
+    ier = f"{ie}: raw_config."                                  # raw_config
+    msg_r14 = (f"{ier} Extra 'p1' profile field: 'v_bool'. Absent 'p1' profile field: 'v_str'. "
+               "Must be equal to expected ('v_str', 'v_int'), but received: 'v_bool', 'v_int'")
+    ie_r01 = InputError(msg=f"{ier} {internal!r} section {ci_p}")
+    ie_r02 = InputError(msg=f"{ier} {internal!r} section {ci_n}")
+    ie_r03 = InputError(msg=f"{ier} {kiv.capitalize()} {ci_p}")
+    ie_r04 = InputError(msg=f"{ier} {kiv.capitalize()} {ci_n}")
+    # ie_r05 = InputError(msg=f"{ier} {kip.capitalize()} {ci_p}")                 waits for version
+    ie_r06 = InputError(msg=f"{ier} {kip.capitalize()} {ci_n}")
+    ie_r07 = InputError(msg=f"{ier} Active profile is not provided: 'Some'")
+    ie_r08 = (InputError(msg=f"{ier} {af_p}: '1'"), exc1)
+    ie_r09 = (InputError(msg=f"{ier} {af_p}: ''"), exc2)
+    ie_r10 = (InputError(msg=f"{ier} {af_p}: '[1]'"), exc3)
+    ie_r11 = InputError(msg=f"{ier} {af_e}")
+    ie_r12 = InputError(msg=f"{ier} {afke}")
+    ie_r13 = InputError(msg=f"{ier} {df_e}")
+    ie_r14 = InputError(msg=msg_r14)
+
+    raises(ie_s1, ics, {}, 'Some')
+    raises(ie_s2, ics, {}, ('IO', 'Some'))
+    raises(ie_s3, icp, vs_ip | vsp, 'Some')
+    raises(ie_s4, icp, vs_ip | vsp | {'1': {}, '2': {}}, 'Some')
+
+    raises(ie_r01, ics, {internal: {}})
+    raises(ie_r02, icp, {})
+    raises(ie_r03, icp, {internal: {kiv: ''}})
+    raises(ie_r04, icv, {internal: {}})
+    # raises(ie_r05, icv, {internal: {kiv: '', kip: ''}})                         waits for version
+    raises(ie_r06, icp, {internal: {}})
+    raises(ie_r07, icp, {internal: {kip: "'Some'"}})
+    raises(ie_r08, icp, {internal: vpp | {kif: '1'}} | vsd)
+    raises(ie_r09, icp, {internal: vpp | {kif: ''}} | vsd)
+    raises(ie_r10, icp, {internal: vpp | {kif: '[1]'}} | vsd)
+    raises(ie_r11, icp, {internal: vpp | {kif: "{'Some': ('v_str',)}"}} | vsd)
+    raises(ie_r12, icp, {internal: vpp | {kif: "{'p1': ('wrong',)}"}} | vsd | vsp)
+    raises(ie_r13, ics, {default_: {'v_bool': True, 'wrong': True}})
+    raises(ie_r13, icp, {default_: {'v_bool': True, 'wrong': True}} | vs_is)
+    raises(ie_r14, icp, vs_ip | vsd | {'p1': {'v_bool': 'True', 'v_int': '1'}})
+
+    # IOImport Errors
+    msg = "Cannot import 'IO' config. "
+    exc4 = NotImplementedError('Version import is not available yet')
+    tmpl = ("Cannot import 'IO' config section {!r}. Errors:\n\tField v_bool=True (bool)"
+            " by literal_eval: ValueError('malformed node or string: True')")
+
+    raises((IOImportError(msg + repr(exc4)), exc4), icv, {internal: {kiv: ''}})
+    raises(IOImportError(tmpl.format(default_)), ics, {default_: {'v_bool': True}})
+    raises(IOImportError(tmpl.format(default_)), icp, {default_: {'v_bool': True}} | vs_is)
+    raises(IOImportError(tmpl.format(simple__)), ics, {simple__: {'v_bool': True}})
+    raises(IOImportError(tmpl.format('Some1')), icp, {'Some1': {'v_bool': True}} | vs_is | vsd)
```

### Comparing `configlayer-0.1/tests/test_7_file.py` & `configlayer-0.1.1/tests/test_7_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,151 +1,149 @@
-from gc import collect
-from pathlib import Path
-from itertools import product
-
-from configlayer.exceptions import InitError, FileError, IOImportError, InputError
-
-from _utilities import raises_init, subtest
-from _data import Config1, Config1Alias, Config2, Config3, Config4, exp_strict
-
-
-TEMP_PATH = Path('_file_data\\temp_config.ini')
-
-
-def test_init():
-    collect()
-
-    # Create config with wrong file path
-    wrong_path = 'not_exists_dir/test_config.ini'
-    fe = FileError("Save to \"not_exists_dir\\test_config.ini\" failed. No such file or directory")
-    raises_init(fe, Config2, wrong_path)
-
-    # Create config, must be no file created
-    TEMP_PATH.unlink(missing_ok=True)
-    data = Config1(TEMP_PATH)
-    assert not TEMP_PATH.exists()
-
-    # Several configs at single file check
-    ie = InitError("Path \"_file_data\\temp_config.ini\" is already used in 'Config1' config")
-    raises_init(ie, Config1, TEMP_PATH)
-    raises_init(ie, Config2, TEMP_PATH)
-
-    # Remove config from memory to free temp path for other configs
-    data.cfg.file.save()
-    del data
-    collect()
-
-    # Import file at temp path from other config
-    ke = KeyError('Valid fields')
-    ie = IOImportError(f"Cannot import 'Valid fields' config. {ke!r}")
-    fe = FileError(f"Load from \"_file_data\\temp_config.ini\" failed. {ie!r}")
-    raises_init((fe, ie, ke), Config2, TEMP_PATH)
-
-
-def test_save():
-    collect()
-
-    sect_name = 'Config1'
-    defaults = {'v_str': "'mod'"}
-    def_data = {'v_bool': 'True', 'v_str': "'Some string'"}
-    for (profiles, ud), bd, bv in product([(False, True), (True, True), (True, False)],
-                                                    [False, True], [False, True]):
-        TEMP_PATH.unlink(missing_ok=True)
-        data = Config1(TEMP_PATH, profiles=bool(profiles))
-        if profiles:
-            data.cfg.profiles.set(sect_name, {'v_bool': False}, defaults=ud)
-            data.cfg.profiles.switch(sect_name)
-        data.v_bool = True
-        data.cfg.set_defaults({'v_str': 'mod'})
-
-        data.cfg.file.save(strict_defaults=bd, strict_data=bv)
-        result = []
-
-        # Internal section in file
-        if profiles:
-            result.extend((f'[{data.cfg.io._key_section}]', f'profile = {sect_name!r}'))
-            if not ud:
-                result.append("fields = {'Config1': ('v_bool',)}")
-            result.append('')
-
-        # Default section in file
-        result.append('[DEFAULT]')
-        result.extend(f'{k} = {v}' for k, v in ((exp_strict if bd else {}) | defaults).items())
-
-        # Data section in file
-        result.extend(('', f'[{sect_name}]'))
-        if ud:
-            result.extend(f'{k} = {v}' for k, v in ((exp_strict if bv else {}) | def_data).items())
-        else:
-            result.append("v_bool = True")
-
-        assert TEMP_PATH.read_text().rstrip() == '\n'.join(result)
-
-        del data
-        collect()
-
-
-def test_load():
-    collect()
-
-    # Get simple and profiles test files paths separately
-    sp, pp = [], []
-    [(sp if '_s' in x.name else pp).append(x) for x in TEMP_PATH.parent.glob('test_config_*.ini')]
-
-    # Get all available configs
-    cfgs = (Config1, Config1Alias, Config2, Config3, Config4)
-
-    # Wrong files check
-    def fmt_exc(fp, exc):
-        if isinstance(exc, Exception):
-            return FileError(f'Load from "{fp}" failed. {exc!r}'), exc
-        return FileError(f'Load from "{fp}" failed. {exc}')
-
-    wsp = TEMP_PATH.with_name('test_wrong_s.ini')
-    ds = "'_DEFAULT' section is forbidden, but provided"
-    raises_init(fmt_exc(wsp, ds), Config1, wsp, profiles=False)
-
-    wpp = TEMP_PATH.with_name('test_wrong_p.ini')
-    dsv = ds + ". Data: {'some key': \"'some value'\"}"
-    raises_init(fmt_exc(wpp, dsv), Config1, wpp, profiles=True)
-
-    def fmt_ie(cls, provided=False):
-        args =  ('', ' not') if provided else (' not', '')
-        return InputError('raw_config', func_name=f'{cls.__name__}.cfg.io.import_config()',
-                          msg="'_CONFIG_LAYER' section is{} needed, but{} provided".format(*args))
-
-    [raises_init(fmt_exc(p, fmt_ie(c)), c, p, profiles=False) for c, p, in product(cfgs, pp)]
-    [raises_init(fmt_exc(p, fmt_ie(c, True)), c, p, profiles=True) for c, p, in product(cfgs, sp)]
-
-    # Check simple
-    se = (({}, {}),
-          ({'v_bool': True}, {'v_str': 'Some', 'v_int': 5}),
-          ({}, {'v_int': 5}),
-          ({'v_int': 5}, {'c3': 'c5'}),
-          ({'v_str': 'some str', 'C4': 1}, {'C4': 44}))
-    dataset = zip(cfgs, sp, se, strict=True)
-    for i, cfg_cls, path, (ed, ef) in (st := subtest('Simple', 5, dataset)):
-        data = cfg_cls(path)
-        defaults = data.cfg.get_factory_defaults | ed
-        st.send(('defaults', data.cfg.get_defaults, defaults))
-        st.send(('data', data.cfg.get_data, defaults | ef))
-
-    # Check profiles
-    pe = (('DEFAULT', {}, {}),
-          ('DEFAULT', {}, {'config_2': {}}),
-          ('config_3', {'v_bool': True}, {'config_3': {'v_str': 'Some', 'v_int': 5}}),
-          ('config_4', {'v_bool': True}, {'config_4': {'v_str': 'Some', 'v_int': 5}}))
-    dataset = product(cfgs, zip(pp, pe, strict=True))
-    for i, cfg_cls, (path, (active, ed, ep)) in (st := subtest('Profiles', 20, dataset)):
-        data = cfg_cls(path, profiles=True)
-        dp = data.cfg.profiles
-
-        defaults = data.cfg.get_factory_defaults | ed
-        st.send(('defaults', data.cfg.get_defaults, defaults))
-        st.send(('data', data.cfg.get_data, defaults | ep.get(dp.active, {})))
-        st.send(('active', dp.active, active))
-        profiles = {k: v if active == 'config_4' else tuple((defaults | v).values())
-                    for k, v in ep.items()}
-        st.send(('profiles', dp._profiles, profiles))
-
-        del data
-        collect()
+from gc import collect
+from itertools import product
+from pathlib import Path
+
+from configlayer.exceptions import InitError, FileError, IOImportError, InputError
+
+from _utilities import raises_init, subtest
+from _data import TEMP_PATH, Config1, Config1Alias, Config2, Config3, Config4, exp_strict
+
+
+def test_init():
+    collect()
+
+    # Create config with wrong file path
+    wrong_path = 'not_exists_dir/test_config.ini'
+    fe = FileError(f'Save to "{Path(wrong_path)}" failed. No such file or directory')
+    raises_init(fe, Config2, wrong_path)
+
+    # Create config, must be no file created
+    TEMP_PATH.unlink(missing_ok=True)
+    data = Config1(TEMP_PATH)
+    assert not TEMP_PATH.exists()
+
+    # Several configs at single file check
+    ie = InitError(f"Path \"{TEMP_PATH}\" is already used in 'Config1' config")
+    raises_init(ie, Config1, TEMP_PATH)
+    raises_init(ie, Config2, TEMP_PATH)
+
+    # Remove config from memory to free temp path for other configs
+    data.cfg.file.save()
+    del data
+    collect()
+
+    # Import file at temp path from other config
+    ke = KeyError('Valid fields')
+    ie = IOImportError(f"Cannot import 'Valid fields' config. {ke!r}")
+    fe = FileError(f"Load from \"{TEMP_PATH}\" failed. {ie!r}")
+    raises_init((fe, ie, ke), Config2, TEMP_PATH)
+
+
+def test_save():
+    collect()
+
+    sect_name = 'Config1'
+    defaults = {'v_str': "'mod'"}
+    def_data = {'v_bool': 'True', 'v_str': "'Some string'"}
+    for (profiles, ud), bd, bv in product([(False, True), (True, True), (True, False)],
+                                          [False, True],
+                                          [False, True]):
+        TEMP_PATH.unlink(missing_ok=True)
+        data = Config1(TEMP_PATH, profiles=bool(profiles))
+        if profiles:
+            data.cfg.profiles.set(sect_name, {'v_bool': False}, defaults=ud)
+            data.cfg.profiles.switch(sect_name)
+        data.v_bool = True
+        data.cfg.set_defaults({'v_str': 'mod'})
+
+        data.cfg.file.save(strict_defaults=bd, strict_data=bv)
+        result = []
+
+        # Internal section in file
+        if profiles:
+            result.extend((f'[{data.cfg.io._key_section}]', f'profile = {sect_name!r}'))
+            if not ud:
+                result.append("fields = {'Config1': ('v_bool',)}")
+            result.append('')
+
+        # Default section in file
+        result.append('[DEFAULT]')
+        result.extend(f'{k} = {v}' for k, v in ((exp_strict if bd else {}) | defaults).items())
+
+        # Data section in file
+        result.extend(('', f'[{sect_name}]'))
+        if ud:
+            result.extend(f'{k} = {v}' for k, v in ((exp_strict if bv else {}) | def_data).items())
+        else:
+            result.append("v_bool = True")
+
+        assert TEMP_PATH.read_text().rstrip() == '\n'.join(result)
+
+        del data
+        collect()
+
+
+def test_load():
+    collect()
+
+    # Get simple and profiles test files paths separately
+    sp, pp = [], []
+    [(sp if '_s' in x.name else pp).append(x) for x in TEMP_PATH.parent.glob('test_config_*.ini')]
+
+    # Get all available configs
+    cfgs = (Config1, Config1Alias, Config2, Config3, Config4)
+
+    # Wrong files check
+    def fmt_exc(fp, exc):
+        if isinstance(exc, Exception):
+            return FileError(f'Load from "{fp}" failed. {exc!r}'), exc
+        return FileError(f'Load from "{fp}" failed. {exc}')
+
+    wsp = TEMP_PATH.with_name('test_wrong_s.ini')
+    ds = "'_DEFAULT' section is forbidden, but provided"
+    raises_init(fmt_exc(wsp, ds), Config1, wsp, profiles=False)
+
+    wpp = TEMP_PATH.with_name('test_wrong_p.ini')
+    dsv = ds + ". Data: {'some key': \"'some value'\"}"
+    raises_init(fmt_exc(wpp, dsv), Config1, wpp, profiles=True)
+
+    def fmt_ie(cls, provided=False):
+        args = ('', ' not') if provided else (' not', '')
+        return InputError('raw_config', func_name=f'{cls.__name__}.cfg.io.import_config()',
+                          msg="'_CONFIG_LAYER' section is{} needed, but{} provided".format(*args))
+
+    [raises_init(fmt_exc(p, fmt_ie(c)), c, p, profiles=False) for c, p, in product(cfgs, pp)]
+    [raises_init(fmt_exc(p, fmt_ie(c, True)), c, p, profiles=True) for c, p, in product(cfgs, sp)]
+
+    # Check simple
+    se = (({}, {}),
+          ({'v_bool': True}, {'v_str': 'Some', 'v_int': 5}),
+          ({}, {'v_int': 5}),
+          ({'v_int': 5}, {'c3': 'c5'}),
+          ({'v_str': 'some str', 'C4': 1}, {'C4': 44}))
+    dataset = zip(cfgs, sp, se, strict=True)
+    for i, cfg_cls, path, (ed, ef) in (st := subtest('Simple', 5, dataset)):
+        data = cfg_cls(path)
+        defaults = data.cfg.get_factory_defaults | ed
+        st.send(('defaults', data.cfg.get_defaults, defaults))
+        st.send(('data', data.cfg.get_data, defaults | ef))
+
+    # Check profiles
+    pe = (('DEFAULT', {}, {}),
+          ('DEFAULT', {}, {'config_2': {}}),
+          ('config_3', {'v_bool': True}, {'config_3': {'v_str': 'Some', 'v_int': 5}}),
+          ('config_4', {'v_bool': True}, {'config_4': {'v_str': 'Some', 'v_int': 5}}))
+    dataset = product(cfgs, zip(pp, pe, strict=True))
+    for i, cfg_cls, (path, (active, ed, ep)) in (st := subtest('Profiles', 20, dataset)):
+        data = cfg_cls(path, profiles=True)
+        dp = data.cfg.profiles
+
+        defaults = data.cfg.get_factory_defaults | ed
+        st.send(('defaults', data.cfg.get_defaults, defaults))
+        st.send(('data', data.cfg.get_data, defaults | ep.get(dp.active, {})))
+        st.send(('active', dp.active, active))
+        profiles = {k: v if active == 'config_4' else tuple((defaults | v).values())
+                    for k, v in ep.items()}
+        st.send(('profiles', dp._profiles, profiles))
+
+        del data
+        collect()
```

