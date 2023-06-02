# Comparing `tmp/openepd-0.5.0.tar.gz` & `tmp/openepd-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.5.0.tar", max compression
+gzip compressed data, was "openepd-0.6.0.tar", max compression
```

## Comparing `openepd-0.5.0.tar` & `openepd-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-01 10:35:52.967121 openepd-0.5.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-06-01 10:35:52.967121 openepd-0.5.0/README.md
--rw-r--r--   0        0        0     3051 2023-06-01 10:35:52.967121 openepd-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     2613 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     2178 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/common.py
--rw-r--r--   0        0        0     7763 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     8887 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3811 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2855 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3342 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 12:58:17.392304 openepd-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2841 2023-06-02 12:58:17.392304 openepd-0.6.0/README.md
+-rw-r--r--   0        0        0     3051 2023-06-02 12:58:17.392304 openepd-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     2613 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     3365 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    12201 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     8887 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3811 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2855 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.6.0/PKG-INFO
```

### Comparing `openepd-0.5.0/LICENSE` & `openepd-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/README.md` & `openepd-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/pyproject.toml` & `openepd-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.5.0"
+version = "0.6.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.5.0"
+version = "0.6.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.5.0/src/openepd/__init__.py` & `openepd-0.6.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/__version__.py` & `openepd-0.6.0/src/openepd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.5.0"
+VERSION = "0.6.0"
```

### Comparing `openepd-0.5.0/src/openepd/model/__init__.py` & `openepd-0.6.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/base.py` & `openepd-0.6.0/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/common.py` & `openepd-0.6.0/src/openepd/model/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,43 +13,74 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Annotated
+from typing import Annotated, Any
 
 import pydantic as pyd
+from pydantic import root_validator
 
 from openepd.model.base import BaseOpenEpdSchema
 
 
 class Amount(BaseOpenEpdSchema):
     """A value-and-unit pairing for amounts that do not have an uncertainty."""
 
-    qty: float | None = pyd.Field(description="How much of this in the amount.")
-    unit: str = pyd.Field(description="Which unit.  SI units are preferred.", example="kg")
+    qty: float | None = pyd.Field(description="How much of this in the amount.", default=None)
+    unit: str | None = pyd.Field(description="Which unit.  SI units are preferred.", example="kg", default=None)
+
+    @root_validator
+    def check_qty_or_unit(cls, values: dict[str, Any]):
+        """Ensure that qty or unit is provided."""
+        if values["qty"] is None and values["unit"] is None:
+            raise ValueError("Either qty or unit must be provided.")
+        return values
+
+    def to_quantity_str(self):
+        """Return a string representation of the amount."""
+        return f"{self.qty or ''} {self.unit or 'str'}".strip()
 
 
 class Measurement(BaseOpenEpdSchema):
     """A scientific value with units and uncertainty."""
 
     mean: float = pyd.Field(description="Mean (expected) value of the measurement")
     unit: str = pyd.Field(description="Measurement unit")
     rsd: pyd.PositiveFloat | None = pyd.Field(
         description="Relative standard deviation, i.e. standard_deviation/mean", default=None
     )
     dist: str | None = pyd.Field(description="Statistical distribution of the measurement error.", default=None)
 
 
+class Ingredient(BaseOpenEpdSchema):
+    """
+    An ingredient of a product.
+
+    The Ingredients list gives the core data references and quantities. This list is used to document supply-chain
+    transparency, such as the EPDs of major components (e.g. cement in concrete, or recycled steel
+    in hot-rolled sections).
+    """
+
+    qty: float | None = pyd.Field(
+        description="Number of declared units of this consumed. Negative values indicate an outflow."
+    )
+    link: pyd.AnyUrl | None = pyd.Field(
+        description="Link to this object's OpenEPD declaration. "
+        "An OpenIndustryEPD or OpenLCI link is also acceptable.",
+        default=None,
+    )
+
+
 class WithAttachmentsMixin:
     """Mixin for objects that can have attachments."""
 
-    attachments: dict[Annotated[str, pyd.constr(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
+    attachments: dict[Annotated[str, pyd.Field(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
         description="Dict of URLs relevant to this entry",
         example={
             "Contact Us": "https://www.c-change-labs.com/en/contact-us/",
             "LinkedIn": "https://www.linkedin.com/company/c-change-labs/",
         },
         default=None,
     )
```

### Comparing `openepd-0.5.0/src/openepd/model/epd.py` & `openepd-0.6.0/src/openepd/model/epd.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
-from typing import Literal
+from typing import Annotated, Literal
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import Amount
+from openepd.model.common import Amount, Ingredient
 from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet
 from openepd.model.org import Org, Plant
+from openepd.model.pcr import Pcr
 from openepd.model.specs import Specs
 from openepd.model.standard import Standard
 
 
 class Epd(BaseOpenEpdSchema):
     """Represent an EPD."""
 
@@ -42,15 +43,31 @@
     doctype: Literal["OpenEPD", "ILCD_EPD"] = pyd.Field(
         description='Describes the type and schema of the document. Must always always read "openEPD".',
         default="OpenEPD",
     )
     product_name: str = pyd.Field(
         max_length=200, description="The name of the product described by this EPD", example="Mix 12345AC"
     )
+    product_sku: str | None = pyd.Field(
+        max_length=200, description="Unique stock keeping identifier assigned by manufacturer"
+    )
+    product_description: str | None = pyd.Field(
+        max_length=2000,
+        description="1-paragraph description of product. " "Supports plain text or github flavored markdown.",
+    )
     # TODO: add product_alt_names? E.g. ILCD has a list of synonymous names
+    product_classes: dict[str, str] = pyd.Field(
+        description="List of classifications, including Masterformat and UNSPC", default_factory=dict
+    )
+    product_image_small: pyd.AnyUrl | None = pyd.Field(
+        description="Pointer to image illustrating the product, which is no more than 200x200 pixels", default=None
+    )
+    product_image: pyd.AnyUrl | None = pyd.Field(
+        description="pointer to image illustrating the product no more than 10MB", default=None
+    )
     version: pyd.PositiveInt = pyd.Field(
         description="Version of this document. The document's issuer should increment it anytime even a single "
         "character changes, as this value is used to determine the most recent version.",
         example=1,
     )
     language: str | None = pyd.Field(
         min_length=2,
@@ -100,22 +117,84 @@
         example=datetime.date(day=11, month=9, year=2019),
         description="Date the EPD was issued. This should be the first day on which the EPD is valid.",
     )
     valid_until: datetime.date | None = pyd.Field(
         example=datetime.date(day=11, month=9, year=2028),
         description="Last date the EPD is valid on, including any extensions.",
     )
-    product_class: dict[str, str] = pyd.Field(
-        description="List of classifications, including Masterformat and UNSPC", default_factory=dict
+    pcr: Pcr | None = pyd.Field(
+        description="JSON object for product category rules. Should point to the "
+        "most-specific PCR that applies; the PCR entry should point to any "
+        "parent PCR.",
+        default=None,
     )
     declared_unit: Amount | None = pyd.Field(
         description="SI declared unit for this EPD.  If a functional unit is "
         "utilized, the declared unit shall refer to the amount of "
         "product associated with the A1-A3 life cycle stage."
     )
+    kg_per_declared_unit: Amount | None = pyd.Field(
+        default=None,
+        description="Mass of the product, in kilograms, per declared unit",
+        example=Amount(qty=12.5, unit="kg"),
+    )
+    kg_C_per_declared_unit: Amount | None = pyd.Field(
+        default=None,
+        description="Mass of elemental carbon, per declared unit, contained in the product itself at the manufacturing "
+        "facility gate.  Used (among other things) to check a carbon balance or calculate incineration "
+        "emissions.  The source of carbon (e.g. biogenic) is not relevant in this field.",
+        example=Amount(qty=8.76, unit="kg"),
+    )
+    kg_C_biogenic_per_declared_unit: Amount | None = pyd.Field(
+        default=None,
+        description="Mass of elemental carbon from biogenic sources, per declared unit, contained in the product "
+        "itself at the manufacturing facility gate.  It may be presumed that any biogenic carbon content "
+        "has been accounted for as -44/12 kgCO2e per kg C in stages A1-A3, per EN15804 and ISO 21930.",
+        example=Amount(qty=8.76, unit="kg"),
+    )
+    product_service_life_years: float | None = pyd.Field(
+        gt=0.0009,
+        lt=101,
+        description="Reference service life of the product, in years.  Serves as a maximum for replacement interval, "
+        "which may also be constrained by usage or the service life of what the product goes into "
+        "(e.g. a building).",
+        example=50.0,
+    )
+    annual_production: float | None = pyd.Field(
+        gt=0,
+        default=None,
+        description="Approximate annual production volume, in declared units, of product covered by this EPD. "
+        "This value is intended to be used for weighting of averages. "
+        "Providing this data is optional, and it is acceptable to round or obfuscate it downwards "
+        "(but not upwards) by any amount desired to protect confidentiality. For example, if the "
+        "product volume is 123,456 m3, a value of 120,000, 100,000 or even 87,654 would be acceptable.",
+        example=10000,
+    )
+    applicable_in: list[Annotated[str, pyd.Field(min_length=2, max_length=2)]] | None = pyd.Field(
+        max_items=100,
+        default=None,
+        description="Jurisdiction(s) in which EPD is applicable. An empty array, or absent properties, "
+        "implies global applicability.",
+        example=["US", "CA", "MX"],
+    )
+    product_usage_description: str | None = pyd.Field(
+        default=None,
+        description="Text description of how product is typically used. Can be used to describe accessories "
+        "like fasteners, adhesives, etc.  Supports plain text or github flavored markdown.",
+    )
+    product_usage_image: pyd.AnyUrl | None = pyd.Field(
+        description="Pointer (url) to image illustrating how the product is used. No more than 10MB.", default=None
+    )
+    manufacturing_description: str | None = pyd.Field(
+        default=None,
+        description="Text description of manufacturing process.  Supports plain text or github flavored markdown.",
+    )
+    manufacturing_image: pyd.AnyUrl | None = pyd.Field(
+        description="Pointer (url) to an image illustrating the manufacturing process. No more than 10MB.", default=None
+    )
     impacts: ImpactSet | None = pyd.Field(
         description="List of environmental impacts, compiled per one of the standard Impact Assessment methods"
     )
     resource_uses: ResourceUseSet | None = pyd.Field(
         description="Set of Resource Use Indicators, over various LCA scopes"
     )
     output_flows: OutputFlowSet | None = pyd.Field(
@@ -125,14 +204,19 @@
     compliance: list[Standard] = pyd.Field(
         description="Standard(s) to which this declaration is compliant.", default_factory=list
     )
     specs: Specs = pyd.Field(
         default_factory=Specs,
         description="Data structure(s) describing performance specs of product. Unique for each material type.",
     )
+    includes: list[Ingredient] = pyd.Field(
+        max_items=255,
+        description="List of JSON objects pointing to product components. "
+        "Each one should be an EPD or digitized LCI process.",
+    )
     lca_discussion: str | None = pyd.Field(
         max_length=20000,
         description="""A rich text description containing information for experts reviewing the EPD contents. 
     Text descriptions required by ISO 14025, ISO 21930, EN 15804,, relevant PCRs, or program instructions and which do not 
     have specific openEPD fields should be entered here.  This field may be large, and may contain multiple sections 
     separated by github flavored markdown formatting.""",
         example="""# Packaging
```

### Comparing `openepd-0.5.0/src/openepd/model/lcia.py` & `openepd-0.6.0/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/org.py` & `openepd-0.6.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/pcr.py` & `openepd-0.6.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/specs/__init__.py` & `openepd-0.6.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/specs/concrete.py` & `openepd-0.6.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/src/openepd/model/standard.py` & `openepd-0.6.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-0.5.0/PKG-INFO` & `openepd-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.5.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.6.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

