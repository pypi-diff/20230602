# Comparing `tmp/num_tini4-0.0.1a3.tar.gz` & `tmp/num_tini4-0.0.1a4.tar.gz`

## Comparing `num_tini4-0.0.1a3.tar` & `num_tini4-0.0.1a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/README-dev.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/num_tini4/__init__.py
--rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/num_tini4/num.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/num_tini4/primes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/tests/__init__.py
--rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/tests/test_num.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.gitignore
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/README-dev.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/num_tini4/__init__.py
+-rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/num_tini4/num.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/num_tini4/primes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/tests/__init__.py
+-rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/tests/test_num.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/PKG-INFO
```

### Comparing `num_tini4-0.0.1a3/README-dev.md` & `num_tini4-0.0.1a4/README-dev.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## Installation
 
 `pip install num-tini4`
 
 ## Usage
 
 ```python
-# Importing the Num class from the library
+# Import the Num class from the library
 from src.num_tini4.num import Num
 
 
 # Declaring variables
 num1: Num = Num()
 num2: Num = Num()
 
@@ -33,45 +33,47 @@
 # Defining variables
 num1.set_fraction(1, 11)  # 1/11
 num2.set_int(-18)         # -18
 
 print(num1)  # [NUMBER, POSITIVE, {11: -1}, {'pi': 0, 'e': 0, 'root': 1}]
 print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}, {'pi': 0, 'e': 0, 'root': 1}]
 
-print(repr(num1))  # Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
-print(repr(num2))  # Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
+print(repr(num1))
+# Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
+print(repr(num2))
+# Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
 
 print(float(num1))  # 0.09090909090909091
 print(float(num2))  # -18.0
 
 
 # Operations
 print((num1 + num2).get_fraction())  # (-197, 11)
 print((num1 + num2).get_float())     # -17.90909090909091
-print((1/11) + -18.0)                # -17.90909090909091
+print((1 / 11) + -18.0)              # -17.90909090909091
 print('--------------------------------------------------')
 
 print((num1 - num2).get_fraction())  # (199, 11)
 print((num1 - num2).get_float())     # 18.09090909090909
-print((1/11) - -18.0)                # 18.09090909090909
+print((1 / 11) - -18.0)              # 18.09090909090909
 print('--------------------------------------------------')
 
 print((num1 * num2).get_fraction())  # (-18, 11)
 print((num1 * num2).get_float())     # -1.6363636363636365
-print((1/11) * -18.0)                # -1.6363636363636365
+print((1 / 11) * -18.0)              # -1.6363636363636365
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
 print((num1 / num2).get_float())     # -0.00505050505050505
-print((1/11) / -18.0)                # -0.005050505050505051
+print((1 / 11) / -18.0)              # -0.005050505050505051
 print('--------------------------------------------------')
 
 print((num1 ** num2).get_fraction())  # (5559917313492231481, 1)
 print((num1 ** num2).get_float())     # 5.559917313492231e+18
-print((1/11) ** -18.0)                # 5.559917313492229e+18
+print((1 / 11) ** -18.0)              # 5.559917313492229e+18
 print('--------------------------------------------------')
 
 
 # todo
 # +=, -=, *=, /=, **=
```

### Comparing `num_tini4-0.0.1a3/.github/workflows/codecov.yml` & `num_tini4-0.0.1a4/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a3/.github/workflows/pylint.yml` & `num_tini4-0.0.1a4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a3/.github/workflows/python-publish.yml` & `num_tini4-0.0.1a4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a3/src/num_tini4/num.py` & `num_tini4-0.0.1a4/src/num_tini4/num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a3/tests/test_num.py` & `num_tini4-0.0.1a4/tests/test_num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a3/README.md` & `num_tini4-0.0.1a4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,45 +33,47 @@
 # Defining variables
 num1.set_fraction(1, 11)  # 1/11
 num2.set_int(-18)         # -18
 
 print(num1)  # [NUMBER, POSITIVE, {11: -1}, {'pi': 0, 'e': 0, 'root': 1}]
 print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}, {'pi': 0, 'e': 0, 'root': 1}]
 
-print(repr(num1))  # Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
-print(repr(num2))  # Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
+print(repr(num1))
+# Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
+print(repr(num2))
+# Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
 
 print(float(num1))  # 0.09090909090909091
 print(float(num2))  # -18.0
 
 
 # Operations
 print((num1 + num2).get_fraction())  # (-197, 11)
 print((num1 + num2).get_float())     # -17.90909090909091
-print((1/11) + -18.0)                # -17.90909090909091
+print((1 / 11) + -18.0)              # -17.90909090909091
 print('--------------------------------------------------')
 
 print((num1 - num2).get_fraction())  # (199, 11)
 print((num1 - num2).get_float())     # 18.09090909090909
-print((1/11) - -18.0)                # 18.09090909090909
+print((1 / 11) - -18.0)              # 18.09090909090909
 print('--------------------------------------------------')
 
 print((num1 * num2).get_fraction())  # (-18, 11)
 print((num1 * num2).get_float())     # -1.6363636363636365
-print((1/11) * -18.0)                # -1.6363636363636365
+print((1 / 11) * -18.0)              # -1.6363636363636365
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
 print((num1 / num2).get_float())     # -0.00505050505050505
-print((1/11) / -18.0)                # -0.005050505050505051
+print((1 / 11) / -18.0)              # -0.005050505050505051
 print('--------------------------------------------------')
 
 print((num1 ** num2).get_fraction())  # (5559917313492231481, 1)
 print((num1 ** num2).get_float())     # 5.559917313492231e+18
-print((1/11) ** -18.0)                # 5.559917313492229e+18
+print((1 / 11) ** -18.0)              # 5.559917313492229e+18
 print('--------------------------------------------------')
 
 
 # todo
 # +=, -=, *=, /=, **=
```

### Comparing `num_tini4-0.0.1a3/pyproject.toml` & `num_tini4-0.0.1a4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "num_tini4"
-version = "0.0.1a3"
+version = "0.0.1a4"
 authors = [
   { name="Tini4", email="tilen.jurican@gmail.com" },
 ]
 description = "Python precise number type."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -17,9 +17,10 @@
     "Programming Language :: Python :: 3.11",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Tini4/Num"
+"Documentation" = "https://github.com/Tini4/Num/wiki"
+"Source Code" = "https://github.com/Tini4/Num"
 "Bug Tracker" = "https://github.com/Tini4/Num/issues"
```

### Comparing `num_tini4-0.0.1a3/PKG-INFO` & `num_tini4-0.0.1a4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: num_tini4
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Python precise number type.
-Project-URL: Homepage, https://github.com/Tini4/Num
+Project-URL: Documentation, https://github.com/Tini4/Num/wiki
+Project-URL: Source Code, https://github.com/Tini4/Num
 Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
 Author-email: Tini4 <tilen.jurican@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -50,45 +51,47 @@
 # Defining variables
 num1.set_fraction(1, 11)  # 1/11
 num2.set_int(-18)         # -18
 
 print(num1)  # [NUMBER, POSITIVE, {11: -1}, {'pi': 0, 'e': 0, 'root': 1}]
 print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}, {'pi': 0, 'e': 0, 'root': 1}]
 
-print(repr(num1))  # Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
-print(repr(num2))  # Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
+print(repr(num1))
+# Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
+print(repr(num2))
+# Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
 
 print(float(num1))  # 0.09090909090909091
 print(float(num2))  # -18.0
 
 
 # Operations
 print((num1 + num2).get_fraction())  # (-197, 11)
 print((num1 + num2).get_float())     # -17.90909090909091
-print((1/11) + -18.0)                # -17.90909090909091
+print((1 / 11) + -18.0)              # -17.90909090909091
 print('--------------------------------------------------')
 
 print((num1 - num2).get_fraction())  # (199, 11)
 print((num1 - num2).get_float())     # 18.09090909090909
-print((1/11) - -18.0)                # 18.09090909090909
+print((1 / 11) - -18.0)              # 18.09090909090909
 print('--------------------------------------------------')
 
 print((num1 * num2).get_fraction())  # (-18, 11)
 print((num1 * num2).get_float())     # -1.6363636363636365
-print((1/11) * -18.0)                # -1.6363636363636365
+print((1 / 11) * -18.0)              # -1.6363636363636365
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
 print((num1 / num2).get_float())     # -0.00505050505050505
-print((1/11) / -18.0)                # -0.005050505050505051
+print((1 / 11) / -18.0)              # -0.005050505050505051
 print('--------------------------------------------------')
 
 print((num1 ** num2).get_fraction())  # (5559917313492231481, 1)
 print((num1 ** num2).get_float())     # 5.559917313492231e+18
-print((1/11) ** -18.0)                # 5.559917313492229e+18
+print((1 / 11) ** -18.0)              # 5.559917313492229e+18
 print('--------------------------------------------------')
 
 
 # todo
 # +=, -=, *=, /=, **=
```

