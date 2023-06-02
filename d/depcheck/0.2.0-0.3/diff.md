# Comparing `tmp/depcheck-0.2.0.tar.gz` & `tmp/depcheck-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depcheck-0.2.0.tar", max compression
+gzip compressed data, was "depcheck-0.3.tar", max compression
```

## Comparing `depcheck-0.2.0.tar` & `depcheck-0.3.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0     1084 2021-08-24 14:11:00.189822 depcheck-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1605 2021-08-24 14:11:00.189822 depcheck-0.2.0/README.md
--rw-r--r--   0        0        0        0 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/__init__.py
--rw-r--r--   0        0        0     1499 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/depchecker.py
--rw-r--r--   0        0        0     6641 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/depchecker_test.py
--rw-r--r--   0        0        0     1087 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/main.py
--rw-r--r--   0        0        0     2720 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/models.py
--rw-r--r--   0        0        0     1333 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/readers.py
--rw-r--r--   0        0        0      139 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/util.py
--rw-r--r--   0        0        0      417 2021-08-24 14:11:00.189822 depcheck-0.2.0/depcheck/util_test.py
--rw-r--r--   0        0        0     1169 2021-08-24 14:11:00.189822 depcheck-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2627 2021-08-24 14:11:15.986445 depcheck-0.2.0/setup.py
--rw-r--r--   0        0        0     2649 2021-08-24 14:11:15.986918 depcheck-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-02 16:01:31.743776 depcheck-0.3/LICENSE.md
+-rw-r--r--   0        0        0     1804 2023-06-02 16:01:31.743776 depcheck-0.3/README.md
+-rw-r--r--   0        0        0     1279 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/depchecker.py
+-rw-r--r--   0        0        0     5513 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/models.py
+-rw-r--r--   0        0        0     1305 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/readers.py
+-rw-r--r--   0        0        0      139 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/util.py
+-rw-r--r--   0        0        0      417 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/util_test.py
+-rw-r--r--   0        0        0      963 2023-06-02 16:01:31.743776 depcheck-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 depcheck-0.3/PKG-INFO
```

### Comparing `depcheck-0.2.0/LICENSE.md` & `depcheck-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `depcheck-0.2.0/README.md` & `depcheck-0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 ![Depcheck: Dependency Checker](https://images2.imgbox.com/da/85/J5OEzbAH_o.jpg)
 
-Depcheck is a tool to check package-dependencies between predefined layers. 
-In the configuration file(`.depcheck.yml`) located in the project root, 
-which packages belong to which layers and allowed dependencies between 
-layers are configurable. In this way, you can enforce constraints and make sure to have decoupled architecture.
+Depcheck is a command line code-quality tool which supports adopting a 
+layered architecture by making it possible to specify dependency constraints
+between packages of your own Python application. 
+The tool aims to achieve the same goals as [Deptrac][deptrac] in PHP and [JDepend][jdepend] in Java
 
 ## Install
 Install from [Pypi][pypi-link] via `pip install depcheck`
-    
+
 ## Usage
 Let's say you have a project with the directory structure below:
 ```text
 example
     root
         foo
         bar
         main.py
         __init__.py
     README.md
     .gitignore
     .depcheck.yml
 ```
 Note: Package directories should contain **\_\_init\_\_.py** to be recognized as a package.
-- Navigate to the `exampe` then run `depcheck` for your project:
+- Navigate to the `example` then run `depcheck` for your project:
     ```shell
-    depcheck root
+    poetry run depcheck example -f .depcheck.ok.yml  # This should be correct
+    poetry run depcheck example -f .depcheck.errors.yml  # This should give errors
     ```
 - As you can see in the directory structure above, we have `.depcheck.yml` 
   configuration file in the project directory. If you would like to change 
   the path of the configuration file, use `-f` or `--file` argument:
     ```shell
     depcheck root -f /path/to/your/custom/depcheck.yml
     ```
@@ -39,7 +40,9 @@
 
 <!-- Links -->
 [hexagonal-architecture]: https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)
 [upgrade-python-version]: ./docs/upgrade-python-version.md
 [update-project-dependencies]: ./docs/upgrade-python-version.md
 [pypi-link]: https://pypi.org/project/depcheck/
 [contribution]: ./CONTRIBUTING.md
+[deptrac]: https://github.com/qossmic/deptrac
+[jdepend]: https://github.com/clarkware/jdepend
```

### Comparing `depcheck-0.2.0/depcheck/main.py` & `depcheck-0.3/depcheck/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 from depcheck.depchecker import DepChecker
 from depcheck.models import DependencyReport, Ruleset
 from depcheck.readers import DependencyReader, RulesetReader
 
 DEFAULT_CONFIG_FILE_PATH = ".depcheck.yml"
 
 
-def main() -> None:
-    parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
-    add_arguments(parser)
-    args = parser.parse_args()
-
-    print("# Reading ruleset...")
-    ruleset: Ruleset = RulesetReader(args.file).read()
-    print("# Reading project packages...")
-    dependency_report: DependencyReport = DependencyReader(ruleset, args.root_package).read()
-    print("# Checking dependencies...")
+def run_depcheck() -> None:
+    command_args = create_argument_parser().parse_args()
+    arg_config_file = command_args.file
+    arg_root_package = command_args.root_package
+
+    print(f"** Reading ruleset from '{arg_config_file}'")
+    ruleset: Ruleset = RulesetReader(arg_config_file).read()
+    print(f"** Reading project packages from root package: '{arg_root_package}'")
+    dependency_report: DependencyReport = DependencyReader(ruleset, arg_root_package).read()
+    print("** Checking dependencies")
     DepChecker(ruleset, dependency_report).run()
 
 
-def add_arguments(parser: ArgumentParser) -> None:
-    parser.add_argument("root_package", help="Root package of the project")
+def create_argument_parser() -> ArgumentParser:
+    parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
 
+    parser.add_argument("root_package", help="Root package of the project")
     parser.add_argument(
         "-f",
         "--file",
         default=DEFAULT_CONFIG_FILE_PATH,
         help="Path to the config file that includes layers and rules.",
     )
 
+    return parser
+
 
-if __name__ == "__main__":
-    main()
+run_depcheck() if __name__ == "__main__" else None
```

### Comparing `depcheck-0.2.0/depcheck/models.py` & `depcheck-0.3/depcheck/depchecker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,56 @@
-from typing import Any, Dict, List, Set
+import sys
+from typing import List, Set
 
-from depcheck.util import flatten
+from depcheck.models import DependencyReport, Ruleset
 
 
-class Ruleset:
-    __rules: Dict[str, List[str]]
-    __layers: Dict[str, List[str]]
-
-    def __init__(self, layers: Dict[str, List[str]], rules: Dict[str, List[str]]) -> None:
-        self.__rules = rules
-        self.__layers = layers
-
-    def layer_packages(self, layer: str) -> List[str]:
-        return self.layers.get(layer, [])
-
-    def whitelist(self, layer: str) -> List[str]:
-        return self.rules.get(layer, [])
-
-    @property
-    def rules(self) -> Dict[str, List[str]]:
-        return self.__rules
-
-    @property
-    def layers(self) -> Dict[str, List[str]]:
-        return self.__layers
-
-
-class DependencyReport:
+class DepChecker:
     __ruleset: Ruleset
-    __graph: Dict[str, Any]
-    __all_packages: List[str]
+    __dependency_report: DependencyReport
 
-    def __init__(self, ruleset: Ruleset, dependency_graph: Dict[str, Any]) -> None:
+    def __init__(self, ruleset: Ruleset, dependency_report: DependencyReport) -> None:
         self.__ruleset = ruleset
-        self.__graph = dependency_graph
-        self.__all_packages = list(self.__graph.keys())
-
-    def layer_dependencies(self, layer: str) -> Set[str]:
-        layer_packages: Set[str] = self.__layer_packages([layer])
-        layer_dependencies = self.__package_dependencies(layer_packages)
-
-        return self.__exclude_inner_dependencies(layer_dependencies, layer_packages)
-
-    def whitelist(self, layer: str) -> Set[str]:
-        whitelist: List[str] = self.__ruleset.whitelist(layer)
-
-        return self.__layer_packages(whitelist)
-
-    @property
-    def root_package(self) -> str:
-        return self.__graph["__main__"]["imports"][0]
-
-    @staticmethod
-    def __exclude_inner_dependencies(raw_dependencies: Set[str], layers: Set[str]) -> Set[str]:
-        return raw_dependencies - layers
-
-    def __layer_packages(self, layers: List[str]) -> Set[str]:
-        if layers is None:
-            return set()
-
-        # Packages within given layers
-        layer_packages: List[str] = flatten([self.__ruleset.layer_packages(layer) for layer in layers])
-
-        # Include subpackages of layer_packages
-        layer_packages.extend(self.__subpackages(layer_packages))
-
-        return set(layer_packages)
+        self.__dependency_report = dependency_report
 
-    def __subpackages(self, packages: List[str]) -> List[str]:
-        subpackages: List[str] = []
+    def run(self) -> None:
+        # Check dependencies if there is any violation for given ruleset
+        errors = {}
+
+        for layer in self.__ruleset.rules:
+            layer_defined_packages = self.__ruleset.layers[layer]
+            detected_dependencies = self.__dependency_report.layer_dependencies(layer)
+
+            print(f"\n### LAYER: '{layer}' WITH PACKAGES: {layer_defined_packages}")
+            print(f"    DEPENDENCIES DETECTED:\n\t{detected_dependencies if detected_dependencies else 'none'}")
+
+            violations = self.__check_rules(layer)
+            if len(violations) > 0:
+                errors[layer] = violations
+
+        print("\n")
+
+        if errors:
+            print(f"!!! {len(errors)} ILLEGAL DEPENDENCIES FOUND:")
+            packages_to_layers = self.__ruleset.packages_to_layers
+            for layer, illegal_dependency_pkg in errors.items():
+                for dependency in illegal_dependency_pkg:
+                    illegal_layer_name = "?"
+                    if dependency in packages_to_layers:
+                        illegal_layer_name = packages_to_layers[dependency]
+                    print(f"- Layer '{layer}' depends on '{dependency}' (Layer: {illegal_layer_name})")
+            sys.exit(1)
+        else:
+            print("OK! All package dependencies look good!")
+            sys.exit(0)
+
+    def __check_rules(self, layer: str) -> List[str]:
+        violation: List[str] = []
+        layer_deps: Set[str] = self.__dependency_report.layer_dependencies(layer)
+        whitelist: Set[str] = self.__dependency_report.whitelist(layer)
 
-        for package in self.__all_packages:
-            if package.startswith(tuple(packages)):
-                subpackages.append(package)
+        black_list = layer_deps.difference(whitelist)
 
-        return subpackages
+        if len(black_list) > 0:
+            violation.extend(list(black_list))
 
-    def __package_dependencies(self, packages: Set[str]) -> Set[str]:
-        """
-        Returns all packages that are used(imported) in given 'packages'.
-        In other words, this returns dependencies of given 'packages'.
-        """
-        return set(flatten([self.__graph.get(i, {}).get("imports", []) for i in packages]))
+        return violation
```

### Comparing `depcheck-0.2.0/depcheck/readers.py` & `depcheck-0.3/depcheck/readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,30 @@
             try:
                 ruleset = yaml.safe_load(stream)
             except yaml.YAMLError:
                 print(
                     "\n\n[!] Command must be run from project root " "and .depcheck.yml file should be in the root\n\n"
                 )
 
-        return Ruleset(layers=ruleset["layers"], rules=ruleset["whitelist"])
+        return Ruleset(ruleset["layers"], ruleset["whitelist"])
 
 
 class DependencyReader:
     __ruleset: Ruleset
     __root_package: str
 
     def __init__(self, ruleset: Ruleset, root_package: str) -> None:
         self.__ruleset = ruleset
         self.__root_package = root_package
 
     def read(self) -> DependencyReport:
         output = (
             subprocess.check_output(
-                "pydeps --show-deps --no-show --no-output --max-bacon 2 " + self.__root_package, shell=True
+                f"pydeps --show-deps --no-show --no-output --max-bacon 2 {self.__root_package}", shell=True
             )
             .decode("u8")
             .strip()
         )
-        dependency_graph: Dict[str, Any] = json.loads(output)
+
+        dependency_graph = json.loads(output)
 
         return DependencyReport(self.__ruleset, dependency_graph)
```

### Comparing `depcheck-0.2.0/pyproject.toml` & `depcheck-0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 [tool.poetry]
 name = "depcheck"
-version = "0.2.0"
+version = "0.3"
 authors = ["FlixMobility Tech <open-source@flixbus.com>"]
-description = "Depcheck is a tool to check package dependencies between predefined layers to make sure that the application always complies with the architecture you defined. It helps you enforcing some constraints and creating a decoupled applications."
+description = "Python code quality package that helps in defining and restricting how components of your code may interact"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/flix-tech/depcheck"
 repository = "https://github.com/flix-tech/depcheck"
 documentation = "https://github.com/flix-tech/depcheck"
-keywords = [
-    "depcheck",
-    "Dependency Checker",
-    "Clean Architecture",
-    "Separation of Concerns"
-]
+keywords = ["dependencies", "hexagonal", "architecture", "jdepend", "deptrac"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-pydeps = "^1.9.13"
+python = "^3.9"
+pydeps = "^1.12.0"
+PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
+pytest = "^7.3.0"
 pyre-check = "^0.9.0"
-flake8 = "^3.9.0"
-coverage = "^5.5"
-black = {version = "^21.7b0", python = "^3.6.2"}
-isort = {version = "^5.9.3", python = "^3.6.1"}
+flake8 = "^6.0.0"
+coverage = "^7.2.0"
+black = "^23.3.0"
+isort = "^5.12.0"
 
 [tool.black]
 line-length = 119
 
 [tool.isort]
 profile = "black"
 line_length = 119
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-depcheck = 'depcheck.main:main'
+depcheck = 'depcheck:run_depcheck'
```

### Comparing `depcheck-0.2.0/PKG-INFO` & `depcheck-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: depcheck
-Version: 0.2.0
-Summary: Depcheck is a tool to check package dependencies between predefined layers to make sure that the application always complies with the architecture you defined. It helps you enforcing some constraints and creating a decoupled applications.
+Version: 0.3
+Summary: Python code quality package that helps in defining and restricting how components of your code may interact
 Home-page: https://github.com/flix-tech/depcheck
 License: MIT
-Keywords: depcheck,Dependency Checker,Clean Architecture,Separation of Concerns
+Keywords: dependencies,hexagonal,architecture,jdepend,deptrac
 Author: FlixMobility Tech
 Author-email: open-source@flixbus.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pydeps (>=1.9.13,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: pydeps (>=1.12.0,<2.0.0)
 Project-URL: Documentation, https://github.com/flix-tech/depcheck
 Project-URL: Repository, https://github.com/flix-tech/depcheck
 Description-Content-Type: text/markdown
 
 ![Depcheck: Dependency Checker](https://images2.imgbox.com/da/85/J5OEzbAH_o.jpg)
 
-Depcheck is a tool to check package-dependencies between predefined layers. 
-In the configuration file(`.depcheck.yml`) located in the project root, 
-which packages belong to which layers and allowed dependencies between 
-layers are configurable. In this way, you can enforce constraints and make sure to have decoupled architecture.
+Depcheck is a command line code-quality tool which supports adopting a 
+layered architecture by making it possible to specify dependency constraints
+between packages of your own Python application. 
+The tool aims to achieve the same goals as [Deptrac][deptrac] in PHP and [JDepend][jdepend] in Java
 
 ## Install
 Install from [Pypi][pypi-link] via `pip install depcheck`
-    
+
 ## Usage
 Let's say you have a project with the directory structure below:
 ```text
 example
     root
         foo
         bar
         main.py
         __init__.py
     README.md
     .gitignore
     .depcheck.yml
 ```
 Note: Package directories should contain **\_\_init\_\_.py** to be recognized as a package.
-- Navigate to the `exampe` then run `depcheck` for your project:
+- Navigate to the `example` then run `depcheck` for your project:
     ```shell
-    depcheck root
+    poetry run depcheck example -f .depcheck.ok.yml  # This should be correct
+    poetry run depcheck example -f .depcheck.errors.yml  # This should give errors
     ```
 - As you can see in the directory structure above, we have `.depcheck.yml` 
   configuration file in the project directory. If you would like to change 
   the path of the configuration file, use `-f` or `--file` argument:
     ```shell
     depcheck root -f /path/to/your/custom/depcheck.yml
     ```
@@ -60,8 +61,10 @@
 
 <!-- Links -->
 [hexagonal-architecture]: https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)
 [upgrade-python-version]: ./docs/upgrade-python-version.md
 [update-project-dependencies]: ./docs/upgrade-python-version.md
 [pypi-link]: https://pypi.org/project/depcheck/
 [contribution]: ./CONTRIBUTING.md
+[deptrac]: https://github.com/qossmic/deptrac
+[jdepend]: https://github.com/clarkware/jdepend
```

