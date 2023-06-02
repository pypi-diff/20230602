# Comparing `tmp/emerge-viz-1.5.0.tar.gz` & `tmp/emerge_viz-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emerge-viz-1.5.0.tar", last modified: Sun Jan  1 20:07:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

