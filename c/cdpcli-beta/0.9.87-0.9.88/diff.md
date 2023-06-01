# Comparing `tmp/cdpcli-beta-0.9.87.tar.gz` & `tmp/cdpcli-beta-0.9.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.87.tar", last modified: Fri May 19 07:55:44 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.88.tar", last modified: Thu Jun  1 21:08:34 2023, max compression
```

## Comparing `cdpcli-beta-0.9.87.tar` & `cdpcli-beta-0.9.88.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    95423 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   143027 2023-05-19 07:55:42.000000 cdpcli-beta-0.9.87/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   104133 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31670 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-05-19 07:55:42.000000 cdpcli-beta-0.9.87/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193583 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   175998 2023-05-19 07:55:39.000000 cdpcli-beta-0.9.87/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    72034 2023-05-19 07:55:42.000000 cdpcli-beta-0.9.87/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.250873 cdpcli-beta-0.9.87/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.266873 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.250873 cdpcli-beta-0.9.87/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.266873 cdpcli-beta-0.9.87/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.266873 cdpcli-beta-0.9.87/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    95423 2023-06-01 21:08:29.000000 cdpcli-beta-0.9.88/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   148743 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   104133 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31670 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-01 21:08:31.000000 cdpcli-beta-0.9.88/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193260 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   175998 2023-06-01 21:08:29.000000 cdpcli-beta-0.9.88/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-06-01 21:08:31.000000 cdpcli-beta-0.9.88/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    72034 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.350914 cdpcli-beta-0.9.88/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.354914 cdpcli-beta-0.9.88/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/versioneer.py
```

### Comparing `cdpcli-beta-0.9.87/LICENSE.txt` & `cdpcli-beta-0.9.88/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.88/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/PKG-INFO` & `cdpcli-beta-0.9.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.87
+Version: 0.9.88
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.87/README.md` & `cdpcli-beta-0.9.88/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/__init__.py` & `cdpcli-beta-0.9.88/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/argparser.py` & `cdpcli-beta-0.9.88/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/argprocess.py` & `cdpcli-beta-0.9.88/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/arguments.py` & `cdpcli-beta-0.9.88/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/auth.py` & `cdpcli-beta-0.9.88/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.88/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/clicommand.py` & `cdpcli-beta-0.9.88/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/clidriver.py` & `cdpcli-beta-0.9.88/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/client.py` & `cdpcli-beta-0.9.88/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/compat.py` & `cdpcli-beta-0.9.88/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/completer.py` & `cdpcli-beta-0.9.88/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/config.py` & `cdpcli-beta-0.9.88/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/configloader.py` & `cdpcli-beta-0.9.88/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/credentials.py` & `cdpcli-beta-0.9.88/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.88/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/cli.json` & `cdpcli-beta-0.9.88/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/datahub/datahub.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -57,14 +57,57 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/ListClustersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/datahub/listScalingActivities:
+    post:
+      summary: Lists Scaling activities for a cluster.
+      description: Lists Scaling activities for a cluster.
+      operationId: listScalingActivities
+      x-mutating: false
+      x-paging-default-max-items: 100
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ListScalingActivitiesRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ListScalingActivitiesResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/datahub/describeScalingActivity:
+    post:
+      summary: Describes the Scaling Activity using Cluster CRN or Cluster NAME and operation ID.
+      description: Describes the Scaling Activity using Cluster CRN or Cluster NAME and operation ID.
+      operationId: describeScalingActivity
+      x-mutating: false
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/DescribeScalingActivityRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/DescribeScalingActivityResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/datahub/listClusterLifecycleEvents:
     post:
       summary: Lists Workload cluster lifecycle events.
       description: Lists Workload cluster lifecycle events.
       operationId: listClusterLifecycleEvents
       x-mutating: false
       x-paging-default-max-items: 100
@@ -1475,14 +1518,41 @@
         description: The related knox entry.
       mode:
         type: string
         description: The SSO mode of the given service.
       open:
         type: boolean
         description: The access status of the given endpoint. Whether its open or not.
+  ScalingActivitySummary:
+    type: object
+    description: Information about a Scaling activity.
+    required:
+      - operationId
+      - startTime
+      - endTime
+      - scalingActivityReason
+      - activityStatus
+    properties:
+      operationId:
+        type: string
+        description: The operation ID of the scaling activity.
+      startTime:
+        type: string
+        format: date-time
+        description: The start time of the scaling activity.
+      endTime:
+        type: string
+        format: date-time
+        description: The end time of the scaling activity.
+      scalingActivityReason:
+        type: string
+        description: The reason of the scaling activity.
+      activityStatus:
+        type: string
+        description: The status of the scaling activity. Supported values- ACTIVITY_PENDING - If scaling activity is in pending state, METRICS_COLLECTION_SUCCESS/FAILED - for success/failure of metrics collection, UPSCALE_TRIGGER_SUCCESS/FAILED - for success/failure at the time of upscaling, DOWNSCALE_TRIGGER_SUCCESS/FAILED for success/failure at the time of downscaling, SCHEDULE_BASED_UPSCALE/DOWNSCALE - if schedule based scaling is used, SCALING_FLOW_IN_PROGRESS/SUCCESS/FAILED - State at which the scaling has reached, POLICY_ADJUSTMENT - if policy adjustment is taking place, UNKNOWN - if the state is not known.
   ClusterSummary:
     type: object
     description: Information about a cluster.
     required:
       - clusterName
       - crn
     properties:
@@ -2070,14 +2140,87 @@
       - clusters
     properties:
       clusters:
         type: array
         items:
           $ref: '#/definitions/ClusterSummary'
         description: The clusters.
+  ListScalingActivitiesRequest:
+    type: object
+    description: Request object for List scaling Activities request.
+    required:
+      - cluster
+    properties:
+      cluster:
+        type: string
+        description: The name or CRN of the cluster.
+      duration:
+        type: integer
+        format: int64
+        description: Duration in minutes for which we want all the scaling activities for the cluster. Either duration or start and end time needs to be provided.
+      startTime:
+        type: integer
+        format: int64
+        description: Start time value in epoch millisecond from which we want to get all the scaling activities. Need to specify end time with it.
+      endTime:
+        type: integer
+        format: int64
+        description: End time value in epoch millisecond until which we want to get all the scaling activities. Need to specify start time with it.
+      onlyFailedScalingActivities:
+        type: boolean
+        description: Flag that decides whether to return only failed scaling activities or return all scaling activities in a given duration or a specific time interval.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of the page for getting scaling activities.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListScalingActivitiesResponse:
+    type: object
+    description: Response object for list scaling activities request.
+    required:
+      - scalingActivity
+    properties:
+      scalingActivity:
+        type: array
+        items:
+          $ref: '#/definitions/ScalingActivitySummary'
+        x-paging-result: true
+        description: The list of scaling activities.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  DescribeScalingActivityRequest:
+    type: object
+    description: Request object for describing a particular scaling activity using clusterCrn or clusterName and operationId.
+    required:
+      - cluster
+      - operationId
+    properties:
+      cluster:
+        type: string
+        description: The name or CRN of the cluster.
+      operationId:
+        type: string
+        description: Operation ID of the scaling activity.
+  DescribeScalingActivityResponse:
+    type: object
+    description: Response object for describe scaling activity request.
+    required:
+      - scalingActivity
+    properties:
+      scalingActivity:
+        $ref: '#/definitions/ScalingActivitySummary'
+        description: The scaling activity.
   AttachedVolumeRequest:
     type: object
     description: Configurations for additional attached volumes.
     required:
       - volumeSize
       - volumeCount
       - volumeType
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/de/de.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/dw/dw.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -2151,19 +2151,14 @@
       privateDNSZoneAKS:
         type: string
         description: Private DNS zone AKS resource ID.
       enablePrivateAks:
         type: boolean
         description: Enable Azure Private AKS mode.
         default: false
-      enableUptimeSLA:
-        x-deprecated: true
-        type: boolean
-        description: Enable uptime SLA for Kubernetes API server. This option is deprecated and will be removed upon the next release of the DWX Public Cloud. The uptime SLA for the Kubernetes API server will be always enabled.
-        default: false
   PrivateCloudActivationOptions:
     type: object
     description: Options for activating a Private Cloud environment.
     required:
       - delegationUsername
       - delegationPassword
     properties:
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/environments/environments.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.88/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.87
+  version: 0.9.88
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.87/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.88/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.88/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/doc/style.py` & `cdpcli-beta-0.9.88/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/docs.py` & `cdpcli-beta-0.9.88/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/endpoint.py` & `cdpcli-beta-0.9.88/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.88/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/exceptions.py` & `cdpcli-beta-0.9.88/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.88/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/formatter.py` & `cdpcli-beta-0.9.88/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/help.py` & `cdpcli-beta-0.9.88/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/loader.py` & `cdpcli-beta-0.9.88/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/main.py` & `cdpcli-beta-0.9.88/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/model.py` & `cdpcli-beta-0.9.88/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/paginate.py` & `cdpcli-beta-0.9.88/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/paramfile.py` & `cdpcli-beta-0.9.88/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.88/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/parser.py` & `cdpcli-beta-0.9.88/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.88/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/schema.py` & `cdpcli-beta-0.9.88/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/serialize.py` & `cdpcli-beta-0.9.88/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/shorthand.py` & `cdpcli-beta-0.9.88/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/signers.py` & `cdpcli-beta-0.9.88/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/table.py` & `cdpcli-beta-0.9.88/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/text.py` & `cdpcli-beta-0.9.88/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/textwriter.py` & `cdpcli-beta-0.9.88/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.88/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/translate.py` & `cdpcli-beta-0.9.88/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/utils.py` & `cdpcli-beta-0.9.88/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli/validate.py` & `cdpcli-beta-0.9.88/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.88/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.87
+Version: 0.9.88
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.87/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.88/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/setup.py` & `cdpcli-beta-0.9.88/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/setup_common.py` & `cdpcli-beta-0.9.88/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/__init__.py` & `cdpcli-beta-0.9.88/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.88/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.88/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.88/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.88/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_auth.py` & `cdpcli-beta-0.9.88/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.88/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_client.py` & `cdpcli-beta-0.9.88/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_completer.py` & `cdpcli-beta-0.9.88/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.88/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_docs.py` & `cdpcli-beta-0.9.88/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.88/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_help.py` & `cdpcli-beta-0.9.88/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.88/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_model.py` & `cdpcli-beta-0.9.88/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.88/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.88/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.88/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.88/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.88/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_signers.py` & `cdpcli-beta-0.9.88/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.88/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_utils.py` & `cdpcli-beta-0.9.88/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/tests/unit/test_validate.py` & `cdpcli-beta-0.9.88/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.87/versioneer.py` & `cdpcli-beta-0.9.88/versioneer.py`

 * *Files identical despite different names*

