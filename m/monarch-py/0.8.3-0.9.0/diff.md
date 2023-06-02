# Comparing `tmp/monarch_py-0.8.3.tar.gz` & `tmp/monarch_py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.8.3.tar", max compression
+gzip compressed data, was "monarch_py-0.9.0.tar", max compression
```

## Comparing `monarch_py-0.8.3.tar` & `monarch_py-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-22 23:39:41.965812 monarch_py-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1630 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7461 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11736 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     9463 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3321 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20534 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4752 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9129 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4145 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      974 2023-06-02 02:55:36.296851 monarch_py-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7319 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11391 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7485 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3321 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20304 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4630 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9017 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3147 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.0/PKG-INFO
```

### Comparing `monarch_py-0.8.3/pyproject.toml` & `monarch_py-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.8.3"
+version = "0.9.0"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
@@ -18,14 +18,16 @@
 typer = "^0.7.0"
 typer-cli = "^0.0.13"
 rich = "*"
 docker = "^6.0.1"
 pystow = ">=0.5.0"
 loguru = "*"
 
+linkml = "^1.5.3"
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.10.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 autoflake = "^1.7.7"
 mkdocs = "^1.4.2"
```

### Comparing `monarch_py-0.8.3/src/monarch_py/cli.py` & `monarch_py-0.9.0/src/monarch_py/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import importlib
 from pathlib import Path
 from typing import List, Optional
 
 import typer
 
 from monarch_py import solr_cli, sql_cli
-from monarch_py.datamodels.model import AssociationTypeEnum
 
 app = typer.Typer()
 app.add_typer(solr_cli.solr_app, name="solr")
 app.add_typer(sql_cli.sql_app, name="sql")
 
 
 @app.callback(invoke_without_command=True)
@@ -69,15 +68,14 @@
     category: str = typer.Option(None, "--category", "-c"),
     subject: str = typer.Option(None, "--subject", "-s"),
     predicate: str = typer.Option(None, "--predicate", "-p"),
     object: str = typer.Option(None, "--object", "-o"),
     entity: str = typer.Option(None, "--entity", "-e"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
-    association_type: str = typer.Option(None, "--association-type"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
@@ -92,29 +90,28 @@
     Args:
         category: The category of the association
         predicate: The predicate of the association
         subject: The subject of the association
         object: The object of the association
         entity: The subject or object of the association
         between: The subject and object of the association
-        association_type: The label of the association
         limit: The number of associations to return
         direct: Whether to exclude associations with subject/object as ancestors
         offset: The offset of the first association to be retrieved
         fmt: The format of the output (json, yaml, tsv, table)
         output: The path to the output file (stdout if not specified)
     """
     solr_cli.associations(**locals())
 
 
 @app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: List[str] = typer.Option(None, "--category", "-c"),
-    taxon: str = typer.Option(None, "--taxon", "-t"),
+    in_taxon: str = typer.Option(None, "--in-taxon", "-t"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
@@ -216,16 +213,17 @@
     """
     solr_cli.association_counts(**locals())
 
 
 @app.command("association-table")
 def association_table(
     entity: str = typer.Argument(..., help="The entity to get associations for"),
-    association_type: AssociationTypeEnum = typer.Argument(
-        ..., help="The association type to get associations for"
+    category: str = typer.Argument(
+        ...,
+        help="The association category to get associations for, ex. biolink:GeneToPhenotypicFeatureAssociation",
     ),
     q: str = typer.Option(None, "--query", "-q"),
     limit: int = typer.Option(5, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
```

### Comparing `monarch_py-0.8.3/src/monarch_py/datamodels/model.py` & `monarch_py-0.9.0/src/monarch_py/datamodels/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from __future__ import annotations
 
+import sys
 from enum import Enum
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
+if sys.version_info >= (3, 8):
+    pass
+else:
+    pass
+
+
 metamodel_version = "None"
 version = "None"
 
 
 class WeakRefShimBaseModel(BaseModel):
     __slots__ = "__weakref__"
 
@@ -17,51 +24,43 @@
 class ConfiguredBaseModel(
     WeakRefShimBaseModel,
     validate_assignment=True,
     validate_all=True,
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
+    use_enum_values=True,
 ):
     pass
 
 
 class AssociationDirectionEnum(str, Enum):
+    """
+    The directionality of an association as it relates to a specified entity, with edges being categorized as incoming or outgoing
+    """
 
+    # An association for which a specified entity is the object or part of the object closure
     incoming = "incoming"
+    # An association for which a specified entity is the subject or part of the subject closure
     outgoing = "outgoing"
 
 
-class AssociationTypeEnum(str, Enum):
-
-    disease_phenotype = "disease_phenotype"
-    gene_phenotype = "gene_phenotype"
-    gene_interaction = "gene_interaction"
-    gene_pathway = "gene_pathway"
-    gene_expression = "gene_expression"
-    gene_orthology = "gene_orthology"
-    chemical_pathway = "chemical_pathway"
-    gene_function = "gene_function"
-    correlated_gene = "correlated_gene"
-    causal_gene = "causal_gene"
-
-
 class Association(ConfiguredBaseModel):
 
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
-    id: str = Field(None)
-    subject: str = Field(None)
+    id: str = Field(...)
+    subject: str = Field(...)
     original_subject: Optional[str] = Field(None)
     subject_namespace: Optional[str] = Field(None)
     subject_category: Optional[List[str]] = Field(default_factory=list)
     subject_closure: Optional[List[str]] = Field(default_factory=list)
     subject_label: Optional[str] = Field(None)
     subject_closure_label: Optional[List[str]] = Field(default_factory=list)
-    predicate: str = Field(None)
-    object: str = Field(None)
+    predicate: str = Field(...)
+    object: str = Field(...)
     original_object: Optional[str] = Field(None)
     object_namespace: Optional[str] = Field(None)
     object_category: Optional[List[str]] = Field(default_factory=list)
     object_closure: Optional[List[str]] = Field(default_factory=list)
     object_label: Optional[str] = Field(None)
     object_closure_label: Optional[List[str]] = Field(default_factory=list)
     primary_knowledge_source: Optional[List[str]] = Field(default_factory=list)
@@ -82,28 +81,28 @@
 
 class DirectionalAssociation(Association):
     """
     An association that gives it's direction relative to a specified entity
     """
 
     direction: AssociationDirectionEnum = Field(
-        None,
+        ...,
         description="""The directionality of the association relative to a given entity for an association_count. If the entity is the subject or in the subject closure, the direction is forwards, if it is the object or in the object closure, the direction is backwards.""",
     )
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
-    id: str = Field(None)
-    subject: str = Field(None)
+    id: str = Field(...)
+    subject: str = Field(...)
     original_subject: Optional[str] = Field(None)
     subject_namespace: Optional[str] = Field(None)
     subject_category: Optional[List[str]] = Field(default_factory=list)
     subject_closure: Optional[List[str]] = Field(default_factory=list)
     subject_label: Optional[str] = Field(None)
     subject_closure_label: Optional[List[str]] = Field(default_factory=list)
-    predicate: str = Field(None)
-    object: str = Field(None)
+    predicate: str = Field(...)
+    object: str = Field(...)
     original_object: Optional[str] = Field(None)
     object_namespace: Optional[str] = Field(None)
     object_category: Optional[List[str]] = Field(default_factory=list)
     object_closure: Optional[List[str]] = Field(default_factory=list)
     object_label: Optional[str] = Field(None)
     object_closure_label: Optional[List[str]] = Field(default_factory=list)
     primary_knowledge_source: Optional[List[str]] = Field(default_factory=list)
@@ -120,165 +119,161 @@
     stage_qualifier: Optional[str] = Field(None)
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
 
 
 class Entity(ConfiguredBaseModel):
 
-    id: str = Field(None)
+    id: str = Field(...)
     category: Optional[List[str]] = Field(default_factory=list)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
-    type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
 
 
 class HistoPheno(ConfiguredBaseModel):
 
-    id: str = Field(None)
+    id: str = Field(...)
     items: List[HistoBin] = Field(
         default_factory=list,
         description="""A collection of items, with the type to be overriden by slot_usage""",
     )
 
 
 class Results(ConfiguredBaseModel):
 
-    limit: int = Field(None, description="""number of items to return in a response""")
-    offset: int = Field(None, description="""offset into the total number of items""")
-    total: int = Field(None, description="""total number of items matching a query""")
+    limit: int = Field(..., description="""number of items to return in a response""")
+    offset: int = Field(..., description="""offset into the total number of items""")
+    total: int = Field(..., description="""total number of items matching a query""")
 
 
 class AssociationResults(Results):
 
     items: List[Association] = Field(
         default_factory=list,
         description="""A collection of items, with the type to be overriden by slot_usage""",
     )
-    limit: int = Field(None, description="""number of items to return in a response""")
-    offset: int = Field(None, description="""offset into the total number of items""")
-    total: int = Field(None, description="""total number of items matching a query""")
+    limit: int = Field(..., description="""number of items to return in a response""")
+    offset: int = Field(..., description="""offset into the total number of items""")
+    total: int = Field(..., description="""total number of items matching a query""")
 
 
 class AssociationTableResults(Results):
 
     items: List[DirectionalAssociation] = Field(
         default_factory=list,
         description="""A collection of items, with the type to be overriden by slot_usage""",
     )
-    limit: int = Field(None, description="""number of items to return in a response""")
-    offset: int = Field(None, description="""offset into the total number of items""")
-    total: int = Field(None, description="""total number of items matching a query""")
+    limit: int = Field(..., description="""number of items to return in a response""")
+    offset: int = Field(..., description="""offset into the total number of items""")
+    total: int = Field(..., description="""total number of items matching a query""")
 
 
 class EntityResults(Results):
 
     items: List[Entity] = Field(
         default_factory=list,
         description="""A collection of items, with the type to be overriden by slot_usage""",
     )
-    limit: int = Field(None, description="""number of items to return in a response""")
-    offset: int = Field(None, description="""offset into the total number of items""")
-    total: int = Field(None, description="""total number of items matching a query""")
+    limit: int = Field(..., description="""number of items to return in a response""")
+    offset: int = Field(..., description="""offset into the total number of items""")
+    total: int = Field(..., description="""total number of items matching a query""")
 
 
 class SearchResult(Entity):
 
     highlight: Optional[str] = Field(
         None, description="""matching text snippet containing html tags"""
     )
     score: Optional[float] = Field(None)
-    id: str = Field(None)
+    id: str = Field(...)
     category: List[str] = Field(default_factory=list)
-    name: str = Field(None)
+    name: str = Field(...)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
-    type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
 
 
 class SearchResults(Results):
 
     items: List[SearchResult] = Field(
         default_factory=list,
         description="""A collection of items, with the type to be overriden by slot_usage""",
     )
-    facet_fields: Optional[Dict[str, FacetField]] = Field(
-        default_factory=dict,
+    facet_fields: Optional[List[FacetField]] = Field(
+        default_factory=list,
         description="""Collection of facet field responses with the field values and counts""",
     )
-    facet_queries: Optional[Dict[str, FacetValue]] = Field(
-        default_factory=dict,
+    facet_queries: Optional[List[FacetValue]] = Field(
+        default_factory=list,
         description="""Collection of facet query responses with the query string values and counts""",
     )
-    limit: int = Field(None, description="""number of items to return in a response""")
-    offset: int = Field(None, description="""offset into the total number of items""")
-    total: int = Field(None, description="""total number of items matching a query""")
+    limit: int = Field(..., description="""number of items to return in a response""")
+    offset: int = Field(..., description="""offset into the total number of items""")
+    total: int = Field(..., description="""total number of items matching a query""")
 
 
 class FacetValue(ConfiguredBaseModel):
 
-    label: str = Field(None)
+    label: str = Field(...)
     count: Optional[int] = Field(None, description="""count of documents""")
 
 
 class HistoBin(FacetValue):
 
-    id: str = Field(None)
-    label: str = Field(None)
+    id: str = Field(...)
+    label: str = Field(...)
     count: Optional[int] = Field(None, description="""count of documents""")
 
 
 class FacetField(ConfiguredBaseModel):
 
-    label: str = Field(None)
-    facet_values: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
+    label: str = Field(...)
+    facet_values: Optional[List[FacetValue]] = Field(
+        default_factory=list,
+        description="""Collection of FacetValue label/value instances belonging to a FacetField""",
+    )
 
 
 class AssociationTypeMapping(ConfiguredBaseModel):
     """
     A data class to hold the necessary information to produce association type counts for given  entities with appropriate directional labels
     """
 
-    association_type: Optional[AssociationTypeEnum] = Field(None)
     subject_label: Optional[str] = Field(
         None,
         description="""A label to describe the subjects of the association type as a whole for use in the UI""",
     )
     object_label: Optional[str] = Field(
         None,
         description="""A label to describe the objects of the association type as a whole for use in the UI""",
     )
     symmetric: bool = Field(
         False,
         description="""Whether the association type is symmetric, meaning that the subject and object labels should be interchangeable""",
     )
-    category: Optional[List[str]] = Field(
-        default_factory=list,
-        description="""The biolink categories to use in queries for this association type, assuming OR semantics""",
-    )
-    predicate: List[str] = Field(
-        default_factory=list,
-        description="""The biolink predicate to use in queries for this association type, assuming OR semantics""",
+    category: str = Field(
+        ...,
+        description="""The biolink category to use in queries for this association type""",
     )
 
 
 class AssociationCount(FacetValue):
 
-    association_type: Optional[AssociationTypeEnum] = Field(None)
-    label: str = Field(None)
+    category: Optional[str] = Field(None)
+    label: str = Field(...)
     count: Optional[int] = Field(None, description="""count of documents""")
 
 
 class AssociationCountList(ConfiguredBaseModel):
     """
     Container class for a list of association counts
     """
```

### Comparing `monarch_py-0.8.3/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.9.0/src/monarch_py/datamodels/model.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -16,58 +16,14 @@
     permissible_values:
       incoming:
         description: >-
           An association for which a specified entity is the object or part of the object closure
       outgoing:
         description: >-
           An association for which a specified entity is the subject or part of the subject closure
-  AssociationTypeEnum:
-    description: >-
-      A grouping label for association types, which are not necessarily 1:1 with
-      biolink categories or predicates
-    permissible_values:
-      disease_phenotype:
-        description: >-
-          Any association between a disease and a phenotype
-        meaning: biolink:GeneToDiseaseAssociation
-      gene_phenotype:
-          description: >-
-              Any association between a gene and a phenotype
-          meaning: biolink:GeneToPhenotypicFeatureAssociation
-      gene_interaction:
-          description: >-
-              Any association between two genes
-          meaning: biolink:PairwiseGeneToGeneInteraction
-      gene_pathway:
-          description: >-
-              Any association between a gene and a pathway
-          meaning: biolink:GeneToPathwayAssociation
-      gene_expression:
-          description: >-
-              Expression association between a gene and an expression site
-          meaning: biolink:GeneToExpressionSiteAssociation
-      gene_orthology:
-          description: >-
-              Any association between two genes based on orthology
-          meaning: biolink:PairwiseGeneToGeneOrthologyAssociation
-      chemical_pathway:
-          description: >-
-              Any association between a chemical and a pathway
-          meaning: biolink:ChemicalToPathwayAssociation
-      gene_function:
-          description: >-
-              Any association between a gene and molecular activity
-          meaning: biolink:MacromolecularMachineToMolecularActivityAssociation
-      correlated_gene:
-        description: >-
-          Association between a gene and a disease that has not been established to be causal
-      causal_gene:
-          description: >-
-              Association between a gene and a disease that is known to be causal
-          meaning: biolink:causal
 
 classes:
   Association:
     slots:
     - aggregator_knowledge_source
     - id
     - subject
@@ -126,15 +82,14 @@
     - name
     - description
     - xref
     - provided_by
     - in_taxon
     - source
     - symbol
-    - type
     - synonym
   EntityResults:
     is_a: Results
     slots: 
       - items
     slot_usage:
       items:
@@ -193,54 +148,51 @@
       label:
         identifier: true
   AssociationTypeMapping:
     description: >-
       A data class to hold the necessary information to produce association type counts for given 
       entities with appropriate directional labels
     slots:
-      - association_type
       - subject_label
       - object_label
       - symmetric
       - category
-      - predicate
     slot_usage:
       subject_label:
         description: A label to describe the subjects of the association type as a whole for use in the UI
       object_label:
         description: A label to describe the objects of the association type as a whole for use in the UI
       symmetric:
         description: >-
           Whether the association type is symmetric, meaning that the subject and object labels should be
           interchangeable
         ifabsent: false
         required: true
       category:
-        description: The biolink categories to use in queries for this association type, assuming OR semantics
-        multivalued: true
-      predicate:
-        description: The biolink predicate to use in queries for this association type, assuming OR semantics
-        multivalued: true
+        description: The biolink category to use in queries for this association type
+        required: true
+        multivalued: false
   AssociationCount:
     is_a: FacetValue
     slots:
-      - association_type
+      - category
+    slot_usage:
+      category:
+        multivalued: false
   AssociationCountList:
     description: Container class for a list of association counts
     slots:
       - items
     slot_usage:
       items:
         range: AssociationCount
 
 slots:
   aggregator_knowledge_source:
     multivalued: true
-  association_type:
-    range: AssociationTypeEnum
   category:
     multivalued: true
   count:
     description: count of documents
     range: integer
   description:
     range: string
@@ -249,24 +201,25 @@
       The directionality of the association relative to a given entity for an association_count.
       If the entity is the subject or in the subject closure, the direction is forwards, if it is
       the object or in the object closure, the direction is backwards.
     range: AssociationDirectionEnum
     required: true
   facet_fields:
     description: Collection of facet field responses with the field values and counts
-    inlined: true
+    inlined_as_list: true
     multivalued: true
     range: FacetField
   facet_queries:
     description: Collection of facet query responses with the query string values and counts
-    inlined: true
+    inlined_as_list: true
     multivalued: true
     range: FacetValue
   facet_values:
-    inlined: true
+    description: Collection of FacetValue label/value instances belonging to a FacetField
+    inlined_as_list: true
     multivalued: true
     range: FacetValue
   frequency_qualifier:
     range: string
   has_evidence:
     range: string
   highlight:
@@ -366,12 +319,10 @@
     range: boolean
   synonym:
     multivalued: true
   total:
     description: total number of items matching a query
     range: integer
     required: true
-  type:
-    range: string
   xref:
     multivalued: true
     range: string
```

### Comparing `monarch_py-0.8.3/src/monarch_py/datamodels/solr.py` & `monarch_py-0.9.0/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.9.0/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from monarch_py.datamodels.model import (
     Association,
     AssociationCount,
     AssociationDirectionEnum,
     AssociationResults,
     AssociationTableResults,
-    AssociationTypeEnum,
     DirectionalAssociation,
     Entity,
     FacetField,
     FacetValue,
     HistoBin,
     HistoPheno,
     SearchResult,
@@ -73,15 +72,14 @@
         subject: str = None,
         object: str = None,
         subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
         direct: bool = None,
-        association_type: AssociationTypeEnum = None,
         offset: int = 0,
         limit: int = 20,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
@@ -107,15 +105,14 @@
             subject=subject,
             object=object,
             subject_closure=subject_closure,
             object_closure=object_closure,
             entity=entity,
             between=between,
             direct=direct,
-            association_type=association_type,
             offset=offset,
             limit=limit,
         )
 
         query_result = solr.query(query)
         total = query_result.response.num_found
 
@@ -141,15 +138,14 @@
         subject: str = None,
         object: str = None,
         subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
         direct: bool = None,
-        association_type: AssociationTypeEnum = None,
         q: str = None,
         offset: int = 0,
         limit: int = 20,
     ) -> SolrQuery:
         """Populate a SolrQuery object with association filters"""
 
         query = SolrQuery(start=offset, rows=limit)
@@ -194,20 +190,14 @@
                 query.add_filter_query(
                     f'subject:"{escape(entity)}" OR subject_closure:"{escape(entity)}" OR object:"{escape(entity)}" OR object_closure:"{escape(entity)}"'
                 )
             else:
                 query.add_filter_query(
                     f'subject:"{escape(entity)}" OR object:"{escape(entity)}"'
                 )
-        if association_type:
-            query.add_filter_query(
-                get_solr_query_fragment(
-                    AssociationTypeMappings().get_mapping(association_type)
-                )
-            )
         if q:
             # We don't yet have tokenization strategies for the association index, initially we'll limit searching to
             # the visible fields in an association table plus their ID equivalents and use a wildcard query for substring matching
             query.q = f"*{q}*"
             query.query_fields = "subject subject_label predicate object object_label"
 
         return query
@@ -448,36 +438,37 @@
                 # when searching for associations by type
                 if label in association_count_dict and agm.symmetric:
                     association_count_dict[label].count += v
                 else:
                     association_count_dict[label] = AssociationCount(
                         label=label,
                         count=v,
-                        association_type=agm.association_type,
+                        category=agm.category,
                     )
 
         association_counts: List[AssociationCount] = list(
             association_count_dict.values()
         )
         return association_counts
 
     def get_association_table(
         self,
         entity: str,
-        association_type: AssociationTypeEnum,
+        category: str,
         q=None,
         sort=None,
         offset=0,
         limit=5,
     ) -> AssociationTableResults:
         if sort:
             raise NotImplementedError("Sorting is not yet implemented")
+
         query = self._populate_association_query(
             entity=entity,
-            association_type=association_type,
+            category=category,
             q=q,
             offset=offset,
             limit=limit,
         )
         solr = SolrService(base_url=self.base_url, core=core.ASSOCIATION)
         query_result = solr.query(query)
         total = query_result.response.num_found
@@ -496,59 +487,71 @@
         )
 
         return results
 
     def _get_association_direction(
         self, entity: str, document: Dict
     ) -> AssociationDirectionEnum:
-        if document.get("subject") == entity \
-                or (document.get("subject_closure") and entity in document.get("subject_closure")):
+        if document.get("subject") == entity or (
+            document.get("subject_closure")
+            and entity in document.get("subject_closure")
+        ):
             direction = AssociationDirectionEnum.outgoing
-        elif document.get("object") == entity \
-                or (document.get("object_closure") and entity in document.get("object_closure")):
+        elif document.get("object") == entity or (
+            document.get("object_closure") and entity in document.get("object_closure")
+        ):
             direction = AssociationDirectionEnum.incoming
         else:
             raise ValueError(f"Entity {entity} not found in association {document}")
         return direction
 
-    def _convert_facet_fields(self, solr_facet_fields: Dict) -> Dict[str, FacetField]:
+    def _convert_facet_fields(self, solr_facet_fields: Dict) -> List[FacetField]:
         """
         Converts a list of raw solr facet fields from the solr response to a list of
         FacetField instances
 
         Args:
             facet_fields (Dict): A list of facet fields from the solr response
 
         Returns:
             List[FacetField]: A list of FacetField instances, with FacetValues populated within
         """
 
-        facet_fields: Dict[str, FacetField] = {}
+        facet_fields: List[FacetField] = []
         for field in solr_facet_fields:
             ff = FacetField(label=field)
             facet_list = solr_facet_fields[field]
             facet_dict = dict(zip(facet_list[::2], facet_list[1::2]))
-            ff.facet_values = {
-                k: FacetValue(label=k, count=v) for k, v in facet_dict.items()
-            }
-            facet_fields[field] = ff
+            ff.facet_values = [
+                FacetValue(label=k, count=v) for k, v in facet_dict.items()
+            ]
+            facet_fields.append(ff)
 
         return facet_fields
 
     def _convert_facet_queries(
         self, solr_facet_queries: Dict[str, int]
-    ) -> Dict[str, FacetValue]:
+    ) -> List[FacetValue]:
         """
         Converts a list of raw solr facet queries from the solr response to a list of
         FacetValue instances
 
         Args:
             facet_queries (Dict): A dictionary of facet queries from the solr response
 
         Returns:
             List[FacetValue]: A list of FacetValue instances
         """
 
-        facet_values = {
-            k: FacetValue(label=k, count=v) for k, v in solr_facet_queries.items()
-        }
+        facet_values = [
+            FacetValue(label=k, count=v) for k, v in solr_facet_queries.items()
+        ]
         return facet_values
+
+    def solr_is_available(self):
+        import requests
+
+        try:
+            response = requests.get(self.base_url)
+            return response.status_code == 200
+        except Exception:
+            return False
```

### Comparing `monarch_py-0.8.3/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.9.0/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.9.0/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.9.0/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.9.0/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.9.0/src/monarch_py/interfaces/search_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 from monarch_py.datamodels.model import (
     AssociationTableResults,
-    AssociationTypeEnum,
     FacetValue,
     SearchResults,
 )
 
 
 class SearchInterface(ABC):
     """Abstract interface for searching the Monarch KG in a Lucene way"""
@@ -64,15 +63,14 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: Tuple[str, str] = None,
-        association_type: AssociationTypeEnum = None,
     ) -> SearchResults:
         """
         Get facet counts and facet query counts for associations
         Args:
             facet_fields (List[str]): Facet fields to return counts for
             facet_queries (List[str]): Facet queries to return counts for
             category (str): Filter to only associations matching the specified category
@@ -98,26 +96,26 @@
             List[FacetValue]: List of FacetValue objects representing the counts of associations for the given entity
         """
         raise NotImplementedError
 
     def get_association_table(
         self,
         entity: str,
-        association_type: AssociationTypeEnum,
+        category: str,
         query=None,
         sort=None,
         offset=0,
         limit=5,
     ) -> AssociationTableResults:
         """
         Get associations for an entity matching a specified type, with optional search and sort parameters
 
         Args:
             entity (str): Entity to get associations for
-            association_type (AssociationTypeEnum): Association type to filter to
+            category (str): Category of associations to return
             query (str): Query string to match against
             sort (str): Sort order, defaults to None
             offset (int): Offset of the first result to return, defaults to 0
             limit (int): Limit the number of results to return, defaults to 20
 
         Returns:
             AssociationResults: Dataclass representing results of an association search.
```

### Comparing `monarch_py-0.8.3/src/monarch_py/service/solr_service.py` & `monarch_py-0.9.0/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/solr_cli.py` & `monarch_py-0.9.0/src/monarch_py/solr_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 import pystow
 import typer
 
-from monarch_py.datamodels.model import AssociationCountList, AssociationTypeEnum
+from monarch_py.datamodels.model import AssociationCountList
 from monarch_py.utils.solr_cli_utils import (
     check_solr_permissions,
     get_solr,
     solr_status,
     start_solr,
     stop_solr,
 )
@@ -92,15 +92,14 @@
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
     object: str = typer.Option(None, "--object"),
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
-    association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
@@ -116,15 +115,14 @@
         category (str, optional): The category of the association.
         subject (str, optional): The subject of the association.
         predicate (str, optional): The predicate of the association.
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
         direct (bool, optional): Exclude associations with the specified subject and objects as ancestors. Default False
-        association_type (str, optional): The association label of the association
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
         fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
     args.pop("update", None)
@@ -136,15 +134,15 @@
     format_output(fmt, response, output)
 
 
 @solr_app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: List[str] = typer.Option(None, "--category", "-c"),
-    taxon: str = typer.Option(None, "--taxon", "-t"),
+    in_taxon: str = typer.Option(None, "--in-taxon", "-t"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
@@ -268,16 +266,17 @@
     counts = AssociationCountList(items=response)
     format_output(fmt, counts, output)
 
 
 @solr_app.command("association-table")
 def association_table(
     entity: str = typer.Argument(..., help="The entity to get associations for"),
-    association_type: AssociationTypeEnum = typer.Argument(
-        ..., help="The association type to get associations for"
+    category: str = typer.Argument(
+        ...,
+        help="The association category to get associations for, ex. biolink:GeneToPhenotypicFeatureAssociation",
     ),
     q: str = typer.Option(None, "--query", "-q"),
     limit: int = typer.Option(5, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
@@ -286,10 +285,10 @@
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     data = get_solr(update=False)
     response = data.get_association_table(
-        entity, association_type, q=q, limit=limit, offset=offset
+        entity=entity, category=category, q=q, limit=limit, offset=offset
     )
     format_output(fmt, response, output)
```

### Comparing `monarch_py-0.8.3/src/monarch_py/sql_cli.py` & `monarch_py-0.9.0/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.9.0/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/src/monarch_py/utils/utils.py` & `monarch_py-0.9.0/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.3/PKG-INFO` & `monarch_py-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.8.3
+Version: 0.9.0
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.0.1,<7.0.0)
+Requires-Dist: linkml (>=1.5.3,<2.0.0)
 Requires-Dist: loguru
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pystow (>=0.5.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: typer-cli (>=0.0.13,<0.0.14)
```

