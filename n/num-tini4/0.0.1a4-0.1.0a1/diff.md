# Comparing `tmp/num_tini4-0.0.1a4.tar.gz` & `tmp/num_tini4-0.1.0a1.tar.gz`

## Comparing `num_tini4-0.0.1a4.tar` & `num_tini4-0.1.0a1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/README-dev.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/num_tini4/__init__.py
--rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/num_tini4/num.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/src/num_tini4/primes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/tests/__init__.py
--rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/tests/test_num.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/.gitignore
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/LICENSE
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 num_tini4-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/README-dev.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/src/num_tini4/__init__.py
+-rw-r--r--   0        0        0    18665 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/src/num_tini4/num.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/src/primes/__init__.py
+-rw-r--r--   0        0        0  6106626 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/src/primes/primes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/tests/__init__.py
+-rw-r--r--   0        0        0   105838 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/tests/test_num.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/.gitignore
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 num_tini4-0.1.0a1/PKG-INFO
```

### Comparing `num_tini4-0.0.1a4/README-dev.md` & `num_tini4-0.1.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 
 `pip install num-tini4`
 
 ## Usage
 
 ```python
 # Import the Num class from the library
-from src.num_tini4.num import Num
+from num_tini4.num import Num
 
 
-# Declaring variables
+# Declare variables
 num1: Num = Num()
 num2: Num = Num()
 
 
-# Defining variables
+# Define variables
 num1.set_fraction(1, 11)  # 1/11
 num2.set_int(-18)         # -18
 
 print(num1)  # [NUMBER, POSITIVE, {11: -1}, {'pi': 0, 'e': 0, 'root': 1}]
 print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}, {'pi': 0, 'e': 0, 'root': 1}]
 
 print(repr(num1))
@@ -63,41 +63,27 @@
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
 print((num1 / num2).get_float())     # -0.00505050505050505
 print((1 / 11) / -18.0)              # -0.005050505050505051
 print('--------------------------------------------------')
 
-print((num1 ** num2).get_fraction())  # (5559917313492231481, 1)
-print((num1 ** num2).get_float())     # 5.559917313492231e+18
-print((1 / 11) ** -18.0)              # 5.559917313492229e+18
-print('--------------------------------------------------')
-
 
 # todo
-# +=, -=, *=, /=, **=
+# +=, -=, *=, /=
 
 
-# Comparison
+# Comparisons
 # <, >, <=, >=, ==, !=
 
 
 # todo
 # -, abs()
 
 
 # Inaccurate!!! Slow!!! Avoid!!!
 num1.set_float(18 / 11)
 print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}, {'pi': 0, 'e': 0, 'root': 1}]
 print(num1.get_fraction())  # (7369526662969903, 4503599627370496)
 print(num1.get_float())     # 1.6363636363636365
 print(18 / 11)              # 1.6363636363636365
 ```
-
-## 1
-- http://www.java2s.com/Tutorials/Python/Class/Overload_divide_operator.htm
-- https://www.geeksforgeeks.org/operator-overloading-in-python/
-
-## 2
-- https://t5k.org/lists/small/millions/
-- https://t5k.org/notes/faq/LongestList.html
-- http://compoasso.free.fr/primelistweb/page/prime/liste_online_en.php
```

### Comparing `num_tini4-0.0.1a4/.github/workflows/codecov.yml` & `num_tini4-0.1.0a1/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a4/.github/workflows/pylint.yml` & `num_tini4-0.1.0a1/.github/workflows/pylint.yml`

 * *Files 25% similar despite different names*

```diff
@@ -16,8 +16,8 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install pylint
     - name: Analysing the code with pylint
       run: |
-        pylint --errors-only $(git ls-files '*.py')
+        pylint --errors-only $(git ls-files '*.py' ':!:primes.py')
```

### Comparing `num_tini4-0.0.1a4/.github/workflows/python-publish.yml` & `num_tini4-0.1.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a4/src/num_tini4/num.py` & `num_tini4-0.1.0a1/src/num_tini4/num.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
-from math import inf, pi, e, sqrt  # , log10
+from math import inf, sqrt  # , log10
 
-
-# from primes import PRIMES, PRIMES_TO
+from src.primes.primes import PRIMES, PRIMES_TO
 
 
 class Num:
     class Sign(Enum):
         POSITIVE = 1
         NEGATIVE = -1
 
@@ -17,23 +16,22 @@
         UNDEFINED = None
 
     def __init__(self):
         """
         Initializes Num to UNDEFINED.
         """
         self.primes: dict[int, int] = {}
-        self.special: dict[str, int] = {'pi': 0, 'e': 0, 'root': 1}  # TODO
         self.sign: Num.Sign = Num.Sign.POSITIVE
         self.case: Num.Case = Num.Case.UNDEFINED
 
     def __repr__(self):
-        return f"Num(primes={self.primes!r}, special={self.special!r}, sign={self.sign!r}, case={self.case!r})"
+        return f"Num(primes={self.primes!r}, sign={self.sign!r}, case={self.case!r})"
 
     def __str__(self):
-        return f'[{self.case.name}, {self.sign.name}, {self.primes}, {self.special}]'
+        return f'[{self.case.name}, {self.sign.name}, {self.primes}]'
 
     def _modify_prime_factorization(self, integer: int, sign: Sign):
         # if integer > PRIMES_TO:
         #     size_integer: int = int(log10(integer)) + 1
         #     size_primes: int = int(log10(PRIMES_TO)) + 1
         #
         #     over: int = size_integer - size_primes + 1
@@ -53,14 +51,15 @@
         #         else:
         #             self.primes[prime] = 1 * sign.value
         #
         #         integer //= prime
         #
         #     if integer <= 1:
         #         break
+        pass
         # todo: Fast precision
         #  PRIMES: list[int] - highest divisor
         #  = [(0, 1, )2, 3, 2, 5, 3, 7, 2, 3, 5]
         #  Jakob
         for i in range(2, int(sqrt(integer)) + 1):
             while integer % i == 0:
                 if i in self.primes:
@@ -503,78 +502,14 @@
             else:
                 out.primes[prime] = -denominator[prime]
 
         out._clean_values()
 
         return out
 
-    def __pow__(self, other):  # , power, modulo=None):
-        if self.__class__ != other.__class__:
-            raise TypeError
-
-        out: Num = Num()
-
-        if (self.case is Num.Case.UNDEFINED) or (other.case is Num.Case.UNDEFINED):
-            out.set_num(case=Num.Case.UNDEFINED)
-
-            return out
-
-        if self.case is Num.Case.ZERO:
-            out.set_num(case=Num.Case.ZERO)
-
-            return out
-
-        if other.case is Num.Case.ZERO:
-            out.set_num({})
-
-            return out
-
-        if (self.primes == {}) and (self.case is Num.Case.NUMBER):
-            if (other.case is Num.Case.INFINITY) or (2 in other.primes):
-                out.set_num({})
-
-                return out
-
-            out.set_num({}, sign=self.sign)
-
-            return out
-
-        if (other.case is Num.Case.INFINITY) and (other.sign is Num.Sign.POSITIVE):
-            out.set_num(case=Num.Case.INFINITY)
-
-            return out
-
-        if (self.case is Num.Case.INFINITY) and (other.sign is Num.Sign.POSITIVE):
-            if (self.sign is Num.Sign.NEGATIVE) and (2 not in other.primes):
-                out.sign = Num.Sign.NEGATIVE
-
-            out.case = Num.Case.INFINITY
-
-            return out
-
-        if (other.case is Num.Case.INFINITY) or (self.case is Num.Case.INFINITY):
-            out.set_num({})
-
-            return out
-
-        out.set_num(self.primes)
-
-        if (self.sign is Num.Sign.NEGATIVE) and (2 not in other.primes):
-            out.sign = Num.Sign.NEGATIVE
-
-        if other.sign is Num.Sign.NEGATIVE:
-            out.primes = {k: -v for k, v in out.primes.items()}
-
-        numerator, denominator = other.get_fraction()
-
-        out.primes = {k: v * abs(numerator) for k, v in out.primes.items()}
-        out.special['root'] *= denominator
-
-        return out
-
     def __lt__(self, other):
         if self.__class__ != other.__class__:
             raise TypeError
 
         if (self.case is Num.Case.UNDEFINED) or (other.case is Num.Case.UNDEFINED):
             return False
 
@@ -648,18 +583,14 @@
         if self.__class__ != other.__class__:
             raise TypeError
 
     def __isub__(self, other):
         if self.__class__ != other.__class__:
             raise TypeError
 
-    def __ipow__(self, other):
-        if self.__class__ != other.__class__:
-            raise TypeError
-
     def __abs__(self):
         out: Num = Num()
 
         out.set_num(self.primes, sign=Num.Sign.POSITIVE, case=self.case)
 
         out._clean_values()
 
@@ -681,17 +612,17 @@
         pass  # todo: ?
 
     def __float__(self):
         return self.get_float()
 
 
 if __name__ == '__main__':
-    try:
-        print(f'Fast precision: {PRIMES_TO:,}\n')
-    except NameError:
+    if PRIMES_TO is not None:
+        print(f'Fast precision to: {PRIMES_TO:,}\n')
+    else:
         print('Precision: infinite\n')
 
     number1 = Num()
     number2 = Num()
 
     number1.set_int(5)
     number2.set_int(2)
@@ -705,12 +636,7 @@
     print(number1 >= number1)
     print()
     print(number1 == number2)
     print(number1 == number1)
     print(number1 != number2)
     print(number2 != number2)
     print()
-
-    # number1.set_num({2: 1, 3: -1, 11: 1})
-    number1.set_num(case=Num.Case.UNDEFINED, sign=Num.Sign.NEGATIVE)
-    print(float(number1))
-    print(number1)
```

### Comparing `num_tini4-0.0.1a4/tests/test_num.py` & `num_tini4-0.1.0a1/tests/test_num.py`

 * *Files 1% similar despite different names*

```diff
@@ -2004,248 +2004,14 @@
         number3 = number1 - number2
         self.assertEqual(number3.primes, {}, 'Primes not subtracted properly.')
         self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not subtracted properly.')
         self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not subtracted properly.')
 
 
 # noinspection DuplicatedCode
-class TestNumPow(unittest.TestCase):
-    def setUp(self):
-        pass
-
-    def test_number_positive(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num({2: 1, 3: 2})
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {2: 11, 3: 22}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({2: 1, 3: 2}, sign=Num.Sign.NEGATIVE)
-        number2.set_num({2: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {2: 2, 3: 4}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-    def test_number_negative(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num({2: 1, 3: 2}, sign=Num.Sign.NEGATIVE)
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {2: 11, 3: 22}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-    def test_zero(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num(case=Num.Case.ZERO)
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.ZERO, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.ZERO)
-        number2.set_num({11: 1}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.ZERO, 'Case not powered properly.')
-
-    def test_infinity_positive(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num(case=Num.Case.INFINITY)
-        number2.set_num(case=Num.Case.INFINITY)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.INFINITY, 'Case not powered properly.')
-
-        number1.set_num({2: 1, 3: 2})
-        number2.set_num(case=Num.Case.INFINITY)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.INFINITY, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.INFINITY)
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.INFINITY, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.INFINITY, sign=Num.Sign.NEGATIVE)
-        number2.set_num({2: 3})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.INFINITY, 'Case not powered properly.')
-
-    def test_infinity_negative(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num(case=Num.Case.INFINITY, sign=Num.Sign.NEGATIVE)
-        number2.set_num({})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.INFINITY, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.INFINITY, sign=Num.Sign.NEGATIVE)
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.INFINITY, 'Case not powered properly.')
-
-    def test_undefined(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num({2: 1, 3: 2})
-        number2.set_num(case=Num.Case.UNDEFINED)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.UNDEFINED, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.UNDEFINED)
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.UNDEFINED, 'Case not powered properly.')
-
-        number1.set_num({2: 1, 3: 2}, sign=Num.Sign.NEGATIVE)
-        number2.set_num(case=Num.Case.UNDEFINED)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.UNDEFINED, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.UNDEFINED)
-        number2.set_num({11: 1}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.UNDEFINED, 'Case not powered properly.')
-
-        number1.set_num(case=Num.Case.UNDEFINED)
-        number2.set_num(case=Num.Case.UNDEFINED)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.UNDEFINED, 'Case not powered properly.')
-
-    def test_one_positive(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num({})
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num({11: 1}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num({2: 3})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num({2: 3}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num({})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num({}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num(case=Num.Case.INFINITY)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({})
-        number2.set_num(case=Num.Case.INFINITY, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.POSITIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-    def test_one_negative(self):
-        number1 = Num()
-        number2 = Num()
-
-        number1.set_num({}, sign=Num.Sign.NEGATIVE)
-        number2.set_num({11: 1})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({}, sign=Num.Sign.NEGATIVE)
-        number2.set_num({11: 1}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({}, sign=Num.Sign.NEGATIVE)
-        number2.set_num({})
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-        number1.set_num({}, sign=Num.Sign.NEGATIVE)
-        number2.set_num({}, sign=Num.Sign.NEGATIVE)
-        number3 = number1 ** number2
-        self.assertEqual(number3.primes, {}, 'Primes not powered properly.')
-        self.assertEqual(number3.sign, Num.Sign.NEGATIVE, 'Sign not powered properly.')
-        self.assertEqual(number3.case, Num.Case.NUMBER, 'Case not powered properly.')
-
-
-# noinspection DuplicatedCode
 class TestNumLt(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_number(self):
         number1 = Num()
         number2 = Num()
```

### Comparing `num_tini4-0.0.1a4/README.md` & `num_tini4-0.1.0a1/README-dev.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,34 +17,32 @@
 ## Installation
 
 `pip install num-tini4`
 
 ## Usage
 
 ```python
-# Importing the Num class from the library
-from num_tini4.num import Num
+# Import the Num class from the library
+from src.num_tini4.num import Num
 
 
-# Declaring variables
+# Declare variables
 num1: Num = Num()
 num2: Num = Num()
 
 
-# Defining variables
+# Define variables
 num1.set_fraction(1, 11)  # 1/11
 num2.set_int(-18)         # -18
 
-print(num1)  # [NUMBER, POSITIVE, {11: -1}, {'pi': 0, 'e': 0, 'root': 1}]
-print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}, {'pi': 0, 'e': 0, 'root': 1}]
+print(num1)  # [NUMBER, POSITIVE, {11: -1}]
+print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}]
 
-print(repr(num1))
-# Num(primes={11: -1}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
-print(repr(num2))
-# Num(primes={2: 1, 3: 2}, special={'pi': 0, 'e': 0, 'root': 1}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
+print(repr(num1))  # Num(primes={11: -1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
+print(repr(num2))  # Num(primes={2: 1, 3: 2}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
 
 print(float(num1))  # 0.09090909090909091
 print(float(num2))  # -18.0
 
 
 # Operations
 print((num1 + num2).get_fraction())  # (-197, 11)
@@ -63,32 +61,36 @@
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
 print((num1 / num2).get_float())     # -0.00505050505050505
 print((1 / 11) / -18.0)              # -0.005050505050505051
 print('--------------------------------------------------')
 
-print((num1 ** num2).get_fraction())  # (5559917313492231481, 1)
-print((num1 ** num2).get_float())     # 5.559917313492231e+18
-print((1 / 11) ** -18.0)              # 5.559917313492229e+18
-print('--------------------------------------------------')
-
 
 # todo
-# +=, -=, *=, /=, **=
+# +=, -=, *=, /=
 
 
-# Comparison
+# Comparisons
 # <, >, <=, >=, ==, !=
 
 
 # todo
 # -, abs()
 
 
 # Inaccurate!!! Slow!!! Avoid!!!
 num1.set_float(18 / 11)
-print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}, {'pi': 0, 'e': 0, 'root': 1}]
+print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}]
 print(num1.get_fraction())  # (7369526662969903, 4503599627370496)
 print(num1.get_float())     # 1.6363636363636365
 print(18 / 11)              # 1.6363636363636365
 ```
+
+## 1
+- http://www.java2s.com/Tutorials/Python/Class/Overload_divide_operator.htm
+- https://www.geeksforgeeks.org/operator-overloading-in-python/
+
+## 2
+- https://t5k.org/lists/small/millions/
+- https://t5k.org/notes/faq/LongestList.html
+- http://compoasso.free.fr/primelistweb/page/prime/liste_online_en.php
```

### Comparing `num_tini4-0.0.1a4/pyproject.toml` & `num_tini4-0.1.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "num_tini4"
-version = "0.0.1a4"
+version = "0.1.0a1"
 authors = [
   { name="Tini4", email="tilen.jurican@gmail.com" },
 ]
 description = "Python precise number type."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `num_tini4-0.0.1a4/PKG-INFO` & `num_tini4-0.1.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: num_tini4
-Version: 0.0.1a4
+Version: 0.1.0a1
 Summary: Python precise number type.
 Project-URL: Documentation, https://github.com/Tini4/Num/wiki
 Project-URL: Source Code, https://github.com/Tini4/Num
 Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
 Author-email: Tini4 <tilen.jurican@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
@@ -35,24 +35,24 @@
 ## Installation
 
 `pip install num-tini4`
 
 ## Usage
 
 ```python
-# Importing the Num class from the library
+# Import the Num class from the library
 from num_tini4.num import Num
 
 
-# Declaring variables
+# Declare variables
 num1: Num = Num()
 num2: Num = Num()
 
 
-# Defining variables
+# Define variables
 num1.set_fraction(1, 11)  # 1/11
 num2.set_int(-18)         # -18
 
 print(num1)  # [NUMBER, POSITIVE, {11: -1}, {'pi': 0, 'e': 0, 'root': 1}]
 print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}, {'pi': 0, 'e': 0, 'root': 1}]
 
 print(repr(num1))
@@ -81,25 +81,20 @@
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
 print((num1 / num2).get_float())     # -0.00505050505050505
 print((1 / 11) / -18.0)              # -0.005050505050505051
 print('--------------------------------------------------')
 
-print((num1 ** num2).get_fraction())  # (5559917313492231481, 1)
-print((num1 ** num2).get_float())     # 5.559917313492231e+18
-print((1 / 11) ** -18.0)              # 5.559917313492229e+18
-print('--------------------------------------------------')
-
 
 # todo
-# +=, -=, *=, /=, **=
+# +=, -=, *=, /=
 
 
-# Comparison
+# Comparisons
 # <, >, <=, >=, ==, !=
 
 
 # todo
 # -, abs()
```

