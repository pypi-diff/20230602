# Comparing `tmp/imops-0.7.4.tar.gz` & `tmp/imops-0.8.0-cp36-cp36m-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imops-0.7.4.tar", last modified: Sun Apr 16 18:03:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

