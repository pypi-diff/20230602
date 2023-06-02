# Comparing `tmp/sarw_spheres-0.0.6.tar.gz` & `tmp/sarw_spheres-0.0.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarw_spheres-0.0.6.tar", last modified: Wed Jan  4 13:20:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

