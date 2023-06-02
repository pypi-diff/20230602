# Comparing `tmp/SmoobuExtractorFormatter-1.0.3.tar.gz` & `tmp/SmoobuExtractorFormatter-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.0.3.tar", last modified: Thu May 11 19:08:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

