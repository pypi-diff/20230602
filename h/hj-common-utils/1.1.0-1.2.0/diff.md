# Comparing `tmp/hj-common-utils-1.1.0.tar.gz` & `tmp/hj_common_utils-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-common-utils-1.1.0.tar", last modified: Wed May 31 13:21:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

