# Comparing `tmp/tesseract_olap-0.7.1.tar.gz` & `tmp/tesseract_olap-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.7.1.tar", max compression
+gzip compressed data, was "tesseract_olap-0.7.2.tar", max compression
```

## Comparing `tesseract_olap-0.7.1.tar` & `tesseract_olap-0.7.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2221 2023-05-29 21:46:22.858263 tesseract_olap-0.7.1/PACKAGE.md
--rw-r--r--   0        0        0      862 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/__init__.py
--rw-r--r--   0        0        0       92 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0       79 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     5868 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     1894 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0     1221 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/enums.py
--rw-r--r--   0        0        0    19408 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     1734 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/exceptions.py
--rw-r--r--   0        0        0     3248 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0      243 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0      219 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/exceptions.py
--rw-r--r--   0        0        0     1570 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      385 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      380 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/exceptions.py
--rw-r--r--   0        0        0      511 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0     6665 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     5677 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     1198 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1129 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     2262 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/calculations.py
--rw-r--r--   0        0        0     2848 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0     3104 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/exceptions.py
--rw-r--r--   0        0        0    10377 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    11603 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0     7990 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1539 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/results.py
--rw-r--r--   0        0        0     1145 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5400 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3533 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     3649 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     3323 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/exceptions.py
--rw-r--r--   0        0        0     2497 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     8559 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0     4645 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23574 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    18440 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0      898 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/exceptions.py
--rw-r--r--   0        0        0     4532 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     4260 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 tesseract_olap-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2221 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/PACKAGE.md
+-rw-r--r--   0        0        0      862 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     5868 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     1894 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0     1221 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/enums.py
+-rw-r--r--   0        0        0    19408 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     1734 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/exceptions.py
+-rw-r--r--   0        0        0     3248 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0      243 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/common/exceptions.py
+-rw-r--r--   0        0        0     1570 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      380 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/exceptions.py
+-rw-r--r--   0        0        0      511 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0     6665 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     5677 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     1198 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1129 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     2262 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/query/calculations.py
+-rw-r--r--   0        0        0     2848 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0     3104 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/query/exceptions.py
+-rw-r--r--   0        0        0    10377 2023-06-02 01:09:23.140955 tesseract_olap-0.7.2/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    11603 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0     7990 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1539 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/query/results.py
+-rw-r--r--   0        0        0     1145 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5400 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3533 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     3649 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     3323 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/exceptions.py
+-rw-r--r--   0        0        0     2497 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     8559 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0     4645 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23574 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    18440 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/server/exceptions.py
+-rw-r--r--   0        0        0     4495 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     4260 2023-06-02 01:09:23.144955 tesseract_olap-0.7.2/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 tesseract_olap-0.7.2/PKG-INFO
```

### Comparing `tesseract_olap-0.7.1/PACKAGE.md` & `tesseract_olap-0.7.2/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/pyproject.toml` & `tesseract_olap-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.7.1"
+version = "0.7.2"
 description = "A simple OLAP library."
 authors = ["Francisco Abarzua <francisco@datawheel.us>"]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/tesseract-python"
 
 [tool.poetry.dependencies]
```

### Comparing `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/enums.py` & `tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.7.2/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/backend/exceptions.py` & `tesseract_olap-0.7.2/tesseract_olap/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/backend/models.py` & `tesseract_olap-0.7.2/tesseract_olap/backend/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/common/strings.py` & `tesseract_olap-0.7.2/tesseract_olap/common/strings.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.7.2/tesseract_olap/logiclayer/dependencies.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.7.2/tesseract_olap/logiclayer/module.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.7.2/tesseract_olap/logiclayer/response.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/__init__.py` & `tesseract_olap-0.7.2/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/calculations.py` & `tesseract_olap-0.7.2/tesseract_olap/query/calculations.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/enums.py` & `tesseract_olap-0.7.2/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/exceptions.py` & `tesseract_olap-0.7.2/tesseract_olap/query/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/models.py` & `tesseract_olap-0.7.2/tesseract_olap/query/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/queries.py` & `tesseract_olap-0.7.2/tesseract_olap/query/queries.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/requests.py` & `tesseract_olap-0.7.2/tesseract_olap/query/requests.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/query/results.py` & `tesseract_olap-0.7.2/tesseract_olap/query/results.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/aggregators.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/csv.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/csv.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/enums.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/exceptions.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/json.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/json.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/models.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.7.2/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/traverse.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/schema/xml.py` & `tesseract_olap-0.7.2/tesseract_olap/schema/xml.py`

 * *Files 23% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 class XMLSchema(models.Schema):
     tag = "Schema"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int = 0):
         """Parse a <Schema> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         cube_gen = _yield_children_nodes(node, XMLCube)
         shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
         sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
 
         return cls(
             name=name,
@@ -86,15 +86,15 @@
 class XMLCube(models.Cube):
     tag = "Cube"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Cube> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         table = _find_table_ref(node)
         if table is None:
             raise MissingXMLNode(node.tag, name, "Table")
 
         dimension_map = OrderedDict(
             _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
@@ -122,15 +122,15 @@
 class XMLDimensionUsage(models.DimensionUsage):
     tag = "DimensionUsage"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <DimensionUsage> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             foreign_key=_get_attr(node, "foreign_key"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
@@ -143,15 +143,15 @@
 class XMLHierarchyUsage(models.HierarchyUsage):
     tag = "HierarchyUsage"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <HierarchyUsage> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             level_map=OrderedDict(
@@ -163,15 +163,15 @@
 class XMLLevelUsage(models.LevelUsage):
     tag = "LevelUsage"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <LevelUsage> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             property_map=OrderedDict(
@@ -183,15 +183,15 @@
 class XMLPropertyUsage(models.PropertyUsage):
     tag = "PropertyUsage"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <PropertyUsage> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
         )
@@ -200,15 +200,15 @@
 class XMLTable(models.Table):
     tag = "Table"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Table> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             schema=node.get("schema"),
             primary_key=node.get("primary_key", "id"),
         )
 
@@ -216,15 +216,15 @@
 class XMLInlineTable(models.InlineTable):
     tag = "InlineTable"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <InlineTable> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         node_format = _get_attr(node, "format")
 
         if node_format == "csv":
             node_format = "text/csv"
 
         if node_format == "tuples":
@@ -273,15 +273,15 @@
 class XMLSharedDimension(models.Dimension):
     tag = "SharedDimension"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a Shared <Dimension> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         dim_type = node.get("type")
 
         return cls(
             name=name,
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             dim_type=DimensionType.from_str(dim_type),
@@ -309,15 +309,15 @@
 class XMLHierarchy(models.Hierarchy):
     tag = "Hierarchy"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Hierarchy> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
         if len(level_map) == 0:
             raise MissingXMLNode(node.tag, name, "Level")
 
         default_pk = ""
         for item in level_map.values():
@@ -342,15 +342,15 @@
 class XMLLevel(models.Level):
     tag = "Level"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Level> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         key_type = node.get("key_type")
 
         return cls(
             name=name,
             depth=index + 1,
             key_column=_get_attr(node, "key_column"),
@@ -365,15 +365,15 @@
 class XMLProperty(models.Property):
     tag = "Property"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Property> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         key_type = node.get("key_type")
 
         keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
         if len(keycol_map) == 0:
             raise MissingXMLAttribute(node.tag, "key_column")
 
@@ -389,15 +389,15 @@
 class XMLMeasure(models.Measure):
     tag = "Measure"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Measure> XML node."""
         name = _get_attr(node, "name")
-        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         aggregator = cls._get_aggregator(node)
         captions = immu.Map(_yield_locale_pairs(node, "caption"))
 
         def _parse_column(node: etree._Element):
             coltype = _get_attr(node, "type").upper()
             colname = node.get("name", f"{name} {coltype}")
```

### Comparing `tesseract_olap-0.7.1/tesseract_olap/server/exceptions.py` & `tesseract_olap-0.7.2/tesseract_olap/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/tesseract_olap/server/schema.py` & `tesseract_olap-0.7.2/tesseract_olap/server/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,19 +102,16 @@
         return parse_xml_schema(source)
 
     # Check if argument is a raw JSON string
     if source.startswith(("{\"", "[{")):
         logger.debug("Parsing JSON schema from string")
         return parse_json_schema(source)
 
-    try:
-        result = parse_csv_schema(source)
-        return result
-    except ValueError:
-        return None
+    # A raw CSV here doesn't provide a valid Schema, so bypass
+    return None
 
 
 def _parse_path_file(item: Path) -> "Schema":
     """Attempts parse the contents of a reference to a local file as a Schema."""
     if item.suffix == ".xml":
         logger.debug("Parsing XML schema from file contents: %s" % item)
         return parse_xml_schema(item)
```

### Comparing `tesseract_olap-0.7.1/tesseract_olap/server/server.py` & `tesseract_olap-0.7.2/tesseract_olap/server/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.1/PKG-INFO` & `tesseract_olap-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.7.1
+Version: 0.7.2
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

