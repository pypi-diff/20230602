# Comparing `tmp/hj-generate-3.0.0.tar.gz` & `tmp/hj-generate-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-3.0.0.tar", last modified: Fri Jun  2 00:37:07 2023, max compression
+gzip compressed data, was "hj-generate-3.1.0.tar", last modified: Fri Jun  2 00:40:23 2023, max compression
```

## Comparing `hj-generate-3.0.0.tar` & `hj-generate-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:37:07.647134 hj-generate-3.0.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-02 00:37:07.646818 hj-generate-3.0.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:37:07.641287 hj-generate-3.0.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-3.0.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     2999 2023-06-01 15:17:39.000000 hj-generate-3.0.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:37:07.644127 hj-generate-3.0.0/generate/templates/
--rw-r--r--   0 hj         (501) staff       (20)      461 2023-06-01 15:19:37.000000 hj-generate-3.0.0/generate/templates/controller.tpl
--rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-3.0.0/generate/templates/service.tpl
--rw-r--r--   0 hj         (501) staff       (20)      111 2023-06-01 15:20:28.000000 hj-generate-3.0.0/generate/templates/sql.tpl
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:37:07.646408 hj-generate-3.0.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-02 00:37:07.000000 hj-generate-3.0.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-02 00:37:07.000000 hj-generate-3.0.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-02 00:37:07.000000 hj-generate-3.0.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-02 00:37:07.000000 hj-generate-3.0.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-02 00:37:07.000000 hj-generate-3.0.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-02 00:37:07.000000 hj-generate-3.0.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-02 00:37:07.647289 hj-generate-3.0.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-02 00:36:47.000000 hj-generate-3.0.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:40:23.016967 hj-generate-3.1.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-02 00:40:23.016645 hj-generate-3.1.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:40:23.013603 hj-generate-3.1.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-3.1.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     2977 2023-06-02 00:40:20.000000 hj-generate-3.1.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:40:23.014551 hj-generate-3.1.0/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      461 2023-06-01 15:19:37.000000 hj-generate-3.1.0/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-3.1.0/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      111 2023-06-01 15:20:28.000000 hj-generate-3.1.0/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-02 00:40:23.016259 hj-generate-3.1.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-02 00:40:22.000000 hj-generate-3.1.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-02 00:40:22.000000 hj-generate-3.1.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-02 00:40:22.000000 hj-generate-3.1.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-02 00:40:22.000000 hj-generate-3.1.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-02 00:40:22.000000 hj-generate-3.1.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-02 00:40:22.000000 hj-generate-3.1.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-02 00:40:23.017064 hj-generate-3.1.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-02 00:40:20.000000 hj-generate-3.1.0/setup.py
```

### Comparing `hj-generate-3.0.0/generate/generate_code.py` & `hj-generate-3.1.0/generate/generate_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
     # controller
     controller_template = env.get_template('controller.tpl')
 
     controller_output = controller_template.render(data)
 
     co_append = """
-from controllers.{{name}}_controller import {{name}}_controller
-blueprint_list.append({{name}}_controller)
+from controllers.{{name}}_controller import {{name}}
+blueprint_list.append({{name}})
             """
     co_str_temp = env.from_string(co_append)
 
     # 追加
     with open('./controllers' + os.sep + '__init__.py', 'a') as f:
         f.write(co_str_temp.render(data))
```

