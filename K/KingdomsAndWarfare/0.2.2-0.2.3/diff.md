# Comparing `tmp/KingdomsAndWarfare-0.2.2.tar.gz` & `tmp/KingdomsAndWarfare-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KingdomsAndWarfare-0.2.2.tar", last modified: Wed May 31 05:16:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

