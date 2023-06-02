# Comparing `tmp/odoo_addons_oca_sale_promotion-15.0.20230531.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_sale_promotion-15.0.20230601.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1672 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2627 b- defN 23-Jun-01 08:25 odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 08:25 odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-01 08:25 odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      429 b- defN 23-Jun-01 08:25 odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/RECORD
-4 files, 3149 bytes uncompressed, 826 bytes compressed:  73.8%
+Zip file size: 1695 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2865 b- defN 23-Jun-02 04:45 odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 04:45 odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 04:45 odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      429 b- defN 23-Jun-02 04:45 odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/RECORD
+4 files, 3387 bytes uncompressed, 849 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/METADATA
+Filename: odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/WHEEL
+Filename: odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/RECORD
+Filename: odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_sale_promotion-15.0.20230531.0.dist-info/METADATA` & `odoo_addons_oca_sale_promotion-15.0.20230601.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-sale-promotion
-Version: 15.0.20230531.0
+Version: 15.0.20230601.1
 Summary: Meta package for oca-sale-promotion Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 15.0
@@ -15,29 +15,32 @@
 Requires-Dist: odoo-addon-coupon-domain-product-discount (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-coupon-incompatibility (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-coupon-limit (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-coupon-mass-mailing (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-coupon-multi-gift (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-coupon-multiplier-free-product (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-coupon-portal (<15.1dev,>=15.0dev)
+Requires-Dist: odoo-addon-coupon-promotion-generate-coupon (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-auto-refresh (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-criteria-multi-product (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-criteria-order-based (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-delivery-auto-refresh (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-domain-free-product (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-domain-product-discount (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-financial-risk (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-incompatibility (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-limit (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-multi-gift (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-multiple-code-program (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-multiplier-free-product (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-order-line-link (<15.1dev,>=15.0dev)
+Requires-Dist: odoo-addon-sale-coupon-order-pending (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-order-suggestion (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-partner (<15.1dev,>=15.0dev)
+Requires-Dist: odoo-addon-sale-coupon-promotion-generate-coupon (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-selection-wizard (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-coupon-validity-notification (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-website-sale-coupon-page (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-website-sale-coupon-restrict (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-website-sale-coupon-selection-wizard (<15.1dev,>=15.0dev)
 
 UNKNOWN
```

