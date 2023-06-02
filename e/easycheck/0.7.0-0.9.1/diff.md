# Comparing `tmp/easycheck-0.7.0.tar.gz` & `tmp/easycheck-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck-0.7.0.tar", last modified: Thu May 11 05:11:12 2023, max compression
+gzip compressed data, was "easycheck-0.9.1.tar", last modified: Fri Jun  2 10:56:26 2023, max compression
```

## Comparing `easycheck-0.7.0.tar` & `easycheck-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-11 05:11:12.181404 easycheck-0.7.0/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1073 2021-01-27 07:58:06.000000 easycheck-0.7.0/LICENSE
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    18030 2023-05-11 05:11:12.179970 easycheck-0.7.0/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    15058 2023-05-11 05:10:55.000000 easycheck-0.7.0/README.rst
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-11 05:11:12.160752 easycheck-0.7.0/easycheck/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      614 2023-05-11 05:10:55.000000 easycheck-0.7.0/easycheck/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    37062 2023-05-11 05:10:55.000000 easycheck-0.7.0/easycheck/easycheck.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      865 2023-03-01 16:15:06.000000 easycheck-0.7.0/easycheck/tmp.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-11 05:11:12.175970 easycheck-0.7.0/easycheck.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    18030 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      253 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       26 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       10 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-05-11 05:11:12.181596 easycheck-0.7.0/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1126 2023-05-11 05:10:55.000000 easycheck-0.7.0/setup.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 10:56:26.026688 easycheck-0.9.1/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1073 2021-01-27 07:58:06.000000 easycheck-0.9.1/LICENSE
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24060 2023-06-02 10:56:26.025693 easycheck-0.9.1/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    20352 2023-06-02 10:56:23.000000 easycheck-0.9.1/README.rst
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 10:56:26.000683 easycheck-0.9.1/easycheck/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      614 2023-06-02 10:17:55.000000 easycheck-0.9.1/easycheck/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    38722 2023-06-02 10:38:03.000000 easycheck-0.9.1/easycheck/easycheck.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      865 2023-03-01 16:15:06.000000 easycheck-0.9.1/easycheck/tmp.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 10:56:26.021731 easycheck-0.9.1/easycheck.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24060 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      253 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       26 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       10 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-02 10:56:26.026688 easycheck-0.9.1/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1134 2023-06-02 10:56:23.000000 easycheck-0.9.1/setup.py
```

### Comparing `easycheck-0.7.0/LICENSE` & `easycheck-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easycheck-0.7.0/PKG-INFO` & `easycheck-0.9.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,294 +1,363 @@
-Metadata-Version: 2.1
-Name: easycheck
-Version: 0.7.0
-Summary: A tool for checking conditions in Python
-Home-page: https://github.com/nyggus/easycheck
-Author: Nyggus & Ke Boan
-Author-email: nyggus@gmail.com
-License: MIT
-Description: easycheck
-        =========
-        
-        The :code:`easycheck` package offers a lightweight tool for running functionized checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases (starting off with :code:`assert_` instead of :code:`check_`).
-        
-        The idea is to use the :code:`easycheck` functions to check conditions that are _not_ assertions. The checks work in the following general way: When a condition is met, nothing happens (in fact, the function returns :code:`None`); if it is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
-        
-        * Assertions are meant to be used conditions that _must_ be true (when only the code is correct). So, if an assertion is incorrect, it means something is wrong with the code. You should never use assertions to handle regular exceptions, like those related to data or arguments.
-        * Unlike assertions, :code:`easycheck` functions are to be used to check conditions related to things like data and argument values, and to handle regular exceptions.
-        * While assertions only raise :code:`AssertionError`, you can choose any exception to be raised by easycheck functions.
-        * When using :code:`easycheck`, instead of raising an exception, you can issue a warning.
-        
-        The main :code:`easycheck` functions (with names starting off with :code:`check_`) are designed in such a way that they can be used as easy-to-understand code that checks whether one or more conditions are met. They can be used instead of :code:`if`-blocks, which are normally used to check conditions and raise exceptions (or issue warnings) if they are not met. So, you can do the following:
-        
-        .. code-block:: python
-        
-            if not isinstance(x, (float, int)):
-                raise TypeError('x must be a number')
-            if x > 10:
-                raise ValueError('Too high value of x')
-        
-        or you can use :code:`easycheck` for this:
-        
-        .. code-block:: python
-        
-            check_type(x, (float, int), message='x must be a number')
-            check_if(x <= 10, ValueError, 'Too high value of x')
-        
-        The :code:`easycheck` approach has two main advantages over this classical approach:
-        
-        * It saves a little space; not much, since most often you'll end up with one line of code instead of two, but not always, particularly when you provide an exception type to be raised and a long message. 
-        * Mainly, it increases code simplicity and readability, since both the names of easycheck functions and their arguments are designed in such a way that the reader immediately understands what is being checked.
-        
-        You can also issue a warning:
-        
-        .. code-block:: python
-        
-            check_if(x <= 10,
-                     Warning,
-                     'For stable functioning of the function, '
-                     'x should not be greater than 10.')
-        
-        The package also offers functions dedicated to testing, e.g.,
-        
-        .. code-block:: python
-        
-            assert_type(x, (float, int))
-            assert_if(x <= 10)
-        
-        The :code:`message` argument has the default value of :code:`None`, which does the following. If the exception class provided in :code:`handle_with` is built-in (that is, can be found in :code:`dir(builtins)`), no message is provided. But if it is not a built-in exception (or warning) class, then the exception/warning class's docstring is taken as the message. This is a convenient way of providing a  typical message. If you want to customize the message (e.g., depending on the value of a variable), you should use a customized string (e.g., through an f-string). But if you do not want to use any message with a custom exception/warning, simply provide an empty string (:code:`message=''`).
-        
-        
-        Read about :code:`easycheck`
-        ----------------------------
-        
-        You will find more about assertions in `this article <https://medium.com/towards-data-science/python-assertions-or-checking-if-a-cat-is-a-dog-ce11c55d143>`_, entitled "Python Assertions, or Checking If a Cat Is a Dog" and published in *Towards Data Science*. It mentions :code:`easycheck`! You will read about :code:`easycheck` also in `the article "Comparing floating-point numbers with easycheck" <https://medium.com/towards-data-science/comparing-floating-point-numbers-with-easycheck-dcbae480f75f>`_  (also from *Towards Data Science*). The *Better Programming* article entitiled `"How to Overwrite AssertionError in Python and Use Custom Exceptions" <https://medium.com/better-programming/how-to-overwrite-asserterror-in-python-and-use-custom-exceptions-c0b252989977>`_, mentions the package, too.
-        
-        
-        Installing
-        ----------
-        
-        Install and update using pip:
-        
-        .. code-block:: text
-        
-            pip install easycheck
-        
-        Testing
-        -------
-        
-        The package is covered with both pytests and doctests. The latter are included in both docstrings of all the functions, but also in `documentation files <https://github.com/nyggus/easycheck/tree/master/docs>`_.
-        
-        Use in code to raise exceptions
-        -------------------------------
-        
-        Here are several examples of a simple use of basic :code:`easycheck` functions. The most basic usage resembles the following:
-        
-        .. code-block:: python
-        
-            check_if(a < 10)
-        	
-        This simply checks if :code:`a` is smaller than 10; if it is, nothing happens (in fact, :code:`check_if(a < 10)` returns :code:`None`). But if the condition is violated, the function raises :code:`AssertionError`. :code:`AssertionError` is the default exception returned by :code:`check_if()`, but you can change this:
-        
-        .. code-block:: python
-        
-            check_if(a < 10, handle_with=ValueError)
-            # or shorter and equally readable:
-            check_if(a < 10, ValueError)
-        
-        For built-in exceptions, like :code:`ValueError`, the default behaviour is to not print any message. For custom exceptions, however, the exception's docstring (`.__doc__`) serves as a message. You can use this when you create custom exceptions:
-        
-        .. code-block:: python
-        
-            class IncorrectNameTypeError(Exception):
-                """Argument name must be a string."""
-            
-            name = 40
-            check_type(name, IncorrectNameTypeError)
-            Traceback (most recent call last):
-              ...
-            IncorrectNameTypeError: Argument name must be a string.
-        
-        If you want to ensure that no message is printed, even for a custom exception, override the default behaviour by passing an empty string :code:`message=''`. You can also add a custom message:
-        
-        .. code-block:: python
-        
-            check_if(a < 10, handle_with=ValueError, message='Too high a')
-            # or shorter and equally readable:
-            check_if(a < 10, ValueError, 'Too high a')
-        
-        Some other functions have different default errors; for instance, this call
-        
-        .. code-block:: python
-        
-            check_type(a, expected_type=str)
-            # or shorter:
-            check_type(a, str)
-        
-        will raise :code:`TypeError` while this
-        
-        .. code-block:: python
-        
-            check_length([1, 2, 3], 1)
-        	
-        will raise :code:`LengthError` (an exception class defined in the :code:`easycheck` module).
-        
-        Here is a list of :code:`easycheck` functions the module offers, along with their aliases to be used for testing:
-        
-        * :code:`check_if()`, with the alias of :code:`assert_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
-        * :code:`check_if_not()`, with the alias of :code:`assert_if_not()`; the opposite of :code:`check_if()`, helpful when you need to assure that a condition is _not_ met;
-        * :code:`check_if_isclose()`, with the alias of :code:`assert_if_isclose()`; to compare two floating-point numbers, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`_);
-        * :code:`check_if_in_limits()`, with the alias of :code:`assert_if_in_limits()`;
-        * :code:`check_length()`, with the alias of :code:`assert_length()`; to compare length (equal to, smaller than, greater than, and the like);
-        * :code:`check_type()`, with the alias of :code:`assert_type()`; to check expected type, similar to :code:`isinstance()`;
-        * :code:`check_if_paths_exist()`, with the alias of :code:`assert_paths()`; to compare paths (or just one path) exist;
-        * :code:`check_comparison()` (used to compare two items); to compare to objectsm just like you would do using :code:`if obj1 != obj2: raise`
-        * :code:`check_all_ifs()`; used to check multiple conditions and return all the checks;
-        * :code:`check_argument()`; used to make one or more checks of a function's argument.
-        
-        You can also use a :code:`catch_check()` function, if you want to catch an exception or a warning the :code:`easycheck` function you use would raise (see examples `here <https://github.com/nyggus/easycheck/blob/master/docs/catch_exceptions_doctest.rst>`_). Sometimes, however, you will do better using a :code:`try-except` block to catch exceptions (`see examples <https://github.com/nyggus/easycheck/blob/master/docs/use_with_try_doctest.rst>`_).
-        
-        > Note that some :code:`easycheck` functions are simple wrappers around built-in functions, but their behavior is different, as they have the typical behavior of an :code:`easycheck` function: if a condition is not met, an exception is raised or an issue is raised.
-        
-        
-        Use in code to issue warnings
-        -----------------------------
-        
-        In order to issue a warning if a condition is violated, simply use a warning class (in the :code:`handle_with` argument) instead of an exception class:
-        
-        .. code-block:: python
-        
-            check_if(2 > 1, Warning, 'Too high a value')
-            check_length([1, 2, 3], 10, Warning, 'Too short list with data')
-        
-        Remember to always use a message with warnings, in order to make them meaningful. (See more in `use_with_warnings_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_with_warnings_doctest.rst>`_).
-        
-        
-        Of course, you can use a custom warning:
-        
-        .. code-block:: python
-        
-            class TooSmallSampleSize(Warning):
-                """Results for samples size below 100 can be unstable."""
-            
-            n = 50
-            check_if(n >= 100, TooSmallSampleSize)
-            ... TooSmallSampleSize: Results for samples size below 100 can be unstable.
-              warnings.warn(message, error)
-        
-        
-        Use in code, an example
-        -----------------------
-        
-        Imagine you want to connect to a database; if the connection fails for any reason, you want to read an archived flat file. (We will use some undefined functions whose names will clearly convey what the functions do.)
-        
-        .. code-block:: python
-        
-            from easycheck import check_if, check_if_paths_exist
-            
-            class DataBaseConnectionError(Exception):
-                pass
-            
-            def get_data_from_db(db_details, db_credentials):
-                try:
-                    connect_to_db(db_details, db_credentials)
-                except:
-                    return False
-                data = get_records_from_db()
-                return data
-        
-        The :code:`easycheck` code could look like the following:
-        
-        .. code-block:: python
-        
-            def get_data(db_details, db_credentials):
-                data = get_data_from_db(db_details, db_credentials)
-                check_if(
-                    data,
-                    handle_with=DataBaseConnectionError,
-                    message='Cannot communicate with the database'
-                    )
-                return data
-                      
-        You can of course handle this exception, for example like here:
-        
-        .. code-block:: python
-        
-            def get_data(db_details, db_credentials, archived_data_file):
-                data = get_data_from_db(db_details, db_credentials)
-                try:
-                    check_if(
-                        data,
-                        handle_with=DataBaseConnectionError,
-                        message='Cannot communicate with the database'
-                    )
-                except DataBaseConnectionError:
-                    check_if_paths_exist(archived_data_file)
-                    with open(archived_data_file) as f:
-                        data = f.readlines()
-                return data
-            
-        Of course, you might use here a dedicated context manager. Sure, you can write it in a shorter way, without :code:`easycheck`, but the flow of information will not be as smooth, resulting in less readability:
-        
-        .. code-block:: python
-        
-            def get_data(db_details, db_credentials, archived_data_file):
-                data = get_data_from_db(db_details, db_credentials)
-                if not data:
-                    with open(archived_data_file) as f:
-                        data = f.readlines()
-                return data
-        
-        Of course, the :code:`open()` context manager will itself throw an error, but when you use the :code:`check_if()` function and explicitly define an exception class, you clearly show the reader that you're checking if this file exists and raise a particular exception if it doesn't.
-                
-        Use in testing
-        --------------
-        
-        As mentioned above, most :code:`easycheck` functions have aliases to be used in testing. Of course, you can use :code:`check_if()`, but to align with the common use of assertions, the :code:`easycheck` module offers those aliases so that the reader will immediately see that you're using these functions to test. Consider these examples:
-        
-        .. code-block:: python
-        
-            # Using assertions
-            def test_something():
-                a, b = my_function_1(), my_function_2()
-        
-                assert a == 2; 
-                assert isinstance(a, int)
-                assert isinstance(b, tuple)
-                assert len(b) == 5
-        		
-            # Using easycheck assert-like functions:
-            def test_something():
-                a, b = my_function_1(), my_function_2()
-                
-                assert_if(a == 2)
-                assert_type(a, int)
-                assert_type(b, tuple)
-                assert_length(b, 5)
-        
-        Note that only the first one will raise :code:`AssertionError` while the others will raise more meaningful errors (:code:`TypeError` and :code:`LengthError`), which may better explain the reasons that the tests did not pass.
-        
-        You will find more about using :code:`easycheck` in `use_in_testing_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_in_testing_doctest.rst>`_.
-        
-        Other examples
-        --------------
-        
-        You will find a number of examples in `doctest files <https://github.com/nyggus/easycheck/tree/master/docs/>`_, which also serve as doctests.
-        
-        
-        Changelog
-        ---------
-        
-        * Version 0.6.0 came with significant optimization of performance. Before, :code:`easycheck` functions performed internal checks of the argument values provided to the function call. Most of these checks are not performed anymore, at least not for the most significant :code:`easycheck` functions, such as :code:`check_if()` or :code:`check_type()`. Some checks, however, are still done. These are mainly checks without which the behavior of the function would be either unwanted or unexpected. We decided to remove all checks that do not change much; for instance, they raise an error due to an incorrect type of an argument value — even though it would be raised anyway, but by the internal Python process, not by the :code:`easycheck` function itself. The point is to remove such unnecessary checks and that way remove the unnecessary :code:`if` blocks, which certainly add some cost to execution time. While one such check costs almost nothing, many of them (e.g., in a long loop) can mean a significant cost. As of version 0.6.0, we will try to optimize the performance of :code:`easycheck` by getting rid of such overhead costs, unless they are important for the behavior of the corresponding :code:`easycheck` function.
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
+easycheck
+=========
+.. image:: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml/badge.svg
+   :target: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml
+.. image:: https://codecov.io/github/nyggus/easycheck/branch/master/graph/badge.svg?token=EH4TLHQQWC 
+   :target: https://codecov.io/github/nyggus/easycheck
+.. image:: https://img.shields.io/pypi/l/easycheck.svg
+   :target: https://pypi.org/project/easycheck     
+.. image:: https://img.shields.io/pypi/v/easycheck.svg
+   :target: https://pypi.org/project/easycheck     
+.. image:: https://img.shields.io/pypi/wheel/easycheck
+   :target: https://pypi.org/project/easycheck     
+.. image:: https://img.shields.io/pypi/pyversions/easycheck
+   :target: https://pypi.org/project/easycheck
+.. image:: https://img.shields.io/github/stars/nyggus/easycheck?style=social
+   :target: https://github.com/nyggus/easycheck
+.. image:: https://img.shields.io/github/last-commit/nyggus/easycheck
+
+The :code:`easycheck` package offers a lightweight tool for running functionized checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases (starting off with :code:`assert_` instead of :code:`check_`). You can also switch off all :code:`easycheck` checks, by setting the :code:`"EASYCHECK_RUN"` environmental variable to :code:`"0"`.
+
+The idea is to use the :code:`easycheck` functions to check conditions that are _not_ assertions. The checks work in the following general way: When a condition is met, nothing happens (in fact, the function returns :code:`None`); if it is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
+
+* Assertions are meant to be used conditions that _must_ be true (when only the code is correct). So, if an assertion is incorrect, it means something is wrong with the code. You should never use assertions to handle regular exceptions, like those related to data or arguments.
+* Unlike assertions, :code:`easycheck` functions are to be used to check conditions related to things like data and argument values, and to handle regular exceptions.
+* While assertions only raise :code:`AssertionError`, you can choose any exception to be raised by easycheck functions.
+* When using :code:`easycheck`, instead of raising an exception, you can issue a warning.
+
+The main :code:`easycheck` functions (with names starting off with :code:`check_`) are designed in such a way that they can be used as easy-to-understand code that checks whether one or more conditions are met. They can be used instead of :code:`if`-blocks, which are normally used to check conditions and raise exceptions (or issue warnings) if they are not met. So, you can do the following:
+
+.. code-block:: python
+
+    if not isinstance(x, (float, int)):
+        raise TypeError('x must be a number')
+    if x > 10:
+        raise ValueError('Too high value of x')
+
+or you can use :code:`easycheck` for this:
+
+.. code-block:: python
+
+    check_type(x, (float, int), message='x must be a number')
+    check_if(x <= 10, ValueError, 'Too high value of x')
+
+The :code:`easycheck` approach has two main advantages over this classical approach:
+
+* It saves a little space; not much, since most often you'll end up with one line of code instead of two, but not always, particularly when you provide an exception type to be raised and a long message. 
+* Mainly, it increases code simplicity and readability, since both the names of easycheck functions and their arguments are designed in such a way that the reader immediately understands what is being checked.
+
+You can also issue a warning:
+
+.. code-block:: python
+
+    check_if(x <= 10,
+             Warning,
+             'For stable functioning of the function, '
+             'x should not be greater than 10.')
+
+The package also offers functions dedicated to testing, e.g.,
+
+.. code-block:: python
+
+    assert_type(x, (float, int))
+    assert_if(x <= 10)
+
+The :code:`message` argument has the default value of :code:`None`, which does the following. If the exception class provided in :code:`handle_with` is built-in (that is, can be found in :code:`dir(builtins)`), no message is provided. But if it is not a built-in exception (or warning) class, then the exception/warning class's docstring is taken as the message. This is a convenient way of providing a  typical message. If you want to customize the message (e.g., depending on the value of a variable), you should use a customized string (e.g., through an f-string). But if you do not want to use any message with a custom exception/warning, simply provide an empty string (:code:`message=''`).
+
+
+Read about :code:`easycheck`
+----------------------------
+
+You will find more about assertions in `this article <https://medium.com/towards-data-science/python-assertions-or-checking-if-a-cat-is-a-dog-ce11c55d143>`_, entitled "Python Assertions, or Checking If a Cat Is a Dog" and published in *Towards Data Science*. It mentions :code:`easycheck`! You will read about :code:`easycheck` also in `the article "Comparing floating-point numbers with easycheck" <https://medium.com/towards-data-science/comparing-floating-point-numbers-with-easycheck-dcbae480f75f>`_  (also from *Towards Data Science*). The *Better Programming* article entitiled `"How to Overwrite AssertionError in Python and Use Custom Exceptions" <https://medium.com/better-programming/how-to-overwrite-asserterror-in-python-and-use-custom-exceptions-c0b252989977>`_, mentions the package, too.
+
+
+Installing
+----------
+
+Install and update using pip:
+
+.. code-block:: text
+
+    pip install easycheck
+
+Testing
+-------
+
+The package is covered with both pytests and doctests. The latter are included in both docstrings of all the functions, but also in `documentation files <https://github.com/nyggus/easycheck/tree/master/docs>`_.
+
+Use in code to raise exceptions
+-------------------------------
+
+Here are several examples of a simple use of basic :code:`easycheck` functions. The most basic usage resembles the following:
+
+.. code-block:: python
+
+    check_if(a < 10)
+	
+This simply checks if :code:`a` is smaller than 10; if it is, nothing happens (in fact, :code:`check_if(a < 10)` returns :code:`None`). But if the condition is violated, the function raises :code:`AssertionError`. :code:`AssertionError` is the default exception returned by :code:`check_if()`, but you can change this:
+
+.. code-block:: python
+
+    check_if(a < 10, handle_with=ValueError)
+    # or shorter and equally readable:
+    check_if(a < 10, ValueError)
+
+For built-in exceptions, like :code:`ValueError`, the default behaviour is to not print any message. For custom exceptions, however, the exception's docstring (`.__doc__`) serves as a message. You can use this when you create custom exceptions:
+
+.. code-block:: python
+
+    class IncorrectNameTypeError(Exception):
+        """Argument name must be a string."""
+    
+    name = 40
+    check_type(name, IncorrectNameTypeError)
+    Traceback (most recent call last):
+      ...
+    IncorrectNameTypeError: Argument name must be a string.
+
+If you want to ensure that no message is printed, even for a custom exception, override the default behaviour by passing an empty string :code:`message=''`. You can also add a custom message:
+
+.. code-block:: python
+
+    check_if(a < 10, handle_with=ValueError, message='Too high a')
+    # or shorter and equally readable:
+    check_if(a < 10, ValueError, 'Too high a')
+
+Some other functions have different default errors; for instance, this call
+
+.. code-block:: python
+
+    check_type(a, expected_type=str)
+    # or shorter:
+    check_type(a, str)
+
+will raise :code:`TypeError` while this
+
+.. code-block:: python
+
+    check_length([1, 2, 3], 1)
+	
+will raise :code:`LengthError` (an exception class defined in the :code:`easycheck` module).
+
+Here is a list of :code:`easycheck` check functions the module offers, discluding assertions, which are listed in the next paragraph:
+
+* :code:`check_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
+* :code:`check_if_not()`; the opposite of :code:`check_if()`, helpful when you need to assure that a condition is *not* met;
+* :code:`check_if_isclose()`; to compare two floating-point numbers, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`__);
+* :code:`check_if_in_limits()`; to check if a number lies between two other numbers;
+* :code:`check_length()`; to compare length (equal to, smaller than, greater than, and the like);
+* :code:`check_type()`; to check expected type, similar to :code:`isinstance()`;
+* :code:`check_if_paths_exist()`; to compare paths (or just one path) exist;
+* :code:`check_comparison()` (used to compare two items); to compare two objects, just like you would do using :code:`if obj1 != obj2: raise`
+* :code:`check_all_ifs()`; used to check multiple conditions and return all the checks;
+* :code:`check_argument()`; used to make one or more checks of a function's argument.
+
+You can also use a :code:`catch_check()` function, if you want to catch an exception or a warning the :code:`easycheck` function you use would raise (see examples `here <https://github.com/nyggus/easycheck/blob/master/docs/catch_exceptions_doctest.rst>`_). Sometimes, however, you will do better using a :code:`try-except` block to catch exceptions (`see examples <https://github.com/nyggus/easycheck/blob/master/docs/use_with_try_doctest.rst>`__).
+
+> Note that some :code:`easycheck` functions are simple wrappers around built-in functions, but their behavior is different, as they have the typical behavior of an :code:`easycheck` function: if a condition is not met, an exception is raised or an issue is raised.
+
+
+Assertions
+----------
+
+In addition to the above checking functions, :code:`easycheck` provides a set of functions for assertions. They can be used in both code and tests, just like regular assertions using the :code:`assert` statement. Assertion functions do have a specific functionality that makes them different from the corresponding check functions. You can read more about it `here <https://towardsdatascience.com/python-assertions-or-checking-if-a-cat-is-a-dog-ce11c55d143>`__. In short, assertions are called only in the development (non-production) mode, that is, when :code:`__debug__` is set to :code:`True`. An assertion should check a condition that should never happen; when the corresponding exception is raised, it means that something went wrong in the code, that something that should never happen has just happened.
+
+Some examples:
+
+You are working only on integers, for example pixels when rendering images, or placing objects on a board. You are sure that output will be integer, so you can assert on integers:
+
+.. code-block:: python
+    
+    def convert_to_pixel_position(real_pos: tuple[float, float]):
+        pos_x = real_pos[0]
+        pos_y = real_pos[1]
+        pixel_pos_x = round(pos_x)
+        pixel_pos_y = round(pos_y)
+        return pixel_pos_x, pixel_pos_y
+
+    pos = convert_to_pixel_position((1.2, 3.4))
+    assert_type(pos, tuple)
+    assert_type(pos[0], int)
+
+Now consider a different example. Imagine you have output from some `len()` method, or any other method calculating the length of something:
+
+.. code-block:: python
+
+    out = len(example_object)
+    # doing something with out, like
+    number_of_elements_required = out * no_of_objects
+    assert_type(out_for_something_else, int)
+
+You are working on subset of some data. So the size of the data should not be larger than the initial one, but also not smaller than 0:
+
+.. code-block:: python
+
+    def subset_of(data: pd.DataFrame, filter_condition: callable) -> pd.DataFrame:
+        # create a data frame that is a subset of `data` based on `filter_condition`
+        ...
+    x = pd.DataFrame({'x': [1, 2, 4], 'y': [3, 3, 5]})
+    x_subset = subset_of(x, lambda value: value < 3)
+    assert_if_in_limits(len(x_subset), 0, len(x))
+
+Here is full list of supported assert functions:
+
+* :code:`assert_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
+* :code:`assert_if_not()`; the opposite of :code:`assert_if()`, helpful when you need to assure that a condition is *not* met;
+* :code:`assert_if_isclose()`; to assert whether two floating-point numbers are close enough, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`__);
+* :code:`assert_if_in_limits()`; to assert whether a number is in range of two other numbers;
+* :code:`assert_length()`; to assert length (equal to, smaller than, greater than, and the like);
+* :code:`assert_type()`;to assert that an object has a particular type, as you would do using :code:`assert isinstance`;
+* :code:`assert_paths()`; to assert that a path exists or paths exist.
+
+Use in code to issue warnings
+-----------------------------
+
+In order to issue a warning if a condition is violated, simply use a warning class (in the :code:`handle_with` argument) instead of an exception class:
+
+.. code-block:: python
+
+    check_if(2 > 1, Warning, 'Too high a value')
+    check_length([1, 2, 3], 10, Warning, 'Too short list with data')
+
+Remember to always use a message with warnings, in order to make them meaningful. (See more in `use_with_warnings_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_with_warnings_doctest.rst>`_).
+
+
+Of course, you can use a custom warning:
+
+.. code-block:: python
+
+    class TooSmallSampleSize(Warning):
+        """Results for samples size below 100 can be unstable."""
+    
+    n = 50
+    check_if(n >= 100, TooSmallSampleSize)
+    ... TooSmallSampleSize: Results for samples size below 100 can be unstable.
+      warnings.warn(message, error)
+
+
+Use in code, an example
+-----------------------
+
+Imagine you want to connect to a database; if the connection fails for any reason, you want to read an archived flat file. (We will use some undefined functions whose names will clearly convey what the functions do.)
+
+.. code-block:: python
+
+    from easycheck import check_if, check_if_paths_exist
+    
+    class DataBaseConnectionError(Exception):
+        pass
+    
+    def get_data_from_db(db_details, db_credentials):
+        try:
+            connect_to_db(db_details, db_credentials)
+        except:
+            return False
+        data = get_records_from_db()
+        return data
+
+The :code:`easycheck` code could look like the following:
+
+.. code-block:: python
+
+    def get_data(db_details, db_credentials):
+        data = get_data_from_db(db_details, db_credentials)
+        check_if(
+            data,
+            handle_with=DataBaseConnectionError,
+            message='Cannot communicate with the database'
+            )
+        return data
+              
+You can of course handle this exception, for example like here:
+
+.. code-block:: python
+
+    def get_data(db_details, db_credentials, archived_data_file):
+        data = get_data_from_db(db_details, db_credentials)
+        try:
+            check_if(
+                data,
+                handle_with=DataBaseConnectionError,
+                message='Cannot communicate with the database'
+            )
+        except DataBaseConnectionError:
+            check_if_paths_exist(archived_data_file)
+            with open(archived_data_file) as f:
+                data = f.readlines()
+        return data
+    
+Of course, you might use here a dedicated context manager. Sure, you can write it in a shorter way, without :code:`easycheck`, but the flow of information will not be as smooth, resulting in less readability:
+
+.. code-block:: python
+
+    def get_data(db_details, db_credentials, archived_data_file):
+        data = get_data_from_db(db_details, db_credentials)
+        if not data:
+            with open(archived_data_file) as f:
+                data = f.readlines()
+        return data
+
+Of course, the :code:`open()` context manager will itself throw an error, but when you use the :code:`check_if()` function and explicitly define an exception class, you clearly show the reader that you're checking if this file exists and raise a particular exception if it doesn't.
+        
+Use in testing
+--------------
+
+As mentioned above, most :code:`easycheck` functions have their asserts counterparts which can be used in testing. Of course, you can use :code:`check_if()`, but to align with the common use of assertions, the :code:`easycheck` module offers those aliases so that the reader will immediately see that you're using these functions to test. Consider these examples:
+
+.. code-block:: python
+
+    # Using assertions
+    def test_something():
+        a, b = my_function_1(), my_function_2()
+
+        assert a == 2; 
+        assert isinstance(a, int)
+        assert isinstance(b, tuple)
+        assert len(b) == 5
+		
+    # Using easycheck assert-like functions:
+    def test_something():
+        a, b = my_function_1(), my_function_2()
+        
+        assert_if(a == 2)
+        assert_type(a, int)
+        assert_type(b, tuple)
+        assert_length(b, 5)
+
+Note that only the first one will raise :code:`AssertionError` while the others will raise more meaningful errors (:code:`TypeError` and :code:`LengthError`), which may better explain the reasons that the tests did not pass.
+
+You will find more about using :code:`easycheck` in `use_in_testing_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_in_testing_doctest.rst>`_.
+
+Other examples
+--------------
+
+You will find a number of examples in `doctest files <https://github.com/nyggus/easycheck/tree/master/docs/>`_, which also serve as doctests.
+
+
+Switching off :code:`easycheck`
+-------------------------------
+
+If you want to maximize performance, you may wish to switch off :code:`easycheck` checks. You would get the greatest increase in performance by removing (or commenting out) all calls to :code:`easycheck` functions, but this can be inconvenient. Hence, :code:`easycheck` offers you a more convenient way of doing so, namely, switching off via an environmental variable. This will be less efficient, as this will mean calling an empty function instead of actual :code:`easycheck` functions. While not the most performant, this approach can increase performance quite significantly. Its obvious advantage is that you do not need to do anything else than just setting the :code:`"EASYCHECK_RUN"` environmental variable to :code:`"0"`:
+
+.. code-block:: shell
+
+    > EASYCHECK_RUN = 0
+    > python my_script.py
+
+The my_script.py script will be run with all :code:`easycheck` functions replaced with an empty function.
+
+You can also switch off easycheck directly from Python:
+
+.. code-block:: python
+
+    import os
+
+    os.environ["EASYCHECK_RUN"] = "0"
+
+> **Warning**: Do remember to use this option wisely. While it will increase performance, it can also change the behavior of the Python program.
+
+
+Changelog
+---------
+
+* Version 0.6.0 came with significant optimization of performance. Before, :code:`easycheck` functions performed internal checks of the argument values provided to the function call. Most of these checks are not performed anymore, at least not for the most significant :code:`easycheck` functions, such as :code:`check_if()` or :code:`check_type()`. Some checks, however, are still done. These are mainly checks without which the behavior of the function would be either unwanted or unexpected. We decided to remove all checks that do not change much; for instance, they raise an error due to an incorrect type of an argument value — even though it would be raised anyway, but by the internal Python process, not by the :code:`easycheck` function itself. The point is to remove such unnecessary checks and that way remove the unnecessary :code:`if` blocks, which certainly add some cost to execution time. While one such check costs almost nothing, many of them (e.g., in a long loop) can mean a significant cost. As of version 0.6.0, we will try to optimize the performance of :code:`easycheck` by getting rid of such overhead costs, unless they are important for the behavior of the corresponding :code:`easycheck` function.
```

### Comparing `easycheck-0.7.0/easycheck/__init__.py` & `easycheck-0.9.1/easycheck/__init__.py`

 * *Files identical despite different names*

### Comparing `easycheck-0.7.0/easycheck/easycheck.py` & `easycheck-0.9.1/easycheck/easycheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 statement, you can use easycheck functions within code.
 
 The module also offers aliases to be used in testing, all of which have the
 word "assert" in their names (assert_if(), assert_if_not(),
 assert_type(), assert_length(), and assert_path()).
 """
 import builtins
+import os
 import warnings
 
 from collections.abc import Iterable, Callable
+from functools import wraps
 from math import isclose
 from numbers import Number
 from operator import eq, le, lt, gt, ge, ne, is_, is_not
 from pathlib import Path
 
+
 class LimitError(Exception):
     """Number out of limit."""
 
 
 class LengthError(Exception):
     """Violated length check."""
 
@@ -30,26 +33,43 @@
 class ComparisonError(Exception):
     """The comparison is not true."""
 
 
 class NotCloseEnoughError(Exception):
     """The two float numbers are not close enough."""
 
+
 class ArgumentValueError(Exception):
     """Argument's value is incorrect."""
 
 
+def switch(func):
+    """Decorator to switch off all easycheck checks.
+
+    It does so by getting the EASYCHECK_RUN environmental variable.
+    When it's set to "0", easycheck is switched off.
+    """
+
+    @wraps(func)
+    def inner(*args, **kwargs):
+        if os.environ.get("EASYCHECK_RUN", 1) != "0":
+            return func(*args, **kwargs)
+
+    return inner
+
+
+@switch
 def check_if(condition, handle_with=AssertionError, message=None):
     """Check if a condition is true.
 
     Args:
         condition (bool): condition to check.
         handle_with (type): the type of exception to be raised or warning to
             be issued
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
 
     Returns:
         None, if check succeeded.
 
@@ -103,21 +123,22 @@
     ...     assert_if("2 is not smaller than 1" in str(w[-1].message))
     """
     __tracebackhide__ = True
     if not condition:
         _raise(handle_with, message)
 
 
+@switch
 def check_if_not(condition, handle_with=AssertionError, message=None):
     """Check if a condition is not true.
 
     Args:
         condition (bool): condition to check.
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
 
 
     Returns:
         None, if check succeeded.
@@ -170,36 +191,37 @@
     >>> with warnings.catch_warnings(record=True) as w:
     ...     check_if_not(2 > 1, Warning, '2 is bigger than 1')
     ...     assert_if("2 is bigger than 1" in str(w[-1].message))
     """
     __tracebackhide__ = True
     if condition:
         _raise(handle_with, message)
-    
 
+
+@switch
 def check_if_in_limits(
-    x, 
-    lower_limit = float('-inf'), 
-    upper_limit = float('inf'), 
-    handle_with=LimitError, 
+    x,
+    lower_limit=float("-inf"),
+    upper_limit=float("inf"),
+    handle_with=LimitError,
     message=None,
-    include_equal=True   
+    include_equal=True,
 ):
     """Check if number is in range of limits
-    
+
     Args:
         x (float): number to be checked if it's within specified limits
         lower_limit (float): the lower limit of the interval
         upper_limit (float): the upper limit of the interval
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
-        include_equal (bool): True for strict checks (lower ≤ x ≤ upper), 
+        include_equal (bool): True for strict checks (lower ≤ x ≤ upper),
         False otherwise (lower < x < upper)
 
     Returns:
         None, if check succeeded.
 
     Raises:
         Exception of the type provided by the handle_with parameter, LengthError
@@ -229,29 +251,31 @@
         condition = lower_limit <= x <= upper_limit
     else:
         condition = lower_limit < x < upper_limit
 
     if not condition:
         _raise(handle_with, message)
 
+
+@switch
 def check_length(
     item,
     expected_length,
     handle_with=LengthError,
     message=None,
     operator=eq,
     assign_length_to_others=False,
 ):
     """Compare item's length with expected_length, using operator.
 
     Args:
         item: the object whose length we want to validate
         expected_length (int): the expected length of the item
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
         operator: one of the functions returned by get_possible_operators()
         assign_length_to_others (bool): treat all numeric types as having the
             length of 1. If False, any attempt to validate a numeric type
             will raise an exception/warning, as numeric types don't implement
@@ -284,22 +308,23 @@
             item = [item]
 
     condition = operator(len(item), expected_length)
     if not condition:
         _raise(handle_with, message)
 
 
+@switch
 def check_type(item, expected_type, handle_with=TypeError, message=None):
     """Check if item has the type of expected_type.
 
     Args:
         item: the object whose type we want to validate
         expected_type (type, Iterable[type]): the expected type of the item
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
 
     Returns:
         None, if check succeeded.
 
@@ -357,46 +382,52 @@
             return None
         expected_type = tuple(t for t in expected_type if t is not None)
 
     if not isinstance(item, expected_type):
         _raise(handle_with, message)
 
 
-def check_if_isclose(x, y, /,
-                     handle_with=NotCloseEnoughError,
-                     message=None,
-                     rel_tol=1e-09, abs_tol=0.0):
+@switch
+def check_if_isclose(
+    x,
+    y,
+    /,
+    handle_with=NotCloseEnoughError,
+    message=None,
+    rel_tol=1e-09,
+    abs_tol=0.0,
+):
     """Check if two floats are close in value.
-    
+
     The function is just a wrapper around math.isclose(), and its defaults
     are exactly the same. Two values (x and y, both being positional-only
     parameters) will be considered close when the difference between them
     (either relative or absolute) is smaller than at least one of the
     tolerances. If you do not want to use any of the two tolerances, set it
     to 0.
-    
+
     Note: Before applying math.isclose(), x and y are first converted to
     floats, so you can provide them as integers or even strings.
-    
+
     At least one tolerance needs to be provided (so not be zero); otherwise
     the function will do nothing.
-    
+
     Unlike most easycheck functions, check_if_isclose() uses two
     positional-only and four keyword-only arguments. So when providing one of
     the two tolerances, you have to specify it using the argument's name. You
     have to do the same also for handle_with and message.
-    
+
     Args:
         x, y (float): two numbers to compare
         rel_tol (float): maximum difference for being considered "close",
             relative to the magnitude of the input values
         abs_tol (float): maximum difference for being considered "close",
             regardless of the magnitude of the input values
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
 
     Returns:
         None, if check succeeded.
 
@@ -406,15 +437,15 @@
 
     >>> check_if_isclose(1.12, 1.12, rel_tol=1e-09)
     >>> check_if_isclose('1.12', '1.12', rel_tol=1e-09)
     >>> check_if_isclose(1.12, 1.13, rel_tol=1e-09)
     Traceback (most recent call last):
         ...
     NotCloseEnoughError: The two float numbers are not close enough.
-    
+
     >>> check_if_isclose(1.12, 1.13, rel_tol=.05)
     >>> check_if_isclose(1.12, 1.13, abs_tol=.05)
     >>> check_if_isclose(1.12, 1.13, abs_tol=.005)
     Traceback (most recent call last):
         ...
     NotCloseEnoughError: The two float numbers are not close enough.
 
@@ -432,27 +463,28 @@
     x = float(x)
     y = float(y)
 
     if not isclose(x, y, rel_tol=rel_tol, abs_tol=abs_tol):
         _raise(handle_with, message)
 
 
+@switch
 def check_if_paths_exist(
     paths, handle_with=FileNotFoundError, message=None, execution_mode="raise"
 ):
     """Check if a path or paths exist.
 
     If it does not, either raise (or return) an exception or issue (or return)
     a warning.
 
     Args:
         paths (str, pathlib.Path, Iterable[str or pathlib.Path]): path or paths
             to validate
         handle_with (type): type of exception or warning to be raised/returned
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
         execution_mode (str): defines what happens if not all the paths exist
             May take one of the following values:
                 - 'raise': exception/warning will be raised
                 - 'return': function will return information about the errors
@@ -494,16 +526,15 @@
     ...    execution_mode='return',
     ...    handle_with=Warning,
     ...    message='Attempt to use a non-existing path')
     (Warning('Attempt to use a non-existing path'), ['Q:/Op/Oop'])
     """
     __tracebackhide__ = True
     if not execution_mode in ("raise", "return"):
-        _raise(ValueError,
-               "execution_mode must be either 'raise' or 'return'")
+        _raise(ValueError, "execution_mode must be either 'raise' or 'return'")
 
     is_allowed_type = isinstance(paths, (str, Path)) or (
         isinstance(paths, Iterable)
         and all(isinstance(path, (str, Path)) for path in paths)
     )
 
     if not is_allowed_type:
@@ -531,25 +562,26 @@
             else:
                 error = handle_with()
 
     if execution_mode == "return":
         return error, non_existing_paths
 
 
+@switch
 def check_comparison(
     item_1, operator, item_2, handle_with=ValueError, message=None
 ):
     """Check if a comparison of two items is true.
 
     Args:
         item_1: the first item to compare
         operator: one of the functions returned by get_possible_operators()
         item_2: the second item to compare
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
 
     Returns:
         None, if check succeeded.
 
@@ -586,14 +618,15 @@
     ...     assert_if("Not less" in str(w[-1].message))
     """
     __tracebackhide__ = True
     if not operator(item_1, item_2):
         _raise(handle_with, message)
 
 
+@switch
 def check_all_ifs(*args):
     """Check all multiple conditions and return all checks.
 
     Args:
         args: tuples of the form (check_function, arguments), where:
             - arguments is a tuple of arguments to be passed to a
               check_function
@@ -668,14 +701,15 @@
             run_this_check = e
 
         results_of_checks[f"{i + 1}: {function.__name__}"] = run_this_check
 
     return results_of_checks
 
 
+@switch
 def check_argument(
     argument,
     argument_name=None,
     expected_type=None,
     expected_choices=None,
     expected_length=None,
     handle_with=ArgumentValueError,
@@ -690,15 +724,15 @@
             function. If argument_name is not defined, the error messages will
             not include the name of the argument, but will instead only report
             the default text 'argument'
         expected_type (type, Iterable[type]): the expected type of the item
         expected_choices (Iterable): a list of acceptable values of argument
         expected_length (int): the expected length of the item
         handle_with (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
         **kwargs: additional arguments passed to check_length (i.e.,
             operator=eq and assign_length_to_others)
 
     Returns:
@@ -777,48 +811,52 @@
         message="argument_name must be string",
     )
 
     if expected_type is not None:
         instance_message = (
             message
             or f"Incorrect type of {argument_name}; valid type(s):"
-               f" {expected_type}"
-            )
+            f" {expected_type}"
+        )
         check_type(
             item=argument,
             expected_type=expected_type,
             handle_with=handle_with,
             message=instance_message,
         )
     if expected_choices is not None:
         choices_message = (
             message
             or f"{argument_name}'s value, {argument}, "
-               f"is not among valid values: {expected_choices}."
-            )
+            f"is not among valid values: {expected_choices}."
+        )
         if argument not in expected_choices:
             _raise(handle_with, choices_message)
     if expected_length is not None:
         length_message = (
             message
             or f"Unexpected length of {argument_name}"
-               f" (should be {expected_length})"
-            )
+            f" (should be {expected_length})"
+        )
         check_length(
             item=argument,
             expected_length=expected_length,
             handle_with=handle_with,
             message=length_message,
             **kwargs,
         )
 
 
+@switch
 def catch_check(check_function, *args, **kwargs):
     """Catch an exception or warning raised/issued by a easycheck function.
 
+    Warning: Be aware that catch_check() is a relatively slow function
+             compared to most other easycheck functions.
+
     Args:
         check_function: function to call (one of the public easycheck functions)
         args: positional arguments to pass on to check_function
         kwargs: keyword arguments to pass on to check_function
 
     Returns:
         Exception or warning instance
@@ -910,14 +948,16 @@
         argument=check_function,
         argument_name=check_function.__name__,
         expected_choices=(
             check_if,
             assert_if,
             check_if_not,
             assert_if_not,
+            check_if_isclose,
+            assert_if_isclose,
             check_if_in_limits,
             assert_if_in_limits,
             check_argument,
             check_comparison,
             check_if_paths_exist,
             assert_paths,
             check_type,
@@ -937,20 +977,21 @@
             check_function(*args, **kwargs)
         if possible_warn:
             return possible_warn[-1].message
     except Exception as e:
         return e
 
 
+@switch
 def _raise(error, message=None):
     """Raise exception or issue a warning, with or without message.
 
     Args:
         error (type): the type of exception or warning to be raised
-        message (str): a text to use as the exception/warning message. 
+        message (str): a text to use as the exception/warning message.
             Defaults to None, which means using no message for built-in
             exceptions/warnings, and the docstrings of the exception/warning
             class as a message for custom exceptions.
 
     Raises:
         Exception of the type provided by the error parameter
         TypeError if error parameter is not an exception or warning class
@@ -976,17 +1017,15 @@
     ...    assert_if('Warning' in str(w[-1].message))
     >>> with warnings.catch_warnings(record=True) as w:
     ...    _raise(Warning, 'Watch out! Something might be wrong.')
     ...    assert_if('Watch out!' in str(w[-1].message))
     """
     __tracebackhide__ = True
     if not isinstance(error, type) or not issubclass(error, Exception):
-        raise TypeError(
-            "The error argument must be an exception or a warning"
-        )
+        raise TypeError("The error argument must be an exception or a warning")
 
     if message is None:
         # Use docstring as a message only for custom exceptions.
         if error.__name__ not in dir(builtins):
             message = error.__doc__
     elif isinstance(message, str):
         if not message:
@@ -1023,26 +1062,60 @@
     8
     """
     return eq, le, lt, gt, ge, ne, is_, is_not
 
 
 # Aliases to be used for testing. Beware not to use warnings with them.
 
-assert_if = check_if
-assert_if_not = check_if_not
-assert_if_in_limits = check_if_in_limits
-assert_length = check_length
-assert_type = check_type
-assert_paths = check_if_paths_exist
-assert_if_isclose = check_if_isclose
+def make_it_true_assertion(func):
+    @wraps(func)
+    def assert_func(*args, **kwargs):
+        if __debug__:
+            return func(*args, **kwargs)
+    return assert_func
+
+@switch
+@make_it_true_assertion
+def assert_if(*args, handle_with=AssertionError, **kwargs): 
+    return check_if(*args, handle_with=handle_with, **kwargs)
+
+@switch
+@make_it_true_assertion
+def assert_if_not(*args, handle_with=AssertionError, **kwargs):
+    return check_if_not(*args, handle_with=handle_with, **kwargs)
+
+@switch
+@make_it_true_assertion
+def assert_if_in_limits(*args, handle_with=AssertionError, **kwargs):
+    return check_if_in_limits(*args, handle_with=handle_with, **kwargs)
+
+@switch
+@make_it_true_assertion
+def assert_length(*args, handle_with=AssertionError, **kwargs):
+    return check_length(*args, handle_with=handle_with, **kwargs)
+
+@switch
+@make_it_true_assertion
+def assert_type(*args, handle_with=AssertionError, **kwargs):
+    return check_type(*args, handle_with=handle_with, **kwargs)
+
+@switch
+@make_it_true_assertion
+def assert_paths(*args, handle_with=AssertionError, **kwargs):
+    return check_if_paths_exist(*args, handle_with=handle_with, **kwargs)
+
+@switch
+@make_it_true_assertion
+def assert_if_isclose(*args, handle_with=AssertionError, **kwargs):
+    return check_if_isclose(*args, handle_with=handle_with, **kwargs)
 
 # Alias to ensure backward compatibility
 
 check_instance = check_type
 assert_instance = assert_type
 
 
 if __name__ == "__main__":
     import doctest
-    
+
     flags = doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
     doctest.testmod(optionflags=flags)
```

### Comparing `easycheck-0.7.0/easycheck/tmp.py` & `easycheck-0.9.1/easycheck/tmp.py`

 * *Files identical despite different names*

### Comparing `easycheck-0.7.0/easycheck.egg-info/PKG-INFO` & `easycheck-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 Metadata-Version: 2.1
 Name: easycheck
-Version: 0.7.0
+Version: 0.9.1
 Summary: A tool for checking conditions in Python
 Home-page: https://github.com/nyggus/easycheck
-Author: Nyggus & Ke Boan
+Author: Nyggus, Ke Boan & Darsoo
 Author-email: nyggus@gmail.com
 License: MIT
 Description: easycheck
         =========
+        .. image:: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml/badge.svg
+           :target: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml
+        .. image:: https://codecov.io/github/nyggus/easycheck/branch/master/graph/badge.svg?token=EH4TLHQQWC 
+           :target: https://codecov.io/github/nyggus/easycheck
+        .. image:: https://img.shields.io/pypi/l/easycheck.svg
+           :target: https://pypi.org/project/easycheck     
+        .. image:: https://img.shields.io/pypi/v/easycheck.svg
+           :target: https://pypi.org/project/easycheck     
+        .. image:: https://img.shields.io/pypi/wheel/easycheck
+           :target: https://pypi.org/project/easycheck     
+        .. image:: https://img.shields.io/pypi/pyversions/easycheck
+           :target: https://pypi.org/project/easycheck
+        .. image:: https://img.shields.io/github/stars/nyggus/easycheck?style=social
+           :target: https://github.com/nyggus/easycheck
+        .. image:: https://img.shields.io/github/last-commit/nyggus/easycheck
         
-        The :code:`easycheck` package offers a lightweight tool for running functionized checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases (starting off with :code:`assert_` instead of :code:`check_`).
+        The :code:`easycheck` package offers a lightweight tool for running functionized checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases (starting off with :code:`assert_` instead of :code:`check_`). You can also switch off all :code:`easycheck` checks, by setting the :code:`"EASYCHECK_RUN"` environmental variable to :code:`"0"`.
         
         The idea is to use the :code:`easycheck` functions to check conditions that are _not_ assertions. The checks work in the following general way: When a condition is met, nothing happens (in fact, the function returns :code:`None`); if it is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
         
         * Assertions are meant to be used conditions that _must_ be true (when only the code is correct). So, if an assertion is incorrect, it means something is wrong with the code. You should never use assertions to handle regular exceptions, like those related to data or arguments.
         * Unlike assertions, :code:`easycheck` functions are to be used to check conditions related to things like data and argument values, and to handle regular exceptions.
         * While assertions only raise :code:`AssertionError`, you can choose any exception to be raised by easycheck functions.
         * When using :code:`easycheck`, instead of raising an exception, you can issue a warning.
@@ -128,32 +143,84 @@
         
         .. code-block:: python
         
             check_length([1, 2, 3], 1)
         	
         will raise :code:`LengthError` (an exception class defined in the :code:`easycheck` module).
         
-        Here is a list of :code:`easycheck` functions the module offers, along with their aliases to be used for testing:
+        Here is a list of :code:`easycheck` check functions the module offers, discluding assertions, which are listed in the next paragraph:
         
-        * :code:`check_if()`, with the alias of :code:`assert_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
-        * :code:`check_if_not()`, with the alias of :code:`assert_if_not()`; the opposite of :code:`check_if()`, helpful when you need to assure that a condition is _not_ met;
-        * :code:`check_if_isclose()`, with the alias of :code:`assert_if_isclose()`; to compare two floating-point numbers, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`_);
-        * :code:`check_if_in_limits()`, with the alias of :code:`assert_if_in_limits()`;
-        * :code:`check_length()`, with the alias of :code:`assert_length()`; to compare length (equal to, smaller than, greater than, and the like);
-        * :code:`check_type()`, with the alias of :code:`assert_type()`; to check expected type, similar to :code:`isinstance()`;
-        * :code:`check_if_paths_exist()`, with the alias of :code:`assert_paths()`; to compare paths (or just one path) exist;
-        * :code:`check_comparison()` (used to compare two items); to compare to objectsm just like you would do using :code:`if obj1 != obj2: raise`
+        * :code:`check_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
+        * :code:`check_if_not()`; the opposite of :code:`check_if()`, helpful when you need to assure that a condition is *not* met;
+        * :code:`check_if_isclose()`; to compare two floating-point numbers, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`__);
+        * :code:`check_if_in_limits()`; to check if a number lies between two other numbers;
+        * :code:`check_length()`; to compare length (equal to, smaller than, greater than, and the like);
+        * :code:`check_type()`; to check expected type, similar to :code:`isinstance()`;
+        * :code:`check_if_paths_exist()`; to compare paths (or just one path) exist;
+        * :code:`check_comparison()` (used to compare two items); to compare two objects, just like you would do using :code:`if obj1 != obj2: raise`
         * :code:`check_all_ifs()`; used to check multiple conditions and return all the checks;
         * :code:`check_argument()`; used to make one or more checks of a function's argument.
         
-        You can also use a :code:`catch_check()` function, if you want to catch an exception or a warning the :code:`easycheck` function you use would raise (see examples `here <https://github.com/nyggus/easycheck/blob/master/docs/catch_exceptions_doctest.rst>`_). Sometimes, however, you will do better using a :code:`try-except` block to catch exceptions (`see examples <https://github.com/nyggus/easycheck/blob/master/docs/use_with_try_doctest.rst>`_).
+        You can also use a :code:`catch_check()` function, if you want to catch an exception or a warning the :code:`easycheck` function you use would raise (see examples `here <https://github.com/nyggus/easycheck/blob/master/docs/catch_exceptions_doctest.rst>`_). Sometimes, however, you will do better using a :code:`try-except` block to catch exceptions (`see examples <https://github.com/nyggus/easycheck/blob/master/docs/use_with_try_doctest.rst>`__).
         
         > Note that some :code:`easycheck` functions are simple wrappers around built-in functions, but their behavior is different, as they have the typical behavior of an :code:`easycheck` function: if a condition is not met, an exception is raised or an issue is raised.
         
         
+        Assertions
+        ----------
+        
+        In addition to the above checking functions, :code:`easycheck` provides a set of functions for assertions. They can be used in both code and tests, just like regular assertions using the :code:`assert` statement. Assertion functions do have a specific functionality that makes them different from the corresponding check functions. You can read more about it `here <https://towardsdatascience.com/python-assertions-or-checking-if-a-cat-is-a-dog-ce11c55d143>`__. In short, assertions are called only in the development (non-production) mode, that is, when :code:`__debug__` is set to :code:`True`. An assertion should check a condition that should never happen; when the corresponding exception is raised, it means that something went wrong in the code, that something that should never happen has just happened.
+        
+        Some examples:
+        
+        You are working only on integers, for example pixels when rendering images, or placing objects on a board. You are sure that output will be integer, so you can assert on integers:
+        
+        .. code-block:: python
+            
+            def convert_to_pixel_position(real_pos: tuple[float, float]):
+                pos_x = real_pos[0]
+                pos_y = real_pos[1]
+                pixel_pos_x = round(pos_x)
+                pixel_pos_y = round(pos_y)
+                return pixel_pos_x, pixel_pos_y
+        
+            pos = convert_to_pixel_position((1.2, 3.4))
+            assert_type(pos, tuple)
+            assert_type(pos[0], int)
+        
+        Now consider a different example. Imagine you have output from some `len()` method, or any other method calculating the length of something:
+        
+        .. code-block:: python
+        
+            out = len(example_object)
+            # doing something with out, like
+            number_of_elements_required = out * no_of_objects
+            assert_type(out_for_something_else, int)
+        
+        You are working on subset of some data. So the size of the data should not be larger than the initial one, but also not smaller than 0:
+        
+        .. code-block:: python
+        
+            def subset_of(data: pd.DataFrame, filter_condition: callable) -> pd.DataFrame:
+                # create a data frame that is a subset of `data` based on `filter_condition`
+                ...
+            x = pd.DataFrame({'x': [1, 2, 4], 'y': [3, 3, 5]})
+            x_subset = subset_of(x, lambda value: value < 3)
+            assert_if_in_limits(len(x_subset), 0, len(x))
+        
+        Here is full list of supported assert functions:
+        
+        * :code:`assert_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
+        * :code:`assert_if_not()`; the opposite of :code:`assert_if()`, helpful when you need to assure that a condition is *not* met;
+        * :code:`assert_if_isclose()`; to assert whether two floating-point numbers are close enough, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`__);
+        * :code:`assert_if_in_limits()`; to assert whether a number is in range of two other numbers;
+        * :code:`assert_length()`; to assert length (equal to, smaller than, greater than, and the like);
+        * :code:`assert_type()`;to assert that an object has a particular type, as you would do using :code:`assert isinstance`;
+        * :code:`assert_paths()`; to assert that a path exists or paths exist.
+        
         Use in code to issue warnings
         -----------------------------
         
         In order to issue a warning if a condition is violated, simply use a warning class (in the :code:`handle_with` argument) instead of an exception class:
         
         .. code-block:: python
         
@@ -239,15 +306,15 @@
                 return data
         
         Of course, the :code:`open()` context manager will itself throw an error, but when you use the :code:`check_if()` function and explicitly define an exception class, you clearly show the reader that you're checking if this file exists and raise a particular exception if it doesn't.
                 
         Use in testing
         --------------
         
-        As mentioned above, most :code:`easycheck` functions have aliases to be used in testing. Of course, you can use :code:`check_if()`, but to align with the common use of assertions, the :code:`easycheck` module offers those aliases so that the reader will immediately see that you're using these functions to test. Consider these examples:
+        As mentioned above, most :code:`easycheck` functions have their asserts counterparts which can be used in testing. Of course, you can use :code:`check_if()`, but to align with the common use of assertions, the :code:`easycheck` module offers those aliases so that the reader will immediately see that you're using these functions to test. Consider these examples:
         
         .. code-block:: python
         
             # Using assertions
             def test_something():
                 a, b = my_function_1(), my_function_2()
         
@@ -271,18 +338,42 @@
         
         Other examples
         --------------
         
         You will find a number of examples in `doctest files <https://github.com/nyggus/easycheck/tree/master/docs/>`_, which also serve as doctests.
         
         
+        Switching off :code:`easycheck`
+        -------------------------------
+        
+        If you want to maximize performance, you may wish to switch off :code:`easycheck` checks. You would get the greatest increase in performance by removing (or commenting out) all calls to :code:`easycheck` functions, but this can be inconvenient. Hence, :code:`easycheck` offers you a more convenient way of doing so, namely, switching off via an environmental variable. This will be less efficient, as this will mean calling an empty function instead of actual :code:`easycheck` functions. While not the most performant, this approach can increase performance quite significantly. Its obvious advantage is that you do not need to do anything else than just setting the :code:`"EASYCHECK_RUN"` environmental variable to :code:`"0"`:
+        
+        .. code-block:: shell
+        
+            > EASYCHECK_RUN = 0
+            > python my_script.py
+        
+        The my_script.py script will be run with all :code:`easycheck` functions replaced with an empty function.
+        
+        You can also switch off easycheck directly from Python:
+        
+        .. code-block:: python
+        
+            import os
+        
+            os.environ["EASYCHECK_RUN"] = "0"
+        
+        > **Warning**: Do remember to use this option wisely. While it will increase performance, it can also change the behavior of the Python program.
+        
+        
         Changelog
         ---------
         
         * Version 0.6.0 came with significant optimization of performance. Before, :code:`easycheck` functions performed internal checks of the argument values provided to the function call. Most of these checks are not performed anymore, at least not for the most significant :code:`easycheck` functions, such as :code:`check_if()` or :code:`check_type()`. Some checks, however, are still done. These are mainly checks without which the behavior of the function would be either unwanted or unexpected. We decided to remove all checks that do not change much; for instance, they raise an error due to an incorrect type of an argument value — even though it would be raised anyway, but by the internal Python process, not by the :code:`easycheck` function itself. The point is to remove such unnecessary checks and that way remove the unnecessary :code:`if` blocks, which certainly add some cost to execution time. While one such check costs almost nothing, many of them (e.g., in a long loop) can mean a significant cost. As of version 0.6.0, we will try to optimize the performance of :code:`easycheck` by getting rid of such overhead costs, unless they are important for the behavior of the corresponding :code:`easycheck` function.
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `easycheck-0.7.0/setup.py` & `easycheck-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 extras_requirements = {
     "dev": ["pytest", "wheel", "black"],
 }
 
 setuptools.setup(
     name="easycheck",
-    version="0.7.0",
-    author="Nyggus & Ke Boan",
+    version="0.9.1",
+    author="Nyggus, Ke Boan & Darsoo",
     author_email="nyggus@gmail.com",
     license="MIT",
     description="A tool for checking conditions in Python",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/nyggus/easycheck",
     packages=setuptools.find_packages(),
```

