# Comparing `tmp/posuto-2023.5.0.tar.gz` & `tmp/posuto-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posuto-2023.5.0.tar", last modified: Sun Apr 30 12:09:50 2023, max compression
+gzip compressed data, was "posuto-2023.6.0.tar", last modified: Fri Jun  2 01:28:54 2023, max compression
```

## Comparing `posuto-2023.5.0.tar` & `posuto-2023.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.217493 posuto-2023.5.0/.github/
--rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.5.0/.github/FUNDING.yml
--rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.5.0/.gitignore
--rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.5.0/LICENSE
--rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.5.0/MANIFEST.in
--rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.5.0/Makefile
--rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-04-30 12:09:50.280827 posuto-2023.5.0/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.5.0/README.md
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.217493 posuto-2023.5.0/examples/
--rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.5.0/examples/sample.py
--rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.5.0/postcharacter.png
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/posuto/
--rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.5.0/posuto/__init__.py
--rw-r--r--   0 23        (1000) u23       (1000) 13104799 2023-04-30 11:44:00.000000 posuto-2023.5.0/posuto/officedata.json
--rw-r--r--   0 23        (1000) u23       (1000) 81154048 2023-04-30 11:44:01.000000 posuto-2023.5.0/posuto/postaldata.db
--rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.5.0/posuto/posuto.py
--rw-r--r--   0 23        (1000) u23       (1000)    11156 2023-03-15 04:34:33.000000 posuto-2023.5.0/posuto/prep.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/posuto/tests/
--rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.5.0/posuto/tests/test_basic.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/posuto.egg-info/
--rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)      367 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/SOURCES.txt
--rw-r--r--   0 23        (1000) u23       (1000)        1 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/dependency_links.txt
--rw-r--r--   0 23        (1000) u23       (1000)        7 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/top_level.txt
--rw-r--r--   0 23        (1000) u23       (1000)      706 2023-04-30 12:09:50.280827 posuto-2023.5.0/setup.cfg
--rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.5.0/setup.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.158424 posuto-2023.6.0/.github/
+-rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.6.0/.github/FUNDING.yml
+-rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.6.0/.gitignore
+-rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.6.0/LICENSE
+-rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.6.0/MANIFEST.in
+-rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.6.0/Makefile
+-rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-06-02 01:28:54.258375 posuto-2023.6.0/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.6.0/README.md
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.158424 posuto-2023.6.0/examples/
+-rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.6.0/examples/sample.py
+-rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.6.0/postcharacter.png
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/posuto/
+-rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.6.0/posuto/__init__.py
+-rw-r--r--   0 23        (1000) u23       (1000) 13065151 2023-06-02 01:27:03.000000 posuto-2023.6.0/posuto/officedata.json
+-rw-r--r--   0 23        (1000) u23       (1000) 81154048 2023-06-02 01:27:04.000000 posuto-2023.6.0/posuto/postaldata.db
+-rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.6.0/posuto/posuto.py
+-rw-r--r--   0 23        (1000) u23       (1000)    11156 2023-03-15 04:34:33.000000 posuto-2023.6.0/posuto/prep.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/posuto/tests/
+-rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.6.0/posuto/tests/test_basic.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/posuto.egg-info/
+-rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)      367 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/SOURCES.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        1 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/dependency_links.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        7 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/top_level.txt
+-rw-r--r--   0 23        (1000) u23       (1000)      706 2023-06-02 01:28:54.261707 posuto-2023.6.0/setup.cfg
+-rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.6.0/setup.py
```

### Comparing `posuto-2023.5.0/.gitignore` & `posuto-2023.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/LICENSE` & `posuto-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/Makefile` & `posuto-2023.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/PKG-INFO` & `posuto-2023.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `posuto-2023.5.0/README.md` & `posuto-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/postcharacter.png` & `posuto-2023.6.0/postcharacter.png`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/posuto/officedata.json` & `posuto-2023.6.0/posuto/officedata.json`

 * *Files 0% similar despite different names*

```diff
@@ -27774,15 +27774,15 @@
     "neighborhood": "大字沖田面",
     "banchi": "字沖中46",
     "postal_code": "0390195",
     "old_code": "03901",
     "post_office": "三戸",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0390592": {
     "jis": "02445",
@@ -27793,15 +27793,15 @@
     "neighborhood": "大字平",
     "banchi": "字広場28番地1",
     "postal_code": "0390592",
     "old_code": "03905",
     "post_office": "上名久井",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0390892": {
     "jis": "02445",
@@ -27812,15 +27812,15 @@
     "neighborhood": "大字苫米地",
     "banchi": "字下宿23-1",
     "postal_code": "0390892",
     "old_code": "03908",
     "post_office": "福地",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0208584": {
     "jis": "03201",
@@ -37846,15 +37846,15 @@
     "neighborhood": "瀬峰",
     "banchi": "長者原37番地2",
     "postal_code": "9894592",
     "old_code": "98945",
     "post_office": "高清水",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9895392": {
     "jis": "04213",
@@ -47688,15 +47688,15 @@
     "neighborhood": "富田町",
     "banchi": "字諏訪内37(郡山郵便局私書箱第37号)",
     "postal_code": "9638637",
     "old_code": "963  ",
     "post_office": "郡山",
     "type": "box",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "トミタマチ",
     "alternates": []
   },
   "9638580": {
     "jis": "07203",
@@ -48582,15 +48582,15 @@
     "neighborhood": "好間工業団地",
     "banchi": "20-1",
     "postal_code": "9701192",
     "old_code": "97011",
     "post_office": "いわき",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "イワキシ",
     "neighborhood_kana": "ヨシマコウギョウダンチ",
     "alternates": []
   },
   "9701193": {
     "jis": "07204",
@@ -59517,29 +59517,29 @@
     "prefecture_kana": "トチギケン",
     "city_kana": "ニッコウシ",
     "neighborhood_kana": "キヌガワオンセンタキ",
     "alternates": []
   },
   "3212593": {
     "jis": "09206",
-    "kana": "ドツキヨウイカダイガク ニツコウイリヨウセンタ-",
-    "name": "獨協医科大学　日光医療センター",
+    "kana": "トウブワ-ルドスクウエア カブシキカイシヤ",
+    "name": "東武ワールドスクウェア　株式会社",
     "prefecture": "栃木県",
     "city": "日光市",
-    "neighborhood": "高徳",
-    "banchi": "632",
+    "neighborhood": "鬼怒川温泉大原",
+    "banchi": "209-1",
     "postal_code": "3212593",
     "old_code": "32125",
     "post_office": "鬼怒川温泉",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トチギケン",
     "city_kana": "ニッコウシ",
-    "neighborhood_kana": "タカトク",
+    "neighborhood_kana": "キヌガワオンセンオオハラ",
     "alternates": []
   },
   "3212596": {
     "jis": "09206",
     "kana": "ニツコウシ フジハラスイドウジムシヨ",
     "name": "日光市　藤原水道事務所",
     "prefecture": "栃木県",
@@ -59908,15 +59908,15 @@
     "neighborhood": "本町",
     "banchi": "2丁目2828-4",
     "postal_code": "3248551",
     "old_code": "324  ",
     "post_office": "大田原",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
     "neighborhood_kana": "ホンチョウ",
     "alternates": []
   },
   "3248641": {
     "jis": "09210",
@@ -59946,15 +59946,15 @@
     "neighborhood": "本町",
     "banchi": "2-2828-4",
     "postal_code": "3248765",
     "old_code": "324  ",
     "post_office": "大田原",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
     "neighborhood_kana": "ホンチョウ",
     "alternates": []
   },
   "3248625": {
     "jis": "09210",
@@ -60080,15 +60080,15 @@
     "neighborhood": "本町",
     "banchi": "2丁目2828-4",
     "postal_code": "3248585",
     "old_code": "324  ",
     "post_office": "大田原",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
     "neighborhood_kana": "ホンチョウ",
     "alternates": []
   },
   "3248686": {
     "jis": "09210",
@@ -65286,15 +65286,15 @@
     "neighborhood": "藤岡",
     "banchi": "1360",
     "postal_code": "3758507",
     "old_code": "375  ",
     "post_office": "藤岡",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "グンマケン",
     "city_kana": "フジオカシ",
     "neighborhood_kana": "フジオカ",
     "alternates": []
   },
   "3758501": {
     "jis": "10209",
@@ -70241,21 +70241,21 @@
   "3368526": {
     "jis": "11108",
     "kana": "コ-プデリセイカツキヨウドウクミアイレンゴウカイ",
     "name": "コープデリ生活協同組合連合会",
     "prefecture": "埼玉県",
     "city": "さいたま市南区",
     "neighborhood": "根岸",
-    "banchi": "1丁目4-13",
+    "banchi": "1丁目5番5号",
     "postal_code": "3368526",
     "old_code": "336  ",
     "post_office": "さいたま中央",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "サイタマケン",
     "city_kana": "サイタマシミナミク",
     "neighborhood_kana": "ネギシ",
     "alternates": []
   },
   "3368586": {
     "jis": "11108",
@@ -78778,15 +78778,15 @@
     "neighborhood": "小室",
     "banchi": "4472-1",
     "postal_code": "3628577",
     "old_code": "362  ",
     "post_office": "上尾",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "サイタマケン",
     "city_kana": "キタアダチグンイナマチ",
     "neighborhood_kana": "コムロ",
     "alternates": []
   },
   "3548565": {
     "jis": "11324",
@@ -79754,14 +79754,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
+  "3670393": {
+    "jis": "11383",
+    "kana": "カミカワマチカミイズミソウゴウシシヨ",
+    "name": "神川町神泉総合支所",
+    "prefecture": "埼玉県",
+    "city": "児玉郡神川町",
+    "neighborhood": "大字下阿久原",
+    "banchi": "1088",
+    "postal_code": "3670393",
+    "old_code": "36703",
+    "post_office": "児玉",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "",
+    "city_kana": "",
+    "neighborhood_kana": "",
+    "alternates": []
+  },
   "3690395": {
     "jis": "11385",
     "kana": "カブシキカイシヤ ヒタチハイテクフアインシステムズ",
     "name": "株式会社　日立ハイテクファインシステムズ",
     "prefecture": "埼玉県",
     "city": "児玉郡上里町",
     "neighborhood": "嘉美",
@@ -80673,21 +80692,21 @@
   "2608508": {
     "jis": "12101",
     "kana": "シヤカイフクシホウジン チバケンシヤカイフクシキヨウギカイ",
     "name": "社会福祉法人　千葉県社会福祉協議会",
     "prefecture": "千葉県",
     "city": "千葉市中央区",
     "neighborhood": "千葉港",
-    "banchi": "4-3",
+    "banchi": "4-5",
     "postal_code": "2608508",
     "old_code": "260  ",
     "post_office": "千葉中央",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "チバケン",
     "city_kana": "チバシチュウオウク",
     "neighborhood_kana": "チバミナト",
     "alternates": []
   },
   "2608521": {
     "jis": "12101",
@@ -87608,25 +87627,25 @@
   },
   "2778551": {
     "jis": "12217",
     "kana": "カシワコウセイソウゴウビヨウイン",
     "name": "柏厚生総合病院",
     "prefecture": "千葉県",
     "city": "柏市",
-    "neighborhood": "あけぼの",
-    "banchi": "3丁目8-20",
+    "neighborhood": "篠籠田",
+    "banchi": "617番地",
     "postal_code": "2778551",
     "old_code": "277  ",
     "post_office": "柏",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "チバケン",
     "city_kana": "カシワシ",
-    "neighborhood_kana": "アケボノ",
+    "neighborhood_kana": "シコダ",
     "alternates": []
   },
   "2778503": {
     "jis": "12217",
     "kana": "カシワシ シヨウナンチヨウシヤ",
     "name": "柏市沼南庁舎",
     "prefecture": "千葉県",
@@ -88248,28 +88267,66 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "カシワシ",
     "neighborhood_kana": "カシワノハ",
     "alternates": []
   },
+  "2778563": {
+    "jis": "12217",
+    "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカカンキヨウトウ",
+    "name": "東京大学大学院　新領域創成科学研究科環境棟",
+    "prefecture": "千葉県",
+    "city": "柏市",
+    "neighborhood": "柏の葉",
+    "banchi": "5-1-5",
+    "postal_code": "2778563",
+    "old_code": "277  ",
+    "post_office": "柏",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "チバケン",
+    "city_kana": "カシワシ",
+    "neighborhood_kana": "カシワノハ",
+    "alternates": []
+  },
   "2778561": {
     "jis": "12217",
-    "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカ",
-    "name": "東京大学大学院　新領域創成科学研究科",
+    "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカキバントウ",
+    "name": "東京大学大学院　新領域創成科学研究科基盤棟",
     "prefecture": "千葉県",
     "city": "柏市",
     "neighborhood": "柏の葉",
-    "banchi": "5丁目1番5号",
+    "banchi": "5-1-5",
     "postal_code": "2778561",
     "old_code": "277  ",
     "post_office": "柏",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
+    "prefecture_kana": "チバケン",
+    "city_kana": "カシワシ",
+    "neighborhood_kana": "カシワノハ",
+    "alternates": []
+  },
+  "2778562": {
+    "jis": "12217",
+    "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカセイメイトウ",
+    "name": "東京大学大学院　新領域創成科学研究科生命棟",
+    "prefecture": "千葉県",
+    "city": "柏市",
+    "neighborhood": "柏の葉",
+    "banchi": "5-1-5",
+    "postal_code": "2778562",
+    "old_code": "277  ",
+    "post_office": "柏",
+    "type": "office",
+    "multiple": false,
+    "new": true,
     "prefecture_kana": "チバケン",
     "city_kana": "カシワシ",
     "neighborhood_kana": "カシワノハ",
     "alternates": []
   },
   "2778587": {
     "jis": "12217",
@@ -97166,33 +97223,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018481": {
-    "jis": "13101",
-    "kana": "アサヒカセイフア-マ カブシキガイシヤ",
-    "name": "旭化成ファーマ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田美土代町",
-    "banchi": "9番地1MD神田ビル",
-    "postal_code": "1018481",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダミトシロチョウ",
-    "alternates": []
-  },
   "1018101": {
     "jis": "13101",
     "kana": "アサヒカセイホ-ムズ カブシキガイシヤ",
     "name": "旭化成ホームズ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田神保町",
@@ -97223,33 +97261,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018604": {
-    "jis": "13101",
-    "kana": "アルフアサイケンカイシユウ カブシキガイシヤ",
-    "name": "アルファ債権回収　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "3丁目12番8号住友不動産秋葉原ビル17階",
-    "postal_code": "1018604",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018512": {
     "jis": "13101",
     "kana": "アルフレツサ カブシキガイシヤ",
     "name": "アルフレッサ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田美土代町",
@@ -97280,14 +97299,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
+  "1018333": {
+    "jis": "13101",
+    "kana": "イツパンザイダンホウジン サンギヨウケイリキヨウカイ",
+    "name": "一般財団法人　産業経理協会",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "神田淡路町",
+    "banchi": "1丁目15-6",
+    "postal_code": "1018333",
+    "old_code": "101  ",
+    "post_office": "神田",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "カンダアワジチョウ",
+    "alternates": []
+  },
   "1018986": {
     "jis": "13101",
     "kana": "イツパンザイダンホウジン ニホンケンチクセンタ-",
     "name": "一般財団法人　日本建築センター",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
@@ -97318,14 +97356,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスダチョウ",
     "alternates": []
   },
+  "1018459": {
+    "jis": "13101",
+    "kana": "イツパンシヤダンホウジン ガクシカイ",
+    "name": "一般社団法人　学士会",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "神田錦町",
+    "banchi": "3丁目28",
+    "postal_code": "1018459",
+    "old_code": "101  ",
+    "post_office": "神田",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "カンダニシキチョウ",
+    "alternates": []
+  },
   "1018534": {
     "jis": "13101",
     "kana": "イツパンシヤダンホウジン ゼンコクシンヨウホシヨウキヨウカイレンゴウカイ",
     "name": "一般社団法人　全国信用保証協会連合会",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田司町",
@@ -97337,14 +97394,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダツカサマチ",
     "alternates": []
   },
+  "1018509": {
+    "jis": "13101",
+    "kana": "イツパンシヤダンホウジン ゼンコクチホウギンコウキヨウカイ",
+    "name": "一般社団法人　全国地方銀行協会",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "内神田",
+    "banchi": "3丁目1-2",
+    "postal_code": "1018509",
+    "old_code": "101  ",
+    "post_office": "神田",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "ウチカンダ",
+    "alternates": []
+  },
   "1018611": {
     "jis": "13101",
     "kana": "イツパンシヤダンホウジン トウキヨウトコウユウカイ",
     "name": "一般社団法人　東京都交友会",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -97451,33 +97527,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ニシカンダ",
     "alternates": []
   },
-  "1018352": {
-    "jis": "13101",
-    "kana": "オオハラボキガツコウ",
-    "name": "大原簿記学校",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "西神田",
-    "banchi": "1丁目3-6-8F",
-    "postal_code": "1018352",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ニシカンダ",
-    "alternates": []
-  },
   "1018228": {
     "jis": "13101",
     "kana": "オオバヤシドウロ カブシキガイシヤ",
     "name": "大林道路　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "猿楽町",
@@ -97527,126 +97584,69 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "イワモトチョウ",
     "alternates": []
   },
-  "1018627": {
-    "jis": "13101",
-    "kana": "カガデンシ カブシキガイシヤ カンキヨウジギヨウブ、ギジユツトウカツブ ホカ",
-    "name": "加賀電子　株式会社　環境事業部、技術統括部　他",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田松永町",
-    "banchi": "19-2-5F",
-    "postal_code": "1018627",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダマツナガチョウ",
-    "alternates": []
-  },
   "1018629": {
     "jis": "13101",
     "kana": "カガデンシ カブシキガイシヤ カンリホンブ、ヒシヨ・コウホウシツ",
     "name": "加賀電子　株式会社　管理本部、秘書・広報室",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田松永町",
-    "banchi": "19-2-10F",
+    "banchi": "20-10F",
     "postal_code": "1018629",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダマツナガチョウ",
     "alternates": []
   },
-  "1018628": {
+  "1018627": {
     "jis": "13101",
-    "kana": "カガデンシ カブシキガイシヤ デンシジギヨウブ、エイギヨウスイシンジギヨウブ、トクハンジギヨウブ",
-    "name": "加賀電子　株式会社　電子事業部、営業推進事業部、特販事業部",
+    "kana": "カガデンシ カブシキガイシヤ ギジユツトウカツブ",
+    "name": "加賀電子　株式会社　技術統括部",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田松永町",
-    "banchi": "19-2-8F",
-    "postal_code": "1018628",
+    "banchi": "20-5F",
+    "postal_code": "1018627",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダマツナガチョウ",
     "alternates": []
   },
-  "1018543": {
-    "jis": "13101",
-    "kana": "カシムラ",
-    "name": "（株）　樫村",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "鍛冶町",
-    "banchi": "1丁目6-14",
-    "postal_code": "1018543",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カジチョウ",
-    "alternates": []
-  },
-  "1018526": {
+  "1018628": {
     "jis": "13101",
-    "kana": "カブ アクテイブ",
-    "name": "（株）　アクティブ",
+    "kana": "カガデンシ カブシキガイシヤ デンシジギヨウブ、ツウシンジギヨウブ、オ-トモ-テイブジギヨウブ",
+    "name": "加賀電子　株式会社　電子事業部、通信事業部、オートモーティブ事業部",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "2丁目16-11内神田渋谷ビル4F",
-    "postal_code": "1018526",
+    "neighborhood": "神田松永町",
+    "banchi": "20-8F",
+    "postal_code": "1018628",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
-  "1018449": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ アイシ-エスコンベンシヨンデザイン",
-    "name": "株式会社　ＩＣＳコンベンションデザイン",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "猿楽町",
-    "banchi": "1丁目5-18千代田ビル",
-    "postal_code": "1018449",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
+    "neighborhood_kana": "カンダマツナガチョウ",
     "alternates": []
   },
   "1018973": {
     "jis": "13101",
     "kana": "カブシキガイシヤ アクセル",
     "name": "株式会社　アクセル",
     "prefecture": "東京都",
@@ -97679,71 +97679,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ニシカンダ",
     "alternates": []
   },
-  "1018202": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ アスクレツプ",
-    "name": "株式会社　アスクレップ",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田練塀町",
-    "banchi": "3番地インテージ秋葉原ビル",
-    "postal_code": "1018202",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダネリベイチョウ",
-    "alternates": []
-  },
-  "1018615": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ アプラス",
-    "name": "株式会社　アプラス",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "3-12-8住友不動産秋葉原ビル",
-    "postal_code": "1018615",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
-  "1018469": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ アンビツト ニンドリヘンシユウブ",
-    "name": "株式会社　アンビット　ニンドリ編集部",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目6共同ビル(錦町3丁目)201",
-    "postal_code": "1018469",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018558": {
     "jis": "13101",
     "kana": "カブシキガイシヤ イワキ",
     "name": "株式会社　イワキ",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田須田町",
@@ -97793,52 +97736,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダネリベイチョウ",
     "alternates": []
   },
-  "1018467": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ エス・エス・コミユニケ-シヨンズ",
-    "name": "株式会社　エス・エス・コミュニケーションズ",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目18-3錦三ビル7階",
-    "postal_code": "1018467",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
-  "1018517": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ エルエスアイメデイエンス",
-    "name": "株式会社　ＬＳＩメディエンス",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1丁目13番4号",
-    "postal_code": "1018517",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
   "1018460": {
     "jis": "13101",
     "kana": "カブシキガイシヤ オ-ムシヤ",
     "name": "株式会社　オーム社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
@@ -97945,52 +97850,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "1018560": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ キンダイエイガシヤ",
-    "name": "株式会社　近代映画社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田小川町",
-    "banchi": "2-12-14晴花ビル4F",
-    "postal_code": "1018560",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダオガワマチ",
-    "alternates": []
-  },
-  "1018316": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ コウノイケグミ トウキヨウホンテン",
-    "name": "株式会社　鴻池組　東京本店",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目3-11",
-    "postal_code": "1018316",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018568": {
     "jis": "13101",
     "kana": "カブシキガイシヤ コクゴ",
     "name": "株式会社　コクゴ",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田富山町",
@@ -98002,33 +97869,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダトミヤマチョウ",
     "alternates": []
   },
-  "1018371": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ サンセイドウ",
-    "name": "株式会社　三省堂",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "三崎町",
-    "banchi": "2丁目22-14",
-    "postal_code": "1018371",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "1018410": {
     "jis": "13101",
     "kana": "カブシキガイシヤ シノテスト",
     "name": "株式会社　シノテスト",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -98173,33 +98021,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ニシカンダ",
     "alternates": []
   },
-  "1018588": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ シライシ",
-    "name": "株式会社　白石",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田岩本町",
-    "banchi": "1番地14",
-    "postal_code": "1018588",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダイワモトチョウ",
-    "alternates": []
-  },
   "1018475": {
     "jis": "13101",
     "kana": "カブシキガイシヤ シンコ-ミユ-ジツク・エンタテイメント",
     "name": "株式会社　シンコーミュージック・エンタテイメント",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田小川町",
@@ -98268,33 +98097,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダサクマガシ",
     "alternates": []
   },
-  "1018465": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ スミテツクス",
-    "name": "株式会社　スミテックス",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目24-1住友商事神保町ビル3F",
-    "postal_code": "1018465",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018418": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ゼンリン",
     "name": "株式会社　ゼンリン",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "西神田",
@@ -98325,33 +98135,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018638": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ソラスト",
-    "name": "株式会社　ソラスト",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田佐久間町",
-    "banchi": "3丁目2番",
-    "postal_code": "1018638",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダサクマチョウ",
-    "alternates": []
-  },
   "1018335": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ソンポカイカン",
     "name": "株式会社　損保會舘",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田淡路町",
@@ -98382,33 +98173,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018577": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ タジマ",
-    "name": "株式会社　タジマ",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "4-14-1秋葉原UDXビル21階",
-    "postal_code": "1018577",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018619": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ダイド-リミテツド",
     "name": "株式会社　ダイドーリミテッド",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "外神田",
@@ -98515,33 +98287,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ヒガシカンダ",
     "alternates": []
   },
-  "1018365": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ トオエンシヨボウ",
-    "name": "株式会社　桃園書房",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "三崎町",
-    "banchi": "2丁目11-7",
-    "postal_code": "1018365",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "1018548": {
     "jis": "13101",
     "kana": "カブシキガイシヤ トクリキホンテン",
     "name": "株式会社　徳力本店",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "鍛冶町",
@@ -98553,33 +98306,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カジチョウ",
     "alternates": []
   },
-  "1018419": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ニゲンシヤ",
-    "name": "株式会社　二玄社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田神保町",
-    "banchi": "2丁目2",
-    "postal_code": "1018419",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダジンボウチョウ",
-    "alternates": []
-  },
   "1018323": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ニホンケイザイコウコクシヤ",
     "name": "株式会社　日本経済広告社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田小川町",
@@ -98591,31 +98325,31 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダオガワマチ",
     "alternates": []
   },
-  "1018576": {
+  "1018359": {
     "jis": "13101",
-    "kana": "カブシキガイシヤ ニホンホウレイ",
-    "name": "株式会社　日本法令",
+    "kana": "カブシキガイシヤ ニホンボウエキホケン",
+    "name": "株式会社　日本貿易保険",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "岩本町",
-    "banchi": "2丁目1-7",
-    "postal_code": "1018576",
+    "neighborhood": "西神田",
+    "banchi": "3丁目8-1千代田ファーストビル",
+    "postal_code": "1018359",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "イワモトチョウ",
+    "neighborhood_kana": "ニシカンダ",
     "alternates": []
   },
   "1018561": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ニホンマンパワ-",
     "name": "株式会社　日本マンパワー",
     "prefecture": "東京都",
@@ -98648,33 +98382,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダヒガシマツシタチョウ",
     "alternates": []
   },
-  "1018454": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ バ-ン・コ-ポレ-シヨン",
-    "name": "株式会社　バーン・コーポレーション",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田小川町",
-    "banchi": "2丁目1番",
-    "postal_code": "1018454",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダオガワマチ",
-    "alternates": []
-  },
   "1018565": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ヒガシニツポンギンコウ カンダシテン",
     "name": "株式会社　東日本銀行　神田支店",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田富山町",
@@ -98781,33 +98496,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "1018381": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ベ-スボ-ル・マガジンシヤ",
-    "name": "株式会社　ベースボール・マガジン社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "三崎町",
-    "banchi": "3丁目10-10",
-    "postal_code": "1018381",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "1018423": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ホウソウシユツパンエ-ジエンシ-",
     "name": "株式会社　放送出版エージェンシー",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田神保町",
@@ -98857,33 +98553,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018305": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ メデイアワ-クス",
-    "name": "株式会社　メディアワークス",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "1丁目8",
-    "postal_code": "1018305",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018648": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ヤクジニツポウシヤ",
     "name": "株式会社　薬事日報社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田和泉町",
@@ -98895,33 +98572,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダイズミチョウ",
     "alternates": []
   },
-  "1018566": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ヤマヤコ-ポレ-シヨン",
-    "name": "株式会社　ヤマヤコーポレーション",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田富山町",
-    "banchi": "22",
-    "postal_code": "1018566",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダトミヤマチョウ",
-    "alternates": []
-  },
   "1018524": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ユニ・プランニング",
     "name": "株式会社　ユニ・プランニング",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "内神田",
@@ -98933,33 +98591,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ウチカンダ",
     "alternates": []
   },
-  "1018519": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ラ-ニングネツト",
-    "name": "株式会社　ラーニングネット",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "2丁目5-6",
-    "postal_code": "1018519",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
   "1018325": {
     "jis": "13101",
     "kana": "カンコウギヨウケンコウホケンクミアイ",
     "name": "管工業健康保険組合",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -98971,33 +98610,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018345": {
-    "jis": "13101",
-    "kana": "カンダシヤカイホケンジムシヨ",
-    "name": "神田社会保険事務所",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "猿楽町",
-    "banchi": "2丁目7-8住友水道橋ビル",
-    "postal_code": "1018345",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "1018464": {
     "jis": "13101",
     "kana": "カンダゼイムシヨ",
     "name": "神田税務署",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
@@ -99123,71 +98743,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018311": {
-    "jis": "13101",
-    "kana": "キヨ-リンセイヤクホ-ルデイングス カブシキガイシヤ",
-    "name": "キョーリン製薬ホールディングス　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "4-6御茶ノ水ソラシティ",
-    "postal_code": "1018311",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
-  "1018510": {
-    "jis": "13101",
-    "kana": "キヨウドウクレジツトサ-ビス カブシキガイシヤ",
-    "name": "協同クレジットサービス　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1丁目1-12",
-    "postal_code": "1018510",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
-  "1018317": {
-    "jis": "13101",
-    "kana": "キヨウドウリ-ス カブシキガイシヤ",
-    "name": "協同リース　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目9-17",
-    "postal_code": "1018317",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018437": {
     "jis": "13101",
     "kana": "キヨウリツジヨシダイガク",
     "name": "共立女子大学",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "一ツ橋",
@@ -99218,107 +98781,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018645": {
-    "jis": "13101",
-    "kana": "キリンビバレツジ カブシキガイシヤ",
-    "name": "キリンビバレッジ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田和泉町",
-    "banchi": "1",
-    "postal_code": "1018645",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダイズミチョウ",
-    "alternates": []
-  },
-  "1018641": {
-    "jis": "13101",
-    "kana": "キンキニホンツ-リスト カブシキガイシヤ",
-    "name": "近畿日本ツーリスト　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "東神田",
-    "banchi": "1-7-8東神田フコク生命ビル",
-    "postal_code": "1018641",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ヒガシカンダ",
-    "alternates": []
-  },
-  "1018356": {
-    "jis": "13101",
-    "kana": "ギンエイシヤ",
-    "name": "（株）　銀英社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "西神田",
-    "banchi": "2丁目8-9林リースビル5F",
-    "postal_code": "1018356",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ニシカンダ",
-    "alternates": []
-  },
-  "1018545": {
+  "1018311": {
     "jis": "13101",
-    "kana": "クメ・クオリテイ・プロダクツ カブシキガイシヤ",
-    "name": "くめ・クオリティ・プロダクツ　株式会社",
+    "kana": "キヨウリンセイヤク カブシキガイシヤ",
+    "name": "杏林製薬　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "神田東松下町",
-    "banchi": "14番地東信神田ビル9階",
-    "postal_code": "1018545",
+    "neighborhood": "神田駿河台",
+    "banchi": "4-6御茶ノ水ソラシティ",
+    "postal_code": "1018311",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダヒガシマツシタチョウ",
+    "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018427": {
+  "1018645": {
     "jis": "13101",
-    "kana": "クリタシユツパンハンバイ カブシキガイシヤ",
-    "name": "栗田出版販売　株式会社",
+    "kana": "キリンビバレツジ カブシキガイシヤ",
+    "name": "キリンビバレッジ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "神田神保町",
-    "banchi": "3-25住友神保町ビル8階",
-    "postal_code": "1018427",
+    "neighborhood": "神田和泉町",
+    "banchi": "1",
+    "postal_code": "1018645",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダジンボウチョウ",
+    "neighborhood_kana": "カンダイズミチョウ",
     "alternates": []
   },
   "1018977": {
     "jis": "13101",
     "kana": "グロ-リ- カブシキカイシヤ トウキヨウホンブ",
     "name": "グローリー　株式会社　東京本部",
     "prefecture": "東京都",
@@ -99370,50 +98876,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "1018559": {
+  "1018307": {
     "jis": "13101",
-    "kana": "サトウキンゾク カブシキガイシヤ",
-    "name": "佐藤金属　株式会社",
+    "kana": "コウエキシヤダンホウジン ニホンカガクカイ",
+    "name": "公益社団法人　日本化学会",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "神田須田町",
-    "banchi": "2丁目13",
-    "postal_code": "1018559",
+    "neighborhood": "神田駿河台",
+    "banchi": "1丁目5",
+    "postal_code": "1018307",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスダチョウ",
+    "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018583": {
+  "1018559": {
     "jis": "13101",
-    "kana": "サンデンホ-ルデイングス カブシキガイシヤ トウキヨウホンシヤ",
-    "name": "サンデンホールディングス　株式会社　東京本社",
+    "kana": "サトウキンゾク カブシキガイシヤ",
+    "name": "佐藤金属　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "1-18-13秋葉原ダイビル",
-    "postal_code": "1018583",
+    "neighborhood": "神田須田町",
+    "banchi": "2丁目13",
+    "postal_code": "1018559",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
+    "neighborhood_kana": "カンダスダチョウ",
     "alternates": []
   },
   "1018682": {
     "jis": "13101",
     "kana": "サンヨウボウエキ",
     "name": "三洋貿易　（株）",
     "prefecture": "東京都",
@@ -99427,33 +98933,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018333": {
-    "jis": "13101",
-    "kana": "ザイダンホウジン サンギヨウケイリキヨウカイ",
-    "name": "財団法人　産業経理協会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田淡路町",
-    "banchi": "1丁目15",
-    "postal_code": "1018333",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダアワジチョウ",
-    "alternates": []
-  },
   "1018346": {
     "jis": "13101",
     "kana": "ザイダンホウジン ニホンガンカガツカイ",
     "name": "財団法人　日本眼科学会",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "猿楽町",
@@ -99503,52 +98990,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018581": {
-    "jis": "13101",
-    "kana": "ザイダンホウジン ポスタルサ-ビスセンタ-",
-    "name": "（財）　ポスタルサービスセンター",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "鍛冶町",
-    "banchi": "1丁目8-3",
-    "postal_code": "1018581",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カジチョウ",
-    "alternates": []
-  },
-  "1018412": {
-    "jis": "13101",
-    "kana": "シヤカイフクシホウジン ゼンコクモウロウシヤキヨウカイ",
-    "name": "社会福祉法人　全国盲ろう者協会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田神保町",
-    "banchi": "2丁目5",
-    "postal_code": "1018412",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダジンボウチョウ",
-    "alternates": []
-  },
   "1018643": {
     "jis": "13101",
     "kana": "シヤカイフクシホウジン ミツイキネンビヨウイン",
     "name": "社会福祉法人　三井記念病院",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田和泉町",
@@ -99560,52 +99009,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダイズミチョウ",
     "alternates": []
   },
-  "1018459": {
-    "jis": "13101",
-    "kana": "シヤダンホウジン ガクシカイ",
-    "name": "社団法人　学士会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目28",
-    "postal_code": "1018459",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
-  "1018544": {
-    "jis": "13101",
-    "kana": "シヤダンホウジン サンギヨウカンキヨウカンリキヨウカイ",
-    "name": "社団法人　産業環境管理協会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "鍛冶町",
-    "banchi": "2丁目2-1",
-    "postal_code": "1018544",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カジチョウ",
-    "alternates": []
-  },
   "1018552": {
     "jis": "13101",
     "kana": "シヤダンホウジン ジヤパンケネルクラブ",
     "name": "社団法人　ジャパンケネルクラブ",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田須田町",
@@ -99617,33 +99028,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスダチョウ",
     "alternates": []
   },
-  "1018328": {
-    "jis": "13101",
-    "kana": "シヤダンホウジン トウキヨウトイシカイ",
-    "name": "社団法人　東京都医師会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目5",
-    "postal_code": "1018328",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018326": {
     "jis": "13101",
     "kana": "シヤダンホウジン トウキヨウトキヨウシヨクインゴジヨカイ サンラクビヨウイン",
     "name": "社団法人　東京都教職員互助会　三楽病院",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -99655,52 +99047,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018307": {
-    "jis": "13101",
-    "kana": "シヤダンホウジン ニホンカガクカイ",
-    "name": "社団法人　日本化学会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "1丁目5",
-    "postal_code": "1018307",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
-  "1018468": {
-    "jis": "13101",
-    "kana": "シヨ-ボンドケンセツ カブシキガイシヤ",
-    "name": "ショーボンド建設　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目18",
-    "postal_code": "1018468",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018521": {
     "jis": "13101",
     "kana": "シヨウワサンギヨウ カブシキガイシヤ",
     "name": "昭和産業　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "内神田",
@@ -99712,33 +99066,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ウチカンダ",
     "alternates": []
   },
-  "1018616": {
-    "jis": "13101",
-    "kana": "シンキ カブシキガイシヤ",
-    "name": "シンキ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "3丁目12-8住友不動産秋葉原ビル",
-    "postal_code": "1018616",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018451": {
     "jis": "13101",
     "kana": "シンセイカミパルプシヨウジ カブシキガイシヤ",
     "name": "新生紙パルプ商事　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
@@ -99750,69 +99085,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018603": {
+  "1018616": {
     "jis": "13101",
-    "kana": "シンセイフイナンシヤル カブシキガイシヤ",
-    "name": "新生フィナンシャル　株式会社",
+    "kana": "シンセイパ-ソナルロ-ン カブシキガイシヤ",
+    "name": "新生パーソナルローン　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "外神田",
-    "banchi": "3丁目12番8号住友不動産秋葉原ビル",
-    "postal_code": "1018603",
+    "banchi": "3丁目12-8住友不動産秋葉原ビル",
+    "postal_code": "1018616",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018447": {
-    "jis": "13101",
-    "kana": "ジ-アンドシ-",
-    "name": "（株）　ジーアンドシー",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "2丁目11",
-    "postal_code": "1018447",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
-  "1018518": {
+  "1018603": {
     "jis": "13101",
-    "kana": "ジエイエイゼンノウタマゴ カブシキガイシヤ",
-    "name": "ＪＡ全農たまご　株式会社",
+    "kana": "シンセイフイナンシヤル カブシキガイシヤ",
+    "name": "新生フィナンシャル　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1-1-12コープビル9F",
-    "postal_code": "1018518",
+    "neighborhood": "外神田",
+    "banchi": "3丁目12番8号住友不動産秋葉原ビル",
+    "postal_code": "1018603",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
+    "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
   "1018430": {
     "jis": "13101",
     "kana": "ジヨウホウ・システムケンキユウキコウ コクリツジヨウホウガクケンキユウジヨ",
     "name": "情報・システム研究機構　国立情報学研究所",
     "prefecture": "東京都",
@@ -99845,33 +99161,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "イワモトチョウ",
     "alternates": []
   },
-  "1018453": {
-    "jis": "13101",
-    "kana": "スミシヨウエレクトロニクス カブシキガイシヤ",
-    "name": "住商エレクトロニクス　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目11住友商事錦町ビル",
-    "postal_code": "1018453",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018425": {
     "jis": "13101",
     "kana": "センシユウダイガク",
     "name": "学校法人　専修大学",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田神保町",
@@ -99902,71 +99199,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ウチカンダ",
     "alternates": []
   },
-  "1018508": {
-    "jis": "13101",
-    "kana": "ゼンコクシンリンクミアイレンゴウカ",
-    "name": "全国森林組合連合会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1丁目1-12",
-    "postal_code": "1018508",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
-  "1018509": {
-    "jis": "13101",
-    "kana": "ゼンコクチホウギンコウキヨウカイ",
-    "name": "（社）　全国地方銀行協会",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "3丁目1-2",
-    "postal_code": "1018509",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
-  "1018501": {
-    "jis": "13101",
-    "kana": "ゼンコクノウギヨウキヨウドウクミアイレンゴウカイゼンノウトウキヨウシシヨ",
-    "name": "全国農業協同組合連合会全農東京支所",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1丁目1-12",
-    "postal_code": "1018501",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
   "1018502": {
     "jis": "13101",
     "kana": "ゼンノウブツリユウ カブシキガイシヤ",
     "name": "全農物流　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
@@ -100016,33 +99256,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018321": {
-    "jis": "13101",
-    "kana": "タカサゴネツガクコウギヨウ カブシキガイシヤ",
-    "name": "高砂熱学工業　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "4丁目2-5",
-    "postal_code": "1018321",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018575": {
     "jis": "13101",
     "kana": "タジマル-フイング カブシキガイシヤ",
     "name": "田島ルーフィング　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "岩本町",
@@ -100076,28 +99297,28 @@
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
   "1018383": {
     "jis": "13101",
     "kana": "タツク カブシキガイシヤ",
-    "name": "タック　株式会社",
+    "name": "ＴＡＣ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "三崎町",
+    "neighborhood": "神田三崎町",
     "banchi": "3丁目2-18",
     "postal_code": "1018383",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "カンダミサキチョウ",
     "alternates": []
   },
   "1018950": {
     "jis": "13101",
     "kana": "ダイケンコウギヨウ カブシキガイシヤ",
     "name": "大建工業　株式会社",
     "prefecture": "東京都",
@@ -100113,26 +99334,26 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
   "1018324": {
     "jis": "13101",
-    "kana": "チユウオウダイガク スルガダイキネンカン",
-    "name": "中央大学　駿河台記念館",
+    "kana": "チユウオウダイガク スルガダイキヤンパス",
+    "name": "中央大学　駿河台キャンパス",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
     "banchi": "3丁目11-5",
     "postal_code": "1018324",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
   "1018646": {
     "jis": "13101",
@@ -100206,33 +99427,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダツカサマチ",
     "alternates": []
   },
-  "1018533": {
-    "jis": "13101",
-    "kana": "トウキヨウト コガタコンピユ-タソフトウエア サンギヨウケンコウホケンクミアイ カンダシブ",
-    "name": "東京都　小型コンピュータソフトウェア　産業健康保険組合　神田支部",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田須田町",
-    "banchi": "2丁目7NKビル9F",
-    "postal_code": "1018533",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスダチョウ",
-    "alternates": []
-  },
   "1018527": {
     "jis": "13101",
     "kana": "トウキヨウトシヨクギヨウノウリヨクカイハツキヨウカイ",
     "name": "東京都職業能力開発協会",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "内神田",
@@ -100320,33 +99522,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ニシカンダ",
     "alternates": []
   },
-  "1018327": {
-    "jis": "13101",
-    "kana": "トウホウホ-ルデイングス カブシキガイシヤ",
-    "name": "東邦ホールディングス　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目5-23",
-    "postal_code": "1018327",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018630": {
     "jis": "13101",
     "kana": "トウヨク シンヨウクミアイ",
     "name": "東浴　信用組合",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "東神田",
@@ -100358,33 +99541,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ヒガシカンダ",
     "alternates": []
   },
-  "1018411": {
-    "jis": "13101",
-    "kana": "トシヨインサツ カブシキガイシヤ",
-    "name": "図書印刷　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田神保町",
-    "banchi": "2丁目17番地神田神保町ビル",
-    "postal_code": "1018411",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダジンボウチョウ",
-    "alternates": []
-  },
   "1018343": {
     "jis": "13101",
     "kana": "トヨタ・コニツク・プロ カブシキガイシヤ",
     "name": "トヨタ・コニック・プロ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田淡路町",
@@ -100396,33 +99560,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダアワジチョウ",
     "alternates": []
   },
-  "1018612": {
-    "jis": "13101",
-    "kana": "トランスネツト",
-    "name": "（株）　トランスネット",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "1丁目17-4JR東日本秋葉原ビル",
-    "postal_code": "1018612",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018617": {
     "jis": "13101",
     "kana": "ドウワコウギヨウ カブシキガイシヤ",
     "name": "同和鉱業　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "外神田",
@@ -100453,52 +99598,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018359": {
-    "jis": "13101",
-    "kana": "ドクリツギヨウセイホウジン ニホンボウエキホケン",
-    "name": "独立行政法人　日本貿易保険",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "西神田",
-    "banchi": "3丁目8-1千代田ファーストビル",
-    "postal_code": "1018359",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ニシカンダ",
-    "alternates": []
-  },
-  "1018662": {
-    "jis": "13101",
-    "kana": "ニシムラシヨテン",
-    "name": "（株）　西村書店",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "1丁目10(神田郵便局私書箱第42号)",
-    "postal_code": "1018662",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018688": {
     "jis": "13101",
     "kana": "ニチイガツカン",
     "name": "（株）　ニチイ学館",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -100510,52 +99617,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018483": {
-    "jis": "13101",
-    "kana": "ニチモ カブシキカイシヤ",
-    "name": "ニチモ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田美土代町",
-    "banchi": "7住友不動産神田ビル10F",
-    "postal_code": "1018483",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダミトシロチョウ",
-    "alternates": []
-  },
-  "1018609": {
-    "jis": "13101",
-    "kana": "ニチモコミユニテイ カブシキガイシヤ",
-    "name": "ニチモコミュニティ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "6丁目5-12偕楽ビル5・7・8F",
-    "postal_code": "1018609",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018329": {
     "jis": "13101",
     "kana": "ニツシンカサイカイジヨウホケン カブシキカイシヤ",
     "name": "日新火災海上保険　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -100795,71 +99864,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスダチョウ",
     "alternates": []
   },
-  "1018407": {
-    "jis": "13101",
-    "kana": "ニホンブンゲイシヤ",
-    "name": "（株）日本文芸社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田神保町",
-    "banchi": "1丁目7",
-    "postal_code": "1018407",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダジンボウチョウ",
-    "alternates": []
-  },
-  "1018506": {
-    "jis": "13101",
-    "kana": "ノウリンギヨギヨウシンヨウキキン",
-    "name": "農林漁業信用基金",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1丁目1-12コープビル",
-    "postal_code": "1018506",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
-  "1018507": {
-    "jis": "13101",
-    "kana": "ノウリンチユウオウキンコ",
-    "name": "農林中央金庫",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "内神田",
-    "banchi": "1丁目1-12コープビル",
-    "postal_code": "1018507",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ウチカンダ",
-    "alternates": []
-  },
   "1018711": {
     "jis": "13101",
     "kana": "ハクセンシヤ",
     "name": "（株）　白泉社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "西神田",
@@ -100909,33 +99921,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018302": {
-    "jis": "13101",
-    "kana": "ヒタチカセイシヨウジ カブシキガイシヤ",
-    "name": "日立化成商事　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2-5-1",
-    "postal_code": "1018302",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018971": {
     "jis": "13101",
     "kana": "ヒタチデンセン カブシキガイシヤ",
     "name": "日立電線　（株）",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "外神田",
@@ -100949,50 +99942,31 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
   "1018439": {
     "jis": "13101",
-    "kana": "ヒトツバシダイガク チヨダキヤンパス",
-    "name": "一橋大学　千代田キャンパス",
+    "kana": "ヒトツバシダイガク チヨダキヤンパスジムシツ",
+    "name": "一橋大学　千代田キャンパス事務室",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "一ツ橋",
     "banchi": "2丁目1-2",
     "postal_code": "1018439",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ヒトツバシ",
     "alternates": []
   },
-  "1018634": {
-    "jis": "13101",
-    "kana": "ビ-・アツプル カブシキガイシヤ",
-    "name": "ビー・アップル　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "東神田",
-    "banchi": "1丁目11-1エリア神田8F",
-    "postal_code": "1018634",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ヒガシカンダ",
-    "alternates": []
-  },
   "1018528": {
     "jis": "13101",
     "kana": "ピツプ カブシキガイシヤ",
     "name": "ピップ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "内神田",
@@ -101004,52 +99978,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ウチカンダ",
     "alternates": []
   },
-  "1018314": {
-    "jis": "13101",
-    "kana": "フジゼロツクスオフイスサプライ カブシキガイシヤ",
-    "name": "富士ゼロックスオフィスサプライ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目5-12駿河台プラザビル",
-    "postal_code": "1018314",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
-  "1018625": {
-    "jis": "13101",
-    "kana": "フジデンキリテイルシステムズ カブシキガイシヤ",
-    "name": "富士電機リテイルシステムズ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "6丁目15-12",
-    "postal_code": "1018625",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018542": {
     "jis": "13101",
     "kana": "フジパン カブシキガイシヤ カントウジギヨウブ",
     "name": "フジパン　（株）　関東事業部",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田富山町",
@@ -101061,33 +99997,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダトミヤマチョウ",
     "alternates": []
   },
-  "1018452": {
-    "jis": "13101",
-    "kana": "フジフイルムグラフイツクシステムズ カブシキガイシヤ",
-    "name": "富士フイルムグラフィックシステムズ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目13竹橋安田ビル1~4F",
-    "postal_code": "1018452",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018606": {
     "jis": "13101",
     "kana": "フマキラ- カブシキガイシヤ",
     "name": "フマキラー　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田美倉町",
@@ -101118,71 +100035,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018409": {
-    "jis": "13101",
-    "kana": "ヘイワシユツパン カブシキガイシヤ",
-    "name": "平和出版　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目3-13鈴木ビル4F",
-    "postal_code": "1018409",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
-  "1018331": {
-    "jis": "13101",
-    "kana": "マルベニガスエナジ- カブシキガイシヤ",
-    "name": "丸紅ガスエナジー　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目2",
-    "postal_code": "1018331",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
-  "1018363": {
-    "jis": "13101",
-    "kana": "マルベニテレコム (カブ)",
-    "name": "丸紅テレコム　（株）",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "西神田",
-    "banchi": "3丁目8-1千代田ファーストビル14F",
-    "postal_code": "1018363",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ニシカンダ",
-    "alternates": []
-  },
   "1018477": {
     "jis": "13101",
     "kana": "ミズノ カブシキガイシヤ",
     "name": "ミズノ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田小川町",
@@ -101213,33 +100073,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018443": {
-    "jis": "13101",
-    "kana": "ミズホジヨウホウソウケン カブシキガイシヤ",
-    "name": "みずほ情報総研　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "2丁目3",
-    "postal_code": "1018443",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018429": {
     "jis": "13101",
     "kana": "ミタニサンギヨウ カブシキガイシヤ",
     "name": "三谷産業　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田神保町",
@@ -101270,33 +100111,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダミトシロチョウ",
     "alternates": []
   },
-  "1018458": {
-    "jis": "13101",
-    "kana": "ミツイスミトモカイジヨウアイオイセイメイホケン カブシキガイシヤ",
-    "name": "三井住友海上あいおい生命保険　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3-11-1",
-    "postal_code": "1018458",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018011": {
     "jis": "13101",
     "kana": "ミツイスミトモカイジヨウカサイホケン カブシキカイシヤ",
     "name": "三井住友海上火災保険　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -101308,33 +100130,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
-  "1018607": {
-    "jis": "13101",
-    "kana": "ミツビシブング カブシキガイシヤ",
-    "name": "三菱文具　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "2丁目17-3アヤベビル4F",
-    "postal_code": "1018607",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018338": {
     "jis": "13101",
     "kana": "ミツビシマテリアル カブシキガイシヤ",
     "name": "三菱マテリアル　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "内神田",
@@ -101403,66 +100206,28 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスダチョウ",
     "alternates": []
   },
-  "1018578": {
-    "jis": "13101",
-    "kana": "モチダシヨウコウ",
-    "name": "持田商工　（株）",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "岩本町",
-    "banchi": "2丁目10-12",
-    "postal_code": "1018578",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "イワモトチョウ",
-    "alternates": []
-  },
   "1018626": {
     "jis": "13101",
-    "kana": "ヤマキ カブシキガイシヤ トウキヨウシテン",
-    "name": "ヤマキ　株式会社　東京支店",
+    "kana": "ヤマキ カブシキガイシヤ",
+    "name": "ヤマキ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "外神田",
     "banchi": "4-8-2",
     "postal_code": "1018626",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
-  "1018620": {
-    "jis": "13101",
-    "kana": "ヤマギワ カブシキガイシヤ",
-    "name": "ヤマギワ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "3丁目12-4",
-    "postal_code": "1018620",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
   "1018585": {
     "jis": "13101",
@@ -101505,21 +100270,21 @@
   "1018531": {
     "jis": "13101",
     "kana": "ユウゲンガイシヤ カガクヒヨウロンシヤ",
     "name": "有限会社　科学評論社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田司町",
-    "banchi": "2丁目10-8",
+    "banchi": "2丁目10-15",
     "postal_code": "1018531",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダツカサマチ",
     "alternates": []
   },
   "1018422": {
     "jis": "13101",
@@ -101555,71 +100320,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダアワジチョウ",
     "alternates": []
   },
-  "1018370": {
-    "jis": "13101",
-    "kana": "リケンビタミン カブシキガイシヤ",
-    "name": "理研ビタミン　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "三崎町",
-    "banchi": "2丁目9-18",
-    "postal_code": "1018370",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "1018446": {
     "jis": "13101",
-    "kana": "リヨウエイ",
-    "name": "菱栄　（株）",
+    "kana": "リヨウエイ カブシキカイシヤ",
+    "name": "菱栄　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
-    "banchi": "1丁目13宝栄錦町ビル8F",
+    "banchi": "1丁目13大手町宝栄ビル7階",
     "postal_code": "1018446",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018385": {
-    "jis": "13101",
-    "kana": "リンリケンキユウジヨ",
-    "name": "（社）　倫理研究所",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "三崎町",
-    "banchi": "3丁目1-10",
-    "postal_code": "1018385",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "1018315": {
     "jis": "13101",
     "kana": "ロウドウキンコカイカン",
     "name": "労働金庫会館",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -101669,52 +100396,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ヒトツバシ",
     "alternates": []
   },
-  "1018077": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ アスカシンシヤ",
-    "name": "株式会社　飛鳥新社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田神保町",
-    "banchi": "3丁目10神田第3アメレックスビル",
-    "postal_code": "1018077",
-    "old_code": "10177",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダジンボウチョウ",
-    "alternates": []
-  },
-  "1018655": {
-    "jis": "13101",
-    "kana": "アサヒカサイカイジヨウホケン カブシキガイシヤ",
-    "name": "朝日火災海上保険　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田美土代町",
-    "banchi": "7番地(神田郵便局私書箱第41号)",
-    "postal_code": "1018655",
-    "old_code": "10191",
-    "post_office": "神田",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダミトシロチョウ",
-    "alternates": []
-  },
   "1018654": {
     "jis": "13101",
     "kana": "イシフクキンゾクコウギヨウ カブシキガイシヤ",
     "name": "石福金属興業　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "内神田",
@@ -102923,14 +101612,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "キオイチョウ",
     "alternates": []
   },
+  "1028191": {
+    "jis": "13101",
+    "kana": "カブシキガイシヤ カテイガホウビジネスパ-トナ-ズ",
+    "name": "株式会社　家庭画報ビジネスパートナーズ",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "九段北",
+    "banchi": "4-2-29",
+    "postal_code": "1028191",
+    "old_code": "102  ",
+    "post_office": "麹町",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "クダンキタ",
+    "alternates": []
+  },
   "1028685": {
     "jis": "13101",
     "kana": "カブシキガイシヤ カドカワヘラルド・ピクチヤ-ズ",
     "name": "株式会社　角川ヘラルド・ピクチャーズ",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "紀尾井町",
@@ -103284,85 +101992,28 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンキタ",
     "alternates": []
   },
-  "1028194": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ セカイブンカライフケア",
-    "name": "株式会社　世界文化ライフケア",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "九段北",
-    "banchi": "4-2-29",
-    "postal_code": "1028194",
-    "old_code": "102  ",
-    "post_office": "麹町",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "クダンキタ",
-    "alternates": []
-  },
-  "1028191": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ セカイブンカリテイリング",
-    "name": "株式会社　世界文化リテイリング",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "九段北",
-    "banchi": "4-2-29",
-    "postal_code": "1028191",
-    "old_code": "102  ",
-    "post_office": "麹町",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "クダンキタ",
-    "alternates": []
-  },
   "1028192": {
     "jis": "13101",
-    "kana": "カブシキガイシヤ セカイブンカワンダ-クリエイト",
-    "name": "株式会社　世界文化ワンダークリエイト",
+    "kana": "カブシキガイシヤ セカイブンカワンダ-グル-プ",
+    "name": "株式会社　世界文化ワンダーグループ",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "九段北",
     "banchi": "4-2-29",
     "postal_code": "1028192",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "クダンキタ",
-    "alternates": []
-  },
-  "1028193": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ セカイブンカワンダ-ハンバイ",
-    "name": "株式会社　世界文化ワンダー販売",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "九段北",
-    "banchi": "4-2-29",
-    "postal_code": "1028193",
-    "old_code": "102  ",
-    "post_office": "麹町",
-    "type": "office",
-    "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンキタ",
     "alternates": []
   },
   "1028437": {
     "jis": "13101",
@@ -104179,26 +102830,26 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ヒラカワチョウ",
     "alternates": []
   },
   "1028417": {
     "jis": "13101",
-    "kana": "カブシキガイシヤ ヨ-クマ-ト",
-    "name": "株式会社　ヨークマート",
+    "kana": "カブシキガイシヤ ヨ-ク",
+    "name": "株式会社　ヨーク",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "二番町",
     "banchi": "8-8",
     "postal_code": "1028417",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ニバンチョウ",
     "alternates": []
   },
   "1028609": {
     "jis": "13101",
@@ -104234,14 +102885,52 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "キオイチョウ",
     "alternates": []
   },
+  "1028194": {
+    "jis": "13101",
+    "kana": "カブシキガイシヤ ワンダ-ウエルネス",
+    "name": "株式会社　ワンダーウェルネス",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "九段北",
+    "banchi": "4-2-29",
+    "postal_code": "1028194",
+    "old_code": "102  ",
+    "post_office": "麹町",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "クダンキタ",
+    "alternates": []
+  },
+  "1028193": {
+    "jis": "13101",
+    "kana": "カブシキガイシヤ ワンダ-ネツトワ-ク",
+    "name": "株式会社　ワンダーネットワーク",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "九段北",
+    "banchi": "4-2-29",
+    "postal_code": "1028193",
+    "old_code": "102  ",
+    "post_office": "麹町",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "クダンキタ",
+    "alternates": []
+  },
   "1028357": {
     "jis": "13101",
     "kana": "ガツコウホウジン オオツマガクイン オオツマジヨシダイガク オオツマジヨシダイガクタンキダイガクブ オオツマチユウガツコウ オオツマコウトウガツコウ",
     "name": "学校法人　大妻学院　大妻女子大学　大妻女子大学短期大学部　大妻中学校　大妻高等学校",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "三番町",
@@ -105368,15 +104057,15 @@
     "neighborhood": "平河町",
     "banchi": "一丁目五番九号厚生会館",
     "postal_code": "1028532",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ヒラカワチョウ",
     "alternates": []
   },
   "1028564": {
     "jis": "13101",
@@ -112260,25 +110949,25 @@
   },
   "1048171": {
     "jis": "13102",
     "kana": "カブシキガイシヤ デンツウマクロミルインサイト",
     "name": "株式会社　電通マクロミルインサイト",
     "prefecture": "東京都",
     "city": "中央区",
-    "neighborhood": "銀座",
-    "banchi": "7-4-17",
+    "neighborhood": "築地",
+    "banchi": "四丁目7番5号",
     "postal_code": "1048171",
     "old_code": "104  ",
-    "post_office": "銀座",
+    "post_office": "晴海",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
-    "neighborhood_kana": "ギンザ",
+    "neighborhood_kana": "ツキジ",
     "alternates": []
   },
   "1048161": {
     "jis": "13102",
     "kana": "カブシキガイシヤ デンツウメイテツコミユニケ-シヨンズ",
     "name": "株式会社　電通名鉄コミュニケーションズ",
     "prefecture": "東京都",
@@ -114135,33 +112824,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ツキジ",
     "alternates": []
   },
-  "1048470": {
-    "jis": "13102",
-    "kana": "トウキヨウシンヨウホシヨウキヨウカイ",
-    "name": "東京信用保証協会",
-    "prefecture": "東京都",
-    "city": "中央区",
-    "neighborhood": "八重洲",
-    "banchi": "2丁目6-17",
-    "postal_code": "1048470",
-    "old_code": "104  ",
-    "post_office": "晴海",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チュウオウク",
-    "neighborhood_kana": "ヤエス",
-    "alternates": []
-  },
   "1048133": {
     "jis": "13102",
     "kana": "トウキヨウデンリヨク カブシキガイシヤ ギンザシテン",
     "name": "東京電力　株式会社　銀座支店",
     "prefecture": "東京都",
     "city": "中央区",
     "neighborhood": "銀座",
@@ -118298,33 +116968,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "トラノモン",
     "alternates": []
   },
-  "1058617": {
-    "jis": "13103",
-    "kana": "ニツポンユウセイ カブシキガイシヤ シユクハクジギヨウブ",
-    "name": "日本郵政　株式会社　宿泊事業部",
-    "prefecture": "東京都",
-    "city": "港区",
-    "neighborhood": "新橋",
-    "banchi": "6-19-15",
-    "postal_code": "1058617",
-    "old_code": "105  ",
-    "post_office": "芝",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "ミナトク",
-    "neighborhood_kana": "シンバシ",
-    "alternates": []
-  },
   "1058788": {
     "jis": "13103",
     "kana": "ニツポンユウセイ カブシキガイシヤ シユトケンシセツセンタ-",
     "name": "日本郵政　株式会社　首都圏施設センター",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "虎ノ門",
@@ -118368,15 +117019,15 @@
     "neighborhood": "虎ノ門",
     "banchi": "4丁目3-13ヒューリック神谷町ビル5F",
     "postal_code": "1058467",
     "old_code": "105  ",
     "post_office": "芝",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "トラノモン",
     "alternates": []
   },
   "1058521": {
     "jis": "13103",
@@ -118869,14 +117520,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "シバウラ",
     "alternates": []
   },
+  "1058317": {
+    "jis": "13103",
+    "kana": "ミネベアミツミ カブシキガイシヤ",
+    "name": "ミネベアミツミ　株式会社",
+    "prefecture": "東京都",
+    "city": "港区",
+    "neighborhood": "東新橋",
+    "banchi": "1-9-3",
+    "postal_code": "1058317",
+    "old_code": "105  ",
+    "post_office": "銀座",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "ミナトク",
+    "neighborhood_kana": "ヒガシシンバシ",
+    "alternates": []
+  },
   "1058437": {
     "jis": "13103",
     "kana": "ミハマ カ)",
     "name": "美浜　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "虎ノ門",
@@ -122708,33 +121378,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "シバウラ",
     "alternates": []
   },
-  "1088338": {
-    "jis": "13103",
-    "kana": "エヌイ-シ-ネクサソリユ-シヨンズカブシキガイシヤ",
-    "name": "ＮＥＣネクサソリューションズ（株）",
-    "prefecture": "東京都",
-    "city": "港区",
-    "neighborhood": "三田",
-    "banchi": "1丁目4-28三田国際ビル",
-    "postal_code": "1088338",
-    "old_code": "108  ",
-    "post_office": "高輪",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "ミナトク",
-    "neighborhood_kana": "ミタ",
-    "alternates": []
-  },
   "1088515": {
     "jis": "13103",
     "kana": "エヌイ-シ-ネツツエスアイ カブシキガイシヤ",
     "name": "ＮＥＣネッツエスアイ　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "芝浦",
@@ -123962,14 +122613,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "コウナン",
     "alternates": []
   },
+  "1088316": {
+    "jis": "13103",
+    "kana": "キヨウセラ カブシキガイシヤ トウキヨウジギヨウシヨ",
+    "name": "京セラ　株式会社　東京事業所",
+    "prefecture": "東京都",
+    "city": "港区",
+    "neighborhood": "三田",
+    "banchi": "三丁目5番19号",
+    "postal_code": "1088316",
+    "old_code": "108  ",
+    "post_office": "高輪",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "ミナトク",
+    "neighborhood_kana": "ミタ",
+    "alternates": []
+  },
   "1088080": {
     "jis": "13103",
     "kana": "クラシエホ-ルデイングス カブシキガイシヤ",
     "name": "クラシエホールディングス　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "海岸",
@@ -125672,33 +124342,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "ミタ",
     "alternates": []
   },
-  "1088330": {
-    "jis": "13103",
-    "kana": "ミネベアミツミ カブシキガイシヤ",
-    "name": "ミネベアミツミ　株式会社",
-    "prefecture": "東京都",
-    "city": "港区",
-    "neighborhood": "三田",
-    "banchi": "3丁目9番6号",
-    "postal_code": "1088330",
-    "old_code": "108  ",
-    "post_office": "高輪",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "ミナトク",
-    "neighborhood_kana": "ミタ",
-    "alternates": []
-  },
   "1088636": {
     "jis": "13103",
     "kana": "メイジガクインダイガク",
     "name": "明治学院大学",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "白金台",
@@ -128006,15 +126657,15 @@
     "neighborhood": "西新宿",
     "banchi": "1-26-1",
     "postal_code": "1608313",
     "old_code": "160  ",
     "post_office": "新宿",
     "type": "office",
     "multiple": true,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
   "1608338": {
     "jis": "13104",
@@ -128025,15 +126676,15 @@
     "neighborhood": "西新宿",
     "banchi": "1-26-1",
     "postal_code": "1608338",
     "old_code": "160  ",
     "post_office": "新宿",
     "type": "office",
     "multiple": true,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
   "1638626": {
     "jis": "13104",
@@ -131408,34 +130059,34 @@
     "neighborhood": "西新宿",
     "banchi": "1-26-1",
     "postal_code": "1638620",
     "old_code": "163  ",
     "post_office": "新宿",
     "type": "office",
     "multiple": true,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
   "1630261": {
     "jis": "13104",
     "kana": "ヒカリビジネスフオ-ム カブシキガイシヤ",
     "name": "光ビジネスフォーム　株式会社",
     "prefecture": "東京都",
     "city": "新宿区",
     "neighborhood": "西新宿",
-    "banchi": "2丁目6番1号新宿住友ビル19階",
+    "banchi": "2丁目6番1号新宿住友ビル22階",
     "postal_code": "1630261",
     "old_code": "163  ",
     "post_office": "新宿",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
   "1638019": {
     "jis": "13104",
@@ -137666,14 +136317,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "タイトウク",
     "neighborhood_kana": "ヒガシウエノ",
     "alternates": []
   },
+  "1108736": {
+    "jis": "13106",
+    "kana": "シマヅダイアグノステイクス カブシキガイシヤ",
+    "name": "島津ダイアグノスティクス　株式会社",
+    "prefecture": "東京都",
+    "city": "台東区",
+    "neighborhood": "上野",
+    "banchi": "3丁目24-6上野フロンティアタワー20階",
+    "postal_code": "1108736",
+    "old_code": "110  ",
+    "post_office": "上野",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "タイトウク",
+    "neighborhood_kana": "ウエノ",
+    "alternates": []
+  },
   "1108567": {
     "jis": "13106",
     "kana": "シヤダンホウジン ニホンドウブツエンスイゾクカンキヨウカイ",
     "name": "社団法人　日本動物園水族館協会",
     "prefecture": "東京都",
     "city": "台東区",
     "neighborhood": "台東",
@@ -138141,33 +136811,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "タイトウク",
     "neighborhood_kana": "ウエノコウエン",
     "alternates": []
   },
-  "1108736": {
-    "jis": "13106",
-    "kana": "ニツスイセイヤク カブシキガイシヤ",
-    "name": "日水製薬　株式会社",
-    "prefecture": "東京都",
-    "city": "台東区",
-    "neighborhood": "上野",
-    "banchi": "3丁目23-9",
-    "postal_code": "1108736",
-    "old_code": "110  ",
-    "post_office": "上野",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "タイトウク",
-    "neighborhood_kana": "ウエノ",
-    "alternates": []
-  },
   "1108660": {
     "jis": "13106",
     "kana": "ニツポンネンキンキコウ ウエノネンキンジムシヨ",
     "name": "日本年金機構　上野年金事務所",
     "prefecture": "東京都",
     "city": "台東区",
     "neighborhood": "池之端",
@@ -140003,14 +138654,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "タイトウク",
     "neighborhood_kana": "コトブキ",
     "alternates": []
   },
+  "1118644": {
+    "jis": "13106",
+    "kana": "ライオン カブシキガイシヤ",
+    "name": "ライオン　株式会社",
+    "prefecture": "東京都",
+    "city": "台東区",
+    "neighborhood": "蔵前",
+    "banchi": "1-3-28",
+    "postal_code": "1118644",
+    "old_code": "111  ",
+    "post_office": "浅草",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "タイトウク",
+    "neighborhood_kana": "クラマエ",
+    "alternates": []
+  },
   "1118666": {
     "jis": "13106",
     "kana": "レデイマドラス カブシキガイシヤ",
     "name": "レデイマドラス　株式会社",
     "prefecture": "東京都",
     "city": "台東区",
     "neighborhood": "浅草",
@@ -142733,15 +141403,15 @@
     "neighborhood": "豊洲",
     "banchi": "5-6-36豊洲プライムスクエア11階",
     "postal_code": "1358165",
     "old_code": "135  ",
     "post_office": "晴海",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "トヨス",
     "alternates": []
   },
   "1358451": {
     "jis": "13108",
@@ -143556,14 +142226,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "アリアケ",
     "alternates": []
   },
+  "1358308": {
+    "jis": "13108",
+    "kana": "クラブツ-リズム カブシキカイシヤ",
+    "name": "クラブツーリズム　株式会社",
+    "prefecture": "東京都",
+    "city": "江東区",
+    "neighborhood": "枝川",
+    "banchi": "1丁目9番6号住友不動産豊洲ビル",
+    "postal_code": "1358308",
+    "old_code": "135  ",
+    "post_office": "深川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "コウトウク",
+    "neighborhood_kana": "エダガワ",
+    "alternates": []
+  },
   "1358310": {
     "jis": "13108",
     "kana": "コアサシヨウジ カブシキガイシヤ トウキヨウシテン",
     "name": "小浅商事　株式会社　東京支店",
     "prefecture": "東京都",
     "city": "江東区",
     "neighborhood": "森下",
@@ -144412,14 +143101,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "エイタイ",
     "alternates": []
   },
+  "1358797": {
+    "jis": "13108",
+    "kana": "ニツポンユウビン カブシキガイシヤ トウキヨウシシヤ",
+    "name": "日本郵便　株式会社　東京支社",
+    "prefecture": "東京都",
+    "city": "江東区",
+    "neighborhood": "東陽",
+    "banchi": "5-29-30ニッテイビル東陽",
+    "postal_code": "1358797",
+    "old_code": "135  ",
+    "post_office": "深川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "コウトウク",
+    "neighborhood_kana": "トウヨウ",
+    "alternates": []
+  },
   "1358511": {
     "jis": "13108",
     "kana": "ニホンアイ・ビ-・エム カブシキガイシヤ トヨスジギヨウシヨ",
     "name": "日本アイ・ビー・エム　株式会社　豊洲事業所",
     "prefecture": "東京都",
     "city": "江東区",
     "neighborhood": "豊洲",
@@ -146478,15 +145186,15 @@
     "neighborhood": "南大井",
     "banchi": "六丁目26-1大森ベルポートA館",
     "postal_code": "1408574",
     "old_code": "140  ",
     "post_office": "品川",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シナガワク",
     "neighborhood_kana": "ミナミオオイ",
     "alternates": []
   },
   "1408619": {
     "jis": "13109",
@@ -163610,14 +162318,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "トシマク",
     "neighborhood_kana": "ミナミオオツカ",
     "alternates": []
   },
+  "1708474": {
+    "jis": "13116",
+    "kana": "カブシキガイシヤ ニホンヒヨウロンシヤ",
+    "name": "株式会社　日本評論社",
+    "prefecture": "東京都",
+    "city": "豊島区",
+    "neighborhood": "南大塚",
+    "banchi": "3丁目12-4",
+    "postal_code": "1708474",
+    "old_code": "170  ",
+    "post_office": "豊島",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "トシマク",
+    "neighborhood_kana": "ミナミオオツカ",
+    "alternates": []
+  },
   "1708466": {
     "jis": "13116",
     "kana": "カブシキガイシヤ ヒタチプラントテクノロジ-",
     "name": "株式会社　日立プラントテクノロジー",
     "prefecture": "東京都",
     "city": "豊島区",
     "neighborhood": "東池袋",
@@ -178368,15 +177095,15 @@
     "neighborhood": "下小山田町",
     "banchi": "1491",
     "postal_code": "1940297",
     "old_code": "19402",
     "post_office": "町田西",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "マチダシ",
     "neighborhood_kana": "シモオヤマダマチ",
     "alternates": []
   },
   "1940294": {
     "jis": "13209",
@@ -184948,31 +183675,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ヨコハマシナカク",
     "neighborhood_kana": "キタナカドオリ",
     "alternates": []
   },
+  "2318750": {
+    "jis": "14104",
+    "kana": "ヨコハマナカゼイムシヨ",
+    "name": "横浜中税務署",
+    "prefecture": "神奈川県",
+    "city": "横浜市中区",
+    "neighborhood": "新港",
+    "banchi": "一丁目6番1号よこはま新港合同庁舎2階・3階",
+    "postal_code": "2318750",
+    "old_code": "231  ",
+    "post_office": "横浜港",
+    "type": "office",
+    "multiple": true,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシナカク",
+    "neighborhood_kana": "シンコウ",
+    "alternates": []
+  },
   "2318550": {
     "jis": "14104",
     "kana": "ヨコハマナカゼイムシヨ",
     "name": "横浜中税務署",
     "prefecture": "神奈川県",
     "city": "横浜市中区",
-    "neighborhood": "山下町",
-    "banchi": "37-9",
+    "neighborhood": "新港",
+    "banchi": "一丁目6番1号よこはま新港合同庁舎2階・3階",
     "postal_code": "2318550",
     "old_code": "231  ",
     "post_office": "横浜港",
     "type": "office",
-    "multiple": false,
-    "new": false,
+    "multiple": true,
+    "new": true,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ヨコハマシナカク",
-    "neighborhood_kana": "ヤマシタチョウ",
+    "neighborhood_kana": "シンコウ",
     "alternates": []
   },
   "2318562": {
     "jis": "14104",
     "kana": "ヨコハマフタバシヨウガツコウ",
     "name": "横浜雙葉小学校",
     "prefecture": "神奈川県",
@@ -195622,15 +194368,15 @@
     "neighborhood": "逗子",
     "banchi": "5丁目2-16",
     "postal_code": "2498686",
     "old_code": "249  ",
     "post_office": "逗子",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ズシシ",
     "neighborhood_kana": "ズシ",
     "alternates": []
   },
   "2380292": {
     "jis": "14210",
@@ -196844,33 +195590,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "エビナシ",
     "neighborhood_kana": "チュウオウ",
     "alternates": []
   },
-  "2430495": {
-    "jis": "14215",
-    "kana": "フジコカ・コ-ラボトリング カブシキガイシヤ",
-    "name": "富士コカ・コーラボトリング　株式会社",
-    "prefecture": "神奈川県",
-    "city": "海老名市",
-    "neighborhood": "上河内",
-    "banchi": "33",
-    "postal_code": "2430495",
-    "old_code": "24304",
-    "post_office": "綾瀬",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "カナガワケン",
-    "city_kana": "エビナシ",
-    "neighborhood_kana": "カミゴウチ",
-    "alternates": []
-  },
   "2430494": {
     "jis": "14215",
     "kana": "フジゼロツクス カブシキガイシヤ エビナジギヨウシヨ",
     "name": "富士ゼロックス　株式会社　海老名事業所",
     "prefecture": "神奈川県",
     "city": "海老名市",
     "neighborhood": "本郷",
@@ -205067,15 +203794,15 @@
     "neighborhood": "大字茨目",
     "banchi": "字二ツ池2071-1",
     "postal_code": "9451392",
     "old_code": "94513",
     "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451395": {
     "jis": "15205",
@@ -205086,15 +203813,15 @@
     "neighborhood": "大字安田",
     "banchi": "7586",
     "postal_code": "9451395",
     "old_code": "94513",
     "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451393": {
     "jis": "15205",
@@ -205105,15 +203832,15 @@
     "neighborhood": "大字軽井川",
     "banchi": "4730",
     "postal_code": "9451393",
     "old_code": "94513",
     "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451397": {
     "jis": "15205",
@@ -205124,15 +203851,15 @@
     "neighborhood": "大字安田",
     "banchi": "2510-2",
     "postal_code": "9451397",
     "old_code": "94513",
     "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451398": {
     "jis": "15205",
@@ -205143,15 +203870,15 @@
     "neighborhood": "大字安田",
     "banchi": "7546",
     "postal_code": "9451398",
     "old_code": "94513",
     "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451595": {
     "jis": "15205",
@@ -211017,15 +209744,15 @@
     "neighborhood": "上滝",
     "banchi": "567",
     "postal_code": "9301392",
     "old_code": "93013",
     "post_office": "上滝",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トヤマケン",
     "city_kana": "トヤマシ",
     "neighborhood_kana": "カミダキ",
     "alternates": []
   },
   "9302198": {
     "jis": "16201",
@@ -217316,14 +216043,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "ケンロクモトマチ",
     "alternates": []
   },
+  "9208535": {
+    "jis": "17201",
+    "kana": "カブシキガイシヤ ヨシカワ",
+    "name": "株式会社　ヨシカワ",
+    "prefecture": "石川県",
+    "city": "金沢市",
+    "neighborhood": "広岡",
+    "banchi": "三丁目3番77号JR金沢駅西第一NKビル6F",
+    "postal_code": "9208535",
+    "old_code": "920  ",
+    "post_office": "金沢中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "イシカワケン",
+    "city_kana": "カナザワシ",
+    "neighborhood_kana": "ヒロオカ",
+    "alternates": []
+  },
   "9208620": {
     "jis": "17201",
     "kana": "ガツコウホウジン イナオキガクエン カナザワセイリヨウダイガク",
     "name": "学校法人　稲置学園　金沢星稜大学",
     "prefecture": "石川県",
     "city": "金沢市",
     "neighborhood": "御所町",
@@ -218419,33 +217165,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "トイヤマチ",
     "alternates": []
   },
-  "9208535": {
-    "jis": "17201",
-    "kana": "ヨシカワ",
-    "name": "ヨシカワ",
-    "prefecture": "石川県",
-    "city": "金沢市",
-    "neighborhood": "北安江",
-    "banchi": "3丁目1-33",
-    "postal_code": "9208535",
-    "old_code": "920  ",
-    "post_office": "金沢中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "イシカワケン",
-    "city_kana": "カナザワシ",
-    "neighborhood_kana": "キタヤスエ",
-    "alternates": []
-  },
   "9208568": {
     "jis": "17201",
     "kana": "ヨシダセンデン カブシキガイシヤ",
     "name": "ヨシダ宣伝　株式会社",
     "prefecture": "石川県",
     "city": "金沢市",
     "neighborhood": "中央通町",
@@ -218793,15 +217520,15 @@
     "neighborhood": "もりの里",
     "banchi": "1丁目70",
     "postal_code": "9201184",
     "old_code": "92011",
     "post_office": "金沢中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "モリノサト",
     "alternates": []
   },
   "9201185": {
     "jis": "17201",
@@ -232323,15 +231050,15 @@
     "neighborhood": "小林",
     "banchi": "430番地1",
     "postal_code": "4000593",
     "old_code": "40005",
     "post_office": "青柳",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ヤマナシケン",
     "city_kana": "ミナミコマグンフジカワチョウ",
     "neighborhood_kana": "コバヤシ",
     "alternates": []
   },
   "4000592": {
     "jis": "19368",
@@ -232361,15 +231088,15 @@
     "neighborhood": "鰍沢",
     "banchi": "1760番地1富士川地方合同庁舎3階",
     "postal_code": "4000693",
     "old_code": "40006",
     "post_office": "鰍沢",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ヤマナシケン",
     "city_kana": "ミナミコマグンフジカワチョウ",
     "neighborhood_kana": "カジカザワ",
     "alternates": []
   },
   "4000695": {
     "jis": "19368",
@@ -237265,15 +235992,15 @@
     "neighborhood": "住吉",
     "banchi": "21番地5",
     "postal_code": "3868666",
     "old_code": "386  ",
     "post_office": "上田",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ナガノケン",
     "city_kana": "ウエダシ",
     "neighborhood_kana": "スミヨシ",
     "alternates": []
   },
   "3868705": {
     "jis": "20203",
@@ -237493,15 +236220,15 @@
     "neighborhood": "大屋",
     "banchi": "300番地",
     "postal_code": "3860192",
     "old_code": "38601",
     "post_office": "上田",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ナガノケン",
     "city_kana": "ウエダシ",
     "neighborhood_kana": "オオヤ",
     "alternates": []
   },
   "3868505": {
     "jis": "20203",
@@ -242347,26 +241074,26 @@
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "3990495": {
     "jis": "20382",
-    "kana": "オリンパス カブシキガイシヤ タツノジギヨウジヨウ",
-    "name": "オリンパス　株式会社　辰野事業場",
+    "kana": "カブシキガイシヤ エビデント ナガノジギヨウジヨウ",
+    "name": "株式会社　エビデント　長野事業場",
     "prefecture": "長野県",
     "city": "上伊那郡辰野町",
     "neighborhood": "大字伊那富",
-    "banchi": "6666",
+    "banchi": "6666番地",
     "postal_code": "3990495",
     "old_code": "39904",
     "post_office": "辰野",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "3990497": {
     "jis": "20382",
@@ -246888,14 +245615,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "オオガキシ",
     "neighborhood_kana": "ミナミノカワチョウ",
     "alternates": []
   },
+  "5038601": {
+    "jis": "21202",
+    "kana": "オオガキシヤクシヨ",
+    "name": "大垣市役所",
+    "prefecture": "岐阜県",
+    "city": "大垣市",
+    "neighborhood": "丸の内",
+    "banchi": "2丁目29",
+    "postal_code": "5038601",
+    "old_code": "503  ",
+    "post_office": "大垣",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ギフケン",
+    "city_kana": "オオガキシ",
+    "neighborhood_kana": "マルノウチ",
+    "alternates": []
+  },
   "5038565": {
     "jis": "21202",
     "kana": "オオガキシヨウコウカイギシヨ",
     "name": "大垣商工会議所",
     "prefecture": "岐阜県",
     "city": "大垣市",
     "neighborhood": "小野",
@@ -247243,15 +245989,15 @@
     "neighborhood": "寿町",
     "banchi": "1番地の1",
     "postal_code": "5038553",
     "old_code": "503  ",
     "post_office": "大垣",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "オオガキシ",
     "neighborhood_kana": "コトブキチョウ",
     "alternates": []
   },
   "5038567": {
     "jis": "21202",
@@ -247515,33 +246261,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "オオガキシ",
     "neighborhood_kana": "カンダチョウ",
     "alternates": []
   },
-  "5038601": {
-    "jis": "21202",
-    "kana": "オオガキシヤクシヨ",
-    "name": "大垣市役所",
-    "prefecture": "岐阜県",
-    "city": "大垣市",
-    "neighborhood": "丸の内",
-    "banchi": "2丁目29(大垣郵便局私書箱第37号)",
-    "postal_code": "5038601",
-    "old_code": "50391",
-    "post_office": "大垣",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ギフケン",
-    "city_kana": "オオガキシ",
-    "neighborhood_kana": "マルノウチ",
-    "alternates": []
-  },
   "5038603": {
     "jis": "21202",
     "kana": "タイヘイヨウコウギヨウ カブシキガイシヤ",
     "name": "太平洋工業　株式会社",
     "prefecture": "岐阜県",
     "city": "大垣市",
     "neighborhood": "久徳町",
@@ -270126,33 +268853,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシナカムラク",
     "neighborhood_kana": "メイエキ",
     "alternates": []
   },
-  "4508626": {
-    "jis": "23105",
-    "kana": "ナゴヤシ ササシマシゼイジムシヨ",
-    "name": "名古屋市　ささしま市税事務所",
-    "prefecture": "愛知県",
-    "city": "名古屋市中村区",
-    "neighborhood": "名駅南",
-    "banchi": "1丁目27番2号日本生命笹島ビル8階",
-    "postal_code": "4508626",
-    "old_code": "450  ",
-    "post_office": "名古屋西",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシナカムラク",
-    "neighborhood_kana": "メイエキミナミ",
-    "alternates": []
-  },
   "4506660": {
     "jis": "23105",
     "kana": "ナゴヤジエイア-ルゲ-トタワ-ホテル",
     "name": "名古屋ＪＲゲートタワーホテル",
     "prefecture": "愛知県",
     "city": "名古屋市中村区",
     "neighborhood": "名駅",
@@ -271058,14 +269766,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシナカムラク",
     "neighborhood_kana": "ミチシタチョウ",
     "alternates": []
   },
+  "4538686": {
+    "jis": "23105",
+    "kana": "ナゴヤナカムラゼイムシヨ",
+    "name": "名古屋中村税務署",
+    "prefecture": "愛知県",
+    "city": "名古屋市中村区",
+    "neighborhood": "太閤",
+    "banchi": "3丁目4-1",
+    "postal_code": "4538686",
+    "old_code": "453  ",
+    "post_office": "中村",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "ナゴヤシナカムラク",
+    "neighborhood_kana": "タイコウ",
+    "alternates": []
+  },
   "4538580": {
     "jis": "23105",
     "kana": "メイジデンキコウギヨウ カブシキガイシヤ",
     "name": "明治電機工業　株式会社",
     "prefecture": "愛知県",
     "city": "名古屋市中村区",
     "neighborhood": "亀島",
@@ -271134,33 +269861,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシナカムラク",
     "neighborhood_kana": "タイコウトオリ",
     "alternates": []
   },
-  "4538686": {
-    "jis": "23105",
-    "kana": "ナゴヤナカムラゼイムシヨ",
-    "name": "名古屋中村税務署",
-    "prefecture": "愛知県",
-    "city": "名古屋市中村区",
-    "neighborhood": "太閤",
-    "banchi": "3丁目4-1(中村郵便局私書箱第20号)",
-    "postal_code": "4538686",
-    "old_code": "45391",
-    "post_office": "中村",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシナカムラク",
-    "neighborhood_kana": "タイコウ",
-    "alternates": []
-  },
   "4608672": {
     "jis": "23106",
     "kana": "アイオイソンガイホケン カブシキガイシヤ",
     "name": "あいおい損害保険　株式会社",
     "prefecture": "愛知県",
     "city": "名古屋市中区",
     "neighborhood": "千代田",
@@ -274537,14 +273245,52 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシショウワク",
     "neighborhood_kana": "ミョウケンチョウ",
     "alternates": []
   },
+  "4668688": {
+    "jis": "23107",
+    "kana": "アイチトヨタイ-スト カブシキガイシヤ",
+    "name": "愛知トヨタＥＡＳＴ　株式会社",
+    "prefecture": "愛知県",
+    "city": "名古屋市昭和区",
+    "neighborhood": "高辻町",
+    "banchi": "6番8号",
+    "postal_code": "4668688",
+    "old_code": "466  ",
+    "post_office": "昭和",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "ナゴヤシショウワク",
+    "neighborhood_kana": "タカツジチョウ",
+    "alternates": []
+  },
+  "4668701": {
+    "jis": "23107",
+    "kana": "アイチトヨタウエスト カブシキガイシヤ",
+    "name": "愛知トヨタＷＥＳＴ　株式会社",
+    "prefecture": "愛知県",
+    "city": "名古屋市昭和区",
+    "neighborhood": "高辻町",
+    "banchi": "6番8号",
+    "postal_code": "4668701",
+    "old_code": "466  ",
+    "post_office": "昭和",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "ナゴヤシショウワク",
+    "neighborhood_kana": "タカツジチョウ",
+    "alternates": []
+  },
   "4668554": {
     "jis": "23107",
     "kana": "アジノモト カブシキガイシヤ ナゴヤシシヤ",
     "name": "味の素　株式会社　名古屋支社",
     "prefecture": "愛知県",
     "city": "名古屋市昭和区",
     "neighborhood": "阿由知通",
@@ -274936,33 +273682,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシショウワク",
     "neighborhood_kana": "タカツジチョウ",
     "alternates": []
   },
-  "4668508": {
-    "jis": "23107",
-    "kana": "トヨタカロ-ラアイホウ カブシキガイシヤ",
-    "name": "トヨタカローラ愛豊　株式会社",
-    "prefecture": "愛知県",
-    "city": "名古屋市昭和区",
-    "neighborhood": "高辻町",
-    "banchi": "6番8号",
-    "postal_code": "4668508",
-    "old_code": "466  ",
-    "post_office": "昭和",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシショウワク",
-    "neighborhood_kana": "タカツジチョウ",
-    "alternates": []
-  },
   "4668555": {
     "jis": "23107",
     "kana": "ナゴヤコウギヨウダイガク",
     "name": "名古屋工業大学",
     "prefecture": "愛知県",
     "city": "名古屋市昭和区",
     "neighborhood": "御器所町",
@@ -275107,52 +273834,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシショウワク",
     "neighborhood_kana": "シラカネ",
     "alternates": []
   },
-  "4668610": {
-    "jis": "23107",
-    "kana": "ネツツトヨタアイチ カブシキガイシヤ",
-    "name": "ネッツトヨタ愛知　株式会社",
-    "prefecture": "愛知県",
-    "city": "名古屋市昭和区",
-    "neighborhood": "高辻町",
-    "banchi": "6番8号",
-    "postal_code": "4668610",
-    "old_code": "466  ",
-    "post_office": "昭和",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシショウワク",
-    "neighborhood_kana": "タカツジチョウ",
-    "alternates": []
-  },
-  "4668688": {
-    "jis": "23107",
-    "kana": "ネツツトヨタトウカイ カブシキガイシヤ",
-    "name": "ネッツトヨタ東海　株式会社",
-    "prefecture": "愛知県",
-    "city": "名古屋市昭和区",
-    "neighborhood": "高辻町",
-    "banchi": "6番8号",
-    "postal_code": "4668688",
-    "old_code": "466  ",
-    "post_office": "昭和",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシショウワク",
-    "neighborhood_kana": "タカツジチョウ",
-    "alternates": []
-  },
   "4668588": {
     "jis": "23107",
     "kana": "パイロツトインキ カブシキガイシヤ",
     "name": "パイロットインキ　株式会社",
     "prefecture": "愛知県",
     "city": "名古屋市昭和区",
     "neighborhood": "緑町",
@@ -275221,33 +273910,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシショウワク",
     "neighborhood_kana": "タカミネチョウ",
     "alternates": []
   },
-  "4668701": {
-    "jis": "23107",
-    "kana": "アイチトヨタジドウシヤ カブシキガイシヤ",
-    "name": "愛知トヨタ自動車　株式会社",
-    "prefecture": "愛知県",
-    "city": "名古屋市昭和区",
-    "neighborhood": "高辻町",
-    "banchi": "6-8(昭和郵便局私書箱第39号)",
-    "postal_code": "4668701",
-    "old_code": "46691",
-    "post_office": "昭和",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシショウワク",
-    "neighborhood_kana": "タカツジチョウ",
-    "alternates": []
-  },
   "4668707": {
     "jis": "23107",
     "kana": "チユウキヨウテレビホウソウ カブシキガイシヤ",
     "name": "中京テレビ放送　株式会社",
     "prefecture": "愛知県",
     "city": "名古屋市昭和区",
     "neighborhood": "高峯町",
@@ -289625,14 +288295,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "トコナメシ",
     "neighborhood_kana": "オオタニ",
     "alternates": []
   },
+  "4798587": {
+    "jis": "23216",
+    "kana": "カブシキガイシヤ リクシル トコナメヒガシコウジヨウ",
+    "name": "株式会社　ＬＩＸＩＬ　常滑東工場",
+    "prefecture": "愛知県",
+    "city": "常滑市",
+    "neighborhood": "奥栄町",
+    "banchi": "1丁目47番地",
+    "postal_code": "4798587",
+    "old_code": "479  ",
+    "post_office": "常滑",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "トコナメシ",
+    "neighborhood_kana": "オクエイチョウ",
+    "alternates": []
+  },
   "4798585": {
     "jis": "23216",
     "kana": "カブシキガイシヤ リクシル トコナメホンシヤ",
     "name": "株式会社　ＬＩＸＩＬ　常滑本社",
     "prefecture": "愛知県",
     "city": "常滑市",
     "neighborhood": "鯉江本町",
@@ -289897,25 +288586,25 @@
   },
   "4798610": {
     "jis": "23216",
     "kana": "トコナメシヤクシヨ",
     "name": "常滑市役所",
     "prefecture": "愛知県",
     "city": "常滑市",
-    "neighborhood": "新開町",
-    "banchi": "4丁目1(常滑郵便局私書箱第1号)",
+    "neighborhood": "飛香台",
+    "banchi": "3丁目3番地の5(常滑郵便局私書箱第1号)",
     "postal_code": "4798610",
     "old_code": "479  ",
     "post_office": "常滑",
     "type": "box",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "アイチケン",
     "city_kana": "トコナメシ",
-    "neighborhood_kana": "シンカイチョウ",
+    "neighborhood_kana": "アスカダイ",
     "alternates": []
   },
   "4798668": {
     "jis": "23216",
     "kana": "トコナメシヨウコウカイギシヨ",
     "name": "常滑商工会議所",
     "prefecture": "愛知県",
@@ -291424,15 +290113,15 @@
     "neighborhood": "長篠",
     "banchi": "字仲野16番地11",
     "postal_code": "4411692",
     "old_code": "44116",
     "post_office": "長篠",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "シンシロシ",
     "neighborhood_kana": "ナガシノ",
     "alternates": []
   },
   "4768666": {
     "jis": "23222",
@@ -291962,14 +290651,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "オオブシ",
     "neighborhood_kana": "キョウエイチョウ",
     "alternates": []
   },
+  "4748668": {
+    "jis": "23223",
+    "kana": "カブシキガイシヤ トヨタジドウシヨツキ オオブコウジヨウ",
+    "name": "株式会社　豊田自動織機　大府工場",
+    "prefecture": "愛知県",
+    "city": "大府市",
+    "neighborhood": "江端町",
+    "banchi": "一丁目一番地",
+    "postal_code": "4748668",
+    "old_code": "474  ",
+    "post_office": "大府",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "オオブシ",
+    "neighborhood_kana": "エバタチョウ",
+    "alternates": []
+  },
   "4748601": {
     "jis": "23223",
     "kana": "カブシキガイシヤ トヨタジドウシヨツキセイサクシヨ キヨウワコウジヨウ",
     "name": "株式会社　豊田自動織機製作所　共和工場",
     "prefecture": "愛知県",
     "city": "大府市",
     "neighborhood": "共和町",
@@ -294256,15 +292964,15 @@
     "neighborhood": "根浦町",
     "banchi": "七丁目2番地1",
     "postal_code": "4700297",
     "old_code": "47002",
     "post_office": "三好",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ミヨシシ",
     "neighborhood_kana": "ネウラマチ",
     "alternates": []
   },
   "4700294": {
     "jis": "23236",
@@ -311817,15 +310525,15 @@
     "neighborhood": "東小橋",
     "banchi": "2丁目9番3号",
     "postal_code": "5378911",
     "old_code": "537  ",
     "post_office": "東成",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシヒガシナリク",
     "neighborhood_kana": "ヒガシオバセ",
     "alternates": []
   },
   "5378501": {
     "jis": "27115",
@@ -317865,15 +316573,15 @@
     "neighborhood": "北浜",
     "banchi": "3丁目5番29号-13階",
     "postal_code": "5418589",
     "old_code": "541  ",
     "post_office": "大阪東",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "キタハマ",
     "alternates": []
   },
   "5418526": {
     "jis": "27128",
@@ -317922,15 +316630,15 @@
     "neighborhood": "瓦町",
     "banchi": "3-6-5",
     "postal_code": "5418528",
     "old_code": "541  ",
     "post_office": "大阪東",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "カワラマチ",
     "alternates": []
   },
   "5416666": {
     "jis": "27128",
@@ -318093,15 +316801,15 @@
     "neighborhood": "今橋",
     "banchi": "2丁目4番10号淀屋橋北浜センタービル2階",
     "postal_code": "5418575",
     "old_code": "541  ",
     "post_office": "大阪東",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "イマバシ",
     "alternates": []
   },
   "5418517": {
     "jis": "27128",
@@ -323300,15 +322008,15 @@
     "neighborhood": "郡川",
     "banchi": "一丁目557GLP八尾Ⅰ",
     "postal_code": "5818502",
     "old_code": "581  ",
     "post_office": "八尾",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "ヤオシ",
     "neighborhood_kana": "コオリガワ",
     "alternates": []
   },
   "5818505": {
     "jis": "27212",
@@ -343079,15 +341787,15 @@
     "neighborhood": "灘町",
     "banchi": "101-6(松江中央郵便局私書箱第7号)",
     "postal_code": "6908601",
     "old_code": "690  ",
     "post_office": "松江中央",
     "type": "box",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "マツエシ",
     "neighborhood_kana": "ナダマチ",
     "alternates": []
   },
   "6908550": {
     "jis": "32201",
@@ -343446,33 +342154,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "マツエシ",
     "neighborhood_kana": "キタタマチ",
     "alternates": []
   },
-  "6908503": {
-    "jis": "32201",
-    "kana": "シマネケン シンヨウホシヨウキヨウカイ",
-    "name": "島根県　信用保証協会",
-    "prefecture": "島根県",
-    "city": "松江市",
-    "neighborhood": "殿町",
-    "banchi": "105",
-    "postal_code": "6908503",
-    "old_code": "690  ",
-    "post_office": "松江中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "シマネケン",
-    "city_kana": "マツエシ",
-    "neighborhood_kana": "トノマチ",
-    "alternates": []
-  },
   "6908551": {
     "jis": "32201",
     "kana": "シマネケン トウブケンミンセンタ-",
     "name": "島根県　東部県民センター",
     "prefecture": "島根県",
     "city": "松江市",
     "neighborhood": "東津田町",
@@ -343503,14 +342192,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "マツエシ",
     "neighborhood_kana": "ソデシチョウ",
     "alternates": []
   },
+  "6908503": {
+    "jis": "32201",
+    "kana": "シマネケンシンヨウホシヨウキヨウカイ",
+    "name": "島根県信用保証協会",
+    "prefecture": "島根県",
+    "city": "松江市",
+    "neighborhood": "灘町",
+    "banchi": "1番地7",
+    "postal_code": "6908503",
+    "old_code": "690  ",
+    "post_office": "松江中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "シマネケン",
+    "city_kana": "マツエシ",
+    "neighborhood_kana": "ナダマチ",
+    "alternates": []
+  },
   "6908501": {
     "jis": "32201",
     "kana": "シマネケンチヨウ",
     "name": "島根県庁",
     "prefecture": "島根県",
     "city": "松江市",
     "neighborhood": "殿町",
@@ -345017,15 +343725,15 @@
     "neighborhood": "駅前町",
     "banchi": "17-1益田駅前ビルEAGA3F",
     "postal_code": "6988506",
     "old_code": "698  ",
     "post_office": "益田",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "マスダシ",
     "neighborhood_kana": "エキマエチョウ",
     "alternates": []
   },
   "6988651": {
     "jis": "32204",
@@ -350736,15 +349444,15 @@
     "neighborhood": "玉島八島",
     "banchi": "1541番1",
     "postal_code": "7138588",
     "old_code": "713  ",
     "post_office": "玉島",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オカヤマケン",
     "city_kana": "クラシキシ",
     "neighborhood_kana": "タマシマヤシマ",
     "alternates": []
   },
   "7138501": {
     "jis": "33202",
@@ -352307,21 +351015,21 @@
   "7014293": {
     "jis": "33212",
     "kana": "セトウチシヤクシヨ オサフネシシヨ",
     "name": "瀬戸内市役所　長船支所",
     "prefecture": "岡山県",
     "city": "瀬戸内市",
     "neighborhood": "長船町土師",
-    "banchi": "291",
+    "banchi": "288番地1",
     "postal_code": "7014293",
     "old_code": "70142",
     "post_office": "邑久",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "オカヤマケン",
     "city_kana": "セトウチシ",
     "neighborhood_kana": "オサフネチョウハジ",
     "alternates": []
   },
   "7014398": {
     "jis": "33212",
@@ -392319,15 +391027,15 @@
     "neighborhood": "長浜",
     "banchi": "1丁目1-1",
     "postal_code": "8108571",
     "old_code": "810  ",
     "post_office": "福岡中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシチュウオウク",
     "neighborhood_kana": "ナガハマ",
     "alternates": [
       {
         "jis": "40133",
         "kana": "ケ-ビ-シ-グル-プホ-ルデイングス カブシキガイシヤ",
@@ -392337,15 +391045,15 @@
         "neighborhood": "長浜",
         "banchi": "1丁目1-1",
         "postal_code": "8108571",
         "old_code": "810  ",
         "post_office": "福岡中央",
         "type": "office",
         "multiple": false,
-        "new": true,
+        "new": false,
         "prefecture_kana": "フクオカケン",
         "city_kana": "フクオカシチュウオウク",
         "neighborhood_kana": "ナガハマ",
         "alternates": []
       }
     ]
   },
@@ -399009,15 +397717,15 @@
     "neighborhood": "彩り台",
     "banchi": "1番1号",
     "postal_code": "8112498",
     "old_code": "81124",
     "post_office": "粕屋南",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "カスヤグンササグリマチ",
     "neighborhood_kana": "イロドリダイ",
     "alternates": []
   },
   "8112492": {
     "jis": "40342",
@@ -406666,15 +405374,15 @@
     "neighborhood": "世安",
     "banchi": "1丁目5番1号",
     "postal_code": "8608506",
     "old_code": "860  ",
     "post_office": "熊本中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
     "neighborhood_kana": "ヨヤス",
     "alternates": []
   },
   "8608539": {
     "jis": "43101",
```

### Comparing `posuto-2023.5.0/posuto/postaldata.db` & `posuto-2023.6.0/posuto/postaldata.db`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -13691,15 +13691,15 @@
 INSERT INTO postal_data VALUES('9872262','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872262", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテカラタケバヤシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館唐竹林", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館唐竹林');
 INSERT INTO postal_data VALUES('9872228','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872228", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテカワゾエ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館川添", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館川添');
 INSERT INTO postal_data VALUES('9872212','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872212", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテキド", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館木戸", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館木戸');
 INSERT INTO postal_data VALUES('9872261','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872261", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテキュウデン", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館久伝", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館久伝');
 INSERT INTO postal_data VALUES('9872204','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872204", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテクロセ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館黒瀬", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館黒瀬');
 INSERT INTO postal_data VALUES('9872211','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872211", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテゲンコウ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館源光", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館源光');
 INSERT INTO postal_data VALUES('9872273','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872273", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコエダテ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館左足", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館左足');
-INSERT INTO postal_data VALUES('9872265','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチニシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵西", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチヒガシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵東", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサカイダ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館境田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサノハラ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館左野原", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館小淵西');
+INSERT INTO postal_data VALUES('9872265','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチニシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵西", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチヒガシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵東", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサカイダ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館境田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサノハラ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館左野原", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館小淵西');
 INSERT INTO postal_data VALUES('9872232','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872232", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサワイリ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館沢入", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館沢入');
 INSERT INTO postal_data VALUES('9872247','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872247", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシモタカモリ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館下高森", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館下高森');
 INSERT INTO postal_data VALUES('9872221','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872221", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシモマチイ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館下待井", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館下待井');
 INSERT INTO postal_data VALUES('9872203','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872203", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシモミヤノ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館下宮野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館下宮野');
 INSERT INTO postal_data VALUES('9872202','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872202", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテジョウノ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館城生野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館城生野');
 INSERT INTO postal_data VALUES('9872263','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872263", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシンデン", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館新田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872263", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテヤクシガオカ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館薬師ケ丘", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館新田');
 INSERT INTO postal_data VALUES('9872274','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872274", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシンナリタニシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館新成田西", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872274", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテナリタ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館成田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館新成田西');
@@ -14348,15 +14348,15 @@
 INSERT INTO postal_data VALUES('9810136','{"jisx0402": "04406", "old_code": "98101", "postal_code": "9810136", "prefecture_kana": "ミヤギケン", "city_kana": "ミヤギグンリフチョウ", "neighborhood_kana": "ミナノオカ", "prefecture": "宮城県", "city": "宮城郡利府町", "neighborhood": "皆の丘", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','宮城郡利府町','皆の丘');
 INSERT INTO postal_data VALUES('9810103','{"jisx0402": "04406", "old_code": "98101", "postal_code": "9810103", "prefecture_kana": "ミヤギケン", "city_kana": "ミヤギグンリフチョウ", "neighborhood_kana": "モリゴウ", "prefecture": "宮城県", "city": "宮城郡利府町", "neighborhood": "森郷", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','宮城郡利府町','森郷');
 INSERT INTO postal_data VALUES('9810112','{"jisx0402": "04406", "old_code": "98101", "postal_code": "9810112", "prefecture_kana": "ミヤギケン", "city_kana": "ミヤギグンリフチョウ", "neighborhood_kana": "リフ", "prefecture": "宮城県", "city": "宮城郡利府町", "neighborhood": "利府", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','宮城郡利府町','利府');
 INSERT INTO postal_data VALUES('9813600','{"jisx0402": "04421", "old_code": "98136", "postal_code": "9813600", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04424", "old_code": "98136", "postal_code": "9813600", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンオオヒラムラ", "neighborhood_kana": "", "prefecture": "宮城県", "city": "黒川郡大衡村", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}], "note": "以下に掲載がない場合"}','宮城県','黒川郡大和町','');
 INSERT INTO postal_data VALUES('9813404','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813404", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイアイカワ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合相川", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合相川');
 INSERT INTO postal_data VALUES('9813401','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813401", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイサンガウチ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合三ケ内", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合三ケ内');
 INSERT INTO postal_data VALUES('9813406','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813406", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイヒルブクロ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合蒜袋", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合蒜袋');
-INSERT INTO postal_data VALUES('9813403','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813403", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイヒワダ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合桧和田", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合桧和田');
+INSERT INTO postal_data VALUES('9813403','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813403", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイヒワダ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合桧和田", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合桧和田');
 INSERT INTO postal_data VALUES('9813402','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813402", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイホウオンジ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合報恩寺", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合報恩寺');
 INSERT INTO postal_data VALUES('9813405','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813405", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイマイノ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合舞野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合舞野');
 INSERT INTO postal_data VALUES('9813407','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813407", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイマツサカ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合松坂", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合松坂');
 INSERT INTO postal_data VALUES('9813623','{"jisx0402": "04421", "old_code": "98136", "postal_code": "9813623", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オノ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "小野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','小野');
 INSERT INTO postal_data VALUES('9813271','{"jisx0402": "04421", "old_code": "981  ", "postal_code": "9813271", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "ガクエン", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "学苑", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','学苑');
 INSERT INTO postal_data VALUES('9813414','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813414", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "ツルスオオタ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "鶴巣太田", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','鶴巣太田');
 INSERT INTO postal_data VALUES('9813411','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813411", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "ツルスオオダイラ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "鶴巣大平", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','鶴巣大平');
@@ -18973,14 +18973,15 @@
 INSERT INTO postal_data VALUES('9608124','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608124", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "サンキョウエ", "prefecture": "福島県", "city": "福島市", "neighborhood": "山居上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','山居上');
 INSERT INTO postal_data VALUES('9608155','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608155", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シミズマチ", "prefecture": "福島県", "city": "福島市", "neighborhood": "清水町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','清水町');
 INSERT INTO postal_data VALUES('9608122','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608122", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シミズヤマ", "prefecture": "福島県", "city": "福島市", "neighborhood": "清水山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','清水山');
 INSERT INTO postal_data VALUES('9608215','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608215", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シモアラコ", "prefecture": "福島県", "city": "福島市", "neighborhood": "下荒子", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','下荒子');
 INSERT INTO postal_data VALUES('9600115','{"jisx0402": "07201", "old_code": "96001", "postal_code": "9600115", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シモイイザカ", "prefecture": "福島県", "city": "福島市", "neighborhood": "下飯坂", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','下飯坂');
 INSERT INTO postal_data VALUES('9601106','{"jisx0402": "07201", "old_code": "96011", "postal_code": "9601106", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シモトリワタ", "prefecture": "福島県", "city": "福島市", "neighborhood": "下鳥渡", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','下鳥渡');
 INSERT INTO postal_data VALUES('9608075','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608075", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シモノデラ", "prefecture": "福島県", "city": "福島市", "neighborhood": "下野寺", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','下野寺');
+INSERT INTO postal_data VALUES('9608058','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608058", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シモヤジ", "prefecture": "福島県", "city": "福島市", "neighborhood": "下谷地", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','福島県','福島市','下谷地');
 INSERT INTO postal_data VALUES('9602153','{"jisx0402": "07201", "old_code": "96021", "postal_code": "9602153", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "ショウノ", "prefecture": "福島県", "city": "福島市", "neighborhood": "庄野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','庄野');
 INSERT INTO postal_data VALUES('9608032','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608032", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "ジンバチョウ", "prefecture": "福島県", "city": "福島市", "neighborhood": "陣場町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','陣場町');
 INSERT INTO postal_data VALUES('9608022','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608022", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シンハマチョウ", "prefecture": "福島県", "city": "福島市", "neighborhood": "新浜町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','新浜町');
 INSERT INTO postal_data VALUES('9608036','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608036", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シンマチ", "prefecture": "福島県", "city": "福島市", "neighborhood": "新町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','新町');
 INSERT INTO postal_data VALUES('9608067','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608067", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スカワチョウ", "prefecture": "福島県", "city": "福島市", "neighborhood": "須川町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','須川町');
 INSERT INTO postal_data VALUES('9608065','{"jisx0402": "07201", "old_code": "960  ", "postal_code": "9608065", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スギツマチョウ", "prefecture": "福島県", "city": "福島市", "neighborhood": "杉妻町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','杉妻町');
 INSERT INTO postal_data VALUES('9600252','{"jisx0402": "07201", "old_code": "96002", "postal_code": "9600252", "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スモモダイラ", "prefecture": "福島県", "city": "福島市", "neighborhood": "李平", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','福島市','李平');
@@ -42086,15 +42087,15 @@
 INSERT INTO postal_data VALUES('9500131','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500131", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "フクロヅ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "袋津", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','袋津');
 INSERT INTO postal_data VALUES('9500202','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500202", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "フジヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "藤山", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','藤山');
 INSERT INTO postal_data VALUES('9500153','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500153", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "フナトヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "船戸山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','船戸山');
 INSERT INTO postal_data VALUES('9500328','{"jisx0402": "15104", "old_code": "95003", "postal_code": "9500328", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マイガタ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "舞潟", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','舞潟');
 INSERT INTO postal_data VALUES('9500112','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500112", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マツヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "松山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','松山');
 INSERT INTO postal_data VALUES('9500146','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500146", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルガタ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸潟", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸潟');
 INSERT INTO postal_data VALUES('9500115','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500115", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸山');
-INSERT INTO postal_data VALUES('9500117','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500117", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルヤマノウチゼンノジョウグミ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸山ノ内善之丞組", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸山ノ内善之丞組');
+INSERT INTO postal_data VALUES('9500117','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500117", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルヤマノウチゼンノジョウグミ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸山ノ内善之丞組", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸山ノ内善之丞組');
 INSERT INTO postal_data VALUES('9500114','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500114", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ミョウガダニ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "茗荷谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','茗荷谷');
 INSERT INTO postal_data VALUES('9500143','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500143", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "モトマチ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "元町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','元町');
 INSERT INTO postal_data VALUES('9500204','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500204", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越');
 INSERT INTO postal_data VALUES('9500210','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500210", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシカミチョウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越上町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越上町');
 INSERT INTO postal_data VALUES('9500211','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500211", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシカワネチョウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越川根町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越川根町');
 INSERT INTO postal_data VALUES('9500208','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500208", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシチュウオウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越中央", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越中央');
 INSERT INTO postal_data VALUES('9500209','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500209", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシヒガシチョウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越東町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越東町');
@@ -55881,15 +55882,15 @@
 INSERT INTO postal_data VALUES('3990039','{"jisx0402": "20202", "old_code": "399  ", "postal_code": "3990039", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "コヤキタ", "prefecture": "長野県", "city": "松本市", "neighborhood": "小屋北", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','小屋北');
 INSERT INTO postal_data VALUES('3990038','{"jisx0402": "20202", "old_code": "399  ", "postal_code": "3990038", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "コヤミナミ", "prefecture": "長野県", "city": "松本市", "neighborhood": "小屋南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','小屋南');
 INSERT INTO postal_data VALUES('3990033','{"jisx0402": "20202", "old_code": "399  ", "postal_code": "3990033", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ササガ", "prefecture": "長野県", "city": "松本市", "neighborhood": "笹賀", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','笹賀');
 INSERT INTO postal_data VALUES('3900847','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900847", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ササベ", "prefecture": "長野県", "city": "松本市", "neighborhood": "笹部", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','笹部');
 INSERT INTO postal_data VALUES('3900221','{"jisx0402": "20202", "old_code": "39002", "postal_code": "3900221", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "サトヤマベ", "prefecture": "長野県", "city": "松本市", "neighborhood": "里山辺", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','里山辺');
 INSERT INTO postal_data VALUES('3900877','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900877", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "サワムラ", "prefecture": "長野県", "city": "松本市", "neighborhood": "沢村", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','沢村');
 INSERT INTO postal_data VALUES('3900301','{"jisx0402": "20202", "old_code": "39003", "postal_code": "3900301", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シナグラ", "prefecture": "長野県", "city": "松本市", "neighborhood": "稲倉", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','稲倉');
-INSERT INTO postal_data VALUES('3900851','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900851", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマウチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島内", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "1〜9819、9822、9831〜9863番地"}','長野県','松本市','島内');
+INSERT INTO postal_data VALUES('3900851','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900851", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマウチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島内", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "1〜9819、9822、9831〜9863番地"}','長野県','松本市','島内');
 INSERT INTO postal_data VALUES('3998251','{"jisx0402": "20202", "old_code": "39982", "postal_code": "3998251", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマウチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島内", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "9820、9821、9823〜9830、9864番地以上"}','長野県','松本市','島内');
 INSERT INTO postal_data VALUES('3900852','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900852", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマダチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島立", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','島立');
 INSERT INTO postal_data VALUES('3900805','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900805", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シミズ", "prefecture": "長野県", "city": "松本市", "neighborhood": "清水", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','清水');
 INSERT INTO postal_data VALUES('3900875','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900875", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウセイ", "prefecture": "長野県", "city": "松本市", "neighborhood": "城西", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','城西');
 INSERT INTO postal_data VALUES('3900807','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900807", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウトウ", "prefecture": "長野県", "city": "松本市", "neighborhood": "城東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','城東');
 INSERT INTO postal_data VALUES('3900828','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900828", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ショウナイ", "prefecture": "長野県", "city": "松本市", "neighborhood": "庄内", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','庄内');
 INSERT INTO postal_data VALUES('3900866','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900866", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウヤマ", "prefecture": "長野県", "city": "松本市", "neighborhood": "城山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','城山');
@@ -85699,15 +85700,15 @@
 INSERT INTO postal_data VALUES('6550006','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550006", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ホンタモン", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "本多聞", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','本多聞');
 INSERT INTO postal_data VALUES('6550044','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550044", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイコザカ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞子坂", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞子坂');
 INSERT INTO postal_data VALUES('6550046','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550046", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイコダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞子台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞子台');
 INSERT INTO postal_data VALUES('6550051','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550051", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイタモンニシ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞多聞西", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞多聞西');
 INSERT INTO postal_data VALUES('6550052','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550052", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイタモンヒガシ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞多聞東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞多聞東');
 INSERT INTO postal_data VALUES('6550004','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550004", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マナビガオカ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "学が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','学が丘');
 INSERT INTO postal_data VALUES('6550025','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550025", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズガオカ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "瑞ケ丘", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','瑞ケ丘');
-INSERT INTO postal_data VALUES('6550855','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550855", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズキダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "みずき台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','みずき台');
+INSERT INTO postal_data VALUES('6550855','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550855", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズキダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "みずき台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','みずき台');
 INSERT INTO postal_data VALUES('6550022','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550022", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズホドオリ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "瑞穂通", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','瑞穂通');
 INSERT INTO postal_data VALUES('6550043','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550043", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミナミタモンダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "南多聞台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','南多聞台');
 INSERT INTO postal_data VALUES('6550874','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550874", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミヤマダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "美山台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','美山台');
 INSERT INTO postal_data VALUES('6550028','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550028", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミヤモトチョウ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "宮本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','宮本町');
 INSERT INTO postal_data VALUES('6550852','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550852", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミョウダニチョウ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "名谷町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','名谷町');
 INSERT INTO postal_data VALUES('6550854','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550854", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "モモヤマダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "桃山台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','桃山台');
 INSERT INTO postal_data VALUES('6550891','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550891", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ヤマテ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "山手", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','山手');
@@ -89436,14 +89437,15 @@
 INSERT INTO postal_data VALUES('6562143','{"jisx0402": "28226", "old_code": "65621", "postal_code": "6562143", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "サト", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "里", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','里');
 INSERT INTO postal_data VALUES('6562212','{"jisx0402": "28226", "old_code": "65622", "postal_code": "6562212", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "サノ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "佐野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','佐野');
 INSERT INTO postal_data VALUES('6562213','{"jisx0402": "28226", "old_code": "65622", "postal_code": "6562213", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "サノニイジマ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "佐野新島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','佐野新島');
 INSERT INTO postal_data VALUES('6562141','{"jisx0402": "28226", "old_code": "65621", "postal_code": "6562141", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シオ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "塩尾", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','塩尾');
 INSERT INTO postal_data VALUES('6562142','{"jisx0402": "28226", "old_code": "65621", "postal_code": "6562142", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シオタニイジマ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "塩田新島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','塩田新島');
 INSERT INTO postal_data VALUES('6562131','{"jisx0402": "28226", "old_code": "65621", "postal_code": "6562131", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シヅキ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "志筑", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','志筑');
 INSERT INTO postal_data VALUES('6562132','{"jisx0402": "28226", "old_code": "65621", "postal_code": "6562132", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シヅキニイジマ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "志筑新島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','志筑新島');
+INSERT INTO postal_data VALUES('6562133','{"jisx0402": "28226", "old_code": "65621", "postal_code": "6562133", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シヅキニイハマ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "志筑新浜", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','志筑新浜');
 INSERT INTO postal_data VALUES('6561522','{"jisx0402": "28226", "old_code": "65615", "postal_code": "6561522", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シモガワイ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "下河合", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','下河合');
 INSERT INTO postal_data VALUES('6562333','{"jisx0402": "28226", "old_code": "65623", "postal_code": "6562333", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シモダ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "下田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','下田');
 INSERT INTO postal_data VALUES('6562322','{"jisx0402": "28226", "old_code": "65623", "postal_code": "6562322", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シラヤマ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "白山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','白山');
 INSERT INTO postal_data VALUES('6561502','{"jisx0402": "28226", "old_code": "65615", "postal_code": "6561502", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "シンムラ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "新村", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','新村');
 INSERT INTO postal_data VALUES('6561521','{"jisx0402": "28226", "old_code": "65615", "postal_code": "6561521", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "タガ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "多賀", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','多賀');
 INSERT INTO postal_data VALUES('6561551','{"jisx0402": "28226", "old_code": "65615", "postal_code": "6561551", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "タカヤマ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "高山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','高山');
 INSERT INTO postal_data VALUES('6561524','{"jisx0402": "28226", "old_code": "65615", "postal_code": "6561524", "prefecture_kana": "ヒョウゴケン", "city_kana": "アワジシ", "neighborhood_kana": "タケダニ", "prefecture": "兵庫県", "city": "淡路市", "neighborhood": "竹谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','淡路市','竹谷');
@@ -100840,15 +100842,15 @@
 INSERT INTO postal_data VALUES('7520903','{"jisx0402": "35201", "old_code": "752  ", "postal_code": "7520903", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カズミツチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "員光町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','員光町');
 INSERT INTO postal_data VALUES('7510884','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510884", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カタチヤマ", "prefecture": "山口県", "city": "下関市", "neighborhood": "形山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','形山');
 INSERT INTO postal_data VALUES('7510888','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510888", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カタチヤマチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "形山町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','形山町');
 INSERT INTO postal_data VALUES('7510885','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510885", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カタチヤマミドリマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "形山みどり町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','形山みどり町');
 INSERT INTO postal_data VALUES('7500061','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500061", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カミシンチチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "上新地町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','上新地町');
 INSERT INTO postal_data VALUES('7500009','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500009", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カミタナカマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "上田中町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','上田中町');
 INSERT INTO postal_data VALUES('7520925','{"jisx0402": "35201", "old_code": "752  ", "postal_code": "7520925", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カメハマチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "亀浜町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','亀浜町');
-INSERT INTO postal_data VALUES('7596602','{"jisx0402": "35201", "old_code": "75966", "postal_code": "7596602", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カモノ", "prefecture": "山口県", "city": "下関市", "neighborhood": "蒲生野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','山口県','下関市','蒲生野');
+INSERT INTO postal_data VALUES('7596602','{"jisx0402": "35201", "old_code": "75966", "postal_code": "7596602", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カモノ", "prefecture": "山口県", "city": "下関市", "neighborhood": "蒲生野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','蒲生野');
 INSERT INTO postal_data VALUES('7500005','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500005", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カラトチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "唐戸町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','唐戸町');
 INSERT INTO postal_data VALUES('7510859','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510859", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カワナカホンマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "川中本町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','川中本町');
 INSERT INTO postal_data VALUES('7510853','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510853", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カワナカユタカマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "川中豊町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','川中豊町');
 INSERT INTO postal_data VALUES('7500032','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500032", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンセイチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "関西町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','関西町');
 INSERT INTO postal_data VALUES('7500022','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500022", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンセイホンマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "関西本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','関西本町');
 INSERT INTO postal_data VALUES('7520907','{"jisx0402": "35201", "old_code": "752  ", "postal_code": "7520907", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンダ", "prefecture": "山口県", "city": "下関市", "neighborhood": "神田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','神田');
 INSERT INTO postal_data VALUES('7500044','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500044", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンダチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "神田町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','神田町');
@@ -121868,17 +121870,17 @@
 INSERT INTO office_data VALUES('0392286','{"jis": "02412", "kana": "ニホンフ-ドパツカ- カブシキガイシヤ アオモリコウジヨウ", "name": "日本フードパッカー　株式会社　青森工場", "prefecture": "青森県", "city": "上北郡おいらせ町", "neighborhood": "松原", "banchi": "2丁目132-1", "postal_code": "0392286", "old_code": "03922", "post_office": "百石", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "カミキタグンオイラセチョウ", "neighborhood_kana": "マツバラ", "alternates": []}');
 INSERT INTO office_data VALUES('0392293','{"jis": "02412", "kana": "モモカワ カブシキガイシヤ", "name": "桃川　株式会社", "prefecture": "青森県", "city": "上北郡おいらせ町", "neighborhood": "上明堂", "banchi": "112", "postal_code": "0392293", "old_code": "03922", "post_office": "百石", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "カミキタグンオイラセチョウ", "neighborhood_kana": "カミアケドウ", "alternates": []}');
 INSERT INTO office_data VALUES('0394692','{"jis": "02423", "kana": "オオママチヤクバ", "name": "大間町役場", "prefecture": "青森県", "city": "下北郡大間町", "neighborhood": "大字大間", "banchi": "字大間104番地", "postal_code": "0394692", "old_code": "03946", "post_office": "大間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0394293','{"jis": "02424", "kana": "トウホクデンリヨク カブシキガイシヤ ヒガシドオリゲンシリヨクハツデンシヨ", "name": "東北電力　株式会社　東通原子力発電所", "prefecture": "青森県", "city": "下北郡東通村", "neighborhood": "大字白糠", "banchi": "字前坂下34-4", "postal_code": "0394293", "old_code": "03942", "post_office": "白糠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0394292','{"jis": "02424", "kana": "ヒガシドオリムラヤクバ", "name": "東通村役場", "prefecture": "青森県", "city": "下北郡東通村", "neighborhood": "大字砂子又", "banchi": "字沢内5番地34", "postal_code": "0394292", "old_code": "03942", "post_office": "白糠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0390198','{"jis": "02441", "kana": "サンノヘマチヤクバ", "name": "三戸町役場", "prefecture": "青森県", "city": "三戸郡三戸町", "neighborhood": "大字在府小路町", "banchi": "43", "postal_code": "0390198", "old_code": "03901", "post_office": "三戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0390292','{"jis": "02443", "kana": "タツコマチヤクバ", "name": "田子町役場", "prefecture": "青森県", "city": "三戸郡田子町", "neighborhood": "大字田子", "banchi": "字天神堂平81", "postal_code": "0390292", "old_code": "03902", "post_office": "田子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390195','{"jis": "02445", "kana": "ナンブシシヨ", "name": "南部支所", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字沖田面", "banchi": "字沖中46", "postal_code": "0390195", "old_code": "03901", "post_office": "三戸", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390592','{"jis": "02445", "kana": "ナンブチヨウヤクバ", "name": "南部町役場", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字平", "banchi": "字広場28番地1", "postal_code": "0390592", "old_code": "03905", "post_office": "上名久井", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390892','{"jis": "02445", "kana": "フクチシシヨ", "name": "福地支所", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字苫米地", "banchi": "字下宿23-1", "postal_code": "0390892", "old_code": "03908", "post_office": "福地", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0390195','{"jis": "02445", "kana": "ナンブシシヨ", "name": "南部支所", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字沖田面", "banchi": "字沖中46", "postal_code": "0390195", "old_code": "03901", "post_office": "三戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0390592','{"jis": "02445", "kana": "ナンブチヨウヤクバ", "name": "南部町役場", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字平", "banchi": "字広場28番地1", "postal_code": "0390592", "old_code": "03905", "post_office": "上名久井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0390892','{"jis": "02445", "kana": "フクチシシヨ", "name": "福地支所", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字苫米地", "banchi": "字下宿23-1", "postal_code": "0390892", "old_code": "03908", "post_office": "福地", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0208584','{"jis": "03201", "kana": "イツパンシヤダンホウジン イワテケンイシカイ", "name": "一般社団法人　岩手県医師会", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "菜園", "banchi": "2丁目8番20号", "postal_code": "0208584", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "サイエン", "alternates": []}');
 INSERT INTO office_data VALUES('0208505','{"jis": "03201", "kana": "イワテイカダイガクフゾク ウチマルメデイカルセンタ-", "name": "岩手医科大学附属　内丸メディカルセンター", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "内丸", "banchi": "19番1号", "postal_code": "0208505", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウチマル", "alternates": []}');
 INSERT INTO office_data VALUES('0208540','{"jis": "03201", "kana": "イワテケン ケイサツホンブ", "name": "岩手県　警察本部", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "内丸", "banchi": "8-10", "postal_code": "0208540", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウチマル", "alternates": []}');
 INSERT INTO office_data VALUES('0208577','{"jis": "03201", "kana": "イワテケンエイセイケンキユウジヨ", "name": "岩手県衛生研究所", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "飯岡新田", "banchi": "1丁目36-1", "postal_code": "0208577", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "イイオカシンデン", "alternates": []}');
 INSERT INTO office_data VALUES('0208510','{"jis": "03201", "kana": "イワテケンジチカイカン", "name": "岩手県自治会館", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "山王町", "banchi": "4-1", "postal_code": "0208510", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "サンノウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0208543','{"jis": "03201", "kana": "イワテケンリツ トリヨウコウトウガツコウ", "name": "岩手県立　杜陵高等学校", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "上田", "banchi": "2丁目3-1", "postal_code": "0208543", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウエダ", "alternates": []}');
 INSERT INTO office_data VALUES('0208515','{"jis": "03201", "kana": "イワテケンリツ モリオカダイイチコウトウガツコウ", "name": "岩手県立　盛岡第一高等学校", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "上田", "banchi": "3丁目2-1", "postal_code": "0208515", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウエダ", "alternates": []}');
@@ -122395,15 +122397,15 @@
 INSERT INTO office_data VALUES('9894792','{"jis": "04212", "kana": "トメシ イシコシソウゴウシシヨ", "name": "登米市　石越総合支所", "prefecture": "宮城県", "city": "登米市", "neighborhood": "石越町", "banchi": "字愛宕81", "postal_code": "9894792", "old_code": "98947", "post_office": "石越", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9872195','{"jis": "04213", "kana": "イトウハムデイリ- カブシキガイシヤ", "name": "伊藤ハムディリー　株式会社", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "高清水来光沢", "banchi": "20", "postal_code": "9872195", "old_code": "98721", "post_office": "高清水", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "タカシミズライコウザワ", "alternates": []}');
 INSERT INTO office_data VALUES('9872293','{"jis": "04213", "kana": "クリハラシヤクシヨ", "name": "栗原市役所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館薬師", "banchi": "1丁目7-1", "postal_code": "9872293", "old_code": "98722", "post_office": "築館", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテヤクシ", "alternates": []}');
 INSERT INTO office_data VALUES('9872292','{"jis": "04213", "kana": "ツキダテゼイムシヨ", "name": "築館税務署", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館伊豆", "banchi": "3丁目1番10号", "postal_code": "9872292", "old_code": "98722", "post_office": "築館", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテイズ", "alternates": []}');
 INSERT INTO office_data VALUES('9872392','{"jis": "04213", "kana": "クリハラシ イチハサマソウゴウシシヨ", "name": "栗原市　一迫総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "一迫真坂", "banchi": "字清水田河前5", "postal_code": "9872392", "old_code": "98723", "post_office": "一迫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "イチハサママサカ", "alternates": []}');
 INSERT INTO office_data VALUES('9872592','{"jis": "04213", "kana": "クリハラシヤクシヨ ハナヤマソウゴウシシヨ", "name": "栗原市役所　花山総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "花山本沢北ノ前", "banchi": "77", "postal_code": "9872592", "old_code": "98725", "post_office": "花山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9872593','{"jis": "04213", "kana": "コクリツ ハナヤマセイシヨウネンシゼンノイエ", "name": "国立　花山青少年自然の家", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "花山", "banchi": "字本沢沼山61-1", "postal_code": "9872593", "old_code": "98725", "post_office": "花山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9894592','{"jis": "04213", "kana": "クリハラシ セミネソウゴウシシヨ", "name": "栗原市　瀬峰総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "瀬峰", "banchi": "長者原37番地2", "postal_code": "9894592", "old_code": "98945", "post_office": "高清水", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9894592','{"jis": "04213", "kana": "クリハラシ セミネソウゴウシシヨ", "name": "栗原市　瀬峰総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "瀬峰", "banchi": "長者原37番地2", "postal_code": "9894592", "old_code": "98945", "post_office": "高清水", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9895392','{"jis": "04213", "kana": "クリハラシ クリコマソウゴウシシヨ", "name": "栗原市　栗駒総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "栗駒岩ケ崎", "banchi": "円鏡寺後155", "postal_code": "9895392", "old_code": "98953", "post_office": "栗駒", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "クリコマイワガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('9895492','{"jis": "04213", "kana": "クリハラシヤクシヨ ウグイスザワソウゴウシシヨ", "name": "栗原市役所　鶯沢総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "鶯沢", "banchi": "南郷辻前74-1", "postal_code": "9895492", "old_code": "98954", "post_office": "鴬沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9895592','{"jis": "04213", "kana": "クリハラシ ワカヤナギソウゴウシシヨ", "name": "栗原市　若柳総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "若柳川南", "banchi": "戸ノ西4", "postal_code": "9895592", "old_code": "98955", "post_office": "若柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ワカヤナギカワミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('9895693','{"jis": "04213", "kana": "クリツコノウギヨウキヨウドウクミアイ", "name": "栗っこ農業協同組合", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "志波姫堀口", "banchi": "見渡2-1", "postal_code": "9895693", "old_code": "98956", "post_office": "志波姫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "シワヒメホリグチ", "alternates": []}');
 INSERT INTO office_data VALUES('9895692','{"jis": "04213", "kana": "クリハラシ シワヒメソウゴウシシヨ", "name": "栗原市　志波姫総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "志波姫沼崎", "banchi": "堰畑143", "postal_code": "9895692", "old_code": "98956", "post_office": "志波姫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "シワヒメヌマザキ", "alternates": []}');
 INSERT INTO office_data VALUES('9810394','{"jis": "04214", "kana": "サメガウラスイヨウビユウビンキヨク", "name": "鮫ヶ浦水曜日郵便局", "prefecture": "宮城県", "city": "東松島市", "neighborhood": "宮戸字観音山", "banchi": "5番地", "postal_code": "9810394", "old_code": "98104", "post_office": "鳴瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9871395','{"jis": "04215", "kana": "オオサキシ マツヤマソウゴウシシヨ", "name": "大崎市　松山総合支所", "prefecture": "宮城県", "city": "大崎市", "neighborhood": "松山千石", "banchi": "字広田30", "postal_code": "9871395", "old_code": "98713", "post_office": "鹿島台", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "オオサキシ", "neighborhood_kana": "マツヤマセンゴク", "alternates": []}');
@@ -122913,15 +122915,15 @@
 INSERT INTO office_data VALUES('9638670','{"jis": "07203", "kana": "タカラカセイキキ カブシキガイシヤ", "name": "宝化成機器　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "喜久田町卸", "banchi": "1丁目62-1(郡山卸町郵便局私書箱第355号)", "postal_code": "9638670", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "キクタマチオロシ", "alternates": []}');
 INSERT INTO office_data VALUES('9638661','{"jis": "07203", "kana": "ダイワシヨウケン カブシキガイシヤ コオリヤマシテン", "name": "大和証券　株式会社　郡山支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "10-10(郡山中町郵便局私書箱第603号)", "postal_code": "9638661", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638570','{"jis": "07203", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ フクシマシテン", "name": "東京海上日動火災保険　株式会社　福島支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "長者", "banchi": "1丁目7-20", "postal_code": "9638570", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "チョウジャ", "alternates": []}');
 INSERT INTO office_data VALUES('9638506','{"jis": "07203", "kana": "トウジルシコオリヤマセイカ カブシキガイシヤ", "name": "東印郡山青果　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富久山町久保田", "banchi": "字太郎殿前193", "postal_code": "9638506", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "フクヤママチクボタ", "alternates": []}');
 INSERT INTO office_data VALUES('9638676','{"jis": "07203", "kana": "トウホクアルフレツサ カブシキガイシヤ", "name": "東北アルフレッサ　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "喜久田町卸", "banchi": "1丁目46-1(郡山卸町郵便局私書箱第357号)", "postal_code": "9638676", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "キクタマチオロシ", "alternates": []}');
 INSERT INTO office_data VALUES('9638575','{"jis": "07203", "kana": "トウホクデンリヨク カブシキガイシヤ コオリヤマエイギヨウシヨ", "name": "東北電力　株式会社　郡山営業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "細沼町", "banchi": "1-5", "postal_code": "9638575", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ホソヌママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638551','{"jis": "07203", "kana": "ニツポンホウソウキヨウカイ フクシマホウソウキヨク コオリヤマシキヨク", "name": "日本放送協会　福島放送局　郡山支局", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目5-21", "postal_code": "9638551", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": []}');
-INSERT INTO office_data VALUES('9638637','{"jis": "07203", "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "ニデックプレシジョン　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字諏訪内37(郡山郵便局私書箱第37号)", "postal_code": "9638637", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9638637','{"jis": "07203", "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "ニデックプレシジョン　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字諏訪内37(郡山郵便局私書箱第37号)", "postal_code": "9638637", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638580','{"jis": "07203", "kana": "ニホンセイメイホケン ソウゴガイシヤ コオリヤマシシヤ", "name": "日本生命保険　相互会社　郡山支社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "駅前", "banchi": "2丁目12-2", "postal_code": "9638580", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "エキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('9638508','{"jis": "07203", "kana": "ニホンタバコサンギヨウ カブシキガイシヤ コオリヤマコウジヨウ", "name": "日本たばこ産業　株式会社　郡山工場", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字外河原", "banchi": "8-1", "postal_code": "9638508", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638556','{"jis": "07203", "kana": "パナソニツク インダストリ- カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "パナソニック　インダストリー　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字石塚", "banchi": "111番地", "postal_code": "9638556", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638540','{"jis": "07203", "kana": "フクシマケンキヨウイクチヨウケンチユウキヨウイクジムシヨ", "name": "福島県教育庁県中教育事務所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目1番1号", "postal_code": "9638540", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": [{"jis": "07203", "kana": "フクシマケンケンチユウチホウシンコウキヨク", "name": "福島県県中地方振興局", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目1番1号", "postal_code": "9638540", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": []}]}');
 INSERT INTO office_data VALUES('9638668','{"jis": "07203", "kana": "フクシマケンシヨウコウシンヨウクミアイ", "name": "福島県商工信用組合", "prefecture": "福島県", "city": "郡山市", "neighborhood": "堂前町", "banchi": "7-7(郡山中町郵便局私書箱第616号)", "postal_code": "9638668", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ドウマエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638502','{"jis": "07203", "kana": "フクシマサクラノウギヨウキヨウドウクミアイ", "name": "福島さくら農業協同組合", "prefecture": "福島県", "city": "郡山市", "neighborhood": "朝日", "banchi": "2丁目14-7", "postal_code": "9638502", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アサヒ", "alternates": []}');
 INSERT INTO office_data VALUES('9638664','{"jis": "07203", "kana": "フクシマシンヨウハンバイ カブシキガイシヤ", "name": "福島信用販売　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "14-26(郡山中町郵便局私書箱第628号)", "postal_code": "9638664", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
@@ -122959,15 +122961,15 @@
 INSERT INTO office_data VALUES('9708551','{"jis": "07204", "kana": "イワキメイセイダイガク", "name": "いわき明星大学", "prefecture": "福島県", "city": "いわき市", "neighborhood": "中央台飯野", "banchi": "5丁目5-1", "postal_code": "9708551", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "チュウオウダイイイノ", "alternates": []}');
 INSERT INTO office_data VALUES('9708703','{"jis": "07204", "kana": "イワキロウドウキジユンカントクシヨ", "name": "いわき労働基準監督署", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字堂根町4-11", "postal_code": "9708703", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708625','{"jis": "07204", "kana": "オカダデンキサンギヨウ カブシキガイシヤ", "name": "岡田電気産業　株式会社", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平谷川瀬", "banchi": "一丁目6-1(いわき郵便局私書箱第25号)", "postal_code": "9708625", "old_code": "970  ", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラヤガワセ", "alternates": []}');
 INSERT INTO office_data VALUES('9708511','{"jis": "07204", "kana": "カブシキカイシヤエヌテイテイヒガシニホンフクシマ イワキシテン", "name": "株式会社　ＮＴＴ東日本－福島　いわき支店", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字堂根町3-2", "postal_code": "9708511", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708516','{"jis": "07204", "kana": "ザイダンホウジン イワキサイセイカイ マツムラソウゴウビヨウイン", "name": "財団法人　磐城済世会　松村総合病院", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字小太郎町1-1", "postal_code": "9708516", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708501','{"jis": "07204", "kana": "ニツポンネンキンキコウ タイラネンキンジムシヨ", "name": "日本年金機構　平年金事務所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字童子町3-21", "postal_code": "9708501", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708410','{"jis": "07204", "kana": "ホテルビ-フオ-テイ- エスパルイワキ", "name": "ホテルＢ４Ｔ　エスパルいわき", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字田町1", "postal_code": "9708410", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
-INSERT INTO office_data VALUES('9701192','{"jis": "07204", "kana": "アルプスアルパイン カブシキガイシヤ イワキカイハツセンタ-", "name": "アルプスアルパイン　株式会社　いわき開発センター", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間工業団地", "banchi": "20-1", "postal_code": "9701192", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシマコウギョウダンチ", "alternates": []}');
+INSERT INTO office_data VALUES('9701192','{"jis": "07204", "kana": "アルプスアルパイン カブシキガイシヤ イワキカイハツセンタ-", "name": "アルプスアルパイン　株式会社　いわき開発センター", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間工業団地", "banchi": "20-1", "postal_code": "9701192", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシマコウギョウダンチ", "alternates": []}');
 INSERT INTO office_data VALUES('9701193','{"jis": "07204", "kana": "アルプスデンキ カブシキガイシヤ ペリフエラルジギヨウブ タイラコウジヨウ", "name": "アルプス電気　株式会社　ペリフェラル事業部　平工場", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間町小谷作", "banchi": "字作畑39-1", "postal_code": "9701193", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシママチオヤサク", "alternates": []}');
 INSERT INTO office_data VALUES('9701194','{"jis": "07204", "kana": "ユウゲンガイシヤ ナガクボシヨクヒン", "name": "有限会社　長久保食品", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間町中好間", "banchi": "字鍛冶内28-2", "postal_code": "9701194", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシママチナカヨシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9708686','{"jis": "07204", "kana": "イワキシヤクシヨ", "name": "いわき市役所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字梅本21(いわき郵便局私書箱第55号)", "postal_code": "9708686", "old_code": "97091", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708646','{"jis": "07204", "kana": "カブシキガイシヤ カチワグミ", "name": "株式会社　加地和組", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字小太郎町4-11(いわき郵便局私書箱第46号)", "postal_code": "9708646", "old_code": "97091", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708635','{"jis": "07204", "kana": "サトウ カブシキガイシヤ イワキシテン", "name": "佐藤　株式会社　いわき支店", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字五町目18-5(いわき郵便局私書箱第35号)", "postal_code": "9708635", "old_code": "97091", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9718555','{"jis": "07204", "kana": "イオンモ-ルイワキオナハマ イオンモ-ルジムシヨ", "name": "イオンモールいわき小名浜　イオンモール事務所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "小名浜", "banchi": "字辰巳町79番地", "postal_code": "9718555", "old_code": "971  ", "post_office": "小名浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "オナハマ", "alternates": []}');
 INSERT INTO office_data VALUES('9728555','{"jis": "07204", "kana": "ジヨウバンコウサン カブシキガイシヤ スパ・リゾ-ト・ハワイアンズ", "name": "常磐興産　株式会社　スパ・リゾート・ハワイアンズ", "prefecture": "福島県", "city": "いわき市", "neighborhood": "常磐藤原町", "banchi": "蕨平50", "postal_code": "9728555", "old_code": "972  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ジョウバンフジワラマチ", "alternates": []}');
@@ -123525,15 +123527,15 @@
 INSERT INTO office_data VALUES('3211293','{"jis": "09206", "kana": "ニツポンネンキンキコウ イマイチネンキンジムシヨ", "name": "日本年金機構　今市年金事務所", "prefecture": "栃木県", "city": "日光市", "neighborhood": "中央町", "banchi": "17-3", "postal_code": "3211293", "old_code": "32112", "post_office": "日光東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3211492','{"jis": "09206", "kana": "ニツコウシヤクシヨ ニツコウソウゴウシシヨ", "name": "日光市役所　日光総合支所", "prefecture": "栃木県", "city": "日光市", "neighborhood": "中鉢石町", "banchi": "999", "postal_code": "3211492", "old_code": "32114", "post_office": "日光", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "ナカハツイシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3211493','{"jis": "09206", "kana": "フルカワデンコウ", "name": "古河電工", "prefecture": "栃木県", "city": "日光市", "neighborhood": "清滝町", "banchi": "500", "postal_code": "3211493", "old_code": "32114", "post_office": "日光", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3212493','{"jis": "09206", "kana": "ジヤスコ イマイチテン", "name": "ジャスコ　今市店", "prefecture": "栃木県", "city": "日光市", "neighborhood": "豊田", "banchi": "79-1", "postal_code": "3212493", "old_code": "32124", "post_office": "大桑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "トヨダ", "alternates": []}');
 INSERT INTO office_data VALUES('3212492','{"jis": "09206", "kana": "トウブケンセツ カブシキガイシヤ", "name": "東武建設　株式会社", "prefecture": "栃木県", "city": "日光市", "neighborhood": "大桑町", "banchi": "138", "postal_code": "3212492", "old_code": "32124", "post_office": "大桑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "オオクワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3212592','{"jis": "09206", "kana": "カナヤホテルカンコウ カブシキガイシヤ キヌガワオンセンホテル", "name": "金谷ホテル観光　株式会社　鬼怒川温泉ホテル", "prefecture": "栃木県", "city": "日光市", "neighborhood": "鬼怒川温泉滝", "banchi": "545", "postal_code": "3212592", "old_code": "32125", "post_office": "鬼怒川温泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "キヌガワオンセンタキ", "alternates": []}');
 INSERT INTO office_data VALUES('3212598','{"jis": "09206", "kana": "カブシキガイシヤ アサヤホテル", "name": "株式会社　あさやホテル", "prefecture": "栃木県", "city": "日光市", "neighborhood": "鬼怒川温泉滝", "banchi": "813", "postal_code": "3212598", "old_code": "32125", "post_office": "鬼怒川温泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "キヌガワオンセンタキ", "alternates": []}');
-INSERT INTO office_data VALUES('3212593','{"jis": "09206", "kana": "ドツキヨウイカダイガク ニツコウイリヨウセンタ-", "name": "獨協医科大学　日光医療センター", "prefecture": "栃木県", "city": "日光市", "neighborhood": "高徳", "banchi": "632", "postal_code": "3212593", "old_code": "32125", "post_office": "鬼怒川温泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "タカトク", "alternates": []}');
+INSERT INTO office_data VALUES('3212593','{"jis": "09206", "kana": "トウブワ-ルドスクウエア カブシキカイシヤ", "name": "東武ワールドスクウェア　株式会社", "prefecture": "栃木県", "city": "日光市", "neighborhood": "鬼怒川温泉大原", "banchi": "209-1", "postal_code": "3212593", "old_code": "32125", "post_office": "鬼怒川温泉", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "キヌガワオンセンオオハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3212596','{"jis": "09206", "kana": "ニツコウシ フジハラスイドウジムシヨ", "name": "日光市　藤原水道事務所", "prefecture": "栃木県", "city": "日光市", "neighborhood": "藤原", "banchi": "1-6", "postal_code": "3212596", "old_code": "32125", "post_office": "鬼怒川温泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "フジハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3212595','{"jis": "09206", "kana": "ニツコウシ フジハラソウゴウシシヨ", "name": "日光市　藤原総合支所", "prefecture": "栃木県", "city": "日光市", "neighborhood": "藤原", "banchi": "1", "postal_code": "3212595", "old_code": "32125", "post_office": "鬼怒川温泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ニッコウシ", "neighborhood_kana": "フジハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3238686','{"jis": "09208", "kana": "オヤマシヤクシヨ", "name": "小山市役所", "prefecture": "栃木県", "city": "小山市", "neighborhood": "中央町", "banchi": "1丁目1-1", "postal_code": "3238686", "old_code": "323  ", "post_office": "小山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オヤマシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3238558','{"jis": "09208", "kana": "カブシキガイシヤ コマツセイサクジヨ オヤマコウジヨウ", "name": "株式会社　小松製作所　小山工場", "prefecture": "栃木県", "city": "小山市", "neighborhood": "大字横倉新田", "banchi": "400", "postal_code": "3238558", "old_code": "323  ", "post_office": "小山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3238755','{"jis": "09208", "kana": "カブシキガイシヤ ワイエスオ-.パ-トナ-ズ", "name": "株式会社　ＹＳＯ．ＰＡＲＴＮＥＲ’Ｓ", "prefecture": "栃木県", "city": "小山市", "neighborhood": "卒島", "banchi": "1291", "postal_code": "3238755", "old_code": "323  ", "post_office": "小山", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オヤマシ", "neighborhood_kana": "ソシマ", "alternates": []}');
 INSERT INTO office_data VALUES('3238756','{"jis": "09208", "kana": "カブシキガイシヤ ワイエスオ-.パ-トナ-ズ メガキヤンペ-ン", "name": "株式会社　ＹＳＯ．ＰＡＲＴＮＥＲ’Ｓ　ＭＥＧＡキャンペーン", "prefecture": "栃木県", "city": "小山市", "neighborhood": "卒島", "banchi": "1291", "postal_code": "3238756", "old_code": "323  ", "post_office": "小山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オヤマシ", "neighborhood_kana": "ソシマ", "alternates": []}');
 INSERT INTO office_data VALUES('3238611','{"jis": "09208", "kana": "コダイラサンギヨウ カブシキガイシヤ", "name": "小平産業　株式会社", "prefecture": "栃木県", "city": "小山市", "neighborhood": "大字稲葉郷", "banchi": "1341-1", "postal_code": "3238611", "old_code": "323  ", "post_office": "小山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -123545,23 +123547,23 @@
 INSERT INTO office_data VALUES('3238601','{"jis": "09208", "kana": "フルカワキカイキンゾク カブシキガイシヤ オヤマコウジヨウ", "name": "古河機械金属　株式会社　小山工場", "prefecture": "栃木県", "city": "小山市", "neighborhood": "若木町", "banchi": "1丁目23-15(小山郵便局私書箱第9号)", "postal_code": "3238601", "old_code": "323  ", "post_office": "小山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オヤマシ", "neighborhood_kana": "ワカギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3214392','{"jis": "09209", "kana": "エスエイチピ-ピ-ジヤパン ゴウドウカイシヤ", "name": "ＳＨＰＰジャパン　合同会社", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "鬼怒ケ丘", "banchi": "2番地2", "postal_code": "3214392", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "キヌガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3214393','{"jis": "09209", "kana": "ダイイチデンシコウギヨウ カブシキガイシヤ", "name": "第一電子工業　株式会社", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "松山町", "banchi": "14", "postal_code": "3214393", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "マツヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3214396','{"jis": "09209", "kana": "フジフアイバ-グラス カブシキガイシヤ", "name": "富士ファイバーグラス　株式会社", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "鬼怒ケ丘", "banchi": "6", "postal_code": "3214396", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "キヌガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3214398','{"jis": "09209", "kana": "モオカケンゼイジムシヨ", "name": "真岡県税事務所", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "荒町", "banchi": "116-1", "postal_code": "3214398", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "アラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3214395','{"jis": "09209", "kana": "モオカシヤクシヨ", "name": "真岡市役所", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "荒町", "banchi": "5191", "postal_code": "3214395", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "アラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3248642','{"jis": "09210", "kana": "オオタワラ ゼイムシヨ", "name": "大田原　税務署", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "紫塚", "banchi": "1丁目5-54(大田原郵便局私書箱第11号)", "postal_code": "3248642", "old_code": "324  ", "post_office": "大田原", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ムラサキヅカ", "alternates": []}');
-INSERT INTO office_data VALUES('3248551','{"jis": "09210", "kana": "オオタワラケンゼイジムシヨ", "name": "大田原県税事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2丁目2828-4", "postal_code": "3248551", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('3248551','{"jis": "09210", "kana": "オオタワラケンゼイジムシヨ", "name": "大田原県税事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2丁目2828-4", "postal_code": "3248551", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248641','{"jis": "09210", "kana": "オオタワラシヤクシヨ", "name": "大田原市役所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "1丁目4-1", "postal_code": "3248641", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('3248765','{"jis": "09210", "kana": "オオタワラドボクジムシヨ", "name": "大田原土木事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2-2828-4", "postal_code": "3248765", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('3248765','{"jis": "09210", "kana": "オオタワラドボクジムシヨ", "name": "大田原土木事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2-2828-4", "postal_code": "3248765", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248625','{"jis": "09210", "kana": "カブシキガイシヤ トチギニコン", "name": "株式会社　栃木ニコン", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "実取", "banchi": "770", "postal_code": "3248625", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ミドリ", "alternates": []}');
 INSERT INTO office_data VALUES('3248520','{"jis": "09210", "kana": "カブシキガイシヤ トチギニコンプレシジヨン", "name": "株式会社　栃木ニコンプレシジョン", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "実取", "banchi": "760番地", "postal_code": "3248520", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ミドリ", "alternates": []}');
 INSERT INTO office_data VALUES('3248550','{"jis": "09210", "kana": "キヤノンデンシカンデバイス カブシキガイシヤ", "name": "キヤノン電子管デバイス　株式会社", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1385番地", "postal_code": "3248550", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": [{"jis": "09210", "kana": "キヤノンメデイカルシステムズ カブシキガイシヤ", "name": "キヤノンメディカルシステムズ　株式会社", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1385", "postal_code": "3248550", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": []}]}');
 INSERT INTO office_data VALUES('3248501','{"jis": "09210", "kana": "コクサイイリヨウフクシダイガク", "name": "国際医療福祉大学", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "北金丸", "banchi": "2600-1", "postal_code": "3248501", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "キタカネマル", "alternates": []}');
 INSERT INTO office_data VALUES('3248516','{"jis": "09210", "kana": "ダイニツポントリヨウ カブシキガイシヤ ナスコウジヨウ", "name": "大日本塗料　株式会社　那須工場", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1382-12", "postal_code": "3248516", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": []}');
-INSERT INTO office_data VALUES('3248585','{"jis": "09210", "kana": "トチギケンケンポクケンコウフクシセンタ-", "name": "栃木県県北健康福祉センター", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2丁目2828-4", "postal_code": "3248585", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('3248585','{"jis": "09210", "kana": "トチギケンケンポクケンコウフクシセンタ-", "name": "栃木県県北健康福祉センター", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2丁目2828-4", "postal_code": "3248585", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248686','{"jis": "09210", "kana": "ナスセキジユウジビヨウイン", "name": "那須赤十字病院", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "中田原", "banchi": "1081番地4(大田原郵便局私書箱第15号)", "postal_code": "3248686", "old_code": "324  ", "post_office": "大田原", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ナカダワラ", "alternates": []}');
 INSERT INTO office_data VALUES('3248540','{"jis": "09210", "kana": "ニツポンネンキンキコウ オオタワラネンキンジムシヨ", "name": "日本年金機構　大田原年金事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "1丁目2695-22", "postal_code": "3248540", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248555','{"jis": "09210", "kana": "フジツウ カブシキガイシヤ ナスコウジヨウ", "name": "富士通　株式会社　那須工場", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1388", "postal_code": "3248555", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": []}');
 INSERT INTO office_data VALUES('3248510','{"jis": "09210", "kana": "フジデンキ カブシキガイシヤ オオタワラコウジヨウ", "name": "富士電機　株式会社　大田原工場", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "中田原", "banchi": "1043", "postal_code": "3248510", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ナカダワラ", "alternates": []}');
 INSERT INTO office_data VALUES('3240292','{"jis": "09210", "kana": "オオタワラシヤクシヨ クロバネシシヨ", "name": "大田原市役所　黒羽支所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "黒羽田町", "banchi": "848", "postal_code": "3240292", "old_code": "32402", "post_office": "黒羽", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "クロバネタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3240293','{"jis": "09210", "kana": "クロバネケイムシヨ", "name": "黒羽刑務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "寒井", "banchi": "1466-2", "postal_code": "3240293", "old_code": "32402", "post_office": "黒羽", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "サブイ", "alternates": []}');
 INSERT INTO office_data VALUES('3240492','{"jis": "09210", "kana": "オオタワラシヤクシヨ ユヅカミチヨウシヤ", "name": "大田原市役所　湯津上庁舎", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "湯津上", "banchi": "5-1081", "postal_code": "3240492", "old_code": "32404", "post_office": "佐良土", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ユヅカミ", "alternates": []}');
@@ -123827,15 +123829,15 @@
 INSERT INTO office_data VALUES('3758604','{"jis": "10209", "kana": "グンマギンコウ", "name": "群馬銀行", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "391(藤岡郵便局私書箱第1号)", "postal_code": "3758604", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758503','{"jis": "10209", "kana": "コウリツ フジオカソウゴウビヨウイン", "name": "公立　藤岡総合病院", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "中栗須", "banchi": "813番地1", "postal_code": "3758503", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "ナカクリス", "alternates": []}');
 INSERT INTO office_data VALUES('3758603','{"jis": "10209", "kana": "タノシンヨウキンコ", "name": "多野信用金庫", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "314(藤岡郵便局私書箱第10号)", "postal_code": "3758603", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758602','{"jis": "10209", "kana": "フジオカ ゼイムシヨ", "name": "藤岡　税務署", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "668-1(藤岡郵便局私書箱第5号)", "postal_code": "3758602", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758504','{"jis": "10209", "kana": "フジオカコウコウ", "name": "藤岡高校", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "1485", "postal_code": "3758504", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758601','{"jis": "10209", "kana": "フジオカシヤクシヨ", "name": "藤岡市役所", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "中栗須", "banchi": "327(藤岡郵便局私書箱第9号)", "postal_code": "3758601", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "ナカクリス", "alternates": []}');
 INSERT INTO office_data VALUES('3758506','{"jis": "10209", "kana": "フジオカシヨウコウカイギシヨ", "name": "藤岡商工会議所", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "853-1", "postal_code": "3758506", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
-INSERT INTO office_data VALUES('3758507','{"jis": "10209", "kana": "ミサトコウギヨウ カブシキカイシヤ", "name": "美里工業　株式会社", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "1360", "postal_code": "3758507", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": true, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
+INSERT INTO office_data VALUES('3758507','{"jis": "10209", "kana": "ミサトコウギヨウ カブシキカイシヤ", "name": "美里工業　株式会社", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "1360", "postal_code": "3758507", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758501','{"jis": "10209", "kana": "ミツビシエンピツ カブシキガイシヤ グンマコウジヨウ", "name": "三菱鉛筆　株式会社　群馬工場", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "立石", "banchi": "1091", "postal_code": "3758501", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "タツイシ", "alternates": []}');
 INSERT INTO office_data VALUES('3758502','{"jis": "10209", "kana": "ヨシモトポ-ル カブシキガイシヤ", "name": "ヨシモトポール　株式会社", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "中栗須", "banchi": "508", "postal_code": "3758502", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "ナカクリス", "alternates": []}');
 INSERT INTO office_data VALUES('3702398','{"jis": "10210", "kana": "カブシキガイシヤ アイエイチアイエアロスペ-ス トミオカジギヨウシヨ", "name": "株式会社　ＩＨＩエアロスペース　富岡事業所", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "藤木", "banchi": "900番地", "postal_code": "3702398", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "フジキ", "alternates": []}');
 INSERT INTO office_data VALUES('3702396','{"jis": "10210", "kana": "カンラトミオカノウギヨウ キヨウドウクミアイ", "name": "甘楽富岡農業　協同組合", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "2638-1", "postal_code": "3702396", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3702393','{"jis": "10210", "kana": "コウリツトミオカソウゴウビヨウイン", "name": "公立富岡総合病院", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "2073-1", "postal_code": "3702393", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3702395','{"jis": "10210", "kana": "シノノメシンヨウキンコ", "name": "しののめ信用金庫", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "1123番地", "postal_code": "3702395", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3702392','{"jis": "10210", "kana": "トミオカシヤクシヨ", "name": "富岡市役所", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "1460-1", "postal_code": "3702392", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
@@ -124085,15 +124087,15 @@
 INSERT INTO office_data VALUES('3308522','{"jis": "11107", "kana": "サイタマケンシヤカイフクシジギヨウダン シヨウガイシヤコウリユウセンタ-", "name": "埼玉県社会福祉事業団　障害者交流センター", "prefecture": "埼玉県", "city": "さいたま市浦和区", "neighborhood": "大原", "banchi": "3丁目10-1", "postal_code": "3308522", "old_code": "338  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシウラワク", "neighborhood_kana": "オオハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3308532','{"jis": "11107", "kana": "サイタマシスイドウキヨク", "name": "さいたま市水道局", "prefecture": "埼玉県", "city": "さいたま市浦和区", "neighborhood": "常盤", "banchi": "6丁目14番16号", "postal_code": "3308532", "old_code": "338  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシウラワク", "neighborhood_kana": "トキワ", "alternates": []}');
 INSERT INTO office_data VALUES('3309850','{"jis": "11107", "kana": "タイヨウセイメイホケン ソウゴガイシヤ", "name": "太陽生命保険　相互会社", "prefecture": "埼玉県", "city": "さいたま市浦和区", "neighborhood": "針ヶ谷", "banchi": "4丁目2-18(さいたま新都心郵便局私書箱第50号)", "postal_code": "3309850", "old_code": "338  ", "post_office": "さいたま新都心", "type": "box", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシウラワク", "neighborhood_kana": "ハリガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('3309311','{"jis": "11107", "kana": "ニツシンカサイカイジヨウホケン カブシキガイシヤ", "name": "日新火災海上保険　株式会社", "prefecture": "埼玉県", "city": "さいたま市浦和区", "neighborhood": "上木崎", "banchi": "2丁目7-5", "postal_code": "3309311", "old_code": "338  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシウラワク", "neighborhood_kana": "カミキザキ", "alternates": []}');
 INSERT INTO office_data VALUES('3309666','{"jis": "11107", "kana": "リソナケツサイサ-ビス カブシキガイシヤ シユウキンダイコウブ", "name": "りそな決済サービス　株式会社　集金代行部", "prefecture": "埼玉県", "city": "さいたま市浦和区", "neighborhood": "針ヶ谷", "banchi": "4丁目2-11さくら浦和ビル", "postal_code": "3309666", "old_code": "338  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシウラワク", "neighborhood_kana": "ハリガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('3368564','{"jis": "11108", "kana": "カブシキガイシヤ カンデンコウ サイタマシテン", "name": "株式会社　関電工　埼玉支店", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "根岸", "banchi": "3丁目22-15", "postal_code": "3368564", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ネギシ", "alternates": []}');
 INSERT INTO office_data VALUES('3368636','{"jis": "11108", "kana": "カブシキガイシヤ コ-ケン", "name": "株式会社　コーケン", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "南本町", "banchi": "1丁目8-9(さいたま中央郵便局私書箱第152号)", "postal_code": "3368636", "old_code": "336  ", "post_office": "さいたま中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ミナミホンチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('3368526','{"jis": "11108", "kana": "コ-プデリセイカツキヨウドウクミアイレンゴウカイ", "name": "コープデリ生活協同組合連合会", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "根岸", "banchi": "1丁目4-13", "postal_code": "3368526", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ネギシ", "alternates": []}');
+INSERT INTO office_data VALUES('3368526','{"jis": "11108", "kana": "コ-プデリセイカツキヨウドウクミアイレンゴウカイ", "name": "コープデリ生活協同組合連合会", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "根岸", "banchi": "1丁目5番5号", "postal_code": "3368526", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ネギシ", "alternates": []}');
 INSERT INTO office_data VALUES('3368586','{"jis": "11108", "kana": "サイタマシミナミクヤクシヨ", "name": "さいたま市南区役所", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "別所", "banchi": "7丁目20番1号(さいたま中央郵便局私書箱第4号)", "postal_code": "3368586", "old_code": "336  ", "post_office": "さいたま中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ベッショ", "alternates": []}');
 INSERT INTO office_data VALUES('3368512','{"jis": "11108", "kana": "サイタマドケンイツパンロウドウクミアイ", "name": "埼玉土建一般労働組合", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "鹿手袋", "banchi": "6丁目18-12", "postal_code": "3368512", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "シカテブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('3368540','{"jis": "11108", "kana": "サイタマミツビシフソウジドウシヤハンバイ カブシキガイシヤ", "name": "埼玉三菱ふそう自動車販売　株式会社", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "根岸", "banchi": "5丁目23-15", "postal_code": "3368540", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ネギシ", "alternates": []}');
 INSERT INTO office_data VALUES('3368515','{"jis": "11108", "kana": "シヤダンホウジン サイタマケンセツサンギヨウダンタイレンゴウカイ", "name": "社団法人　埼玉建設産業団体連合会", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "鹿手袋", "banchi": "4丁目1-7", "postal_code": "3368515", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "シカテブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('3368523','{"jis": "11108", "kana": "セイカツキヨウドウクミアイ コ-プミライ", "name": "生活共同組合　コープみらい", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "根岸", "banchi": "1丁目5番5号", "postal_code": "3368523", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ネギシ", "alternates": []}');
 INSERT INTO office_data VALUES('3368508','{"jis": "11108", "kana": "ゼンコクセイカツキヨウドウクミアイレンゴウカイ", "name": "全国生活協同組合連合会", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "沼影", "banchi": "1丁目10-1", "postal_code": "3368508", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ヌマカゲ", "alternates": []}');
 INSERT INTO office_data VALUES('3368666','{"jis": "11108", "kana": "タカタセイヤク カブシキガイシヤ", "name": "高田製薬　株式会社", "prefecture": "埼玉県", "city": "さいたま市南区", "neighborhood": "沼影", "banchi": "1-11-1", "postal_code": "3368666", "old_code": "336  ", "post_office": "さいたま中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシミナミク", "neighborhood_kana": "ヌマカゲ", "alternates": []}');
@@ -124534,15 +124536,15 @@
 INSERT INTO office_data VALUES('3490292','{"jis": "11246", "kana": "シラオカシヤクシヨ", "name": "白岡市役所", "prefecture": "埼玉県", "city": "白岡市", "neighborhood": "千駄野", "banchi": "432番地", "postal_code": "3490292", "old_code": "34902", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "シラオカシ", "neighborhood_kana": "センダノ", "alternates": []}');
 INSERT INTO office_data VALUES('3490293','{"jis": "11246", "kana": "タイセイラミツク カブシキガイシヤ", "name": "大成ラミック　株式会社", "prefecture": "埼玉県", "city": "白岡市", "neighborhood": "下大崎", "banchi": "873", "postal_code": "3490293", "old_code": "34902", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "シラオカシ", "neighborhood_kana": "シモオオサキ", "alternates": []}');
 INSERT INTO office_data VALUES('3490294','{"jis": "11246", "kana": "ニツサンカガクコウギヨウ カブシキガイシヤ", "name": "日産化学工業　株式会社", "prefecture": "埼玉県", "city": "白岡市", "neighborhood": "白岡", "banchi": "1470", "postal_code": "3490294", "old_code": "34902", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "シラオカシ", "neighborhood_kana": "シラオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3628517','{"jis": "11301", "kana": "イナマチヤクバ", "name": "伊奈町役場", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小室", "banchi": "9493", "postal_code": "3628517", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628539','{"jis": "11301", "kana": "カブシキガイシヤ サイサン", "name": "株式会社　サイサン", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小室", "banchi": "字道上10360", "postal_code": "3628539", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628553','{"jis": "11301", "kana": "カブシキガイシヤ ニツポンアクセス イナチルドブツリユウセンタ-", "name": "株式会社　日本アクセス　伊奈チルド物流センター", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小針新宿", "banchi": "字梶川847番地", "postal_code": "3628553", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628542','{"jis": "11301", "kana": "カブシキガイシヤ ニツポンアクセス サイタマシテン", "name": "株式会社　日本アクセス　埼玉支店", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小針新宿", "banchi": "字梶川833番地", "postal_code": "3628542", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3628577','{"jis": "11301", "kana": "デイ-アイシ- カブシキガイシヤ サイタマコウジヨウ", "name": "ＤＩＣ　株式会社　埼玉工場", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "小室", "banchi": "4472-1", "postal_code": "3628577", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "キタアダチグンイナマチ", "neighborhood_kana": "コムロ", "alternates": []}');
+INSERT INTO office_data VALUES('3628577','{"jis": "11301", "kana": "デイ-アイシ- カブシキガイシヤ サイタマコウジヨウ", "name": "ＤＩＣ　株式会社　埼玉工場", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "小室", "banchi": "4472-1", "postal_code": "3628577", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "キタアダチグンイナマチ", "neighborhood_kana": "コムロ", "alternates": []}');
 INSERT INTO office_data VALUES('3548565','{"jis": "11324", "kana": "アスクル ロジ パ-ク シユトケン", "name": "ＡＳＫＵＬ　Ｌｏｇｉ　ＰＡＲＫ　首都圏", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "上富", "banchi": "1163", "postal_code": "3548565", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "イルマグンミヨシマチ", "neighborhood_kana": "カミトメ", "alternates": []}');
 INSERT INTO office_data VALUES('3548501','{"jis": "11324", "kana": "オオサキデンキ カブシキガイシヤ サイタマジギヨウシヨ", "name": "大崎電気　株式会社　埼玉事業所", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字藤久保", "banchi": "1131", "postal_code": "3548501", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3548504','{"jis": "11324", "kana": "カブシキガイシヤ ガツケンロジステイクス", "name": "（株）　学研ロジスティクス", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字上富", "banchi": "279-1", "postal_code": "3548504", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3548505','{"jis": "11324", "kana": "カブシキガイシヤ シユフノトモシヤ", "name": "株式会社　主婦の友社", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "みよし台", "banchi": "13-10", "postal_code": "3548505", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "イルマグンミヨシマチ", "neighborhood_kana": "ミヨシダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3548577','{"jis": "11324", "kana": "カブシキガイシヤ テイ-アンドケイトオカ", "name": "株式会社　Ｔ＆Ｋ　ＴＯＫＡ", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字竹間沢", "banchi": "283-1", "postal_code": "3548577", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3548533','{"jis": "11324", "kana": "カブシキガイシヤシユフノトモシヤ ツウハンジギヨウブ", "name": "株式会社主婦の友社　通販事業部", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "竹間沢東", "banchi": "7番地5", "postal_code": "3548533", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "イルマグンミヨシマチ", "neighborhood_kana": "チクマザワヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3548510','{"jis": "11324", "kana": "シユクトクダイガク コクサイコミユニケ-シヨンガクブ", "name": "淑徳大学　国際コミュニケーション学部", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字藤久保", "banchi": "1150-1", "postal_code": "3548510", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -124585,14 +124587,15 @@
 INSERT INTO office_data VALUES('3680292','{"jis": "11365", "kana": "オガノマチヤクバ リヨウカミチヨウシヤ", "name": "小鹿野町役場　両神庁舎", "prefecture": "埼玉県", "city": "秩父郡小鹿野町", "neighborhood": "両神薄", "banchi": "2906", "postal_code": "3680292", "old_code": "36802", "post_office": "両神", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "チチブグンオガノマチ", "neighborhood_kana": "リョウカミススキ", "alternates": []}');
 INSERT INTO office_data VALUES('3670198','{"jis": "11381", "kana": "エ-ザイ カブシキガイシヤ ミサトコウジヨウ", "name": "エーザイ　株式会社　美里工場", "prefecture": "埼玉県", "city": "児玉郡美里町", "neighborhood": "大字広木", "banchi": "950", "postal_code": "3670198", "old_code": "36701", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": [{"jis": "11381", "kana": "ブシユウセイヤク カブシキガイシヤ ミサトコウジヨウ", "name": "武州製薬　株式会社　美里工場", "prefecture": "埼玉県", "city": "児玉郡美里町", "neighborhood": "大字広木", "banchi": "950", "postal_code": "3670198", "old_code": "36701", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}]}');
 INSERT INTO office_data VALUES('3670192','{"jis": "11381", "kana": "キヤノンデンシ カブシキガイシヤ ミサトコウジヨウ", "name": "キヤノン電子　株式会社　美里工場", "prefecture": "埼玉県", "city": "児玉郡美里町", "neighborhood": "大字甘粕", "banchi": "1611", "postal_code": "3670192", "old_code": "36701", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3670194','{"jis": "11381", "kana": "ミサトマチヤクバ", "name": "美里町役場", "prefecture": "埼玉県", "city": "児玉郡美里町", "neighborhood": "大字木部", "banchi": "323-1", "postal_code": "3670194", "old_code": "36701", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3670292','{"jis": "11383", "kana": "カミカワマチヤクバ", "name": "神川町役場", "prefecture": "埼玉県", "city": "児玉郡神川町", "neighborhood": "大字植竹", "banchi": "909", "postal_code": "3670292", "old_code": "36702", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3670297','{"jis": "11383", "kana": "サイタマニツポンデンキ カブシキガイシヤ", "name": "埼玉日本電気　株式会社", "prefecture": "埼玉県", "city": "児玉郡神川町", "neighborhood": "大字元原", "banchi": "300-18", "postal_code": "3670297", "old_code": "36702", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3670296','{"jis": "11383", "kana": "タイホウヤクヒンコウギヨウ カブシキガイシヤ コダマソウコ", "name": "大鵬薬品工業　株式会社　児玉倉庫", "prefecture": "埼玉県", "city": "児玉郡神川町", "neighborhood": "大字元原", "banchi": "200-22", "postal_code": "3670296", "old_code": "36702", "post_office": "児玉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('3670393','{"jis": "11383", "kana": "カミカワマチカミイズミソウゴウシシヨ", "name": "神川町神泉総合支所", "prefecture": "埼玉県", "city": "児玉郡神川町", "neighborhood": "大字下阿久原", "banchi": "1088", "postal_code": "3670393", "old_code": "36703", "post_office": "児玉", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3690395','{"jis": "11385", "kana": "カブシキカイシヤ ヒタチハイテクフアインシステムズ", "name": "株式会社　日立ハイテクファインシステムズ", "prefecture": "埼玉県", "city": "児玉郡上里町", "neighborhood": "嘉美", "banchi": "1600番地", "postal_code": "3690395", "old_code": "36903", "post_office": "上里", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "コダマグンカミサトマチ", "neighborhood_kana": "カミ", "alternates": []}');
 INSERT INTO office_data VALUES('3690392','{"jis": "11385", "kana": "カミサトマチヤクバ", "name": "上里町役場", "prefecture": "埼玉県", "city": "児玉郡上里町", "neighborhood": "大字七本木", "banchi": "982", "postal_code": "3690392", "old_code": "36903", "post_office": "上里", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3690393','{"jis": "11385", "kana": "キヤノン・コンポ-ネンツ カブシキガイシヤ", "name": "キヤノン・コンポーネンツ　株式会社", "prefecture": "埼玉県", "city": "児玉郡上里町", "neighborhood": "大字七本木", "banchi": "3461-1", "postal_code": "3690393", "old_code": "36903", "post_office": "上里", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3691298','{"jis": "11408", "kana": "カブシキガイシヤ ベルク", "name": "株式会社　ベルク", "prefecture": "埼玉県", "city": "大里郡寄居町", "neighborhood": "大字用土", "banchi": "5456", "postal_code": "3691298", "old_code": "36912", "post_office": "寄居", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3691292','{"jis": "11408", "kana": "ヨリイマチヤクバ", "name": "寄居町役場", "prefecture": "埼玉県", "city": "大里郡寄居町", "neighborhood": "大字寄居", "banchi": "1180-1", "postal_code": "3691292", "old_code": "36912", "post_office": "寄居", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3458501','{"jis": "11442", "kana": "ニツポンコウギヨウダイガク", "name": "日本工業大学", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "学園台", "banchi": "4丁目1", "postal_code": "3458501", "old_code": "345  ", "post_office": "杉戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ガクエンダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3458504','{"jis": "11442", "kana": "ミヤシロマチヤクバ", "name": "宮代町役場", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "笠原", "banchi": "1丁目4-1", "postal_code": "3458504", "old_code": "345  ", "post_office": "杉戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "カサハラ", "alternates": []}');
@@ -124633,15 +124636,15 @@
 INSERT INTO office_data VALUES('2608566','{"jis": "12101", "kana": "コウエキシヤダンホウジン チバケンボウハンキヨウカイ", "name": "公益社団法人　千葉県防犯協会", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "中央", "banchi": "4丁目13番10号千葉県教育会館別館4階", "postal_code": "2608566", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608619','{"jis": "12101", "kana": "コウリツガツコウキヨウサイクミアイ チバシブ", "name": "公立学校共済組合　千葉支部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "市場町", "banchi": "1-1", "postal_code": "2608619", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "イチバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608534','{"jis": "12101", "kana": "コバヤシシヨウジ カブシキガイシヤ", "name": "小林商事　株式会社", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "問屋町", "banchi": "14-2", "postal_code": "2608534", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "トンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608559','{"jis": "12101", "kana": "サンケイリビングシンブンシヤ チバホンブ", "name": "サンケイリビング新聞社　千葉本部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "新町", "banchi": "3-13千葉TNビル5F", "postal_code": "2608559", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "シンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('2608629','{"jis": "12101", "kana": "ザイダンホウジン チバケンコウリツガツコウキヨウシヨクインゴジヨカイ", "name": "財団法人　千葉県公立学校教職員互助会", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "市場町", "banchi": "1番1号", "postal_code": "2608629", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "イチバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608562','{"jis": "12101", "kana": "ザイダンホウジン ニホンボウサイツウシンキヨウカイ チバケンシブ", "name": "財団法人　日本防災通信協会　千葉県支部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "都町", "banchi": "1丁目1-30千葉県警都町庁舎内", "postal_code": "2608562", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ミヤコチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608607','{"jis": "12101", "kana": "ザイムシヨウ カントウザイムキヨク チバザイムジムシヨ", "name": "財務省　関東財務局　千葉財務事務所", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "椿森", "banchi": "5丁目6-1", "postal_code": "2608607", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ツバキモリ", "alternates": []}');
-INSERT INTO office_data VALUES('2608508','{"jis": "12101", "kana": "シヤカイフクシホウジン チバケンシヤカイフクシキヨウギカイ", "name": "社会福祉法人　千葉県社会福祉協議会", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "千葉港", "banchi": "4-3", "postal_code": "2608508", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "チバミナト", "alternates": []}');
+INSERT INTO office_data VALUES('2608508','{"jis": "12101", "kana": "シヤカイフクシホウジン チバケンシヤカイフクシキヨウギカイ", "name": "社会福祉法人　千葉県社会福祉協議会", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "千葉港", "banchi": "4-5", "postal_code": "2608508", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "チバミナト", "alternates": []}');
 INSERT INTO office_data VALUES('2608521','{"jis": "12101", "kana": "シヤカイホケンシンリヨウホウシユウシハライキキン チバシブ", "name": "社会保険診療報酬支払基金　千葉支部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "問屋町", "banchi": "2-1", "postal_code": "2608521", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "トンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608703','{"jis": "12101", "kana": "シユクトクダイガク カンゴエイヨウガクブ", "name": "淑徳大学　看護栄養学部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "仁戸名町", "banchi": "673", "postal_code": "2608703", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ニトナチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608701','{"jis": "12101", "kana": "シユクトクダイガク チバキヤンパス", "name": "淑徳大学　千葉キャンパス", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "大巌寺町", "banchi": "200", "postal_code": "2608701", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ダイガンジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608621','{"jis": "12101", "kana": "スミトモセイメイホケン ソウゴガイシヤ チバシシヤ", "name": "住友生命保険　相互会社　千葉支社", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "中央", "banchi": "1丁目1番3号住友・りそな千葉ビル6F", "postal_code": "2608621", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608645','{"jis": "12101", "kana": "ゼンコクケンコウホケンキヨウカイ チバシブ", "name": "全国健康保険協会　千葉支部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "新町", "banchi": "3番地13日本生命千葉駅前ビル", "postal_code": "2608645", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "シンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('2608512','{"jis": "12101", "kana": "ゼンロウサイ チバケンホンブ", "name": "全労済　千葉県本部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "弁天", "banchi": "1丁目17-1", "postal_code": "2608512", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ベンテン", "alternates": []}');
 INSERT INTO office_data VALUES('2608560','{"jis": "12101", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "弁天", "banchi": "1-15-3リードシー千葉駅前ビル", "postal_code": "2608560", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ベンテン", "alternates": []}');
@@ -124993,15 +124996,15 @@
 INSERT INTO office_data VALUES('2758575','{"jis": "12216", "kana": "ニホンダイガク セイサンコウガクブ", "name": "日本大学　生産工学部", "prefecture": "千葉県", "city": "習志野市", "neighborhood": "泉町", "banchi": "1丁目2-1", "postal_code": "2758575", "old_code": "275  ", "post_office": "習志野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ナラシノシ", "neighborhood_kana": "イズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2758576','{"jis": "12216", "kana": "ニホンダイガク セイサンコウガクブ ミモミコウシヤ", "name": "日本大学　生産工学部　実籾校舎", "prefecture": "千葉県", "city": "習志野市", "neighborhood": "新栄", "banchi": "2丁目11-1", "postal_code": "2758576", "old_code": "275  ", "post_office": "習志野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ナラシノシ", "neighborhood_kana": "シンエイ", "alternates": []}');
 INSERT INTO office_data VALUES('2778571','{"jis": "12217", "kana": "アマゾンジヤパン ブイジエイエヌエ-", "name": "アマゾンジャパン　ＶＪＮＡ", "prefecture": "千葉県", "city": "柏市", "neighborhood": "藤ケ谷", "banchi": "1823ナカノ商会柏沼南物流センター内", "postal_code": "2778571", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "フジガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2778586','{"jis": "12217", "kana": "イトウハム カブシキガイシヤ トウキヨウコウジヨウ", "name": "伊藤ハム　株式会社　東京工場", "prefecture": "千葉県", "city": "柏市", "neighborhood": "根戸", "banchi": "1-3", "postal_code": "2778586", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "ネド", "alternates": []}');
 INSERT INTO office_data VALUES('2778572','{"jis": "12217", "kana": "エデイオンカシワイ-シ-・テイ-シ-ダイイチ", "name": "エディオン柏ＥＣ・ＴＣ第一", "prefecture": "千葉県", "city": "柏市", "neighborhood": "新十余二", "banchi": "13-1SGリアルティ柏B棟2F", "postal_code": "2778572", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "シントヨフタ", "alternates": []}');
 INSERT INTO office_data VALUES('2778573','{"jis": "12217", "kana": "エデイオンカシワイ-シ-・テイ-シ-ダイニ", "name": "エディオン柏ＥＣ・ＴＣ第二", "prefecture": "千葉県", "city": "柏市", "neighborhood": "新十余二", "banchi": "13-1SGリアルティ柏A棟5F", "postal_code": "2778573", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "シントヨフタ", "alternates": []}');
 INSERT INTO office_data VALUES('2778554','{"jis": "12217", "kana": "カシワケイサツシヨ", "name": "柏警察署", "prefecture": "千葉県", "city": "柏市", "neighborhood": "松ケ崎", "banchi": "722-1", "postal_code": "2778554", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "マツガサキ", "alternates": []}');
-INSERT INTO office_data VALUES('2778551','{"jis": "12217", "kana": "カシワコウセイソウゴウビヨウイン", "name": "柏厚生総合病院", "prefecture": "千葉県", "city": "柏市", "neighborhood": "あけぼの", "banchi": "3丁目8-20", "postal_code": "2778551", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "アケボノ", "alternates": []}');
+INSERT INTO office_data VALUES('2778551','{"jis": "12217", "kana": "カシワコウセイソウゴウビヨウイン", "name": "柏厚生総合病院", "prefecture": "千葉県", "city": "柏市", "neighborhood": "篠籠田", "banchi": "617番地", "postal_code": "2778551", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "シコダ", "alternates": []}');
 INSERT INTO office_data VALUES('2778503','{"jis": "12217", "kana": "カシワシ シヨウナンチヨウシヤ", "name": "柏市沼南庁舎", "prefecture": "千葉県", "city": "柏市", "neighborhood": "大島田", "banchi": "48-1", "postal_code": "2778503", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "オオシマタ", "alternates": []}');
 INSERT INTO office_data VALUES('2778505','{"jis": "12217", "kana": "カシワシヤクシヨ", "name": "柏市役所", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏", "banchi": "5丁目10-1", "postal_code": "2778505", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワ", "alternates": []}');
 INSERT INTO office_data VALUES('2778522','{"jis": "12217", "kana": "カシワゼイムシヨ", "name": "柏税務署", "prefecture": "千葉県", "city": "柏市", "neighborhood": "あけぼの", "banchi": "2丁目1-30", "postal_code": "2778522", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "アケボノ", "alternates": []}');
 INSERT INTO office_data VALUES('2778550','{"jis": "12217", "kana": "カシワタカシマヤステ-シヨンモ-ル", "name": "柏高島屋ステーションモール", "prefecture": "千葉県", "city": "柏市", "neighborhood": "末広町", "banchi": "1-1", "postal_code": "2778550", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "スエヒロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2778521','{"jis": "12217", "kana": "カブシキガイシヤ ソゴウ カシワテン", "name": "株式会社　そごう　柏店", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏", "banchi": "1丁目1-21", "postal_code": "2778521", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワ", "alternates": []}');
 INSERT INTO office_data VALUES('2778666','{"jis": "12217", "kana": "カブシキガイシヤ タカシマヤ カシワテン", "name": "株式会社　高島屋　柏店", "prefecture": "千葉県", "city": "柏市", "neighborhood": "末広町", "banchi": "3-16", "postal_code": "2778666", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "スエヒロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2778531','{"jis": "12217", "kana": "カブシキガイシヤ デイ-エヌピ-テクノフイルム", "name": "株式会社　ＤＮＰテクノフィルム", "prefecture": "千葉県", "city": "柏市", "neighborhood": "十余二", "banchi": "赤坂台409", "postal_code": "2778531", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "トヨフタ", "alternates": []}');
@@ -125027,15 +125030,17 @@
 INSERT INTO office_data VALUES('2778582','{"jis": "12217", "kana": "トウキヨウダイガク ウチユウセンケンキユウジヨ", "name": "東京大学　宇宙線研究所", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5丁目1-5", "postal_code": "2778582", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778569','{"jis": "12217", "kana": "トウキヨウダイガク カシワキヤンパス セツビセンタ-", "name": "東京大学　柏キャンパス　設備センター", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778569", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778589','{"jis": "12217", "kana": "トウキヨウダイガク カシワチクダイニソウゴウケンキユウトウ", "name": "東京大学　柏地区第２総合研究棟", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5丁目1番5号", "postal_code": "2778589", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778584','{"jis": "12217", "kana": "トウキヨウダイガク カシワトシヨカン", "name": "東京大学　柏図書館", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778584", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778574','{"jis": "12217", "kana": "トウキヨウダイガク セイサンギジユツケンキユウジヨ チバジツケンジヨ", "name": "東京大学　生産技術研究所　千葉実験所", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778574", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778564','{"jis": "12217", "kana": "トウキヨウダイガク タイキカイヨウケンキユウシヨ", "name": "東京大学　大気海洋研究所", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778564", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778581','{"jis": "12217", "kana": "トウキヨウダイガク ブツセイケンキユウジヨ", "name": "東京大学　物性研究所", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5丁目1-5", "postal_code": "2778581", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
-INSERT INTO office_data VALUES('2778561','{"jis": "12217", "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカ", "name": "東京大学大学院　新領域創成科学研究科", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5丁目1番5号", "postal_code": "2778561", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
+INSERT INTO office_data VALUES('2778563','{"jis": "12217", "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカカンキヨウトウ", "name": "東京大学大学院　新領域創成科学研究科環境棟", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778563", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
+INSERT INTO office_data VALUES('2778561','{"jis": "12217", "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカキバントウ", "name": "東京大学大学院　新領域創成科学研究科基盤棟", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778561", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
+INSERT INTO office_data VALUES('2778562','{"jis": "12217", "kana": "トウキヨウダイガクダイガクイン シンリヨウイキソウセイカガクケンキユウカセイメイトウ", "name": "東京大学大学院　新領域創成科学研究科生命棟", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778562", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778587','{"jis": "12217", "kana": "ドクリツギヨウセイホウジン ニホンゲンシリヨクケンキユウカイハツキコウ システムケイサンカガクセンタ-", "name": "独立行政法人　日本原子力研究開発機構　システム計算科学センター", "prefecture": "千葉県", "city": "柏市", "neighborhood": "柏の葉", "banchi": "5-1-5", "postal_code": "2778587", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "カシワノハ", "alternates": []}');
 INSERT INTO office_data VALUES('2778585','{"jis": "12217", "kana": "ニシヨウガクシヤダイガク", "name": "二松学舎大学", "prefecture": "千葉県", "city": "柏市", "neighborhood": "大井", "banchi": "2590", "postal_code": "2778585", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "オオイ", "alternates": []}');
 INSERT INTO office_data VALUES('2778557','{"jis": "12217", "kana": "パウダ-テツク カブシキガイシヤ", "name": "パウダーテック　株式会社", "prefecture": "千葉県", "city": "柏市", "neighborhood": "十余二", "banchi": "217", "postal_code": "2778557", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "トヨフタ", "alternates": []}');
 INSERT INTO office_data VALUES('2778655','{"jis": "12217", "kana": "ミツイセイメイホケン カブシキガイシヤ ジムセンタ-", "name": "三井生命保険　株式会社　事務センター", "prefecture": "千葉県", "city": "柏市", "neighborhood": "東上町", "banchi": "8-18(柏郵便局私書箱第33号)", "postal_code": "2778655", "old_code": "277  ", "post_office": "柏", "type": "box", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "アズマカミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2778566','{"jis": "12217", "kana": "ヨミウリリヨコウ カシワエイギヨウシヨ", "name": "読売旅行　柏営業所", "prefecture": "千葉県", "city": "柏市", "neighborhood": "末広町", "banchi": "5-19第12関口ビル2F", "postal_code": "2778566", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "スエヒロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2778518','{"jis": "12217", "kana": "ララポ-ト カシワノハ", "name": "ららぽーと　柏の葉", "prefecture": "千葉県", "city": "柏市", "neighborhood": "若柴", "banchi": "175", "postal_code": "2778518", "old_code": "277  ", "post_office": "柏", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カシワシ", "neighborhood_kana": "ワカシバ", "alternates": []}');
 INSERT INTO office_data VALUES('2995292','{"jis": "12218", "kana": "カツウラシヤクシヨ", "name": "勝浦市役所", "prefecture": "千葉県", "city": "勝浦市", "neighborhood": "新官", "banchi": "1343-1", "postal_code": "2995292", "old_code": "29952", "post_office": "勝浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カツウラシ", "neighborhood_kana": "シンカン", "alternates": []}');
@@ -125477,253 +125482,181 @@
 INSERT INTO office_data VALUES('1006051','{"jis": "13101", "kana": "カブシキガイシヤ ジエイテイ-ビ-ホウジントウキヨウ カスミガセキエイギヨウブ", "name": "株式会社　ＪＴＢ法人東京　霞が関営業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "3-2-5霞が関ビル23階", "postal_code": "1006051", "old_code": "10060", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1006162','{"jis": "13101", "kana": "デイ・エグゼクテイブ・センタ-・ジヤパン カブシキガイシヤ", "name": "ディ・エグゼクティブ・センター・ジャパン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "永田町", "banchi": "2-11-1山王パークタワー3階", "postal_code": "1006162", "old_code": "10061", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ナガタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008077','{"jis": "13101", "kana": "カブシキガイシヤ サンギヨウケイザイシンブンシヤ", "name": "株式会社　産業経済新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目7-2", "postal_code": "1008077", "old_code": "10077", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008078','{"jis": "13101", "kana": "カブシキガイシヤ サンギヨウケイザイシンブンシヤ", "name": "株式会社　産業経済新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目7-2", "postal_code": "1008078", "old_code": "10077", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008079','{"jis": "13101", "kana": "カブシキガイシヤ サンギヨウケイザイシンブンシヤ", "name": "株式会社　産業経済新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目7-2", "postal_code": "1008079", "old_code": "10077", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008086','{"jis": "13101", "kana": "ミツビシシヨウジ カブシキガイシヤ", "name": "三菱商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2丁目3-1", "postal_code": "1008086", "old_code": "10086", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018480','{"jis": "13101", "kana": "アサヒカセイアミダス カブシキガイシヤ", "name": "旭化成アミダス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目22番地", "postal_code": "1018480", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018481','{"jis": "13101", "kana": "アサヒカセイフア-マ カブシキガイシヤ", "name": "旭化成ファーマ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "9番地1MD神田ビル", "postal_code": "1018481", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018101','{"jis": "13101", "kana": "アサヒカセイホ-ムズ カブシキガイシヤ", "name": "旭化成ホームズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "1丁目105番地神保町三井ビルディング", "postal_code": "1018101", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018318','{"jis": "13101", "kana": "アデカクリ-ンエイド カブシキガイシヤ", "name": "ＡＤＥＫＡクリーンエイド　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2-5-12NMF駿河台ビル2階", "postal_code": "1018318", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018604','{"jis": "13101", "kana": "アルフアサイケンカイシユウ カブシキガイシヤ", "name": "アルファ債権回収　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目12番8号住友不動産秋葉原ビル17階", "postal_code": "1018604", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018512','{"jis": "13101", "kana": "アルフレツサ カブシキガイシヤ", "name": "アルフレッサ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7番地住友不動産神田ビル13F", "postal_code": "1018512", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018445','{"jis": "13101", "kana": "イオンクレジツトサ-ビス", "name": "イオンクレジットサービス　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目1", "postal_code": "1018445", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1018333','{"jis": "13101", "kana": "イツパンザイダンホウジン サンギヨウケイリキヨウカイ", "name": "一般財団法人　産業経理協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "1丁目15-6", "postal_code": "1018333", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018986','{"jis": "13101", "kana": "イツパンザイダンホウジン ニホンケンチクセンタ-", "name": "一般財団法人　日本建築センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1-9東京天理ビル", "postal_code": "1018986", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018555','{"jis": "13101", "kana": "イツパンザイダンホウジン ニホンヒンシツホシヨウキコウ", "name": "一般財団法人　日本品質保証機構", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目25番", "postal_code": "1018555", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1018459','{"jis": "13101", "kana": "イツパンシヤダンホウジン ガクシカイ", "name": "一般社団法人　学士会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目28", "postal_code": "1018459", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018534','{"jis": "13101", "kana": "イツパンシヤダンホウジン ゼンコクシンヨウホシヨウキヨウカイレンゴウカイ", "name": "一般社団法人　全国信用保証協会連合会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目1オーク神田ビル内", "postal_code": "1018534", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1018509','{"jis": "13101", "kana": "イツパンシヤダンホウジン ゼンコクチホウギンコウキヨウカイ", "name": "一般社団法人　全国地方銀行協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3丁目1-2", "postal_code": "1018509", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018611','{"jis": "13101", "kana": "イツパンシヤダンホウジン トウキヨウトコウユウカイ", "name": "一般社団法人　東京都交友会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2-11-1駿河台サンライズビル2F", "postal_code": "1018611", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018362','{"jis": "13101", "kana": "エヌイ-シ-ト-キン (カブ)", "name": "ＮＥＣトーキン　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目8-1", "postal_code": "1018362", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018532','{"jis": "13101", "kana": "エヌイ-シ-プラツトフオ-ムズ カブシキガイシヤ", "name": "ＮＥＣプラットフォームズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目3番地", "postal_code": "1018532", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018347','{"jis": "13101", "kana": "エヌテイテイコムソリユ-シヨンズ カブシキガイシヤ", "name": "ＮＴＴコムソリューションズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "1丁目5番15号", "postal_code": "1018347", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018535','{"jis": "13101", "kana": "オオツカセイヤク カブシキガイシヤ", "name": "大塚製薬　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目9", "postal_code": "1018535", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018353','{"jis": "13101", "kana": "オオハラホウリツセンモンガツコウ", "name": "大原法律専門学校", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "2丁目5-4", "postal_code": "1018353", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018352','{"jis": "13101", "kana": "オオハラボキガツコウ", "name": "大原簿記学校", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "1丁目3-6-8F", "postal_code": "1018352", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018228','{"jis": "13101", "kana": "オオバヤシドウロ カブシキガイシヤ", "name": "大林道路　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "2丁目8番8号住友不動産猿楽町ビル16階", "postal_code": "1018228", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018504','{"jis": "13101", "kana": "オザツクス カブシキカイシヤ", "name": "オザックス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田三崎町", "banchi": "3-1-16神保町北東急ビル", "postal_code": "1018504", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018586','{"jis": "13101", "kana": "カイジルシ カブシキガイシヤ", "name": "貝印　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "3丁目9-5", "postal_code": "1018586", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018627','{"jis": "13101", "kana": "カガデンシ カブシキガイシヤ カンキヨウジギヨウブ、ギジユツトウカツブ ホカ", "name": "加賀電子　株式会社　環境事業部、技術統括部　他", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田松永町", "banchi": "19-2-5F", "postal_code": "1018627", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダマツナガチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018629','{"jis": "13101", "kana": "カガデンシ カブシキガイシヤ カンリホンブ、ヒシヨ・コウホウシツ", "name": "加賀電子　株式会社　管理本部、秘書・広報室", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田松永町", "banchi": "19-2-10F", "postal_code": "1018629", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダマツナガチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018628','{"jis": "13101", "kana": "カガデンシ カブシキガイシヤ デンシジギヨウブ、エイギヨウスイシンジギヨウブ、トクハンジギヨウブ", "name": "加賀電子　株式会社　電子事業部、営業推進事業部、特販事業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田松永町", "banchi": "19-2-8F", "postal_code": "1018628", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダマツナガチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018543','{"jis": "13101", "kana": "カシムラ", "name": "（株）　樫村", "prefecture": "東京都", "city": "千代田区", "neighborhood": "鍛冶町", "banchi": "1丁目6-14", "postal_code": "1018543", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018526','{"jis": "13101", "kana": "カブ アクテイブ", "name": "（株）　アクティブ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目16-11内神田渋谷ビル4F", "postal_code": "1018526", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018449','{"jis": "13101", "kana": "カブシキガイシヤ アイシ-エスコンベンシヨンデザイン", "name": "株式会社　ＩＣＳコンベンションデザイン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "1丁目5-18千代田ビル", "postal_code": "1018449", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('1018629','{"jis": "13101", "kana": "カガデンシ カブシキガイシヤ カンリホンブ、ヒシヨ・コウホウシツ", "name": "加賀電子　株式会社　管理本部、秘書・広報室", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田松永町", "banchi": "20-10F", "postal_code": "1018629", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダマツナガチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1018627','{"jis": "13101", "kana": "カガデンシ カブシキガイシヤ ギジユツトウカツブ", "name": "加賀電子　株式会社　技術統括部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田松永町", "banchi": "20-5F", "postal_code": "1018627", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダマツナガチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1018628','{"jis": "13101", "kana": "カガデンシ カブシキガイシヤ デンシジギヨウブ、ツウシンジギヨウブ、オ-トモ-テイブジギヨウブ", "name": "加賀電子　株式会社　電子事業部、通信事業部、オートモーティブ事業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田松永町", "banchi": "20-8F", "postal_code": "1018628", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダマツナガチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018973','{"jis": "13101", "kana": "カブシキガイシヤ アクセル", "name": "株式会社　アクセル", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDX", "postal_code": "1018973", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018355','{"jis": "13101", "kana": "カブシキガイシヤ アサヒシユツパンシヤ", "name": "株式会社　朝日出版社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目3-5", "postal_code": "1018355", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018202','{"jis": "13101", "kana": "カブシキガイシヤ アスクレツプ", "name": "株式会社　アスクレップ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田練塀町", "banchi": "3番地インテージ秋葉原ビル", "postal_code": "1018202", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダネリベイチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018615','{"jis": "13101", "kana": "カブシキガイシヤ アプラス", "name": "株式会社　アプラス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3-12-8住友不動産秋葉原ビル", "postal_code": "1018615", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018469','{"jis": "13101", "kana": "カブシキガイシヤ アンビツト ニンドリヘンシユウブ", "name": "株式会社　アンビット　ニンドリ編集部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目6共同ビル(錦町3丁目)201", "postal_code": "1018469", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018558','{"jis": "13101", "kana": "カブシキガイシヤ イワキ", "name": "株式会社　イワキ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "2丁目6-6", "postal_code": "1018558", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018201','{"jis": "13101", "kana": "カブシキガイシヤ インテ-ジ", "name": "株式会社　インテージ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田練塀町", "banchi": "3番地インテージ秋葉原ビル", "postal_code": "1018201", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダネリベイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018204','{"jis": "13101", "kana": "カブシキガイシヤ インテ-ジ・アソシエイツ", "name": "株式会社　インテージ・アソシエイツ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田練塀町", "banchi": "3インテージ秋葉原ビル", "postal_code": "1018204", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダネリベイチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018467','{"jis": "13101", "kana": "カブシキガイシヤ エス・エス・コミユニケ-シヨンズ", "name": "株式会社　エス・エス・コミュニケーションズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目18-3錦三ビル7階", "postal_code": "1018467", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018517','{"jis": "13101", "kana": "カブシキガイシヤ エルエスアイメデイエンス", "name": "株式会社　ＬＳＩメディエンス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目13番4号", "postal_code": "1018517", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018460','{"jis": "13101", "kana": "カブシキガイシヤ オ-ムシヤ", "name": "株式会社　オーム社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目1", "postal_code": "1018460", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018461','{"jis": "13101", "kana": "カブシキガイシヤ オオゾラシユツパン", "name": "株式会社　宙出版", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目17番地廣瀬第1ビル", "postal_code": "1018461", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018624','{"jis": "13101", "kana": "カブシキガイシヤ カンソウシン", "name": "株式会社　かんそうしん", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "2丁目18-10", "postal_code": "1018624", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018476','{"jis": "13101", "kana": "カブシキガイシヤ キツズステ-シヨン", "name": "（株）　キッズステーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目26一ツ橋SIビル10階", "postal_code": "1018476", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018589','{"jis": "13101", "kana": "カブシキガイシヤ キヨクトウシヨウカイ/カブシキガイシヤ カパス", "name": "株式会社　極東商会／株式会社　カパス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-10-6", "postal_code": "1018589", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018672','{"jis": "13101", "kana": "カブシキガイシヤ キヨクトウシヨテン", "name": "株式会社　極東書店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2-7-10帝都三崎町ビル(神田郵便局私書箱第72号)", "postal_code": "1018672", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('1018560','{"jis": "13101", "kana": "カブシキガイシヤ キンダイエイガシヤ", "name": "株式会社　近代映画社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "2-12-14晴花ビル4F", "postal_code": "1018560", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1018316','{"jis": "13101", "kana": "カブシキガイシヤ コウノイケグミ トウキヨウホンテン", "name": "株式会社　鴻池組　東京本店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目3-11", "postal_code": "1018316", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018568','{"jis": "13101", "kana": "カブシキガイシヤ コクゴ", "name": "株式会社　コクゴ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "25", "postal_code": "1018568", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018371','{"jis": "13101", "kana": "カブシキガイシヤ サンセイドウ", "name": "株式会社　三省堂", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目22-14", "postal_code": "1018371", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018410','{"jis": "13101", "kana": "カブシキガイシヤ シノテスト", "name": "株式会社　シノテスト", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3-7-9", "postal_code": "1018410", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018448','{"jis": "13101", "kana": "カブシキガイシヤ シマヅセイサクシヨ トウキヨウシシヤ", "name": "株式会社　島津製作所　東京支社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目3", "postal_code": "1018448", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018522','{"jis": "13101", "kana": "カブシキガイシヤ シヤカイホケンケンキユウシヨ", "name": "株式会社　社会保険研究所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2-15-9TheKanda282", "postal_code": "1018522", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018050','{"jis": "13101", "kana": "カブシキガイシヤ シユウエイシヤ", "name": "株式会社　集英社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目5-10", "postal_code": "1018050", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018054','{"jis": "13101", "kana": "カブシキガイシヤ シユウエイシヤ シシヨバコ19ゴウ", "name": "株式会社　集英社　私書箱１９号", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2-5-10", "postal_code": "1018054", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018001','{"jis": "13101", "kana": "カブシキガイシヤ シヨウガクカン", "name": "株式会社　小学館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目3-1", "postal_code": "1018001", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018415','{"jis": "13101", "kana": "カブシキガイシヤ シヨウガクカンシユウエイシヤプロダクシヨン", "name": "株式会社　小学館集英社プロダクション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目30", "postal_code": "1018415", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018388','{"jis": "13101", "kana": "カブシキガイシヤ シヨウネンガホウシヤ", "name": "株式会社　少年画報社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "2-8-5", "postal_code": "1018388", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018588','{"jis": "13101", "kana": "カブシキガイシヤ シライシ", "name": "株式会社　白石", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田岩本町", "banchi": "1番地14", "postal_code": "1018588", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイワモトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018475','{"jis": "13101", "kana": "カブシキガイシヤ シンコ-ミユ-ジツク・エンタテイメント", "name": "株式会社　シンコーミュージック・エンタテイメント", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "2丁目1", "postal_code": "1018475", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018450','{"jis": "13101", "kana": "カブシキガイシヤ シンコ-ミユ-ジツク・エンタテイメント", "name": "株式会社　シンコーミュージック・エンタテイメント", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目14", "postal_code": "1018450", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018421','{"jis": "13101", "kana": "カブシキガイシヤ ジホウ", "name": "株式会社　じほう", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "1-5-15猿楽町SSビル", "postal_code": "1018421", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018636','{"jis": "13101", "kana": "カブシキガイシヤ スズケン", "name": "株式会社　スズケン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田佐久間河岸", "banchi": "59", "postal_code": "1018636", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダサクマガシ", "alternates": []}');
-INSERT INTO office_data VALUES('1018465','{"jis": "13101", "kana": "カブシキガイシヤ スミテツクス", "name": "株式会社　スミテックス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目24-1住友商事神保町ビル3F", "postal_code": "1018465", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018418','{"jis": "13101", "kana": "カブシキガイシヤ ゼンリン", "name": "株式会社　ゼンリン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "1-1-1", "postal_code": "1018418", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018610','{"jis": "13101", "kana": "カブシキガイシヤ ソフマツプ", "name": "株式会社　ソフマップ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "1丁目16-9", "postal_code": "1018610", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018638','{"jis": "13101", "kana": "カブシキガイシヤ ソラスト", "name": "株式会社　ソラスト", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田佐久間町", "banchi": "3丁目2番", "postal_code": "1018638", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダサクマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018335','{"jis": "13101", "kana": "カブシキガイシヤ ソンポカイカン", "name": "株式会社　損保會舘", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目9", "postal_code": "1018335", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018466','{"jis": "13101", "kana": "カブシキガイシヤ タイシユウカンシヨテン", "name": "株式会社　大修館書店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目24", "postal_code": "1018466", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018577','{"jis": "13101", "kana": "カブシキガイシヤ タジマ", "name": "株式会社　タジマ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-14-1秋葉原UDXビル21階", "postal_code": "1018577", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018619','{"jis": "13101", "kana": "カブシキガイシヤ ダイド-リミテツド", "name": "株式会社　ダイドーリミテッド", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目1-16", "postal_code": "1018619", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018408','{"jis": "13101", "kana": "カブシキガイシヤ ツリビトシヤ", "name": "株式会社　つり人社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "1丁目30-13", "postal_code": "1018408", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008610','{"jis": "13101", "kana": "カブシキガイシヤ デイ-エムエス", "name": "株式会社　ディーエムエス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "1丁目11(銀座郵便局私書箱第777号)", "postal_code": "1008610", "old_code": "101  ", "post_office": "銀座", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018470','{"jis": "13101", "kana": "カブシキガイシヤ デイ-エムエス", "name": "株式会社　ディーエムエス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "1丁目11", "postal_code": "1018470", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018667','{"jis": "13101", "kana": "カブシキガイシヤ デツク", "name": "株式会社　デック", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目23(神田郵便局私書箱第2号)", "postal_code": "1018667", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018631','{"jis": "13101", "kana": "カブシキガイシヤ トウワエンジニアリング", "name": "株式会社　東和エンジニアリング", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "1-7-8ユニゾ東神田一丁目ビル", "postal_code": "1018631", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018365','{"jis": "13101", "kana": "カブシキガイシヤ トオエンシヨボウ", "name": "株式会社　桃園書房", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目11-7", "postal_code": "1018365", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018548','{"jis": "13101", "kana": "カブシキガイシヤ トクリキホンテン", "name": "株式会社　徳力本店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "鍛冶町", "banchi": "2丁目9番12号", "postal_code": "1018548", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018419','{"jis": "13101", "kana": "カブシキガイシヤ ニゲンシヤ", "name": "株式会社　二玄社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目2", "postal_code": "1018419", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018323','{"jis": "13101", "kana": "カブシキガイシヤ ニホンケイザイコウコクシヤ", "name": "株式会社　日本経済広告社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "2丁目10", "postal_code": "1018323", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1018576','{"jis": "13101", "kana": "カブシキガイシヤ ニホンホウレイ", "name": "株式会社　日本法令", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "2丁目1-7", "postal_code": "1018576", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1018359','{"jis": "13101", "kana": "カブシキガイシヤ ニホンボウエキホケン", "name": "株式会社　日本貿易保険", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目8-1千代田ファーストビル", "postal_code": "1018359", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018561','{"jis": "13101", "kana": "カブシキガイシヤ ニホンマンパワ-", "name": "株式会社　日本マンパワー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田東松下町", "banchi": "47-1", "postal_code": "1018561", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダヒガシマツシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018901','{"jis": "13101", "kana": "カブシキガイシヤ ニホンマンパワ-ナイ カンポエルシ-ジムキヨク", "name": "株式会社　日本マンパワー内かんぽＬＣ事務局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田東松下町", "banchi": "47-1", "postal_code": "1018901", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダヒガシマツシタチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018454','{"jis": "13101", "kana": "カブシキガイシヤ バ-ン・コ-ポレ-シヨン", "name": "株式会社　バーン・コーポレーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "2丁目1番", "postal_code": "1018454", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018565','{"jis": "13101", "kana": "カブシキガイシヤ ヒガシニツポンギンコウ カンダシテン", "name": "株式会社　東日本銀行　神田支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "2", "postal_code": "1018565", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018562','{"jis": "13101", "kana": "カブシキガイシヤ ヒガシニツポンギンコウ ジムセンタ-", "name": "株式会社　東日本銀行　事務センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "2番地", "postal_code": "1018562", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018941','{"jis": "13101", "kana": "カブシキガイシヤ ヒタチビルシステム", "name": "株式会社　日立ビルシステム", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番", "postal_code": "1018941", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028644','{"jis": "13101", "kana": "カブシキガイシヤ ビ-エスニツポン(ビ-エスニツテレ)", "name": "株式会社　ビーエス日本（ビーエス日テレ）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "14番地日テレ麹町ビル南館3F", "postal_code": "1028644", "old_code": "101  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018189','{"jis": "13101", "kana": "カブシキガイシヤ フジヤクヒン", "name": "株式会社　富士薬品", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目2番地1KANDASQUARE9階", "postal_code": "1018189", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018405','{"jis": "13101", "kana": "カブシキガイシヤ フタミシヨボウ", "name": "株式会社　二見書房", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目18-11堀内三崎町ビル", "postal_code": "1018405", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('1018381','{"jis": "13101", "kana": "カブシキガイシヤ ベ-スボ-ル・マガジンシヤ", "name": "株式会社　ベースボール・マガジン社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "3丁目10-10", "postal_code": "1018381", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018423','{"jis": "13101", "kana": "カブシキガイシヤ ホウソウシユツパンエ-ジエンシ-", "name": "株式会社　放送出版エージェンシー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-7-3神保町NKビル", "postal_code": "1018423", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018424','{"jis": "13101", "kana": "カブシキガイシヤ ホウソウシユツパンプロモ-シヨン ニホンアマチユアカヨウレンメイ ホンブジムキヨク", "name": "株式会社　放送出版プロモーション　日本アマチュア歌謡連盟　本部事務局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-7-3神保町NKビル", "postal_code": "1018424", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018972','{"jis": "13101", "kana": "カブシキガイシヤ ミツウロコ", "name": "株式会社　ミツウロコ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1", "postal_code": "1018972", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018305','{"jis": "13101", "kana": "カブシキガイシヤ メデイアワ-クス", "name": "株式会社　メディアワークス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目8", "postal_code": "1018305", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018648','{"jis": "13101", "kana": "カブシキガイシヤ ヤクジニツポウシヤ", "name": "株式会社　薬事日報社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018648", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018566','{"jis": "13101", "kana": "カブシキガイシヤ ヤマヤコ-ポレ-シヨン", "name": "株式会社　ヤマヤコーポレーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "22", "postal_code": "1018566", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018524','{"jis": "13101", "kana": "カブシキガイシヤ ユニ・プランニング", "name": "株式会社　ユニ・プランニング", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目12-12美土代ビル4F", "postal_code": "1018524", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018519','{"jis": "13101", "kana": "カブシキガイシヤ ラ-ニングネツト", "name": "株式会社　ラーニングネット", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目5-6", "postal_code": "1018519", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018325','{"jis": "13101", "kana": "カンコウギヨウケンコウホケンクミアイ", "name": "管工業健康保険組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目1", "postal_code": "1018325", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018345','{"jis": "13101", "kana": "カンダシヤカイホケンジムシヨ", "name": "神田社会保険事務所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "2丁目7-8住友水道橋ビル", "postal_code": "1018345", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018464','{"jis": "13101", "kana": "カンダゼイムシヨ", "name": "神田税務署", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目3", "postal_code": "1018464", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018712','{"jis": "13101", "kana": "カンダブツサン", "name": "神田物産　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目16-13(神田郵便局私書箱第122号)", "postal_code": "1018712", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018351','{"jis": "13101", "kana": "ガツコウホウジン オオハラガクエン", "name": "学校法人　大原学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "2丁目4-11大原簿記学校本館", "postal_code": "1018351", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018433','{"jis": "13101", "kana": "ガツコウホウジン キヨウリツジヨシガクエン", "name": "学校法人　共立女子学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目2-1", "postal_code": "1018433", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018313','{"jis": "13101", "kana": "ガツコウホウジン スルガダイガクエン スンダイヨビガツコウ", "name": "学校法人　駿河台学園　駿台予備学校", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5-17", "postal_code": "1018313", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018456','{"jis": "13101", "kana": "ガツコウホウジン セイソクガクエン", "name": "学校法人　正則学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目1", "postal_code": "1018456", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018301','{"jis": "13101", "kana": "ガツコウホウジン メイジダイガク", "name": "学校法人　明治大学", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目1", "postal_code": "1018301", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018311','{"jis": "13101", "kana": "キヨ-リンセイヤクホ-ルデイングス カブシキガイシヤ", "name": "キョーリン製薬ホールディングス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6御茶ノ水ソラシティ", "postal_code": "1018311", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018510','{"jis": "13101", "kana": "キヨウドウクレジツトサ-ビス カブシキガイシヤ", "name": "協同クレジットサービス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目1-12", "postal_code": "1018510", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018317','{"jis": "13101", "kana": "キヨウドウリ-ス カブシキガイシヤ", "name": "協同リース　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目9-17", "postal_code": "1018317", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018437','{"jis": "13101", "kana": "キヨウリツジヨシダイガク", "name": "共立女子大学", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目2-1", "postal_code": "1018437", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018621','{"jis": "13101", "kana": "キヨウリツメンテナンス", "name": "（株）　共立メンテナンス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "2丁目18-8", "postal_code": "1018621", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
+INSERT INTO office_data VALUES('1018311','{"jis": "13101", "kana": "キヨウリンセイヤク カブシキガイシヤ", "name": "杏林製薬　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6御茶ノ水ソラシティ", "postal_code": "1018311", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018645','{"jis": "13101", "kana": "キリンビバレツジ カブシキガイシヤ", "name": "キリンビバレッジ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018645", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018641','{"jis": "13101", "kana": "キンキニホンツ-リスト カブシキガイシヤ", "name": "近畿日本ツーリスト　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "1-7-8東神田フコク生命ビル", "postal_code": "1018641", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018356','{"jis": "13101", "kana": "ギンエイシヤ", "name": "（株）　銀英社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "2丁目8-9林リースビル5F", "postal_code": "1018356", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018545','{"jis": "13101", "kana": "クメ・クオリテイ・プロダクツ カブシキガイシヤ", "name": "くめ・クオリティ・プロダクツ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田東松下町", "banchi": "14番地東信神田ビル9階", "postal_code": "1018545", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダヒガシマツシタチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018427','{"jis": "13101", "kana": "クリタシユツパンハンバイ カブシキガイシヤ", "name": "栗田出版販売　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "3-25住友神保町ビル8階", "postal_code": "1018427", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018977','{"jis": "13101", "kana": "グロ-リ- カブシキカイシヤ トウキヨウホンブ", "name": "グローリー　株式会社　東京本部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDXビル19F", "postal_code": "1018977", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018372','{"jis": "13101", "kana": "コウエキザイダンホウジン ケツカクヨボウカイ ソウゴウケンシンスイシンセンタ-", "name": "公益財団法人　結核予防会　総合健診推進センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "1丁目3-12", "postal_code": "1018372", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018378','{"jis": "13101", "kana": "コウエキシヤダンホウジン ゼンニホンビヨウインキヨウカイ", "name": "公益社団法人　全日本病院協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "2丁目8番8号住友不動産猿楽町ビル7階", "postal_code": "1018378", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('1018307','{"jis": "13101", "kana": "コウエキシヤダンホウジン ニホンカガクカイ", "name": "公益社団法人　日本化学会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目5", "postal_code": "1018307", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018559','{"jis": "13101", "kana": "サトウキンゾク カブシキガイシヤ", "name": "佐藤金属　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "2丁目13", "postal_code": "1018559", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018583','{"jis": "13101", "kana": "サンデンホ-ルデイングス カブシキガイシヤ トウキヨウホンシヤ", "name": "サンデンホールディングス　株式会社　東京本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "1-18-13秋葉原ダイビル", "postal_code": "1018583", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018682','{"jis": "13101", "kana": "サンヨウボウエキ", "name": "三洋貿易　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目11(神田郵便局私書箱第215号)", "postal_code": "1018682", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018333','{"jis": "13101", "kana": "ザイダンホウジン サンギヨウケイリキヨウカイ", "name": "財団法人　産業経理協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "1丁目15", "postal_code": "1018333", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018346','{"jis": "13101", "kana": "ザイダンホウジン ニホンガンカガツカイ", "name": "財団法人　日本眼科学会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "2丁目4-11-402", "postal_code": "1018346", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018358','{"jis": "13101", "kana": "ザイダンホウジン ニホンシヨドウキヨウイクガツカイ", "name": "財団法人　日本書道教育学会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "2丁目2-3", "postal_code": "1018358", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018983','{"jis": "13101", "kana": "ザイダンホウジン ボシエイセイケンキユウカイ", "name": "財団法人　母子衛生研究会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "2丁目18-7", "postal_code": "1018983", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018581','{"jis": "13101", "kana": "ザイダンホウジン ポスタルサ-ビスセンタ-", "name": "（財）　ポスタルサービスセンター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "鍛冶町", "banchi": "1丁目8-3", "postal_code": "1018581", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018412','{"jis": "13101", "kana": "シヤカイフクシホウジン ゼンコクモウロウシヤキヨウカイ", "name": "社会福祉法人　全国盲ろう者協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目5", "postal_code": "1018412", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018643','{"jis": "13101", "kana": "シヤカイフクシホウジン ミツイキネンビヨウイン", "name": "社会福祉法人　三井記念病院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018643", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018459','{"jis": "13101", "kana": "シヤダンホウジン ガクシカイ", "name": "社団法人　学士会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目28", "postal_code": "1018459", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018544','{"jis": "13101", "kana": "シヤダンホウジン サンギヨウカンキヨウカンリキヨウカイ", "name": "社団法人　産業環境管理協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "鍛冶町", "banchi": "2丁目2-1", "postal_code": "1018544", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018552','{"jis": "13101", "kana": "シヤダンホウジン ジヤパンケネルクラブ", "name": "社団法人　ジャパンケネルクラブ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目5", "postal_code": "1018552", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018328','{"jis": "13101", "kana": "シヤダンホウジン トウキヨウトイシカイ", "name": "社団法人　東京都医師会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5", "postal_code": "1018328", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018326','{"jis": "13101", "kana": "シヤダンホウジン トウキヨウトキヨウシヨクインゴジヨカイ サンラクビヨウイン", "name": "社団法人　東京都教職員互助会　三楽病院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5", "postal_code": "1018326", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018307','{"jis": "13101", "kana": "シヤダンホウジン ニホンカガクカイ", "name": "社団法人　日本化学会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目5", "postal_code": "1018307", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018468','{"jis": "13101", "kana": "シヨ-ボンドケンセツ カブシキガイシヤ", "name": "ショーボンド建設　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目18", "postal_code": "1018468", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018521','{"jis": "13101", "kana": "シヨウワサンギヨウ カブシキガイシヤ", "name": "昭和産業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目2-1鎌倉河岸ビル", "postal_code": "1018521", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018616','{"jis": "13101", "kana": "シンキ カブシキガイシヤ", "name": "シンキ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目12-8住友不動産秋葉原ビル", "postal_code": "1018616", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018451','{"jis": "13101", "kana": "シンセイカミパルプシヨウジ カブシキガイシヤ", "name": "新生紙パルプ商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目8", "postal_code": "1018451", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1018616','{"jis": "13101", "kana": "シンセイパ-ソナルロ-ン カブシキガイシヤ", "name": "新生パーソナルローン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目12-8住友不動産秋葉原ビル", "postal_code": "1018616", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018603','{"jis": "13101", "kana": "シンセイフイナンシヤル カブシキガイシヤ", "name": "新生フィナンシャル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目12番8号住友不動産秋葉原ビル", "postal_code": "1018603", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018447','{"jis": "13101", "kana": "ジ-アンドシ-", "name": "（株）　ジーアンドシー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目11", "postal_code": "1018447", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018518','{"jis": "13101", "kana": "ジエイエイゼンノウタマゴ カブシキガイシヤ", "name": "ＪＡ全農たまご　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1-1-12コープビル9F", "postal_code": "1018518", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018430','{"jis": "13101", "kana": "ジヨウホウ・システムケンキユウキコウ コクリツジヨウホウガクケンキユウジヨ", "name": "情報・システム研究機構　国立情報学研究所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目1-2", "postal_code": "1018430", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018633','{"jis": "13101", "kana": "スガツネコウギヨウ カブシキガイシヤ", "name": "スガツネ工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "2-9-13", "postal_code": "1018633", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018453','{"jis": "13101", "kana": "スミシヨウエレクトロニクス カブシキガイシヤ", "name": "住商エレクトロニクス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目11住友商事錦町ビル", "postal_code": "1018453", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018425','{"jis": "13101", "kana": "センシユウダイガク", "name": "学校法人　専修大学", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "3丁目8-1", "postal_code": "1018425", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018525','{"jis": "13101", "kana": "センモンガツコウ カンダガイゴガクイン(ガツコウホウジン サノガクエン)", "name": "専門学校　神田外語学院（学校法人　佐野学園）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目13-13", "postal_code": "1018525", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018508','{"jis": "13101", "kana": "ゼンコクシンリンクミアイレンゴウカ", "name": "全国森林組合連合会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目1-12", "postal_code": "1018508", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018509','{"jis": "13101", "kana": "ゼンコクチホウギンコウキヨウカイ", "name": "（社）　全国地方銀行協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3丁目1-2", "postal_code": "1018509", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018501','{"jis": "13101", "kana": "ゼンコクノウギヨウキヨウドウクミアイレンゴウカイゼンノウトウキヨウシシヨ", "name": "全国農業協同組合連合会全農東京支所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目1-12", "postal_code": "1018501", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018502','{"jis": "13101", "kana": "ゼンノウブツリユウ カブシキガイシヤ", "name": "全農物流　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目13-7名古路ビル本館", "postal_code": "1018502", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018416','{"jis": "13101", "kana": "タイヘイデンギヨウ カブシキガイシヤ", "name": "太平電業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目4", "postal_code": "1018416", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018444','{"jis": "13101", "kana": "タイホウヤクヒンコウギヨウ カブシキガイシヤ", "name": "大鵬薬品工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目27", "postal_code": "1018444", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018321','{"jis": "13101", "kana": "タカサゴネツガクコウギヨウ カブシキガイシヤ", "name": "高砂熱学工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目2-5", "postal_code": "1018321", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018575','{"jis": "13101", "kana": "タジマル-フイング カブシキガイシヤ", "name": "田島ルーフィング　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "3-11-13", "postal_code": "1018575", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018579','{"jis": "13101", "kana": "タジマル-フイング カブシキガイシヤ", "name": "田島ルーフィング　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-14-1秋葉原UDXビル21階", "postal_code": "1018579", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018383','{"jis": "13101", "kana": "タツク カブシキガイシヤ", "name": "タック　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "3丁目2-18", "postal_code": "1018383", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('1018383','{"jis": "13101", "kana": "タツク カブシキガイシヤ", "name": "ＴＡＣ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田三崎町", "banchi": "3丁目2-18", "postal_code": "1018383", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018950','{"jis": "13101", "kana": "ダイケンコウギヨウ カブシキガイシヤ", "name": "大建工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目12-8", "postal_code": "1018950", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018324','{"jis": "13101", "kana": "チユウオウダイガク スルガダイキネンカン", "name": "中央大学　駿河台記念館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3丁目11-5", "postal_code": "1018324", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
+INSERT INTO office_data VALUES('1018324','{"jis": "13101", "kana": "チユウオウダイガク スルガダイキヤンパス", "name": "中央大学　駿河台キャンパス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3丁目11-5", "postal_code": "1018324", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018646','{"jis": "13101", "kana": "ツルオカ カブシキガイシヤ", "name": "鶴岡　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "2", "postal_code": "1018646", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018366','{"jis": "13101", "kana": "テツケンケンセツ", "name": "鉄建建設　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目5-3", "postal_code": "1018366", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018703','{"jis": "13101", "kana": "ト-アサイホケン カブシキガイシヤ", "name": "トーア再保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3丁目6", "postal_code": "1018703", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018530','{"jis": "13101", "kana": "トウアシヨウジ カブシキガイシヤ", "name": "東亜商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目19", "postal_code": "1018530", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1018533','{"jis": "13101", "kana": "トウキヨウト コガタコンピユ-タソフトウエア サンギヨウケンコウホケンクミアイ カンダシブ", "name": "東京都　小型コンピュータソフトウェア　産業健康保険組合　神田支部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "2丁目7NKビル9F", "postal_code": "1018533", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018527','{"jis": "13101", "kana": "トウキヨウトシヨクギヨウノウリヨクカイハツキヨウカイ", "name": "東京都職業能力開発協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1-1-5東京都産業労働局神田庁舎5階", "postal_code": "1018527", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018523','{"jis": "13101", "kana": "トウキヨウトスイドウキヨク チヨダエイギヨウシヨ", "name": "東京都水道局　千代田営業所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目1-12", "postal_code": "1018523", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018520','{"jis": "13101", "kana": "トウキヨウトチヨダトゼイジムシヨ", "name": "東京都千代田都税事務所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目1-12", "postal_code": "1018520", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018515','{"jis": "13101", "kana": "トウキヨウロイヤルプラザ カンリクミアイ", "name": "東京ロイヤルプラザ　管理組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目18-11", "postal_code": "1018515", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018350','{"jis": "13101", "kana": "トウコウデンキコウジ カブシキガイシヤ", "name": "東光電気工事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "1丁目4-5", "postal_code": "1018350", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018327','{"jis": "13101", "kana": "トウホウホ-ルデイングス カブシキガイシヤ", "name": "東邦ホールディングス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5-23", "postal_code": "1018327", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018630','{"jis": "13101", "kana": "トウヨク シンヨウクミアイ", "name": "東浴　信用組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "1丁目10-2", "postal_code": "1018630", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018411','{"jis": "13101", "kana": "トシヨインサツ カブシキガイシヤ", "name": "図書印刷　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目17番地神田神保町ビル", "postal_code": "1018411", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018343','{"jis": "13101", "kana": "トヨタ・コニツク・プロ カブシキガイシヤ", "name": "トヨタ・コニック・プロ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2-101ワテラスタワー10F", "postal_code": "1018343", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018612','{"jis": "13101", "kana": "トランスネツト", "name": "（株）　トランスネット", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "1丁目17-4JR東日本秋葉原ビル", "postal_code": "1018612", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018617','{"jis": "13101", "kana": "ドウワコウギヨウ カブシキガイシヤ", "name": "同和鉱業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1", "postal_code": "1018617", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018008','{"jis": "13101", "kana": "ドクリツギヨウセイホウジン ウチユウコウクウケンキユウカイハツキコウ", "name": "独立行政法人　宇宙航空研究開発機構", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目6番", "postal_code": "1018008", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018359','{"jis": "13101", "kana": "ドクリツギヨウセイホウジン ニホンボウエキホケン", "name": "独立行政法人　日本貿易保険", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目8-1千代田ファーストビル", "postal_code": "1018359", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018662','{"jis": "13101", "kana": "ニシムラシヨテン", "name": "（株）　西村書店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目10(神田郵便局私書箱第42号)", "postal_code": "1018662", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018688','{"jis": "13101", "kana": "ニチイガツカン", "name": "（株）　ニチイ学館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目9(神田郵便局私書箱第25号)", "postal_code": "1018688", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018483','{"jis": "13101", "kana": "ニチモ カブシキカイシヤ", "name": "ニチモ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7住友不動産神田ビル10F", "postal_code": "1018483", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018609','{"jis": "13101", "kana": "ニチモコミユニテイ カブシキガイシヤ", "name": "ニチモコミュニティ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "6丁目5-12偕楽ビル5・7・8F", "postal_code": "1018609", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018329','{"jis": "13101", "kana": "ニツシンカサイカイジヨウホケン カブシキカイシヤ", "name": "日新火災海上保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目3番地", "postal_code": "1018329", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018441','{"jis": "13101", "kana": "ニツシンセイフン カブシキガイシヤ", "name": "日清製粉　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目25", "postal_code": "1018441", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018210','{"jis": "13101", "kana": "ニツポンカミツウシヨウ カブシキガイシヤ", "name": "日本紙通商　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目6番", "postal_code": "1018210", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018215','{"jis": "13101", "kana": "ニツポンセイシクレシア カブシキガイシヤ", "name": "日本製紙クレシア　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6", "postal_code": "1018215", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018213','{"jis": "13101", "kana": "ニツポンセイシモクザイ カブシキガイシヤ", "name": "日本製紙木材　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目6番", "postal_code": "1018213", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018647','{"jis": "13101", "kana": "ニツポンツウウン カブシキガイシヤ", "name": "日本通運　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "2番地", "postal_code": "1018647", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018946','{"jis": "13101", "kana": "ニツポンレンタカ-ア-バンネツト カブシキガイシヤ トウキヨウデイビジヨン", "name": "ニッポンレンタカーアーバンネット　株式会社　東京ディビジョン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "2丁目1-11第一坂本ビル", "postal_code": "1018946", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018710','{"jis": "13101", "kana": "ニホンシユツパンハンバイ", "name": "日本出版販売　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目3(神田郵便局私書箱第13号)", "postal_code": "1018710", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018310','{"jis": "13101", "kana": "ニホンダイガク シガクブ", "name": "日本大学　歯学部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目8-13", "postal_code": "1018310", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018354','{"jis": "13101", "kana": "ニホンダイガク ツウシンキヨウイクブ", "name": "日本大学　通信教育部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目2-3", "postal_code": "1018354", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018375','{"jis": "13101", "kana": "ニホンダイガク ホウガクブ", "name": "日本大学　法学部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目3-1", "postal_code": "1018375", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018308','{"jis": "13101", "kana": "ニホンダイガク リコウガクブ", "name": "日本大学　理工学部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目8-14", "postal_code": "1018308", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018707','{"jis": "13101", "kana": "ニホンパ-ソナルセンタ-", "name": "（株）　日本パーソナルセンター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目5新須田町ビル3F(神田郵便局私書箱第209号)", "postal_code": "1018707", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018407','{"jis": "13101", "kana": "ニホンブンゲイシヤ", "name": "（株）日本文芸社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "1丁目7", "postal_code": "1018407", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018506','{"jis": "13101", "kana": "ノウリンギヨギヨウシンヨウキキン", "name": "農林漁業信用基金", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目1-12コープビル", "postal_code": "1018506", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018507','{"jis": "13101", "kana": "ノウリンチユウオウキンコ", "name": "農林中央金庫", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目1-12コープビル", "postal_code": "1018507", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018711','{"jis": "13101", "kana": "ハクセンシヤ", "name": "（株）　白泉社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目6-4(神田郵便局私書箱第92号)", "postal_code": "1018711", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018605','{"jis": "13101", "kana": "ハシモトサンギヨウ", "name": "橋本産業　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田紺屋町", "banchi": "34", "postal_code": "1018605", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダコンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018462','{"jis": "13101", "kana": "パシフイツクコンサルタンツ カブシキガイシヤ", "name": "パシフィックコンサルタンツ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目22番地", "postal_code": "1018462", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018302','{"jis": "13101", "kana": "ヒタチカセイシヨウジ カブシキガイシヤ", "name": "日立化成商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2-5-1", "postal_code": "1018302", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018971','{"jis": "13101", "kana": "ヒタチデンセン カブシキガイシヤ", "name": "日立電線　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDX", "postal_code": "1018971", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018439','{"jis": "13101", "kana": "ヒトツバシダイガク チヨダキヤンパス", "name": "一橋大学　千代田キャンパス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目1-2", "postal_code": "1018439", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1018634','{"jis": "13101", "kana": "ビ-・アツプル カブシキガイシヤ", "name": "ビー・アップル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "1丁目11-1エリア神田8F", "postal_code": "1018634", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
+INSERT INTO office_data VALUES('1018439','{"jis": "13101", "kana": "ヒトツバシダイガク チヨダキヤンパスジムシツ", "name": "一橋大学　千代田キャンパス事務室", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目1-2", "postal_code": "1018439", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018528','{"jis": "13101", "kana": "ピツプ カブシキガイシヤ", "name": "ピップ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3-3-7", "postal_code": "1018528", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018314','{"jis": "13101", "kana": "フジゼロツクスオフイスサプライ カブシキガイシヤ", "name": "富士ゼロックスオフィスサプライ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5-12駿河台プラザビル", "postal_code": "1018314", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018625','{"jis": "13101", "kana": "フジデンキリテイルシステムズ カブシキガイシヤ", "name": "富士電機リテイルシステムズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "6丁目15-12", "postal_code": "1018625", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018542','{"jis": "13101", "kana": "フジパン カブシキガイシヤ カントウジギヨウブ", "name": "フジパン　（株）　関東事業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "10-1", "postal_code": "1018542", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018452','{"jis": "13101", "kana": "フジフイルムグラフイツクシステムズ カブシキガイシヤ", "name": "富士フイルムグラフィックシステムズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目13竹橋安田ビル1~4F", "postal_code": "1018452", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018606','{"jis": "13101", "kana": "フマキラ- カブシキガイシヤ", "name": "フマキラー　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美倉町", "banchi": "11", "postal_code": "1018606", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミクラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018970','{"jis": "13101", "kana": "フルカワスカイ カブシキガイシヤ", "name": "古河スカイ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDX", "postal_code": "1018970", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018409','{"jis": "13101", "kana": "ヘイワシユツパン カブシキガイシヤ", "name": "平和出版　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目3-13鈴木ビル4F", "postal_code": "1018409", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018331','{"jis": "13101", "kana": "マルベニガスエナジ- カブシキガイシヤ", "name": "丸紅ガスエナジー　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目2", "postal_code": "1018331", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018363','{"jis": "13101", "kana": "マルベニテレコム (カブ)", "name": "丸紅テレコム　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目8-1千代田ファーストビル14F", "postal_code": "1018363", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018477','{"jis": "13101", "kana": "ミズノ カブシキガイシヤ", "name": "ミズノ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "3丁目22", "postal_code": "1018477", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018219','{"jis": "13101", "kana": "ミズホシヨウケン カブシキガイシヤ", "name": "みずほ証券　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6御茶ノ水ソラシティ", "postal_code": "1018219", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018443','{"jis": "13101", "kana": "ミズホジヨウホウソウケン カブシキガイシヤ", "name": "みずほ情報総研　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目3", "postal_code": "1018443", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018429','{"jis": "13101", "kana": "ミタニサンギヨウ カブシキガイシヤ", "name": "三谷産業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-36-1千代田ファーストウイング", "postal_code": "1018429", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018485','{"jis": "13101", "kana": "ミツイカガクトウセロ カブシキガイシヤ", "name": "三井化学東セロ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7", "postal_code": "1018485", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018458','{"jis": "13101", "kana": "ミツイスミトモカイジヨウアイオイセイメイホケン カブシキガイシヤ", "name": "三井住友海上あいおい生命保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3-11-1", "postal_code": "1018458", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018011','{"jis": "13101", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキカイシヤ", "name": "三井住友海上火災保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3丁目9(神田郵便局私書箱第23号)", "postal_code": "1018011", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
-INSERT INTO office_data VALUES('1018607','{"jis": "13101", "kana": "ミツビシブング カブシキガイシヤ", "name": "三菱文具　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "2丁目17-3アヤベビル4F", "postal_code": "1018607", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018338','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目16-11内神田渋谷ビル9階", "postal_code": "1018338", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018637','{"jis": "13101", "kana": "ミツビシユ-エフジエ-フアクタ- カブシキガイシヤ", "name": "三菱ＵＦＪファクター　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番ワテラスタワー", "postal_code": "1018637", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018676','{"jis": "13101", "kana": "ムサシノギンコウ トウキヨウシテン", "name": "（株）　武蔵野銀行　東京支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目15-9(神田郵便局私書箱第45号)", "postal_code": "1018676", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018554','{"jis": "13101", "kana": "メタウオ-タ- カブシキガイシヤ", "name": "メタウォーター　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目25番", "postal_code": "1018554", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018578','{"jis": "13101", "kana": "モチダシヨウコウ", "name": "持田商工　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "2丁目10-12", "postal_code": "1018578", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018626','{"jis": "13101", "kana": "ヤマキ カブシキガイシヤ トウキヨウシテン", "name": "ヤマキ　株式会社　東京支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-8-2", "postal_code": "1018626", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018620','{"jis": "13101", "kana": "ヤマギワ カブシキガイシヤ", "name": "ヤマギワ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "3丁目12-4", "postal_code": "1018620", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
+INSERT INTO office_data VALUES('1018626','{"jis": "13101", "kana": "ヤマキ カブシキガイシヤ", "name": "ヤマキ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-8-2", "postal_code": "1018626", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018585','{"jis": "13101", "kana": "ヤマザキセイパン カブシキガイシヤ", "name": "山崎製パン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "3丁目10-1", "postal_code": "1018585", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018580','{"jis": "13101", "kana": "ユアサシヨウジ カブシキガイシヤ", "name": "ユアサ商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7番住友不動産神田ビル", "postal_code": "1018580", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018531','{"jis": "13101", "kana": "ユウゲンガイシヤ カガクヒヨウロンシヤ", "name": "有限会社　科学評論社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目10-8", "postal_code": "1018531", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1018531','{"jis": "13101", "kana": "ユウゲンガイシヤ カガクヒヨウロンシヤ", "name": "有限会社　科学評論社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目10-15", "postal_code": "1018531", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018422','{"jis": "13101", "kana": "ユウセントラベル", "name": "郵船トラベル　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目2", "postal_code": "1018422", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018336','{"jis": "13101", "kana": "リケンテクノス カブシキガイシヤ", "name": "リケンテクノス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番地ワテラスタワー", "postal_code": "1018336", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018370','{"jis": "13101", "kana": "リケンビタミン カブシキガイシヤ", "name": "理研ビタミン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目9-18", "postal_code": "1018370", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('1018446','{"jis": "13101", "kana": "リヨウエイ", "name": "菱栄　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目13宝栄錦町ビル8F", "postal_code": "1018446", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018385','{"jis": "13101", "kana": "リンリケンキユウジヨ", "name": "（社）　倫理研究所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "3丁目1-10", "postal_code": "1018385", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('1018446','{"jis": "13101", "kana": "リヨウエイ カブシキカイシヤ", "name": "菱栄　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目13大手町宝栄ビル7階", "postal_code": "1018446", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018315','{"jis": "13101", "kana": "ロウドウキンコカイカン", "name": "労働金庫会館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5-15", "postal_code": "1018315", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018642','{"jis": "13101", "kana": "ワイケイケイ カブシキガイシヤ", "name": "ＹＫＫ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018642", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018002','{"jis": "13101", "kana": "カブシキガイシヤ イワナミシヨテン", "name": "株式会社　岩波書店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目5-5", "postal_code": "1018002", "old_code": "10102", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1018077','{"jis": "13101", "kana": "カブシキガイシヤ アスカシンシヤ", "name": "株式会社　飛鳥新社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "3丁目10神田第3アメレックスビル", "postal_code": "1018077", "old_code": "10177", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018655','{"jis": "13101", "kana": "アサヒカサイカイジヨウホケン カブシキガイシヤ", "name": "朝日火災海上保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7番地(神田郵便局私書箱第41号)", "postal_code": "1018655", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018654','{"jis": "13101", "kana": "イシフクキンゾクコウギヨウ カブシキガイシヤ", "name": "石福金属興業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3丁目20-7(神田郵便局私書箱第57号)", "postal_code": "1018654", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018701','{"jis": "13101", "kana": "カブシキガイシヤ シヨウデンシヤ", "name": "株式会社　祥伝社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "3丁目6-5(神田郵便局私書箱第152号)", "postal_code": "1018701", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1048650','{"jis": "13101", "kana": "カブシキガイシヤ デイ-エムエス", "name": "株式会社　ディーエムエス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "1丁目11(晴海郵便局私書箱第230号)", "postal_code": "1048650", "old_code": "10191", "post_office": "晴海", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018718','{"jis": "13101", "kana": "カブシキガイシヤ ニホンイジシンポウシヤ", "name": "株式会社　日本醫事新報社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目9(神田郵便局私書箱第18号)", "postal_code": "1018718", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018715','{"jis": "13101", "kana": "ゼンニホンシヨゲイブンカイン", "name": "全日本書芸文化院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目20(神田郵便局私書箱第37号)", "postal_code": "1018715", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018670','{"jis": "13101", "kana": "トウキヨウセ-ルスプロデユ-ス カブシキガイシヤ", "name": "東京セールスプロデュース　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "1丁目11(神田郵便局私書箱第191号)", "postal_code": "1018670", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018651','{"jis": "13101", "kana": "マルタカコウギヨウ カブシキガイシヤ", "name": "丸高興業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "1丁目7(神田郵便局私書箱第50号)", "postal_code": "1018651", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
@@ -125780,14 +125713,15 @@
 INSERT INTO office_data VALUES('1028565','{"jis": "13101", "kana": "カブシキガイシヤ オ-タニコ-ポレ-シヨン", "name": "株式会社　オータニコーポレーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "4-1", "postal_code": "1028565", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028573','{"jis": "13101", "kana": "カブシキガイシヤ オオツカシヨウカイ", "name": "株式会社　大塚商会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "2丁目18-4", "postal_code": "1028573", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028025','{"jis": "13101", "kana": "カブシキガイシヤ オズマピ-ア-ル", "name": "株式会社　オズマピーアール", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-23", "postal_code": "1028025", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028503','{"jis": "13101", "kana": "カブシキガイシヤ オリエントコ-ポレ-シヨン", "name": "株式会社　オリエントコーポレーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "5丁目2-1", "postal_code": "1028503", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028504','{"jis": "13101", "kana": "カブシキガイシヤ オリエントコ-ポレ-シヨン シユトケンカンリセンタ-", "name": "株式会社　オリエントコーポレーション　首都圏管理センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "5丁目2-1", "postal_code": "1028504", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028301','{"jis": "13101", "kana": "カブシキガイシヤ カ-・アンド・ドライバ-", "name": "株式会社　カー・アンド・ドライバー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "4丁目6-1九段シルバーパレス706号", "postal_code": "1028301", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028622','{"jis": "13101", "kana": "カブシキガイシヤ カ-ビユ-", "name": "株式会社　カービュー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1番3号東京ガーデンテラス紀尾井町紀尾井タワー22階", "postal_code": "1028622", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1028191','{"jis": "13101", "kana": "カブシキガイシヤ カテイガホウビジネスパ-トナ-ズ", "name": "株式会社　家庭画報ビジネスパートナーズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028191", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028685','{"jis": "13101", "kana": "カブシキガイシヤ カドカワヘラルド・ピクチヤ-ズ", "name": "株式会社　角川ヘラルド・ピクチャーズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-6紀尾井町パークビル8F", "postal_code": "1028685", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028540','{"jis": "13101", "kana": "カブシキガイシヤ カンキシユツパン", "name": "株式会社　かんき出版", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "4丁目1-4西脇ビル", "postal_code": "1028540", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028228','{"jis": "13101", "kana": "カブシキガイシヤ カント-", "name": "株式会社　カントー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "1丁目11-2", "postal_code": "1028228", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028522','{"jis": "13101", "kana": "カブシキガイシヤ キヨウドウセンデン", "name": "株式会社　協同宣伝", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "3-8泉館三番町", "postal_code": "1028522", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028152','{"jis": "13101", "kana": "カブシキガイシヤ ケンキユウシヤホンシヤ", "name": "株式会社　研究社本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目11-3", "postal_code": "1028152", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028230','{"jis": "13101", "kana": "カブシキガイシヤ コ-エ-テクモゲ-ムス", "name": "株式会社　コーエーテクモゲームス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-1-34九段明善堂ビル", "postal_code": "1028230", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028515','{"jis": "13101", "kana": "カブシキガイシヤ サンケイリビングシンブンシヤ", "name": "株式会社　サンケイリビング新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-23文芸春秋ビル新館", "postal_code": "1028515", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
@@ -125799,18 +125733,15 @@
 INSERT INTO office_data VALUES('1028221','{"jis": "13101", "kana": "カブシキガイシヤ ジエイコミツクテラス", "name": "株式会社　Ｊコミックテラス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1-3東京ガーデンテラス紀尾井町紀尾井タワー21階", "postal_code": "1028221", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028612','{"jis": "13101", "kana": "カブシキガイシヤ スイチユウゾウケイセンタ-", "name": "株式会社　水中造形センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1-7相互半蔵門ビル2F", "postal_code": "1028612", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028558','{"jis": "13101", "kana": "カブシキガイシヤ スタツフ.サ-ビス チヨダシシヤ", "name": "株式会社　スタッフ・サービス　千代田支社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-12", "postal_code": "1028558", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028488','{"jis": "13101", "kana": "カブシキガイシヤ スポ-ツマ-ケテイングプロパテイ-ズ", "name": "株式会社　スポーツマーケティングプロパティーズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "1丁目11-5森会館", "postal_code": "1028488", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028528','{"jis": "13101", "kana": "カブシキガイシヤ セイサンニホンシヤ", "name": "株式会社　生産日本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "3-2", "postal_code": "1028528", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028187','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカシヤ", "name": "株式会社　世界文化社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4丁目2-29", "postal_code": "1028187", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028195','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカブツクス", "name": "株式会社　世界文化ブックス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028195", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
-INSERT INTO office_data VALUES('1028194','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカライフケア", "name": "株式会社　世界文化ライフケア", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028194", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
-INSERT INTO office_data VALUES('1028191','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカリテイリング", "name": "株式会社　世界文化リテイリング", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028191", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
-INSERT INTO office_data VALUES('1028192','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカワンダ-クリエイト", "name": "株式会社　世界文化ワンダークリエイト", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028192", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
-INSERT INTO office_data VALUES('1028193','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカワンダ-ハンバイ", "name": "株式会社　世界文化ワンダー販売", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028193", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
+INSERT INTO office_data VALUES('1028192','{"jis": "13101", "kana": "カブシキガイシヤ セカイブンカワンダ-グル-プ", "name": "株式会社　世界文化ワンダーグループ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028192", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028437','{"jis": "13101", "kana": "カブシキガイシヤ セブン・カ-ドサ-ビス", "name": "株式会社　セブン・カードサービス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "4-5", "postal_code": "1028437", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028426','{"jis": "13101", "kana": "カブシキガイシヤ セブン・ミ-ルサ-ビス", "name": "株式会社　セブン・ミールサービス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028426", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028455','{"jis": "13101", "kana": "カブシキガイシヤ セブン-イレブン・ジヤパン", "name": "株式会社　セブン―イレブン・ジャパン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028455", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028452','{"jis": "13101", "kana": "カブシキガイシヤ セブンアンドアイ・ホ-ルデイングス", "name": "株式会社　セブン＆アイ・ホールディングス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028452", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028466','{"jis": "13101", "kana": "カブシキガイシヤ セブンドリ-ム・ドツトコム", "name": "株式会社　セブンドリーム・ドットコム", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028466", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028211','{"jis": "13101", "kana": "カブシキガイシヤ センシユウ", "name": "株式会社　千修", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4丁目2-4", "postal_code": "1028211", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028627','{"jis": "13101", "kana": "カブシキガイシヤ ゼンニホンツウキヨウ", "name": "株式会社　全日本通教", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "3丁目5番9号", "postal_code": "1028627", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
@@ -125846,17 +125777,19 @@
 INSERT INTO office_data VALUES('1028520','{"jis": "13101", "kana": "カブシキガイシヤ ミカミ", "name": "株式会社　ミカミ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1丁目10-1", "postal_code": "1028520", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028582','{"jis": "13101", "kana": "カブシキガイシヤ ミスミ", "name": "株式会社　ミスミ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028582", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028343','{"jis": "13101", "kana": "カブシキガイシヤ ミスミ カスタマ-・サ-ビス・センタ-", "name": "株式会社　ミスミ　カスタマー・サービス・センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028343", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028583','{"jis": "13101", "kana": "カブシキガイシヤ ミスミグル-プホンシヤ", "name": "株式会社　ミスミグループ本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028583", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028621','{"jis": "13101", "kana": "カブシキガイシヤ ミライケンセツグル-プ", "name": "株式会社　みらい建設グループ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "1丁目4-9", "postal_code": "1028621", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028372','{"jis": "13101", "kana": "カブシキガイシヤ メイコウシヨウカイ", "name": "株式会社　明光商会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "五番町", "banchi": "1-1", "postal_code": "1028372", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ゴバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028642','{"jis": "13101", "kana": "カブシキガイシヤ ユ-ラシアリヨコウシヤ", "name": "株式会社　ユーラシア旅行社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目7-4", "postal_code": "1028642", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1028417','{"jis": "13101", "kana": "カブシキガイシヤ ヨ-クマ-ト", "name": "株式会社　ヨークマート", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028417", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1028417','{"jis": "13101", "kana": "カブシキガイシヤ ヨ-ク", "name": "株式会社　ヨーク", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028417", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028609','{"jis": "13101", "kana": "カブシキガイシヤ ヨミウリジヨウホウカイハツ ヨミウリフアミリ-・サ-クル", "name": "株式会社　読売情報開発　読売ファミリー・サークル", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目13-3", "postal_code": "1028609", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028401','{"jis": "13101", "kana": "カブシキガイシヤ リビングプロシ-ド", "name": "株式会社　リビングプロシード", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-23文芸春秋ビル新館", "postal_code": "1028401", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1028194','{"jis": "13101", "kana": "カブシキガイシヤ ワンダ-ウエルネス", "name": "株式会社　ワンダーウェルネス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028194", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
+INSERT INTO office_data VALUES('1028193','{"jis": "13101", "kana": "カブシキガイシヤ ワンダ-ネツトワ-ク", "name": "株式会社　ワンダーネットワーク", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028193", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028357','{"jis": "13101", "kana": "ガツコウホウジン オオツマガクイン オオツマジヨシダイガク オオツマジヨシダイガクタンキダイガクブ オオツマチユウガツコウ オオツマコウトウガツコウ", "name": "学校法人　大妻学院　大妻女子大学　大妻女子大学短期大学部　大妻中学校　大妻高等学校", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "12番地", "postal_code": "1028357", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028178','{"jis": "13101", "kana": "ガツコウホウジン カエツガクエン", "name": "学校法人　嘉悦学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目15-1", "postal_code": "1028178", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028185','{"jis": "13101", "kana": "ガツコウホウジン シラユリガクエン", "name": "学校法人　白百合学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "2丁目4-1", "postal_code": "1028185", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028341','{"jis": "13101", "kana": "ガツコウホウジン トウキヨウカセイガクイン", "name": "学校法人　東京家政学院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "22", "postal_code": "1028341", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028336','{"jis": "13101", "kana": "ガツコウホウジン ニシヨウガクシヤ", "name": "学校法人　二松学舎", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "6-16", "postal_code": "1028336", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028470','{"jis": "13101", "kana": "ガツコウホウジン フタバガクエン", "name": "学校法人　雙葉学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "六番町", "banchi": "14-1", "postal_code": "1028470", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ロクバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028628','{"jis": "13101", "kana": "キンデン トウキヨウホンシヤ", "name": "きんでん　東京本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "2丁目1-21", "postal_code": "1028628", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
@@ -125908,15 +125841,15 @@
 INSERT INTO office_data VALUES('1028610','{"jis": "13101", "kana": "セイカツキヨウドウクミアイゼンコクトシシヨクインサイガイキヨウサイカイ", "name": "生活協同組合全国都市職員災害共済会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目4-2全国都市会館内", "postal_code": "1028610", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028645','{"jis": "13101", "kana": "セコムソンガイホケン カブシキガイシヤ", "name": "セコム損害保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目6-2", "postal_code": "1028645", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028125','{"jis": "13101", "kana": "セントラルソウゴウカイハツ カブシキガイシヤ", "name": "セントラル総合開発　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "3丁目3番7号", "postal_code": "1028125", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028120','{"jis": "13101", "kana": "ゼネラルエレクトリツクキヤピタルカ-システム カブシキガイシヤ", "name": "ゼネラルエレクトリックキャピタルカーシステム　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "1丁目12-7", "postal_code": "1028120", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028630','{"jis": "13101", "kana": "ゼンコクキヨウサイノウギヨウキヨウドウクミアイレンゴウカイ ゼンコクホンブ", "name": "全国共済農業協同組合連合会　全国本部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目7番9号JA共済ビル", "postal_code": "1028630", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028016','{"jis": "13101", "kana": "ゼンコクケンコウホケンキヨウカイ センインホケンブ", "name": "全国健康保険協会　船員保険部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目7-2ステージビルディング14階", "postal_code": "1028016", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028635','{"jis": "13101", "kana": "ゼンコクシチヨウカイ", "name": "全国市長会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目4-2", "postal_code": "1028635", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1028532','{"jis": "13101", "kana": "ゼンコクドボクケンチク コクミンケンコウホケンクミアイ カントウジムシヨ", "name": "全国土木建築　国民健康保険組合　関東事務所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "一丁目五番九号厚生会館", "postal_code": "1028532", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1028532','{"jis": "13101", "kana": "ゼンコクドボクケンチク コクミンケンコウホケンクミアイ カントウジムシヨ", "name": "全国土木建築　国民健康保険組合　関東事務所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "一丁目五番九号厚生会館", "postal_code": "1028532", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028564','{"jis": "13101", "kana": "ゼンコクドボクケンチクコクミンケンコウホケンクミアイ", "name": "全国土木建築国民健康保険組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "1-5-9厚生会館", "postal_code": "1028564", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028464','{"jis": "13101", "kana": "ゼンニホンジチダンタイ ロウドウクミアイ", "name": "全日本自治団体　労働組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "六番町", "banchi": "1", "postal_code": "1028464", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ロクバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028795','{"jis": "13101", "kana": "ソウムシヨウ カントウソウゴウツウシンキヨク", "name": "総務省　関東総合通信局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "1丁目2-1", "postal_code": "1028795", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028170','{"jis": "13101", "kana": "タカヤマコウギヨウ カブシキガイシヤ", "name": "高山工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "1丁目11-21", "postal_code": "1028170", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028430','{"jis": "13101", "kana": "ダイイチカサイカイジヨウホケン ソウゴガイシヤ", "name": "第一火災海上保険　相互会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "5-1", "postal_code": "1028430", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028175','{"jis": "13101", "kana": "ダイダン カブシキガイシヤ トウキヨウホンシヤ", "name": "ダイダン　株式会社　東京本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目15-10", "postal_code": "1028175", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028730','{"jis": "13101", "kana": "ダイトロン カブシキガイシヤ", "name": "ダイトロン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "3丁目6番地住友不動産麹町ビル3号館", "postal_code": "1028730", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
@@ -126263,15 +126196,15 @@
 INSERT INTO office_data VALUES('1048178','{"jis": "13102", "kana": "カブシキガイシヤ ジジツウシンシヤ", "name": "株式会社　時事通信社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "5丁目15-8", "postal_code": "1048178", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048142','{"jis": "13102", "kana": "カブシキガイシヤ ジヤパン・エンタ-テイメント・ネツトワ-ク", "name": "株式会社　ジャパン・エンターテイメント・ネットワーク", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "6-18-2銀座MTR11階", "postal_code": "1048142", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048266','{"jis": "13102", "kana": "カブシキガイシヤ スズノヤ", "name": "株式会社　鈴乃屋", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目6-1", "postal_code": "1048266", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048138','{"jis": "13102", "kana": "カブシキガイシヤ ゼアリズ", "name": "株式会社　ゼアリズ", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "4丁目14-19第2カタヤマビル4F", "postal_code": "1048138", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048685','{"jis": "13102", "kana": "カブシキガイシヤ テイコクデ-タバンクビジネスサ-ビス", "name": "株式会社　帝国データバンクビジネスサービス", "prefecture": "東京都", "city": "中央区", "neighborhood": "新富", "banchi": "1丁目12-2(晴海郵便局私書箱第4号)", "postal_code": "1048685", "old_code": "104  ", "post_office": "晴海", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シントミ", "alternates": []}');
 INSERT INTO office_data VALUES('1008617','{"jis": "13102", "kana": "カブシキガイシヤ デツク", "name": "株式会社　デック", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "6丁目3-12(銀座郵便局私書箱第666号)", "postal_code": "1008617", "old_code": "104  ", "post_office": "銀座", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048210','{"jis": "13102", "kana": "カブシキガイシヤ デンツウパブリツクリレ-シヨンズ", "name": "株式会社　電通パブリックリレーションズ", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "2丁目16-7", "postal_code": "1048210", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
-INSERT INTO office_data VALUES('1048171','{"jis": "13102", "kana": "カブシキガイシヤ デンツウマクロミルインサイト", "name": "株式会社　電通マクロミルインサイト", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "7-4-17", "postal_code": "1048171", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
+INSERT INTO office_data VALUES('1048171','{"jis": "13102", "kana": "カブシキガイシヤ デンツウマクロミルインサイト", "name": "株式会社　電通マクロミルインサイト", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "四丁目7番5号", "postal_code": "1048171", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048161','{"jis": "13102", "kana": "カブシキガイシヤ デンツウメイテツコミユニケ-シヨンズ", "name": "株式会社　電通名鉄コミュニケーションズ", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "2丁目6番7号電通恒産第3ビル", "postal_code": "1048161", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048150','{"jis": "13102", "kana": "カブシキガイシヤ トウキヨウソワ-ル", "name": "株式会社　東京ソワール", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "7-16-12G-7ビルディング7F", "postal_code": "1048150", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048415','{"jis": "13102", "kana": "カブシキガイシヤ トウキヨウニユ-ス ツウシンシヤ", "name": "株式会社　東京ニュース　通信社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "7丁目16番3号日鐵木換ビル", "postal_code": "1048415", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048004','{"jis": "13102", "kana": "カブシキガイシヤ トウキヨウニユ-スツウシンシヤ", "name": "株式会社　東京ニュース通信社", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5丁目3-3築地浜離宮ビル", "postal_code": "1048004", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048183','{"jis": "13102", "kana": "カブシキガイシヤ トウセイシヤ", "name": "株式会社　東成社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "8丁目10-7東成ビル5F", "postal_code": "1048183", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048335','{"jis": "13102", "kana": "カブシキガイシヤ トモエガワセイシジヨ", "name": "株式会社　巴川製紙所", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目1番3号京橋トラストタワー7階", "postal_code": "1048335", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048431','{"jis": "13102", "kana": "カブシキガイシヤ ナカムラジコウ", "name": "株式会社　中村自工", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "3丁目10番10号築地ナジコビル", "postal_code": "1048431", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
@@ -126362,15 +126295,14 @@
 INSERT INTO office_data VALUES('1048381','{"jis": "13102", "kana": "ト-ヨ-カラ- カブシキガイシヤ", "name": "トーヨーカラー　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2-2-1", "postal_code": "1048381", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048379','{"jis": "13102", "kana": "ト-ヨ-ケム カブシキガイシヤ", "name": "トーヨーケム　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2-1", "postal_code": "1048379", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048108','{"jis": "13102", "kana": "トウエイ カブシキガイシヤ", "name": "東映　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "3丁目2-17", "postal_code": "1048108", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048317','{"jis": "13102", "kana": "トウカイトウキヨウシヨウケン カブシキガイシヤ", "name": "東海東京証券　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目17-21茅場町ファーストビル", "postal_code": "1048317", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048151','{"jis": "13102", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ", "name": "東京海上日動火災保険　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "5丁目13番7号", "postal_code": "1048151", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048405','{"jis": "13102", "kana": "トウキヨウキヨウクキヨウムシヨ", "name": "東京教区教務所", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "3丁目15-1築地本願寺内", "postal_code": "1048405", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048449','{"jis": "13102", "kana": "トウキヨウコクゼイキヨク", "name": "東京国税局", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5丁目3番1号", "postal_code": "1048449", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
-INSERT INTO office_data VALUES('1048470','{"jis": "13102", "kana": "トウキヨウシンヨウホシヨウキヨウカイ", "name": "東京信用保証協会", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "2丁目6-17", "postal_code": "1048470", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1048133','{"jis": "13102", "kana": "トウキヨウデンリヨク カブシキガイシヤ ギンザシテン", "name": "東京電力　株式会社　銀座支店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "3丁目3-18", "postal_code": "1048133", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048404','{"jis": "13102", "kana": "トウキヨウトチユウオウクヤクシヨ", "name": "東京都中央区役所", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "1丁目1番1号", "postal_code": "1048404", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048558','{"jis": "13102", "kana": "トウキヨウトチユウオウトゼイジムシヨ", "name": "東京都中央都税事務所", "prefecture": "東京都", "city": "中央区", "neighborhood": "新富", "banchi": "2丁目6番1号", "postal_code": "1048558", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シントミ", "alternates": []}');
 INSERT INTO office_data VALUES('1048378','{"jis": "13102", "kana": "トウヨウインキ カブシキガイシヤ", "name": "東洋インキ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2-1", "postal_code": "1048378", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048377','{"jis": "13102", "kana": "トウヨウインキエスシ-ホ-ルデイングス カブシキガイシヤ", "name": "東洋インキＳＣホールディングス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2-1", "postal_code": "1048377", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048678','{"jis": "13102", "kana": "トウヨウシヨウケン カブシキガイシヤ", "name": "東洋証券　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "4丁目7番1号(晴海郵便局私書箱第15号)", "postal_code": "1048678", "old_code": "104  ", "post_office": "晴海", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048324','{"jis": "13102", "kana": "トウヨウネツコウギヨウ カブシキガイシヤ", "name": "東洋熱工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目5番12号", "postal_code": "1048324", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
@@ -126579,18 +126511,17 @@
 INSERT INTO office_data VALUES('1058555','{"jis": "13103", "kana": "ニチアス カブシキガイシヤ", "name": "ニチアス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝大門", "banchi": "1丁目1-26", "postal_code": "1058555", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバダイモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058567','{"jis": "13103", "kana": "ニツシヨウサンギヨウ カブシキガイシヤ", "name": "日昭産業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目3-13ヒューリック神谷町ビル4階", "postal_code": "1058567", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058411','{"jis": "13103", "kana": "ニツセイ カブシキガイシヤ", "name": "日精　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目18-17明産西新橋ビル", "postal_code": "1058411", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058681','{"jis": "13103", "kana": "ニツポンケイキンゾクグル-プ", "name": "日本軽金属グループ", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "1丁目1番13号アーバンネット内幸町ビル", "postal_code": "1058681", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058322','{"jis": "13103", "kana": "ニツポンツウウン カブシキガイシヤ", "name": "日本通運　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目9-3", "postal_code": "1058322", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058540','{"jis": "13103", "kana": "ニツポンデンキ カブシキガイシヤ セレステインビル", "name": "日本電気　株式会社　セレスティンビル", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3-23-1セレスティン芝三井ビルディング", "postal_code": "1058540", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058456','{"jis": "13103", "kana": "ニツポンポラロイド カブシキガイシヤ", "name": "日本ポラロイド　（株）", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "3丁目18-19虎ノ門マリンビル", "postal_code": "1058456", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
-INSERT INTO office_data VALUES('1058617','{"jis": "13103", "kana": "ニツポンユウセイ カブシキガイシヤ シユクハクジギヨウブ", "name": "日本郵政　株式会社　宿泊事業部", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "6-19-15", "postal_code": "1058617", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058788','{"jis": "13103", "kana": "ニツポンユウセイ カブシキガイシヤ シユトケンシセツセンタ-", "name": "日本郵政　株式会社　首都圏施設センター", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "3丁目17番1号TOKYUREIT虎ノ門ビル7階", "postal_code": "1058788", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058408','{"jis": "13103", "kana": "ニホンギジユツボウエキ カブシキガイシヤ", "name": "日本技術貿易　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目7-13虎ノ門イーストビルディング", "postal_code": "1058408", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1058467','{"jis": "13103", "kana": "ニホンコクドカイハツ (カ)", "name": "日本国土開発　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目3-13ヒューリック神谷町ビル5F", "postal_code": "1058467", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
+INSERT INTO office_data VALUES('1058467','{"jis": "13103", "kana": "ニホンコクドカイハツ (カ)", "name": "日本国土開発　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目3-13ヒューリック神谷町ビル5F", "postal_code": "1058467", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058521','{"jis": "13103", "kana": "ニホンセキジユウジシヤ", "name": "日本赤十字社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝大門", "banchi": "1丁目1-3", "postal_code": "1058521", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバダイモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058508','{"jis": "13103", "kana": "ニホンタタ・コンサルタンシ-・サ-ビシズ カブシキガイシヤ", "name": "日本タタ・コンサルタンシー・サービシズ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "4丁目1番4号", "postal_code": "1058508", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1057444','{"jis": "13103", "kana": "ニホンテレビホウソウモウ カブシキガイシヤ", "name": "日本テレビ放送網　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目6-1", "postal_code": "1057444", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058457','{"jis": "13103", "kana": "ニホンデスコ カブシキガイシヤ", "name": "日本デスコ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目3-13秀和神谷町ビル", "postal_code": "1058457", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058578','{"jis": "13103", "kana": "ニホンビジネスシステムズ カブシキガイシヤ", "name": "日本ビジネスシステムズ　（株）", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目8番2号芝公園ファーストビル13F", "postal_code": "1058578", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058579','{"jis": "13103", "kana": "ニホンマスタ-トラストシンタクギンコウ カブシキガイシヤ", "name": "日本マスタートラスト信託銀行　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "浜松町", "banchi": "2丁目11-3MTBJビル", "postal_code": "1058579", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ハママツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1058301','{"jis": "13103", "kana": "パナソニツク カブシキガイシヤ", "name": "パナソニック　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目5-1", "postal_code": "1058301", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
@@ -126608,14 +126539,15 @@
 INSERT INTO office_data VALUES('1058466','{"jis": "13103", "kana": "ミツイシヨクヒン カブシキガイシヤ", "name": "三井食品　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目1番1号", "postal_code": "1058466", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058574','{"jis": "13103", "kana": "ミツイスミトモシンタクギンコウ カブシキガイシヤ", "name": "三井住友信託銀行　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3-33-1", "postal_code": "1058574", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058464','{"jis": "13103", "kana": "ミツイスミトモフアイナンスアンドリ-ス カブシキガイシヤ", "name": "三井住友ファイナンス＆リース　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "3丁目9-4", "postal_code": "1058464", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058427','{"jis": "13103", "kana": "ミツイノウリン カブシキガイシヤ", "name": "三井農林　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目2-9日比谷セントラルビル", "postal_code": "1058427", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058712','{"jis": "13103", "kana": "ミツビシエイチシ-キヤピタル カブシキガイシヤ", "name": "三菱ＨＣキャピタル　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目3番1号", "postal_code": "1058712", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058501','{"jis": "13103", "kana": "ミツビシユ-エフジエイリサ-チアンドコンサルテイング カブシキガイシヤ", "name": "三菱ＵＦＪリサーチ＆コンサルティング　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "5丁目11番2号", "postal_code": "1058501", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058516','{"jis": "13103", "kana": "ミナトクシバウラコウナンチク ソウゴウシシヨ", "name": "港区芝浦港南地区　総合支所", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目16番1号", "postal_code": "1058516", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
+INSERT INTO office_data VALUES('1058317','{"jis": "13103", "kana": "ミネベアミツミ カブシキガイシヤ", "name": "ミネベアミツミ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1-9-3", "postal_code": "1058317", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058437','{"jis": "13103", "kana": "ミハマ カ)", "name": "美浜　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "1丁目2-8虎ノ門琴平タワー18階", "postal_code": "1058437", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058510','{"jis": "13103", "kana": "ミワロツク カブシキガイシヤ", "name": "美和ロック　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目1-12", "postal_code": "1058510", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058582','{"jis": "13103", "kana": "メルパルク トウキヨウ", "name": "メルパルク　ＴＯＫＹＯ", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "2丁目5-20", "postal_code": "1058582", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1058451','{"jis": "13103", "kana": "モリムラシヨウジ カブシキガイシヤ", "name": "森村商事　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目1番28号虎ノ門タワーズオフィス", "postal_code": "1058451", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058686','{"jis": "13103", "kana": "ヤシマデンキ カブシキガイシヤ", "name": "八洲電機　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "3丁目1番1号", "postal_code": "1058686", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058577','{"jis": "13103", "kana": "ユ-シ-シ-ウエシマコ-ヒ- カブシキガイシヤ トウキヨウホンブ", "name": "ＵＣＣ上島珈琲　株式会社　東京本部", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "6丁目1-11タウィンチ御成門", "postal_code": "1058577", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058449','{"jis": "13103", "kana": "ユ-ビ-イ- カブシキカイシヤ", "name": "ＵＢＥ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目2番1号シーバンスN館20階", "postal_code": "1058449", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
@@ -126809,15 +126741,14 @@
 INSERT INTO office_data VALUES('1088707','{"jis": "13103", "kana": "イツパンザイダンホウジン ニツポンモ-タ-ボ-トキヨウソウカイ", "name": "一般財団法人　日本モーターボート競走会", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3丁目12-12(高輪郵便局私書箱第18号)", "postal_code": "1088707", "old_code": "108  ", "post_office": "高輪", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088525','{"jis": "13103", "kana": "イトウチユウエネクス カブシキガイシヤ", "name": "伊藤忠エネクス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3丁目4-1グランパークタワー", "postal_code": "1088525", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088373','{"jis": "13103", "kana": "ウツノミヤラシ カブシキガイシヤ", "name": "宇都宮螺子　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "4丁目6-5", "postal_code": "1088373", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088566','{"jis": "13103", "kana": "エイ・エイ・ピ-・シ-・ジヤパン カブシキガイシヤ プルマントウキヨウタマチ", "name": "エイ・エイ・ピー・シー・ジャパン　株式会社　プルマン東京田町", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3丁目1番21号", "postal_code": "1088566", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1086350','{"jis": "13103", "kana": "エスエムビ-シ-フアイナンスサ-ビス カブシキガイシヤ", "name": "ＳＭＢＣファイナンスサービス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3丁目5-27住友不動産三田ツインビル西館7階", "postal_code": "1086350", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088118','{"jis": "13103", "kana": "エヌ・テイ・テイ・コミユニケ-シヨンズ カブシキガイシヤ", "name": "エヌ・ティ・ティ・コミュニケーションズ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3-4-1グランパークタワー", "postal_code": "1088118", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088202','{"jis": "13103", "kana": "エヌ・テイ・テイ・テクノクロス カブシキガイシヤ", "name": "ＮＴＴテクノクロス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3-4-1田町グランパークタワー15F", "postal_code": "1088202", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
-INSERT INTO office_data VALUES('1088338','{"jis": "13103", "kana": "エヌイ-シ-ネクサソリユ-シヨンズカブシキガイシヤ", "name": "ＮＥＣネクサソリューションズ（株）", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4-28三田国際ビル", "postal_code": "1088338", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088515','{"jis": "13103", "kana": "エヌイ-シ-ネツツエスアイ カブシキガイシヤ", "name": "ＮＥＣネッツエスアイ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "三丁目9番14号", "postal_code": "1088515", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088005','{"jis": "13103", "kana": "エネオス カブシキガイシヤ", "name": "ＥＮＥＯＳ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-8-15Wビル", "postal_code": "1088005", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088212','{"jis": "13103", "kana": "エフ・デイ-・ケイ カブシキカイシヤ", "name": "ＦＤＫ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-6-41品川クリスタルスクエア8F", "postal_code": "1088212", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088361','{"jis": "13103", "kana": "オ-ストラリアタイシカン オ-ストラリアエンバシイ", "name": "オーストラリア大使館　ＡＵＳＴＲＡＬＩＡＮ　ＥＭＢＡＳＳＹ", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "2丁目1-14", "postal_code": "1088361", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088242','{"jis": "13103", "kana": "オオツカセイヤク カブシキガイシヤ", "name": "大塚製薬　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16番4号品川グランドセントラルタワー", "postal_code": "1088242", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088241','{"jis": "13103", "kana": "オオツカホ-ルデイングス カブシキガイシヤ", "name": "大塚ホールディングス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16-4品川グランドセントラルタワー", "postal_code": "1088241", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088551','{"jis": "13103", "kana": "オキデンキコウギヨウ カブシキガイシヤ", "name": "沖電気工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "4丁目10-16", "postal_code": "1088551", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
@@ -126875,14 +126806,15 @@
 INSERT INTO office_data VALUES('1088530','{"jis": "13103", "kana": "カンサホウジン ト-マツ", "name": "監査法人　トーマツ", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "4丁目13-23", "postal_code": "1088530", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088203','{"jis": "13103", "kana": "ガイコクジンギノウジツシユウキコウ トウキヨウジムシヨ", "name": "外国人技能実習機構　東京事務所", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1丁目6番31号品川東急ビル", "postal_code": "1088203", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088641','{"jis": "13103", "kana": "ガツコウホウジン キタサトケンキユウシヨ", "name": "学校法人　北里研究所", "prefecture": "東京都", "city": "港区", "neighborhood": "白金", "banchi": "5丁目9-1", "postal_code": "1088641", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シロカネ", "alternates": []}');
 INSERT INTO office_data VALUES('1088642','{"jis": "13103", "kana": "キタサトケンキユウシヨビヨウイン", "name": "北里研究所病院", "prefecture": "東京都", "city": "港区", "neighborhood": "白金", "banchi": "5丁目9-1", "postal_code": "1088642", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シロカネ", "alternates": []}');
 INSERT INTO office_data VALUES('1088225','{"jis": "13103", "kana": "キヤノンシステムアンドサポ-ト カブシキガイシヤ", "name": "キヤノンシステムアンドサポート　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2-16-6", "postal_code": "1088225", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088011','{"jis": "13103", "kana": "キヤノンマ-ケテイングジヤパン カブシキガイシヤ", "name": "キヤノンマーケティングジャパン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16-6", "postal_code": "1088011", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088234','{"jis": "13103", "kana": "キヨウエイシヨクサン (カブ) トウキヨウエイギヨウシヨ", "name": "共栄殖産　（株）　東京営業所", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目18-1", "postal_code": "1088234", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
+INSERT INTO office_data VALUES('1088316','{"jis": "13103", "kana": "キヨウセラ カブシキガイシヤ トウキヨウジギヨウシヨ", "name": "京セラ　株式会社　東京事業所", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "三丁目5番19号", "postal_code": "1088316", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088080','{"jis": "13103", "kana": "クラシエホ-ルデイングス カブシキガイシヤ", "name": "クラシエホールディングス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "3丁目20-20", "postal_code": "1088080", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
 INSERT INTO office_data VALUES('1088448','{"jis": "13103", "kana": "クリバヤシウンユ カブシキガイシヤ", "name": "栗林運輸　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "3丁目22-34", "postal_code": "1088448", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
 INSERT INTO office_data VALUES('1088345','{"jis": "13103", "kana": "ケイオウギジユク", "name": "慶應義塾", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "2丁目15-45", "postal_code": "1088345", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088201','{"jis": "13103", "kana": "ケイデイ-デイ-アイ カブシキガイシヤ", "name": "ＫＤＤＩ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16-1", "postal_code": "1088201", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088456','{"jis": "13103", "kana": "ケイヒン カブシキガイシヤ", "name": "ケイヒン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "3丁目4-20", "postal_code": "1088456", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
 INSERT INTO office_data VALUES('1088206','{"jis": "13103", "kana": "コウエキザイダンホウジン ジエ-ケ-エ-", "name": "公益財団法人　ＪＫＡ", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1丁目2番70号品川シーズンテラス25階", "postal_code": "1088206", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088329','{"jis": "13103", "kana": "コクサイイリヨウフクシダイガクフゾクミタビヨウイン", "name": "国際医療福祉大学附属三田病院", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4-3", "postal_code": "1088329", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
@@ -126965,15 +126897,14 @@
 INSERT INTO office_data VALUES('1088248','{"jis": "13103", "kana": "マクセル カブシキガイシヤ", "name": "マクセル　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16番2号", "postal_code": "1088248", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088411','{"jis": "13103", "kana": "ミツビシオ-トリ-ス カブシキガイシヤ", "name": "三菱オートリース　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5丁目34-7", "postal_code": "1088411", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088415','{"jis": "13103", "kana": "ミツビシカガクメデイア カブシキガイシヤ", "name": "三菱化学メディア　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "4丁目1-23", "postal_code": "1088415", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088410','{"jis": "13103", "kana": "ミツビシジドウシヤコウギヨウ カブシキガイシヤ", "name": "三菱自動車工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3丁目1番21号田町ステーションタワーS", "postal_code": "1088410", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088407','{"jis": "13103", "kana": "ミツビシジドウシヤフアイナンス カブシキガイシヤ", "name": "三菱自動車ファイナンス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3-1-21田町ステーションタワーS29階", "postal_code": "1088407", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088215','{"jis": "13103", "kana": "ミツビシジユウコウギヨウ カブシキガイシヤ", "name": "三菱重工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16番5号", "postal_code": "1088215", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088315','{"jis": "13103", "kana": "ミナトク ミナトホケンジヨ", "name": "港区　みなと保健所", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4番10号", "postal_code": "1088315", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
-INSERT INTO office_data VALUES('1088330','{"jis": "13103", "kana": "ミネベアミツミ カブシキガイシヤ", "name": "ミネベアミツミ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3丁目9番6号", "postal_code": "1088330", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088636','{"jis": "13103", "kana": "メイジガクインダイガク", "name": "明治学院大学", "prefecture": "東京都", "city": "港区", "neighborhood": "白金台", "banchi": "1丁目2-37", "postal_code": "1088636", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シロカネダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1088403','{"jis": "13103", "kana": "モリナガセイカ カブシキガイシヤ", "name": "森永製菓　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5丁目33-1", "postal_code": "1088403", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088384','{"jis": "13103", "kana": "モリナガニユウギヨウ カブシキガイシヤ", "name": "森永乳業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5丁目33-1", "postal_code": "1088384", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088333','{"jis": "13103", "kana": "ヤザキソウギヨウ カブシキガイシヤ", "name": "矢崎総業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4-28", "postal_code": "1088333", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088568','{"jis": "13103", "kana": "ヤマハ カブシキガイシヤ トウキヨウエイギヨウジムシヨ", "name": "ヤマハ　株式会社　東京営業事務所", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "2丁目17-11", "postal_code": "1088568", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
 INSERT INTO office_data VALUES('1088575','{"jis": "13103", "kana": "ユニ・チヤ-ム カブシキガイシヤ", "name": "ユニ・チャーム　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3丁目5-27住友不動産三田ツインビル西館", "postal_code": "1088575", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088388','{"jis": "13103", "kana": "ヨコハマカセイ カブシキガイシヤ", "name": "横浜化成　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "2-21-43YCC高輪ビル", "postal_code": "1088388", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
@@ -127081,16 +127012,16 @@
 INSERT INTO office_data VALUES('1608522','{"jis": "13104", "kana": "ジヨシガクセイカイカン <メイセン>", "name": "女子学生会館　「明泉」", "prefecture": "東京都", "city": "新宿区", "neighborhood": "南元町", "banchi": "6-2", "postal_code": "1608522", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ミナミモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1608512','{"jis": "13104", "kana": "セイカツキヨウドウクミアイ トウキヨウマイコ-プ", "name": "生活協同組合　東京マイコープ", "prefecture": "東京都", "city": "新宿区", "neighborhood": "四谷", "banchi": "4丁目28-7", "postal_code": "1608512", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨツヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1630831','{"jis": "13104", "kana": "セントラルケイビホシヨウ カブシキガイシヤ", "name": "セントラル警備保障　（株）", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目4-1新宿NSビル", "postal_code": "1630831", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608361','{"jis": "13104", "kana": "ゼンケンホンシヤ カブシキガイシヤ", "name": "全研本社　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6-18-1住友不動産新宿セントラルパークタワー18階・19階", "postal_code": "1608361", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608507','{"jis": "13104", "kana": "ゼンコクケンコウホケンキヨウカイ ホンブ", "name": "全国健康保険協会　本部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "四谷", "banchi": "1丁目6番1号6階", "postal_code": "1608507", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨツヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1608373','{"jis": "13104", "kana": "ゼンホレン カブシキガイシヤ", "name": "全保連　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-24-1エステック情報ビル16F", "postal_code": "1608373", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608583','{"jis": "13104", "kana": "ソウカガツカイ", "name": "創価学会", "prefecture": "東京都", "city": "新宿区", "neighborhood": "信濃町", "banchi": "32", "postal_code": "1608583", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シナノマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1608313','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608313", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('1608338','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608338", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1608313','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608313", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1608338','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608338", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638626','{"jis": "13104", "kana": "ソンポジヤパンニツポンコウアヒマワリセイメイホケン カブシキガイシヤ", "name": "損保ジャパン日本興亜ひまわり生命保険　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6丁目13番1号新宿セントラルパークビル(新宿郵便局私書箱第123号)", "postal_code": "1638626", "old_code": "160  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638639','{"jis": "13104", "kana": "タイセイヤツカコウギヨウ", "name": "大正薬化工業", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "3丁目10-8(新宿郵便局私書箱第343号)", "postal_code": "1638639", "old_code": "160  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608401','{"jis": "13104", "kana": "ダイワシヨウケン カブシキガイシヤ シンジユクシテン", "name": "大和証券　株式会社　新宿支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "3丁目30-11", "postal_code": "1608401", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630663','{"jis": "13104", "kana": "ダイワシヨウケン カブシキガイシヤ シンジユクセンタ-ビルシテン", "name": "大和証券　株式会社　新宿センタービル支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目25-1新宿センタービル", "postal_code": "1630663", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608327','{"jis": "13104", "kana": "チユウオウシヨクギヨウノウリヨクカイハツキヨウカイ", "name": "中央職業能力開発協会", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "7丁目5番25号西新宿木村屋ビルディング", "postal_code": "1608327", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1631053','{"jis": "13104", "kana": "トウキヨウガストシカイハツ カブシキガイシヤ", "name": "東京ガス都市開発　（株）", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3丁目7-1新宿パークタワー", "postal_code": "1631053", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630560','{"jis": "13104", "kana": "トウキヨウジツギヨウケンコウホケンクミアイ ジヨウサイシブ", "name": "東京実業健康保険組合　城西支部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目26-2新宿野村ビル", "postal_code": "1630560", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
@@ -127259,16 +127190,16 @@
 INSERT INTO office_data VALUES('1628717','{"jis": "13104", "kana": "カブシキガイシヤ ガクブンシヤ", "name": "株式会社　学文社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "早稲田町", "banchi": "5-4(牛込郵便局私書箱第77号)", "postal_code": "1628717", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ワセダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628718','{"jis": "13104", "kana": "カブシキガイシヤ ガクブンシヤ", "name": "株式会社　学文社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "早稲田町", "banchi": "5-4(牛込郵便局私書箱第77号)", "postal_code": "1628718", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ワセダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628711','{"jis": "13104", "kana": "カブシキガイシヤ シンチヨウシヤ", "name": "株式会社　新潮社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "矢来町", "banchi": "71(牛込郵便局私書箱第20号)", "postal_code": "1628711", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヤライチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628710','{"jis": "13104", "kana": "カブシキガイシヤ ト-ハン", "name": "株式会社　トーハン", "prefecture": "東京都", "city": "新宿区", "neighborhood": "東五軒町", "banchi": "6-24(牛込郵便局私書箱第5号)", "postal_code": "1628710", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヒガシゴケンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1631537','{"jis": "13104", "kana": "エムエステイホケンサ-ビス (カ", "name": "エムエスティ保険サービス　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-6-1新宿エルタワー10階", "postal_code": "1631537", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630553','{"jis": "13104", "kana": "ケ-オ-デンタル カブシキカイシヤ", "name": "ケーオーデンタル　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-2新宿野村ビル19階(新宿野村ビル内郵便局私書箱第3074号)", "postal_code": "1630553", "old_code": "163  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630287','{"jis": "13104", "kana": "シホウシヨシホウジン チユウオウジムシヨ", "name": "司法書士法人　中央事務所", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2-6-1新宿住友ビル16階", "postal_code": "1630287", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('1638620','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1638620", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('1630261','{"jis": "13104", "kana": "ヒカリビジネスフオ-ム カブシキガイシヤ", "name": "光ビジネスフォーム　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目6番1号新宿住友ビル19階", "postal_code": "1630261", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1638620','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1638620", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1630261','{"jis": "13104", "kana": "ヒカリビジネスフオ-ム カブシキガイシヤ", "name": "光ビジネスフォーム　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目6番1号新宿住友ビル22階", "postal_code": "1630261", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638019','{"jis": "13104", "kana": "ヒガシニホンデンシンデンワ カブシキカイシヤ", "name": "東日本電信電話　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3-19-2", "postal_code": "1638019", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638602','{"jis": "13104", "kana": "ミツビシユ-エフジエイシンタクギンコウ カブシキガイシヤ シンジユクシテン", "name": "三菱ＵＦＪ信託銀行　株式会社　新宿支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-10-2(新宿郵便局私書箱第227号)", "postal_code": "1638602", "old_code": "163  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630575','{"jis": "13104", "kana": "スミコウジユンカツザイ カブシキガイシヤ", "name": "住鉱潤滑剤　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-2新宿野村ビル14階", "postal_code": "1630575", "old_code": "16305", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630570','{"jis": "13104", "kana": "リ-ドエグジビシヨンジヤパン カブシキガイシヤ", "name": "リードエグジビションジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目26-2新宿野村ビル", "postal_code": "1630570", "old_code": "16305", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630727','{"jis": "13104", "kana": "セキスイカセイヒンコウギヨウ カブシキガイシヤ トウキヨウホンブ", "name": "積水化成品工業　株式会社　東京本部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目7-1小田急第一生命ビル", "postal_code": "1630727", "old_code": "16306", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630655','{"jis": "13104", "kana": "テイ-ビイ-シ-グル-プ カブシキガイシヤ", "name": "ＴＢＣグループ　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目25-1新宿センタービル43F", "postal_code": "1630655", "old_code": "16306", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630777','{"jis": "13104", "kana": "カブシキガイシヤ ニツポンシステムデイベロツプメント", "name": "株式会社　日本システムディベロップメント", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目7-1小田急第一生命ビル", "postal_code": "1630777", "old_code": "16307", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
@@ -127586,14 +127517,15 @@
 INSERT INTO office_data VALUES('1108677','{"jis": "13106", "kana": "サンキコウギヨウ カブシキガイシヤ", "name": "三輝工業　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "下谷", "banchi": "3丁目4-4", "postal_code": "1108677", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "シタヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1108550','{"jis": "13106", "kana": "サンキヨウスポ-ツ カブシキガイシヤ", "name": "三共スポーツ　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "1丁目9-3", "postal_code": "1108550", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108555','{"jis": "13106", "kana": "サンデンホ-ルデイングス カブシキガイシヤ トウキヨウホンシヤ", "name": "サンデンホールディングス　株式会社　東京本社", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "1-31-7", "postal_code": "1108555", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108534','{"jis": "13106", "kana": "サンヨウデンキ カブシキガイシヤ", "name": "三洋電機　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "1丁目1-10", "postal_code": "1108534", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108676','{"jis": "13106", "kana": "ザイダンホウジン シゼンカンキヨウケンキユウセンタ-", "name": "財団法人　自然環境研究センター", "prefecture": "東京都", "city": "台東区", "neighborhood": "下谷", "banchi": "3丁目10-10", "postal_code": "1108676", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "シタヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1108687','{"jis": "13106", "kana": "ザイダンホウジン トウキヨウカシカイカン", "name": "（財）東京菓子会館", "prefecture": "東京都", "city": "台東区", "neighborhood": "入谷", "banchi": "1丁目18-7", "postal_code": "1108687", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "イリヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1108645','{"jis": "13106", "kana": "ザイダンホウジン ライフ・エクステンシヨンケンキユウジヨ フゾク エイジユソウゴウビヨウイン", "name": "財団法人　ライフ・エクステンション研究所　附属　永寿総合病院", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "2丁目23-16", "postal_code": "1108645", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
+INSERT INTO office_data VALUES('1108736','{"jis": "13106", "kana": "シマヅダイアグノステイクス カブシキガイシヤ", "name": "島津ダイアグノスティクス　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "3丁目24-6上野フロンティアタワー20階", "postal_code": "1108736", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108567','{"jis": "13106", "kana": "シヤダンホウジン ニホンドウブツエンスイゾクカンキヨウカイ", "name": "社団法人　日本動物園水族館協会", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "4丁目23-10ヴェラハイツ御徒町402号", "postal_code": "1108567", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108723','{"jis": "13106", "kana": "シヨウエイシヨクヒンコウギヨウ カブシキガイシヤ", "name": "正栄食品工業　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "秋葉原", "banchi": "5-7", "postal_code": "1108723", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アキハバラ", "alternates": []}');
 INSERT INTO office_data VALUES('1108576','{"jis": "13106", "kana": "シヨウワシツナイコウギヨウ (カブ)", "name": "昭和室内工業　（株）", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "5丁目23-11スグルビル6F", "postal_code": "1108576", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108620','{"jis": "13106", "kana": "シンメイワコウギヨウ カブシキガイシヤ パ-キングシステムジギヨウブ", "name": "新明和工業　株式会社　パーキングシステム事業部", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "5-16-5新明和上野ビル", "postal_code": "1108620", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108638','{"jis": "13106", "kana": "ジエイ・アキユレ-ト カブシキガイシヤ", "name": "ジェイ・アキュレート　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "6-27-5レジディア上野101", "postal_code": "1108638", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108618','{"jis": "13106", "kana": "ジエイ-ネツトチユウオウ カブシキガイシヤ", "name": "Ｊ－ＮＥＴ中央　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "1丁目6-2", "postal_code": "1108618", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108537','{"jis": "13106", "kana": "スズノヤ", "name": "（株）　鈴乃屋", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "1丁目20-11", "postal_code": "1108537", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
@@ -127611,15 +127543,14 @@
 INSERT INTO office_data VALUES('1108561','{"jis": "13106", "kana": "トウキヨウホウムキヨク タイトウシユツチヨウジヨ", "name": "東京法務局　台東出張所", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "1丁目26-2", "postal_code": "1108561", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108725','{"jis": "13106", "kana": "トウヨウロ-プ カブシキガイシヤ", "name": "東洋ロープ　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "秋葉原", "banchi": "1-10", "postal_code": "1108725", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アキハバラ", "alternates": []}');
 INSERT INTO office_data VALUES('1108586','{"jis": "13106", "kana": "トウワツウシヨウ カブシキガイシヤ", "name": "東和通商　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "1丁目11-3", "postal_code": "1108586", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108685','{"jis": "13106", "kana": "トクダマシモエ-ス カブシキガイシヤ", "name": "トクダマシモエース　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "入谷", "banchi": "2-7-1", "postal_code": "1108685", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "イリヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1108605','{"jis": "13106", "kana": "トクテイヒエイリカツドウホウジン ニホンコクサイボランテイアセンタ-", "name": "特定非営利活動法人　日本国際ボランティアセンター", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "5-22-1東鈴ビル4階", "postal_code": "1108605", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108560','{"jis": "13106", "kana": "トツパンインサツ カブシキガイシヤ", "name": "凸版印刷　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "1丁目5-1", "postal_code": "1108560", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108713','{"jis": "13106", "kana": "ドクリツギヨウセイホウジン ブンカザイケンキユウシヨ トウキヨウブンカザイケンキユウシヨ", "name": "独立行政法人　文化財研究所　東京文化財研究所", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野公園", "banchi": "13-43", "postal_code": "1108713", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノコウエン", "alternates": []}');
-INSERT INTO office_data VALUES('1108736','{"jis": "13106", "kana": "ニツスイセイヤク カブシキガイシヤ", "name": "日水製薬　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "3丁目23-9", "postal_code": "1108736", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108660','{"jis": "13106", "kana": "ニツポンネンキンキコウ ウエノネンキンジムシヨ", "name": "日本年金機構　上野年金事務所", "prefecture": "東京都", "city": "台東区", "neighborhood": "池之端", "banchi": "1-2-18MG池之端ビル", "postal_code": "1108660", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "イケノハタ", "alternates": []}');
 INSERT INTO office_data VALUES('1108686','{"jis": "13106", "kana": "ニホンエア-テツク カブシキガイシヤ", "name": "日本エアーテック　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "入谷", "banchi": "1丁目14-9", "postal_code": "1108686", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "イリヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1108653','{"jis": "13106", "kana": "ニホンツウシンシ カブシキガイシヤ", "name": "日本通信紙　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "下谷", "banchi": "1丁目7番5号", "postal_code": "1108653", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "シタヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1108706','{"jis": "13106", "kana": "ニホンデンセツコウギヨウ カブシキガイシヤ", "name": "日本電設工業　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "池之端", "banchi": "1丁目2-23", "postal_code": "1108706", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "イケノハタ", "alternates": []}');
 INSERT INTO office_data VALUES('1108708','{"jis": "13106", "kana": "ニホンユウセイグル-プロウドウクミアイ", "name": "日本郵政グループ労働組合", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "5丁目2-2", "postal_code": "1108708", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108562','{"jis": "13106", "kana": "ニホンリテイルシステム カブシキガイシヤ", "name": "日本リテイルシステム　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "2丁目1-1東秋葉原ビル", "postal_code": "1108562", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108580','{"jis": "13106", "kana": "ノウリンギヨギヨウダンタイシヨクインキヨウサイクミアイ", "name": "農林漁業団体職員共済組合", "prefecture": "東京都", "city": "台東区", "neighborhood": "秋葉原", "banchi": "2-3日本農業新聞本社ビル3~4F", "postal_code": "1108580", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アキハバラ", "alternates": []}');
@@ -127709,14 +127640,15 @@
 INSERT INTO office_data VALUES('1118560','{"jis": "13106", "kana": "ミツワ カブシキガイシヤ", "name": "ミツワ　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "花川戸", "banchi": "2丁目7-1", "postal_code": "1118560", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ハナカワド", "alternates": []}');
 INSERT INTO office_data VALUES('1118622','{"jis": "13106", "kana": "ミツワサンギヨウ カブシキガイシヤ", "name": "ミツワ産業　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "浅草", "banchi": "6丁目22-2", "postal_code": "1118622", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アサクサ", "alternates": []}');
 INSERT INTO office_data VALUES('1118650','{"jis": "13106", "kana": "ミドリカワカセイコウギヨウ カブシキガイシヤ", "name": "緑川化成工業　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "駒形", "banchi": "1丁目4-18", "postal_code": "1118650", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "コマガタ", "alternates": []}');
 INSERT INTO office_data VALUES('1118575','{"jis": "13106", "kana": "モリト カブシキガイシヤ トウキヨウシシヤ", "name": "モリト　株式会社　東京支社", "prefecture": "東京都", "city": "台東区", "neighborhood": "駒形", "banchi": "2丁目4-8", "postal_code": "1118575", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "コマガタ", "alternates": []}');
 INSERT INTO office_data VALUES('1118648','{"jis": "13106", "kana": "ヤチヨエンジニヤリング カブシキガイシヤ", "name": "八千代エンジニヤリング　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "浅草橋", "banchi": "5丁目20-8CSタワー", "postal_code": "1118648", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アサクサバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1118628','{"jis": "13106", "kana": "ユウゲンガイシヤ ニイミヨウシヨツキテン", "name": "有限会社　ニイミ洋食器店", "prefecture": "東京都", "city": "台東区", "neighborhood": "松が谷", "banchi": "1丁目1-1", "postal_code": "1118628", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "マツガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1118710','{"jis": "13106", "kana": "ユウユウ<カブシキガイシヤユウメデイア>", "name": "ユウユウ〈株式会社ユウメディア〉", "prefecture": "東京都", "city": "台東区", "neighborhood": "寿", "banchi": "1丁目5-9(浅草郵便局私書箱第108号)", "postal_code": "1118710", "old_code": "111  ", "post_office": "浅草", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "コトブキ", "alternates": []}');
+INSERT INTO office_data VALUES('1118644','{"jis": "13106", "kana": "ライオン カブシキガイシヤ", "name": "ライオン　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "蔵前", "banchi": "1-3-28", "postal_code": "1118644", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "クラマエ", "alternates": []}');
 INSERT INTO office_data VALUES('1118666','{"jis": "13106", "kana": "レデイマドラス カブシキガイシヤ", "name": "レデイマドラス　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "浅草", "banchi": "6丁目30-8", "postal_code": "1118666", "old_code": "111  ", "post_office": "浅草", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アサクサ", "alternates": []}');
 INSERT INTO office_data VALUES('1308577','{"jis": "13107", "kana": "アカツキシヨウジ カブシキガイシヤ", "name": "アカツキ商事　株式会社", "prefecture": "東京都", "city": "墨田区", "neighborhood": "両国", "banchi": "2丁目1-3", "postal_code": "1308577", "old_code": "130  ", "post_office": "本所", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "スミダク", "neighborhood_kana": "リョウゴク", "alternates": []}');
 INSERT INTO office_data VALUES('1308602','{"jis": "13107", "kana": "アサヒビ-ル カブシキガイシヤ", "name": "アサヒビール　株式会社", "prefecture": "東京都", "city": "墨田区", "neighborhood": "吾妻橋", "banchi": "1丁目23-1", "postal_code": "1308602", "old_code": "130  ", "post_office": "本所", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "スミダク", "neighborhood_kana": "アヅマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1308604','{"jis": "13107", "kana": "イシカワガング カブシキガイシヤ", "name": "石川玩具　株式会社", "prefecture": "東京都", "city": "墨田区", "neighborhood": "本所", "banchi": "1丁目25-7", "postal_code": "1308604", "old_code": "130  ", "post_office": "本所", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "スミダク", "neighborhood_kana": "ホンジョ", "alternates": []}');
 INSERT INTO office_data VALUES('1308512','{"jis": "13107", "kana": "イシヅカデンシ カブシキガイシヤ", "name": "石塚電子　株式会社", "prefecture": "東京都", "city": "墨田区", "neighborhood": "錦糸", "banchi": "1丁目7-7", "postal_code": "1308512", "old_code": "130  ", "post_office": "本所", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "スミダク", "neighborhood_kana": "キンシ", "alternates": []}');
 INSERT INTO office_data VALUES('1308585','{"jis": "13107", "kana": "イツパンザイダンホウジン オオクラザイムキヨウカイ", "name": "一般財団法人　大蔵財務協会", "prefecture": "東京都", "city": "墨田区", "neighborhood": "東駒形", "banchi": "1-14-1財協ビル", "postal_code": "1308585", "old_code": "130  ", "post_office": "本所", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "スミダク", "neighborhood_kana": "ヒガシコマガタ", "alternates": []}');
 INSERT INTO office_data VALUES('1308606','{"jis": "13107", "kana": "イツパンザイダンホウジン シゼンカンキヨウケンキユウセンタ-", "name": "一般財団法人　自然環境研究センター", "prefecture": "東京都", "city": "墨田区", "neighborhood": "江東橋", "banchi": "3-3-7", "postal_code": "1308606", "old_code": "130  ", "post_office": "本所", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "スミダク", "neighborhood_kana": "コウトウバシ", "alternates": []}');
@@ -127852,15 +127784,15 @@
 INSERT INTO office_data VALUES('1358717','{"jis": "13108", "kana": "カブシキガイシヤ オ-トバツクスセブン", "name": "株式会社　オートバックスセブン", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6番52号", "postal_code": "1358717", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358567','{"jis": "13108", "kana": "カブシキガイシヤ クメセツケイ", "name": "株式会社　久米設計", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2丁目1-22", "postal_code": "1358567", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358659','{"jis": "13108", "kana": "カブシキガイシヤ コツクス", "name": "株式会社　コックス", "prefecture": "東京都", "city": "江東区", "neighborhood": "新大橋", "banchi": "1丁目8-11三井生命新大橋ビル", "postal_code": "1358659", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンオオハシ", "alternates": []}');
 INSERT INTO office_data VALUES('1358402','{"jis": "13108", "kana": "カブシキガイシヤ ザ マイラ", "name": "株式会社　ザ　マイラ", "prefecture": "東京都", "city": "江東区", "neighborhood": "佐賀", "banchi": "1丁目1-14", "postal_code": "1358402", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "サガ", "alternates": []}');
 INSERT INTO office_data VALUES('1358670','{"jis": "13108", "kana": "カブシキガイシヤ システムソフト トウキヨウセンタ-", "name": "株式会社　システムソフト　東京センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2丁目10-24", "postal_code": "1358670", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358303','{"jis": "13108", "kana": "カブシキガイシヤ シモダ", "name": "株式会社　シモダ", "prefecture": "東京都", "city": "江東区", "neighborhood": "森下", "banchi": "3丁目8-11", "postal_code": "1358303", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "モリシタ", "alternates": []}');
 INSERT INTO office_data VALUES('1358668','{"jis": "13108", "kana": "カブシキガイシヤ ジエイ・スポ-ツ", "name": "株式会社　ジェイ・スポーツ", "prefecture": "東京都", "city": "江東区", "neighborhood": "青海", "banchi": "2-5-10テレコムセンタービル20F", "postal_code": "1358668", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アオミ", "alternates": []}');
-INSERT INTO office_data VALUES('1358165','{"jis": "13108", "kana": "カブシキガイシヤ ジエイテイビ-パブリツシング", "name": "株式会社　ＪＴＢパブリッシング", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5-6-36豊洲プライムスクエア11階", "postal_code": "1358165", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
+INSERT INTO office_data VALUES('1358165','{"jis": "13108", "kana": "カブシキガイシヤ ジエイテイビ-パブリツシング", "name": "株式会社　ＪＴＢパブリッシング", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5-6-36豊洲プライムスクエア11階", "postal_code": "1358165", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358451','{"jis": "13108", "kana": "カブシキガイシヤ ジエイピ-ビジネスサ-ビス", "name": "株式会社　ＪＰビジネスサービス", "prefecture": "東京都", "city": "江東区", "neighborhood": "深川", "banchi": "2丁目2-18", "postal_code": "1358451", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "フカガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1008666','{"jis": "13108", "kana": "カブシキガイシヤ スポ-ツニツポンシンブンシヤ", "name": "株式会社　スポーツニッポン新聞社", "prefecture": "東京都", "city": "江東区", "neighborhood": "越中島", "banchi": "2丁目1-30(銀座郵便局私書箱第277号)", "postal_code": "1008666", "old_code": "135  ", "post_office": "銀座", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エッチュウジマ", "alternates": []}');
 INSERT INTO office_data VALUES('1358555','{"jis": "13108", "kana": "カブシキガイシヤ タキネツト", "name": "株式会社　タキネット", "prefecture": "東京都", "city": "江東区", "neighborhood": "新大橋", "banchi": "2丁目13-4", "postal_code": "1358555", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンオオハシ", "alternates": []}');
 INSERT INTO office_data VALUES('1358461','{"jis": "13108", "kana": "カブシキガイシヤ ダイワソウケン トウキヨウセンタ-", "name": "株式会社　大和総研　東京センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "1丁目14-6大和永代ビル", "postal_code": "1358461", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358460','{"jis": "13108", "kana": "カブシキガイシヤ ダイワソウケン ホンシヤ", "name": "株式会社　大和総研　本社", "prefecture": "東京都", "city": "江東区", "neighborhood": "冬木", "banchi": "15-6", "postal_code": "1358460", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "フユキ", "alternates": []}');
 INSERT INTO office_data VALUES('1358150','{"jis": "13108", "kana": "カブシキガイシヤ チユウオウコンピユ-タシステム", "name": "株式会社　中央コンピュータシステム", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "6丁目4番34号メブクス豊洲", "postal_code": "1358150", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358502','{"jis": "13108", "kana": "カブシキガイシヤ トウシバパ-ソナルアンドクライアントソリユ-シヨンシヤ", "name": "株式会社　東芝パーソナル＆クライアントソリューション社", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6番15号", "postal_code": "1358502", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
@@ -127896,14 +127828,15 @@
 INSERT INTO office_data VALUES('1358470','{"jis": "13108", "kana": "カブシキガイシヤ レナウン", "name": "株式会社　レナウン", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "2丁目37-25", "postal_code": "1358470", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358210','{"jis": "13108", "kana": "カブシキガイシヤ レナウン", "name": "株式会社　レナウン", "prefecture": "東京都", "city": "江東区", "neighborhood": "有明", "banchi": "3丁目6番11号TFTビル東館6階(TFT内郵便局私書箱第2045号)", "postal_code": "1358210", "old_code": "135  ", "post_office": "晴海", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アリアケ", "alternates": []}');
 INSERT INTO office_data VALUES('1358180','{"jis": "13108", "kana": "カブシキガイシヤ ワ-ルドサプライ", "name": "株式会社　ワールドサプライ", "prefecture": "東京都", "city": "江東区", "neighborhood": "有明", "banchi": "1-2-22", "postal_code": "1358180", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アリアケ", "alternates": []}');
 INSERT INTO office_data VALUES('1358080','{"jis": "13108", "kana": "カブシキガイシヤ ワウワウ ホウソウセンタ-", "name": "株式会社　ＷＯＷＯＷ　放送センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1番58号", "postal_code": "1358080", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358375','{"jis": "13108", "kana": "カントウシンリンカンリキヨク トウキヨウジムシヨ", "name": "関東森林管理局　東京事務所", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "6丁目1-42", "postal_code": "1358375", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358404','{"jis": "13108", "kana": "ガツコウホウジン ナカムラガクエン", "name": "学校法人　中村学園", "prefecture": "東京都", "city": "江東区", "neighborhood": "清澄", "banchi": "2丁目3-15", "postal_code": "1358404", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "キヨスミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358181','{"jis": "13108", "kana": "ガツコウホウジン ムサシノダイガク ホウジンホンブ(アリアケキヤンパス)", "name": "学校法人　武蔵野大学　法人本部（有明キャンパス）", "prefecture": "東京都", "city": "江東区", "neighborhood": "有明", "banchi": "3丁目3番3号", "postal_code": "1358181", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アリアケ", "alternates": []}');
+INSERT INTO office_data VALUES('1358308','{"jis": "13108", "kana": "クラブツ-リズム カブシキカイシヤ", "name": "クラブツーリズム　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "枝川", "banchi": "1丁目9番6号住友不動産豊洲ビル", "postal_code": "1358308", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エダガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1358310','{"jis": "13108", "kana": "コアサシヨウジ カブシキガイシヤ トウキヨウシテン", "name": "小浅商事　株式会社　東京支店", "prefecture": "東京都", "city": "江東区", "neighborhood": "森下", "banchi": "1丁目2-2", "postal_code": "1358310", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "モリシタ", "alternates": []}');
 INSERT INTO office_data VALUES('1358440','{"jis": "13108", "kana": "コウトウオ-ルインサツ カブシキガイシヤ", "name": "江東オール印刷　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "清澄", "banchi": "1丁目2-1読売江東ビル", "postal_code": "1358440", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "キヨスミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358311','{"jis": "13108", "kana": "コウトウニシゼイムシヨ", "name": "江東西税務署", "prefecture": "東京都", "city": "江東区", "neighborhood": "猿江", "banchi": "2丁目16-12", "postal_code": "1358311", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "サルエ", "alternates": []}');
 INSERT INTO office_data VALUES('1358630','{"jis": "13108", "kana": "コクサイケンキユウコウリユウダイガクムラ トウキヨウコクサイコウリユウカン", "name": "国際研究交流大学村　東京国際交流館", "prefecture": "東京都", "city": "江東区", "neighborhood": "青海", "banchi": "2丁目79番", "postal_code": "1358630", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358550','{"jis": "13108", "kana": "ザイダンホウジン ガンケンキユウカイ", "name": "財団法人　癌研究会", "prefecture": "東京都", "city": "江東区", "neighborhood": "有明", "banchi": "3丁目10-6", "postal_code": "1358550", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アリアケ", "alternates": []}');
 INSERT INTO office_data VALUES('1358538','{"jis": "13108", "kana": "ザイダンホウジン ゼンニホンカラテドウレンメイ", "name": "財団法人　全日本空手道連盟", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "1丁目1番20号日本空手道会館", "postal_code": "1358538", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358473','{"jis": "13108", "kana": "ザイダンホウジン ミライコウガクケンキユウジヨ", "name": "財団法人　未来工学研究所", "prefecture": "東京都", "city": "江東区", "neighborhood": "深川", "banchi": "2丁目6-11富岡橋ビル", "postal_code": "1358473", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "フカガワ", "alternates": []}');
@@ -127940,14 +127873,15 @@
 INSERT INTO office_data VALUES('1358383','{"jis": "13108", "kana": "トウキヨウトコウトウクヤクシヨ", "name": "東京都江東区役所", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "4丁目11-28", "postal_code": "1358383", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358639','{"jis": "13108", "kana": "トウキヨウトセキジユウジケツエキセンタ-", "name": "東京都赤十字血液センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358639", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": [{"jis": "13108", "kana": "ニホンセキジユウジシヤ カントウコウシンエツブロツクケツエキセンタ-", "name": "日本赤十字社　関東甲信越ブロック血液センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358639", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}]}');
 INSERT INTO office_data VALUES('1358134','{"jis": "13108", "kana": "トウトスイサン カブシキカイシヤ", "name": "東都水産　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "6-6-2", "postal_code": "1358134", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358532','{"jis": "13108", "kana": "ニツコウビジネスシステムズ カブシキガイシヤ", "name": "日興ビジネスシステムズ　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "木場", "banchi": "1丁目5-55", "postal_code": "1358532", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "キバ", "alternates": []}');
 INSERT INTO office_data VALUES('1358570','{"jis": "13108", "kana": "ニツシンセイトウ カブシキガイシヤ トヨスコウジヨウ", "name": "日新製糖　株式会社　豊洲工場", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "4丁目9-11", "postal_code": "1358570", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358553','{"jis": "13108", "kana": "ニツシンセイトウ カブシキガイシヤ ヨカカイハツホンブ ドウ.スポ-ツプラザハルミ", "name": "日新製糖　株式会社　余暇開発本部　ドゥ・スポーツプラザ晴海", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6-41", "postal_code": "1358553", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358477','{"jis": "13108", "kana": "ニツポンチユウオウケイバカイ デンワトウヒヨウセンタ-", "name": "日本中央競馬会　電話投票センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "1丁目14-5永代ダイヤビル内", "postal_code": "1358477", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
+INSERT INTO office_data VALUES('1358797','{"jis": "13108", "kana": "ニツポンユウビン カブシキガイシヤ トウキヨウシシヤ", "name": "日本郵便　株式会社　東京支社", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "5-29-30ニッテイビル東陽", "postal_code": "1358797", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358511','{"jis": "13108", "kana": "ニホンアイ・ビ-・エム カブシキガイシヤ トヨスジギヨウシヨ", "name": "日本アイ・ビー・エム　株式会社　豊洲事業所", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6-52", "postal_code": "1358511", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358552','{"jis": "13108", "kana": "ニホンエイセイホウソウ (カブ) ワウワウ", "name": "日本衛星放送　（株）　ＷＯＷＯＷ", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-58", "postal_code": "1358552", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358568','{"jis": "13108", "kana": "ニホンオフイス・システム カブシキガイシヤ", "name": "日本オフィス・システム　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "有明", "banchi": "3-4-10", "postal_code": "1358568", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アリアケ", "alternates": []}');
 INSERT INTO office_data VALUES('1358427','{"jis": "13108", "kana": "ニホンクウチヨウサ-ビス カブシキガイシヤ", "name": "日本空調サービス　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2-1-7", "postal_code": "1358427", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358521','{"jis": "13108", "kana": "ニホンセキジユウジシヤ ケツエキジギヨウホンブ タツミブンシツ", "name": "日本赤十字社　血液事業本部　辰巳分室", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358521", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358523','{"jis": "13108", "kana": "ニホンセキジユウジシヤ ケツエキジギヨウホンブ チユウオウコツズイデ-タセンタ-", "name": "日本赤十字社　血液事業本部　中央骨髄データセンター", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358523", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358554','{"jis": "13108", "kana": "ニホンデンシケイサン カブシキガイシヤ", "name": "日本電子計算　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "福住", "banchi": "2丁目5-4IXINAL門前仲町", "postal_code": "1358554", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "フクズミ", "alternates": []}');
@@ -128047,15 +127981,15 @@
 INSERT INTO office_data VALUES('1408522','{"jis": "13109", "kana": "イリヨウホウジンシヤダンミドリノカイ トウキヨウシナガワビヨウイン", "name": "医療法人社団緑野会　東京品川病院", "prefecture": "東京都", "city": "品川区", "neighborhood": "東大井", "banchi": "6-3-22", "postal_code": "1408522", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408547','{"jis": "13109", "kana": "インタ-ワイヤ-ド カブシキガイシヤ", "name": "インターワイヤード　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "5丁目19-8", "postal_code": "1408547", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408688','{"jis": "13109", "kana": "オキデンキコウジ カブシキガイシヤ", "name": "沖電気工事　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "北品川", "banchi": "1丁目19-4", "postal_code": "1408688", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "キタシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408511','{"jis": "13109", "kana": "カブシキカイシヤ ニツセイコム", "name": "株式会社　ニッセイコム", "prefecture": "東京都", "city": "品川区", "neighborhood": "大井", "banchi": "1丁目47-1", "postal_code": "1408511", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "オオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408572','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシングル-プ", "name": "株式会社　日立製作所　情報・通信グループ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目27-18日立大森第二別館", "postal_code": "1408572", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408573','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシングル-プ", "name": "株式会社　日立製作所　情報・通信グループ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目26-2大森ベルポートB館", "postal_code": "1408573", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408512','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシンシステムシヤ", "name": "株式会社　日立製作所　情報・通信システム社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6-23-1日立大森ビル", "postal_code": "1408512", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
-INSERT INTO office_data VALUES('1408574','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨデジタルシステムアンドサ-ビストウカツホンブ", "name": "株式会社　日立製作所デジタルシステム＆サービス統括本部", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "六丁目26-1大森ベルポートA館", "postal_code": "1408574", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
+INSERT INTO office_data VALUES('1408574','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨデジタルシステムアンドサ-ビストウカツホンブ", "name": "株式会社　日立製作所デジタルシステム＆サービス統括本部", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "六丁目26-1大森ベルポートA館", "postal_code": "1408574", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408619','{"jis": "13109", "kana": "カブシキガイシヤ アクセスコクサイネツトワ-ク", "name": "株式会社　アクセス国際ネットワーク", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目4番11号野村不動産天王洲ビル", "postal_code": "1408619", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408630','{"jis": "13109", "kana": "カブシキガイシヤ ウエツクス", "name": "株式会社　ＵＥＸ", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目2-24", "postal_code": "1408630", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408702','{"jis": "13109", "kana": "カブシキガイシヤ カツマタデンキセイサクジヨ", "name": "株式会社　勝亦電機製作所", "prefecture": "東京都", "city": "品川区", "neighborhood": "北品川", "banchi": "4-10-9", "postal_code": "1408702", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "キタシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408538','{"jis": "13109", "kana": "カブシキガイシヤ カトウセイサクシヨ", "name": "株式会社　加藤製作所", "prefecture": "東京都", "city": "品川区", "neighborhood": "東大井", "banchi": "1丁目9-37", "postal_code": "1408538", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408614','{"jis": "13109", "kana": "カブシキガイシヤ コスモトレ-ドアンドサ-ビス", "name": "株式会社　コスモトレード＆サービス", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目5-8", "postal_code": "1408614", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408678','{"jis": "13109", "kana": "カブシキガイシヤ コニシデンキ", "name": "株式会社　古西電機", "prefecture": "東京都", "city": "品川区", "neighborhood": "南品川", "banchi": "2丁目16-6", "postal_code": "1408678", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408611','{"jis": "13109", "kana": "カブシキガイシヤ サンゲツ トウキヨウテン", "name": "株式会社　サンゲツ　東京店", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "3丁目20-17", "postal_code": "1408611", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
@@ -128933,14 +128867,15 @@
 INSERT INTO office_data VALUES('1708460','{"jis": "13116", "kana": "カブシキカイシヤ ギンコウケンシユウシヤ", "name": "株式会社　銀行研修社", "prefecture": "東京都", "city": "豊島区", "neighborhood": "北大塚", "banchi": "3丁目10-5", "postal_code": "1708460", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "キタオオツカ", "alternates": []}');
 INSERT INTO office_data VALUES('1708450','{"jis": "13116", "kana": "カブシキガイシヤ ア-バンウエスト", "name": "株式会社　アーバンウエスト", "prefecture": "東京都", "city": "豊島区", "neighborhood": "南大塚", "banchi": "3丁目3-4", "postal_code": "1708450", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ミナミオオツカ", "alternates": []}');
 INSERT INTO office_data VALUES('1708433','{"jis": "13116", "kana": "カブシキガイシヤ イケブクロシヨツピングパ-ク", "name": "株式会社　池袋ショッピングパーク", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "1丁目5番6号", "postal_code": "1708433", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708417','{"jis": "13116", "kana": "カブシキガイシヤ クラモトサンギヨウ", "name": "株式会社　倉本産業", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "3丁目7-4", "postal_code": "1708417", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708402','{"jis": "13116", "kana": "カブシキガイシヤ クレデイセゾン トウキヨウエイギヨウシヨ", "name": "株式会社　クレディセゾン　東京営業所", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "2丁目56-3", "postal_code": "1708402", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708427','{"jis": "13116", "kana": "カブシキガイシヤ ゲイブンシヤ", "name": "株式会社　芸文社", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "2丁目45-9", "postal_code": "1708427", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708465','{"jis": "13116", "kana": "カブシキガイシヤ トウキヨウメイラク", "name": "株式会社　東京めいらく", "prefecture": "東京都", "city": "豊島区", "neighborhood": "南大塚", "banchi": "2丁目45-8NSビル3F", "postal_code": "1708465", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ミナミオオツカ", "alternates": []}');
+INSERT INTO office_data VALUES('1708474','{"jis": "13116", "kana": "カブシキガイシヤ ニホンヒヨウロンシヤ", "name": "株式会社　日本評論社", "prefecture": "東京都", "city": "豊島区", "neighborhood": "南大塚", "banchi": "3丁目12-4", "postal_code": "1708474", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ミナミオオツカ", "alternates": []}');
 INSERT INTO office_data VALUES('1708466','{"jis": "13116", "kana": "カブシキガイシヤ ヒタチプラントテクノロジ-", "name": "株式会社　日立プラントテクノロジー", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "4丁目5-2", "postal_code": "1708466", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708438','{"jis": "13116", "kana": "カブシキガイシヤ ビ-エフ", "name": "株式会社　ビーエフ", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "1丁目33-8", "postal_code": "1708438", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708404','{"jis": "13116", "kana": "カブシキガイシヤ フアミリ-マ-ト ホンブ", "name": "株式会社　ファミリーマート　本部", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "4丁目26-10", "postal_code": "1708404", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708457','{"jis": "13116", "kana": "カブシキガイシヤ ベストセラ-ズ", "name": "株式会社　ベストセラーズ", "prefecture": "東京都", "city": "豊島区", "neighborhood": "南大塚", "banchi": "2丁目29番7号", "postal_code": "1708457", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ミナミオオツカ", "alternates": []}');
 INSERT INTO office_data VALUES('1708401','{"jis": "13116", "kana": "カブシキガイシヤ マルエツ", "name": "株式会社　マルエツ", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "5丁目51-12", "postal_code": "1708401", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708432','{"jis": "13116", "kana": "カブシキガイシヤ ミキ", "name": "株式会社　三貴", "prefecture": "東京都", "city": "豊島区", "neighborhood": "東池袋", "banchi": "3丁目4-3", "postal_code": "1708432", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ヒガシイケブクロ", "alternates": []}');
 INSERT INTO office_data VALUES('1708459','{"jis": "13116", "kana": "カブシキガイシヤ ユ-コ-", "name": "株式会社　ユーコー", "prefecture": "東京都", "city": "豊島区", "neighborhood": "南大塚", "banchi": "2丁目26-15", "postal_code": "1708459", "old_code": "170  ", "post_office": "豊島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "トシマク", "neighborhood_kana": "ミナミオオツカ", "alternates": []}');
@@ -129708,15 +129643,15 @@
 INSERT INTO office_data VALUES('1948577','{"jis": "13209", "kana": "ホ-チキ カブシキガイシヤ マチダジギヨウシヨ", "name": "ホーチキ　株式会社　町田事業所", "prefecture": "東京都", "city": "町田市", "neighborhood": "南町田", "banchi": "3丁目7番1号", "postal_code": "1948577", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ミナミマチダ", "alternates": []}');
 INSERT INTO office_data VALUES('1948520','{"jis": "13209", "kana": "マチダシヤクシヨ", "name": "町田市役所", "prefecture": "東京都", "city": "町田市", "neighborhood": "森野", "banchi": "2-2-22", "postal_code": "1948520", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "モリノ", "alternates": []}');
 INSERT INTO office_data VALUES('1948580','{"jis": "13209", "kana": "マチダシヤクシヨ シミンカ", "name": "町田市役所　市民課", "prefecture": "東京都", "city": "町田市", "neighborhood": "森野", "banchi": "2丁目2番22号", "postal_code": "1948580", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "モリノ", "alternates": []}');
 INSERT INTO office_data VALUES('1948567','{"jis": "13209", "kana": "マチダゼイムシヨ", "name": "町田税務署", "prefecture": "東京都", "city": "町田市", "neighborhood": "中町", "banchi": "3丁目3-6", "postal_code": "1948567", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1948501','{"jis": "13209", "kana": "マチダトウキユウツインズ", "name": "町田東急ツインズ", "prefecture": "東京都", "city": "町田市", "neighborhood": "原町田", "banchi": "6丁目4番1号", "postal_code": "1948501", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ハラマチダ", "alternates": []}');
 INSERT INTO office_data VALUES('1948586','{"jis": "13209", "kana": "マチダユウビンチヨキンチイキブンカカツドウシエンシセツ", "name": "町田郵便貯金地域文化活動支援施設", "prefecture": "東京都", "city": "町田市", "neighborhood": "原町田", "banchi": "4丁目1-14", "postal_code": "1948586", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ハラマチダ", "alternates": []}');
 INSERT INTO office_data VALUES('1948511','{"jis": "13209", "kana": "ミツビシカガクセイメイカガクケンキユウジヨ", "name": "三菱化学生命科学研究所", "prefecture": "東京都", "city": "町田市", "neighborhood": "南大谷", "banchi": "11号", "postal_code": "1948511", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ミナミオオヤ", "alternates": []}');
-INSERT INTO office_data VALUES('1940297','{"jis": "13209", "kana": "イリヨウホウジンシヤダン コウリユウカイ タマキユウリヨウリハビリテ-シヨンビヨウイン", "name": "医療法人社団　幸隆会　多摩丘陵リハビリテーション病院", "prefecture": "東京都", "city": "町田市", "neighborhood": "下小山田町", "banchi": "1491", "postal_code": "1940297", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "シモオヤマダマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1940297','{"jis": "13209", "kana": "イリヨウホウジンシヤダン コウリユウカイ タマキユウリヨウリハビリテ-シヨンビヨウイン", "name": "医療法人社団　幸隆会　多摩丘陵リハビリテーション病院", "prefecture": "東京都", "city": "町田市", "neighborhood": "下小山田町", "banchi": "1491", "postal_code": "1940297", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "シモオヤマダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940294','{"jis": "13209", "kana": "オウビリンガクエン", "name": "桜美林学園", "prefecture": "東京都", "city": "町田市", "neighborhood": "常盤町", "banchi": "3758", "postal_code": "1940294", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "トキワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940295','{"jis": "13209", "kana": "カブシキガイシヤ オ-クセイサクシヨ", "name": "株式会社　オーク製作所", "prefecture": "東京都", "city": "町田市", "neighborhood": "小山ケ丘", "banchi": "3丁目9-6", "postal_code": "1940295", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1940293','{"jis": "13209", "kana": "チユウオウキヨウドウクミアイガクエン", "name": "中央協同組合学園", "prefecture": "東京都", "city": "町田市", "neighborhood": "相原町", "banchi": "4771", "postal_code": "1940293", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "アイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940292','{"jis": "13209", "kana": "トウキヨウカセイガクインダイガク", "name": "東京家政学院大学", "prefecture": "東京都", "city": "町田市", "neighborhood": "相原町", "banchi": "2600", "postal_code": "1940292", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "アイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940296','{"jis": "13209", "kana": "トウキヨウコウクウケイキ カブシキガイシヤ", "name": "東京航空計器　株式会社", "prefecture": "東京都", "city": "町田市", "neighborhood": "小山ヶ丘", "banchi": "2丁目2番6号", "postal_code": "1940296", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "オヤマガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('1940298','{"jis": "13209", "kana": "ホウセイダイガク", "name": "法政大学", "prefecture": "東京都", "city": "町田市", "neighborhood": "相原町", "banchi": "4342", "postal_code": "1940298", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "アイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1958555','{"jis": "13209", "kana": "ガツコウホウジン ワコウガクエン", "name": "学校法人　和光学園", "prefecture": "東京都", "city": "町田市", "neighborhood": "金井町", "banchi": "2160番地", "postal_code": "1958555", "old_code": "195  ", "post_office": "鶴川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "カナイマチ", "alternates": []}');
@@ -130055,15 +129990,16 @@
 INSERT INTO office_data VALUES('2318313','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ノウゼイカンリカ", "name": "横浜市財政局主税部　納税管理課", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318313", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318312','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ホウジンカゼイカ ジギヨウシヨゼイタントウ", "name": "横浜市財政局主税部　法人課税課　事業所税担当", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318312", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318314','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ホウジンカゼイカ トクベツチヨウシユウセンタ-", "name": "横浜市財政局主税部　法人課税課　特別徴収センター", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318314", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318316','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ホウジンカゼイカ ホウジンシミンゼイタントウ", "name": "横浜市財政局主税部　法人課税課　法人市民税担当", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318316", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318307','{"jis": "14104", "kana": "ヨコハマシユウソウセイキユウジムセンタ-", "name": "横浜市郵送請求事務センター", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "桜木町", "banchi": "1丁目1-56", "postal_code": "2318307", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318682','{"jis": "14104", "kana": "ヨコハマシリツ ミナトセキジユウジビヨウイン", "name": "横浜市立　みなと赤十字病院", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "新山下", "banchi": "3丁目12-1", "postal_code": "2318682", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "シンヤマシタ", "alternates": []}');
 INSERT INTO office_data VALUES('2318411','{"jis": "14104", "kana": "ヨコハマチホウホウムキヨク", "name": "横浜地方法務局", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "北仲通", "banchi": "5丁目57横浜第2合同庁舎", "postal_code": "2318411", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "キタナカドオリ", "alternates": []}');
-INSERT INTO office_data VALUES('2318550','{"jis": "14104", "kana": "ヨコハマナカゼイムシヨ", "name": "横浜中税務署", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "37-9", "postal_code": "2318550", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('2318750','{"jis": "14104", "kana": "ヨコハマナカゼイムシヨ", "name": "横浜中税務署", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "新港", "banchi": "一丁目6番1号よこはま新港合同庁舎2階・3階", "postal_code": "2318750", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": true, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "シンコウ", "alternates": []}');
+INSERT INTO office_data VALUES('2318550','{"jis": "14104", "kana": "ヨコハマナカゼイムシヨ", "name": "横浜中税務署", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "新港", "banchi": "一丁目6番1号よこはま新港合同庁舎2階・3階", "postal_code": "2318550", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": true, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "シンコウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318562','{"jis": "14104", "kana": "ヨコハマフタバシヨウガツコウ", "name": "横浜雙葉小学校", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山手町", "banchi": "226", "postal_code": "2318562", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマテチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318689','{"jis": "14104", "kana": "ヨシカワシヨウジ カブシキカイシヤ", "name": "吉川商事　株式会社", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "上野町", "banchi": "2丁目88番地", "postal_code": "2318689", "old_code": "23108", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ウエノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318588','{"jis": "14104", "kana": "カナガワケンチヨウ", "name": "神奈川県庁", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "日本大通", "banchi": "1", "postal_code": "2318588", "old_code": "23188", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ニホンオオドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2318711','{"jis": "14104", "kana": "シヨウコウクミアイチユウオウキンコ ヨコハマシテン", "name": "商工組合中央金庫　横浜支店", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "本町", "banchi": "4丁目34(横浜港郵便局私書箱第69号)", "postal_code": "2318711", "old_code": "23191", "post_office": "横浜港", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2328602','{"jis": "14105", "kana": "カナガワケンジドウシヤゼイカンリジムシヨ", "name": "神奈川県自動車税管理事務所", "prefecture": "神奈川県", "city": "横浜市南区", "neighborhood": "弘明寺町", "banchi": "31", "postal_code": "2328602", "old_code": "232  ", "post_office": "横浜南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシミナミク", "neighborhood_kana": "グミョウジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2328555','{"jis": "14105", "kana": "カナガワケンリツコドモイリヨウセンタ-", "name": "神奈川県立こども医療センター", "prefecture": "神奈川県", "city": "横浜市南区", "neighborhood": "六ツ川", "banchi": "2丁目138-4", "postal_code": "2328555", "old_code": "232  ", "post_office": "横浜南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシミナミク", "neighborhood_kana": "ムツカワ", "alternates": []}');
 INSERT INTO office_data VALUES('2328531','{"jis": "14105", "kana": "カブシキガイシヤ ノグチ ヨコハマシテン", "name": "株式会社　ノグチ　横浜支店", "prefecture": "神奈川県", "city": "横浜市南区", "neighborhood": "永田台", "banchi": "1-12", "postal_code": "2328531", "old_code": "232  ", "post_office": "横浜南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシミナミク", "neighborhood_kana": "ナガタダイ", "alternates": []}');
@@ -130612,15 +130548,15 @@
 INSERT INTO office_data VALUES('2538660','{"jis": "14207", "kana": "チガサキシホケンジヨ", "name": "茅ヶ崎市保健所", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "茅ヶ崎", "banchi": "一丁目8番7号", "postal_code": "2538660", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "チガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('2538686','{"jis": "14207", "kana": "チガサキシヤクシヨ", "name": "茅ヶ崎市役所", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "茅ヶ崎", "banchi": "1丁目1-1(茅ヶ崎郵便局私書箱第6号)", "postal_code": "2538686", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "チガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('2538577','{"jis": "14207", "kana": "ト-ト- カブシキガイシヤ チガサキコウジヨウ", "name": "ＴＯＴＯ株式会社　茅ヶ崎工場", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "本村", "banchi": "2丁目8-1", "postal_code": "2538577", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "ホンソン", "alternates": []}');
 INSERT INTO office_data VALUES('2538510','{"jis": "14207", "kana": "トウホウチタニウム カブシキガイシヤ", "name": "東邦チタニウム　株式会社", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "茅ヶ崎", "banchi": "3丁目3-5", "postal_code": "2538510", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "チガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('2538550','{"jis": "14207", "kana": "ブンキヨウダイガク シヨウナンコウシヤ ブンキヨウダイガク ジヨシタンキダイガクブ", "name": "文教大学　湘南校舎　文教大学　女子短期大学部", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "行谷", "banchi": "1100", "postal_code": "2538550", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "ナメガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2538588','{"jis": "14207", "kana": "モリタミヤタコウギヨウ カブシキガイシヤ チガサキコウジヨウ", "name": "モリタ宮田工業　株式会社　茅ヶ崎工場", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "下町屋", "banchi": "1丁目1-1", "postal_code": "2538588", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "シモマチヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2498510','{"jis": "14208", "kana": "ズシカイセイチユウガク・コウトウガツコウ", "name": "逗子開成中学・高等学校", "prefecture": "神奈川県", "city": "逗子市", "neighborhood": "新宿", "banchi": "2丁目5-1", "postal_code": "2498510", "old_code": "249  ", "post_office": "逗子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ズシシ", "neighborhood_kana": "シンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('2498686','{"jis": "14208", "kana": "ズシシヤクシヨ", "name": "逗子市役所", "prefecture": "神奈川県", "city": "逗子市", "neighborhood": "逗子", "banchi": "5丁目2-16", "postal_code": "2498686", "old_code": "249  ", "post_office": "逗子", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ズシシ", "neighborhood_kana": "ズシ", "alternates": []}');
+INSERT INTO office_data VALUES('2498686','{"jis": "14208", "kana": "ズシシヤクシヨ", "name": "逗子市役所", "prefecture": "神奈川県", "city": "逗子市", "neighborhood": "逗子", "banchi": "5丁目2-16", "postal_code": "2498686", "old_code": "249  ", "post_office": "逗子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ズシシ", "neighborhood_kana": "ズシ", "alternates": []}');
 INSERT INTO office_data VALUES('2380292','{"jis": "14210", "kana": "ソノラス・コ-トアブラツボ", "name": "ソノラス・コート油壺", "prefecture": "神奈川県", "city": "三浦市", "neighborhood": "尾上町", "banchi": "18", "postal_code": "2380292", "old_code": "23802", "post_office": "三浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミウラシ", "neighborhood_kana": "オガミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2380298','{"jis": "14210", "kana": "ミウラシヤクシヨ", "name": "三浦市役所", "prefecture": "神奈川県", "city": "三浦市", "neighborhood": "城山町", "banchi": "1-1", "postal_code": "2380298", "old_code": "23802", "post_office": "三浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミウラシ", "neighborhood_kana": "シロヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2578502','{"jis": "14211", "kana": "カブシキガイシヤ ワイデイ-ケ-テクノロジ-ズ", "name": "株式会社　ＹＤＫテクノロジーズ", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "曽屋", "banchi": "500", "postal_code": "2578502", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "ソヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2578511','{"jis": "14211", "kana": "キヨウセラ カブシキガイシヤ カナガワハダノコウジヨウ", "name": "京セラ　株式会社　神奈川秦野工場", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "曽屋", "banchi": "1204番地", "postal_code": "2578511", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "ソヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2578566','{"jis": "14211", "kana": "クア-ズテツク カブシキガイシヤ ハダノジギヨウシヨ", "name": "クアーズテック　株式会社　秦野事業所", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "曽屋", "banchi": "30", "postal_code": "2578566", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "ソヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2578585','{"jis": "14211", "kana": "コクリツリヨウヨウジヨ カナガワビヨウイン", "name": "国立療養所　神奈川病院", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "落合", "banchi": "666-1", "postal_code": "2578585", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "オチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('2578523','{"jis": "14211", "kana": "シヨクヒンヤクヒンアンゼンセンタ-", "name": "食品薬品安全センター", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "落合", "banchi": "729-5", "postal_code": "2578523", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "オチアイ", "alternates": []}');
@@ -130677,15 +130613,14 @@
 INSERT INTO office_data VALUES('2430492','{"jis": "14215", "kana": "エビナシヤクシヨ", "name": "海老名市役所", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "勝瀬", "banchi": "175番地の1", "postal_code": "2430492", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "カツセ", "alternates": []}');
 INSERT INTO office_data VALUES('2430487','{"jis": "14215", "kana": "オイシツクスステ-シヨン", "name": "オイシックスステーション", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "今里", "banchi": "3-26-11", "postal_code": "2430487", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "イマザト", "alternates": []}');
 INSERT INTO office_data VALUES('2430489','{"jis": "14215", "kana": "オダキユウデンテツ カブシキガイシヤ", "name": "小田急電鉄　株式会社", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "めぐみ町", "banchi": "2番2号", "postal_code": "2430489", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "メグミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430483','{"jis": "14215", "kana": "カブシキカイシヤ マルイ マルイフアミリ-エビナ", "name": "株式会社　丸井　マルイファミリー海老名", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "中央", "banchi": "1丁目6-1小田急ビナウォーク3番館", "postal_code": "2430483", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430486','{"jis": "14215", "kana": "トウホウシネマズエビナ", "name": "ＴＯＨＯシネマズ海老名", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "中央", "banchi": "1-2-1ビナウォーク6番館", "postal_code": "2430486", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430485','{"jis": "14215", "kana": "ビナウオ-クカンリセンタ-", "name": "ビナウォーク管理センター", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "中央", "banchi": "1-4-1ビナウォーク5番館", "postal_code": "2430485", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430484','{"jis": "14215", "kana": "ビナウオ-クヨンバンカン", "name": "ビナウォーク４番館", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "中央", "banchi": "1-13-1ビナウォーク4番館", "postal_code": "2430484", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
-INSERT INTO office_data VALUES('2430495','{"jis": "14215", "kana": "フジコカ・コ-ラボトリング カブシキガイシヤ", "name": "富士コカ・コーラボトリング　株式会社", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "上河内", "banchi": "33", "postal_code": "2430495", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "カミゴウチ", "alternates": []}');
 INSERT INTO office_data VALUES('2430494','{"jis": "14215", "kana": "フジゼロツクス カブシキガイシヤ エビナジギヨウシヨ", "name": "富士ゼロックス　株式会社　海老名事業所", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "本郷", "banchi": "2274", "postal_code": "2430494", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430497','{"jis": "14215", "kana": "フジゼロツクスマニユフアクチユアリング カブシキガイシヤ エビナ(ホンシヤ)", "name": "富士ゼロックスマニュファクチュアリング　株式会社　海老名（本社）", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "本郷", "banchi": "2274番地", "postal_code": "2430497", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430496','{"jis": "14215", "kana": "モノミノトウセイシヨサツシキヨウカイ", "name": "ものみの塔聖書冊子協会", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "中新田", "banchi": "4丁目7番1号", "postal_code": "2430496", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "ナカシンデン", "alternates": []}');
 INSERT INTO office_data VALUES('2430482','{"jis": "14215", "kana": "ララポ-トエビナ", "name": "ららぽーと海老名", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "扇町", "banchi": "13番1号", "postal_code": "2430482", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "オウギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430460','{"jis": "14215", "kana": "リコ-テクノロジ-センタ-", "name": "リコーテクノロジーセンター", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "泉", "banchi": "二丁目7番1号", "postal_code": "2430460", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "イズミ", "alternates": []}');
 INSERT INTO office_data VALUES('2528540','{"jis": "14216", "kana": "エヌピ-オ-ホウジン カナガワケンシカクシヨウガイシヤフクシキヨウカイ", "name": "ＮＰＯ法人　神奈川県視覚障害者福祉協会", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "入谷", "banchi": "3丁目1707-16星野ハイツC102号", "postal_code": "2528540", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('2528567','{"jis": "14216", "kana": "カブシキガイシヤ シ-イ-シ-", "name": "株式会社　シーイーシー", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "東原", "banchi": "5丁目1-11", "postal_code": "2528567", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒガシハラ", "alternates": []}');
@@ -131107,19 +131042,19 @@
 INSERT INTO office_data VALUES('9458540','{"jis": "15205", "kana": "カブシキガイシヤ ウエキグミ", "name": "株式会社　植木組", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "駅前", "banchi": "1丁目5番45号", "postal_code": "9458540", "old_code": "945  ", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "エキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('9458585','{"jis": "15205", "kana": "コクリツビヨウインキコウ ニイガタビヨウイン", "name": "国立病院機構　新潟病院", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "赤坂町", "banchi": "3-52", "postal_code": "9458585", "old_code": "945  ", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "アカサカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9450192','{"jis": "15205", "kana": "カシワザキユ-エステツク カブシキガイシヤ", "name": "柏崎ユーエステック　株式会社", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤井", "banchi": "字西沖1350", "postal_code": "9450192", "old_code": "94501", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9450194','{"jis": "15205", "kana": "カトウスプリング カブシキガイシヤ", "name": "カトウスプリング　株式会社", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤井", "banchi": "字西沖1355番地2", "postal_code": "9450194", "old_code": "94501", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9450193','{"jis": "15205", "kana": "カブシキガイシヤ アドバネクス", "name": "株式会社　アドバネクス", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤井", "banchi": "字西沖1355", "postal_code": "9450193", "old_code": "94501", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9458601','{"jis": "15205", "kana": "トウキヨウデンリヨク カブシキガイシヤ カシワザキカリワゲンシリヨクハツデンシヨ", "name": "東京電力　株式会社　柏崎刈羽原子力発電所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "青山町", "banchi": "16-46", "postal_code": "9458601", "old_code": "94503", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "アオヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9451195','{"jis": "15205", "kana": "ニイガタコウカダイガク", "name": "新潟工科大学", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤橋", "banchi": "1719", "postal_code": "9451195", "old_code": "94511", "post_office": "新道", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451392','{"jis": "15205", "kana": "カシワザキコウセイビヨウイン", "name": "柏崎厚生病院", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字茨目", "banchi": "字二ツ池2071-1", "postal_code": "9451392", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451395','{"jis": "15205", "kana": "カブシキガイシヤ サイカワ", "name": "株式会社　サイカワ", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7586", "postal_code": "9451395", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451393','{"jis": "15205", "kana": "ニイガタサンギヨウダイガク", "name": "新潟産業大学", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字軽井川", "banchi": "4730", "postal_code": "9451393", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451397','{"jis": "15205", "kana": "ニイガタサンギヨウダイガクフゾクコウトウガツコウ", "name": "新潟産業大学附属高等学校", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "2510-2", "postal_code": "9451397", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451398','{"jis": "15205", "kana": "フジゼロツクスマニユフアクチユアリング カブシキガイシヤ ニイガタジギヨウシヨ", "name": "富士ゼロックスマニュファクチュアリング　株式会社　新潟事業所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7546", "postal_code": "9451398", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451392','{"jis": "15205", "kana": "カシワザキコウセイビヨウイン", "name": "柏崎厚生病院", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字茨目", "banchi": "字二ツ池2071-1", "postal_code": "9451392", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451395','{"jis": "15205", "kana": "カブシキガイシヤ サイカワ", "name": "株式会社　サイカワ", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7586", "postal_code": "9451395", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451393','{"jis": "15205", "kana": "ニイガタサンギヨウダイガク", "name": "新潟産業大学", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字軽井川", "banchi": "4730", "postal_code": "9451393", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451397','{"jis": "15205", "kana": "ニイガタサンギヨウダイガクフゾクコウトウガツコウ", "name": "新潟産業大学附属高等学校", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "2510-2", "postal_code": "9451397", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451398','{"jis": "15205", "kana": "フジゼロツクスマニユフアクチユアリング カブシキガイシヤ ニイガタジギヨウシヨ", "name": "富士ゼロックスマニュファクチュアリング　株式会社　新潟事業所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7546", "postal_code": "9451398", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9451595','{"jis": "15205", "kana": "カシワザキシヤクシヨ タカヤナギマチジムシヨ", "name": "柏崎市役所　高柳町事務所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "高柳町岡野町", "banchi": "1849-1", "postal_code": "9451595", "old_code": "94515", "post_office": "中鯖石", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "タカヤナギチョウオカノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9494194','{"jis": "15205", "kana": "イキイキカン", "name": "いきいき館", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "西山町池浦", "banchi": "877", "postal_code": "9494194", "old_code": "94941", "post_office": "礼拝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "ニシヤマチョウイケウラ", "alternates": []}');
 INSERT INTO office_data VALUES('9494193','{"jis": "15205", "kana": "カシワザキシヤクシヨ ニシヤママチジムシヨ", "name": "柏崎市役所　西山町事務所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "西山町池浦", "banchi": "117-2", "postal_code": "9494193", "old_code": "94941", "post_office": "礼拝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "ニシヤマチョウイケウラ", "alternates": []}');
 INSERT INTO office_data VALUES('9494192','{"jis": "15205", "kana": "ナガイコンクリ-トコウギヨウ カブシキガイシヤ", "name": "永井コンクリート工業　株式会社", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "西山町礼拝", "banchi": "457", "postal_code": "9494192", "old_code": "94941", "post_office": "礼拝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "ニシヤマチョウライハイ", "alternates": []}');
 INSERT INTO office_data VALUES('9578701','{"jis": "15206", "kana": "キヨウセラ カブシキガイシヤ ニイガタシバタコウジヨウ", "name": "京セラ　株式会社　新潟新発田工場", "prefecture": "新潟県", "city": "新発田市", "neighborhood": "五十公野", "banchi": "字山崎5270番地", "postal_code": "9578701", "old_code": "957  ", "post_office": "新発田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "シバタシ", "neighborhood_kana": "イジミノ", "alternates": []}');
 INSERT INTO office_data VALUES('9578585','{"jis": "15206", "kana": "ケイワガクエンダイガク", "name": "敬和学園大学", "prefecture": "新潟県", "city": "新発田市", "neighborhood": "大字富塚", "banchi": "1270", "postal_code": "9578585", "old_code": "957  ", "post_office": "新発田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9578601','{"jis": "15206", "kana": "シバタケンセツ カブシキガイシヤ", "name": "新発田建設　株式会社", "prefecture": "新潟県", "city": "新発田市", "neighborhood": "富塚", "banchi": "1942(新発田郵便局私書箱第25号)", "postal_code": "9578601", "old_code": "957  ", "post_office": "新発田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -131412,15 +131347,15 @@
 INSERT INTO office_data VALUES('9308517','{"jis": "16201", "kana": "トヤマケン シチヨウソンシヨクインキヨウサイクミアイ", "name": "富山県　市町村職員共済組合", "prefecture": "富山県", "city": "富山市", "neighborhood": "下野", "banchi": "995-5", "postal_code": "9308517", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "シモノ", "alternates": []}');
 INSERT INTO office_data VALUES('9308540','{"jis": "16201", "kana": "トヤマケンリツ トヤマシヨウギヨウコウトウガツコウ", "name": "富山県立　富山商業高等学校", "prefecture": "富山県", "city": "富山市", "neighborhood": "庄高田", "banchi": "413", "postal_code": "9308540", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ショウタカタ", "alternates": []}');
 INSERT INTO office_data VALUES('9308555','{"jis": "16201", "kana": "トヤマダイガク", "name": "富山大学", "prefecture": "富山県", "city": "富山市", "neighborhood": "五福", "banchi": "3190", "postal_code": "9308555", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ゴフク", "alternates": []}');
 INSERT INTO office_data VALUES('9308556','{"jis": "16201", "kana": "トヤマダイガク キヨウイクガクブフゾクガツコウ", "name": "富山大学　教育学部附属学校", "prefecture": "富山県", "city": "富山市", "neighborhood": "五艘", "banchi": "1300", "postal_code": "9308556", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ゴソウ", "alternates": []}');
 INSERT INTO office_data VALUES('9301295','{"jis": "16201", "kana": "カブシキガイシヤ イチカワゴルフコウギヨウ", "name": "株式会社　市川ゴルフ興業", "prefecture": "富山県", "city": "富山市", "neighborhood": "東福沢", "banchi": "130", "postal_code": "9301295", "old_code": "93012", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヒガシフクサワ", "alternates": []}');
 INSERT INTO office_data VALUES('9301298','{"jis": "16201", "kana": "トヤマコクサイシヨクゲイガクエン", "name": "富山国際職藝学園", "prefecture": "富山県", "city": "富山市", "neighborhood": "東黒牧", "banchi": "298", "postal_code": "9301298", "old_code": "93012", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヒガシクロマキ", "alternates": []}');
 INSERT INTO office_data VALUES('9301292','{"jis": "16201", "kana": "トヤマコクサイダイガク", "name": "富山国際大学", "prefecture": "富山県", "city": "富山市", "neighborhood": "東黒牧", "banchi": "65-1", "postal_code": "9301292", "old_code": "93012", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヒガシクロマキ", "alternates": []}');
-INSERT INTO office_data VALUES('9301392','{"jis": "16201", "kana": "トヤマシオオヤマカイカン(オオヤマギヨウセイサ-ビスセンタ-・オオヤマホケンフクシセンタ-)", "name": "富山市大山会館（大山行政サービスセンター・大山保健福祉センター）", "prefecture": "富山県", "city": "富山市", "neighborhood": "上滝", "banchi": "567", "postal_code": "9301392", "old_code": "93013", "post_office": "上滝", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "カミダキ", "alternates": []}');
+INSERT INTO office_data VALUES('9301392','{"jis": "16201", "kana": "トヤマシオオヤマカイカン(オオヤマギヨウセイサ-ビスセンタ-・オオヤマホケンフクシセンタ-)", "name": "富山市大山会館（大山行政サービスセンター・大山保健福祉センター）", "prefecture": "富山県", "city": "富山市", "neighborhood": "上滝", "banchi": "567", "postal_code": "9301392", "old_code": "93013", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "カミダキ", "alternates": []}');
 INSERT INTO office_data VALUES('9302198','{"jis": "16201", "kana": "トヤマシヤマダソウゴウギヨウセイセンタ-", "name": "富山市山田総合行政センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "山田湯", "banchi": "780", "postal_code": "9302198", "old_code": "93021", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヤマダユ", "alternates": []}');
 INSERT INTO office_data VALUES('9318515','{"jis": "16201", "kana": "ダイイチヤクヒンコウギヨウ カブシキガイシヤ", "name": "第一薬品工業　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "草島", "banchi": "15-1", "postal_code": "9318515", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "クサジマ", "alternates": []}');
 INSERT INTO office_data VALUES('9318585','{"jis": "16201", "kana": "トヤマツウウン カブシキガイシヤ", "name": "富山通運　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "八町", "banchi": "3309", "postal_code": "9318585", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ハッチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9318522','{"jis": "16201", "kana": "ニホンカイセキユ カブシキガイシヤ", "name": "日本海石油　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "四方北窪", "banchi": "字前島平均500", "postal_code": "9318522", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヨカタキタクボ", "alternates": []}');
 INSERT INTO office_data VALUES('9318523','{"jis": "16201", "kana": "ユ-デイ-トラツクス カブシキガイシヤ", "name": "ＵＤトラックス　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "八町", "banchi": "7900番地", "postal_code": "9318523", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ハッチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9318543','{"jis": "16201", "kana": "カブシキガイシヤ アライドマテリアル トヤマセイサクシヨ", "name": "株式会社　アライドマテリアル　富山製作所", "prefecture": "富山県", "city": "富山市", "neighborhood": "岩瀬古志町", "banchi": "2", "postal_code": "9318543", "old_code": "931  ", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "イワセコシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9318511','{"jis": "16201", "kana": "カブシキガイシヤ フジコシマテリアルセイゾウジヨ", "name": "株式会社　不二越マテリアル製造所", "prefecture": "富山県", "city": "富山市", "neighborhood": "米田町", "banchi": "3丁目1-1", "postal_code": "9318511", "old_code": "931  ", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヨネダマチ", "alternates": []}');
@@ -131734,14 +131669,15 @@
 INSERT INTO office_data VALUES('9208521','{"jis": "17201", "kana": "カブシキガイシヤ ヘイワドウアル・プラザカナザワ", "name": "（株）　平和堂アル・プラザ金沢", "prefecture": "石川県", "city": "金沢市", "neighborhood": "諸江町", "banchi": "上丁30-1", "postal_code": "9208521", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "モロエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208515','{"jis": "17201", "kana": "カブシキガイシヤ ホクツウ", "name": "株式会社　ほくつう", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "1丁目65番地", "postal_code": "9208515", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208556','{"jis": "17201", "kana": "カブシキガイシヤ ホクリクアイテイエス", "name": "株式会社　北陸アイティエス", "prefecture": "石川県", "city": "金沢市", "neighborhood": "本多町", "banchi": "3丁目2番1号", "postal_code": "9208556", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ホンダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208686','{"jis": "17201", "kana": "カブシキガイシヤ ホクリクギンコウ カナザワシテン", "name": "株式会社　北陸銀行　金沢支店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "尾山町", "banchi": "2-22(金沢中央郵便局私書箱第88号)", "postal_code": "9208686", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "オヤママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208588','{"jis": "17201", "kana": "カブシキガイシヤ ホツコクシンブンシヤ", "name": "株式会社　北國新聞社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "香林坊", "banchi": "2丁目5-1", "postal_code": "9208588", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コウリンボウ", "alternates": []}');
 INSERT INTO office_data VALUES('9208625','{"jis": "17201", "kana": "カブシキガイシヤ ミナミシヨウテン", "name": "株式会社　南商店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "京町", "banchi": "25-15", "postal_code": "9208625", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "キョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208665','{"jis": "17201", "kana": "カブシキガイシヤ ヤマコシ", "name": "株式会社　山越", "prefecture": "石川県", "city": "金沢市", "neighborhood": "兼六元町", "banchi": "3-78", "postal_code": "9208665", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ケンロクモトマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9208535','{"jis": "17201", "kana": "カブシキガイシヤ ヨシカワ", "name": "株式会社　ヨシカワ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "三丁目3番77号JR金沢駅西第一NKビル6F", "postal_code": "9208535", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": []}');
 INSERT INTO office_data VALUES('9208620','{"jis": "17201", "kana": "ガツコウホウジン イナオキガクエン カナザワセイリヨウダイガク", "name": "学校法人　稲置学園　金沢星稜大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "御所町", "banchi": "丑10番地1", "postal_code": "9208620", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ゴショマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208554','{"jis": "17201", "kana": "ガツコウホウジン ヒシヨウ カナザワジヨウホウビジネスセンモンガツコウ", "name": "学校法人　飛翔　金沢情報ビジネス専門学校", "prefecture": "石川県", "city": "金沢市", "neighborhood": "高岡町", "banchi": "3番20号", "postal_code": "9208554", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タカオカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208543','{"jis": "17201", "kana": "キタムラデンキサンギヨウ カブシキガイシヤ", "name": "北村電機産業　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "1丁目11", "postal_code": "9208543", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208648','{"jis": "17201", "kana": "コクドコウツウシヨウ ホクリクチホウセイビキヨク カナザワコウジジムシヨ", "name": "国土交通省　北陸地方整備局　金沢工事事務所", "prefecture": "石川県", "city": "金沢市", "neighborhood": "西念", "banchi": "4丁目23番5号", "postal_code": "9208648", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "サイネン", "alternates": []}');
 INSERT INTO office_data VALUES('9208565','{"jis": "17201", "kana": "コトブキカンコウ カブシキガイシヤ", "name": "寿観光　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "片町", "banchi": "2丁目21-35", "postal_code": "9208565", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208777','{"jis": "17201", "kana": "ザイダンホウジン ポスタルサ-ビスセンタ- ホクリクチホウホンブ", "name": "財団法人　ポスタルサービスセンター　北陸地方本部", "prefecture": "石川県", "city": "金沢市", "neighborhood": "博労町", "banchi": "68岡田ビル4F", "postal_code": "9208777", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "バクロマチ", "alternates": [{"jis": "17201", "kana": "ユウビンキヨク カブシキガイシヤ カタログハンバイセンタ-", "name": "郵便局　株式会社　カタログ販売センター", "prefecture": "石川県", "city": "金沢市", "neighborhood": "博労町", "banchi": "68岡田ビル4F", "postal_code": "9208777", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "バクロマチ", "alternates": []}]}');
 INSERT INTO office_data VALUES('9208681','{"jis": "17201", "kana": "シブヤコウギヨウ カブシキガイシヤ", "name": "澁谷工業　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "大豆田本町", "banchi": "甲58(金沢中央郵便局私書箱第10号)", "postal_code": "9208681", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "マメダホンマチ", "alternates": []}');
@@ -131791,15 +131727,14 @@
 INSERT INTO office_data VALUES('9208719','{"jis": "17201", "kana": "マルカイシカワチユウオウセイカ カブシキガイシヤ", "name": "丸果石川中央青果　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "西念", "banchi": "4丁目7-1(金沢中央郵便局私書箱第100号)", "postal_code": "9208719", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "サイネン", "alternates": []}');
 INSERT INTO office_data VALUES('9208602','{"jis": "17201", "kana": "マルベニ カブシキガイシヤ", "name": "丸紅　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "此花町", "banchi": "6-10", "postal_code": "9208602", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コノハナマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208504','{"jis": "17201", "kana": "マルヨシヨウジ カブシキガイシヤ", "name": "丸与商事　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "2丁目60", "postal_code": "9208504", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208685','{"jis": "17201", "kana": "ミタニサンギヨウ カブシキガイシヤ", "name": "三谷産業　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "玉川町", "banchi": "1-5(金沢中央郵便局私書箱第118号)", "postal_code": "9208685", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タマガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9208631','{"jis": "17201", "kana": "ミツイカイジヨウカサイホケン カブシキガイシヤ", "name": "三井海上火災保険　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "尾山町", "banchi": "6-25", "postal_code": "9208631", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "オヤママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208718','{"jis": "17201", "kana": "ミツイスミトモシンタクギンコウ カブシキガイシヤ カナザワシテン", "name": "三井住友信託銀行　株式会社　金沢支店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "上堤町", "banchi": "1番18号(金沢中央郵便局私書箱第5号)", "postal_code": "9208718", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カミツツミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9208503','{"jis": "17201", "kana": "ヤギコ-ポレ-シヨン", "name": "ヤギコーポレーション", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "2丁目80", "postal_code": "9208503", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9208535','{"jis": "17201", "kana": "ヨシカワ", "name": "ヨシカワ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "北安江", "banchi": "3丁目1-33", "postal_code": "9208535", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "キタヤスエ", "alternates": []}');
 INSERT INTO office_data VALUES('9208568','{"jis": "17201", "kana": "ヨシダセンデン カブシキガイシヤ", "name": "ヨシダ宣伝　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "中央通町", "banchi": "1-22", "postal_code": "9208568", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "チュウオウドオリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9203198','{"jis": "17201", "kana": "イシカワケン ノウギヨウソウゴウケンキユウセンタ-", "name": "石川県　農業総合研究センター", "prefecture": "石川県", "city": "金沢市", "neighborhood": "才田町", "banchi": "戊295-1", "postal_code": "9203198", "old_code": "92001", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "サイダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9200192','{"jis": "17201", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ イオウビヨウイン", "name": "独立行政法人　国立病院機構　医王病院", "prefecture": "石川県", "city": "金沢市", "neighborhood": "岩出町", "banchi": "ニ73", "postal_code": "9200192", "old_code": "92001", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "イワデマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9200295','{"jis": "17201", "kana": "カブシキガイシヤ フアイネス", "name": "株式会社　ファイネス", "prefecture": "石川県", "city": "金沢市", "neighborhood": "大浦町", "banchi": "ハ55", "postal_code": "9200295", "old_code": "92002", "post_office": "粟崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "オオウラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208658','{"jis": "17201", "kana": "シンコ-ル カブシキガイシヤ", "name": "シンコール　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "直江町", "banchi": "イ12番地", "postal_code": "9208658", "old_code": "92002", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ナオエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208614','{"jis": "17201", "kana": "ホクリクロウドウキンコ", "name": "北陸労働金庫", "prefecture": "石川県", "city": "金沢市", "neighborhood": "直江町", "banchi": "イ27番地", "postal_code": "9208614", "old_code": "92002", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ナオエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208657','{"jis": "17201", "kana": "ユニベ-ル カブシキガイシヤ", "name": "ユニベール　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "直江町", "banchi": "イ12番地", "postal_code": "9208657", "old_code": "92002", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ナオエマチ", "alternates": []}');
@@ -131810,15 +131745,15 @@
 INSERT INTO office_data VALUES('9200398','{"jis": "17201", "kana": "カブシキガイシヤ イシカワコンピユ-タセンタ-", "name": "株式会社　石川コンピュータセンター", "prefecture": "石川県", "city": "金沢市", "neighborhood": "無量寺町", "banchi": "ハ6-1", "postal_code": "9200398", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ムリョウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9218531','{"jis": "17201", "kana": "カブシキガイシヤ ジエスクホリウチ", "name": "株式会社　ジェスクホリウチ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "古府", "banchi": "2丁目74番地", "postal_code": "9218531", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コブ", "alternates": []}');
 INSERT INTO office_data VALUES('9200386','{"jis": "17201", "kana": "テレビカナザワ", "name": "テレビ金沢", "prefecture": "石川県", "city": "金沢市", "neighborhood": "古府", "banchi": "2丁目136", "postal_code": "9200386", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コブ", "alternates": []}');
 INSERT INTO office_data VALUES('9200396','{"jis": "17201", "kana": "ニツセイビルドコウギヨウ カブシキガイシヤ", "name": "日成ビルド工業　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "金石北", "banchi": "3丁目16-10", "postal_code": "9200396", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カナイワキタ", "alternates": []}');
 INSERT INTO office_data VALUES('9200393','{"jis": "17201", "kana": "ホクリクアサヒホウソウ カブシキガイシヤ", "name": "北陸朝日放送　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "松島", "banchi": "1丁目32-2", "postal_code": "9200393", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9200381','{"jis": "17201", "kana": "ホクリヨウデンコウ カブシキガイシヤ", "name": "北菱電興　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "古府", "banchi": "3丁目12", "postal_code": "9200381", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コブ", "alternates": []}');
 INSERT INTO office_data VALUES('9200385','{"jis": "17201", "kana": "マルブンツウシヨウ カブシキガイシヤ", "name": "丸文通商　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "松島", "banchi": "1丁目40", "postal_code": "9200385", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "マツシマ", "alternates": []}');
-INSERT INTO office_data VALUES('9201184','{"jis": "17201", "kana": "イオンリテ-ル カブシキガイシヤ イオンモリノサトテン", "name": "イオンリテール　株式会社　イオンもりの里店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "もりの里", "banchi": "1丁目70", "postal_code": "9201184", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "モリノサト", "alternates": []}');
+INSERT INTO office_data VALUES('9201184','{"jis": "17201", "kana": "イオンリテ-ル カブシキガイシヤ イオンモリノサトテン", "name": "イオンリテール　株式会社　イオンもりの里店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "もりの里", "banchi": "1丁目70", "postal_code": "9201184", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "モリノサト", "alternates": []}');
 INSERT INTO office_data VALUES('9201185','{"jis": "17201", "kana": "イリヨウホウジン ジユウゼンカイ", "name": "医療法人　十全会", "prefecture": "石川県", "city": "金沢市", "neighborhood": "田上本町", "banchi": "カ45-1", "postal_code": "9201185", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タガミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201182','{"jis": "17201", "kana": "カナザワケイムシヨ", "name": "金沢刑務所", "prefecture": "石川県", "city": "金沢市", "neighborhood": "田上町", "banchi": "公1", "postal_code": "9201182", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タガミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201192','{"jis": "17201", "kana": "カナザワダイガク (カクマキヤンパス)", "name": "金沢大学　（角間キャンパス）", "prefecture": "石川県", "city": "金沢市", "neighborhood": "角間町", "banchi": "1", "postal_code": "9201192", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カクママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201180','{"jis": "17201", "kana": "ホクリクダイガク", "name": "北陸大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "太陽が丘", "banchi": "1丁目1", "postal_code": "9201180", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タイヨウガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('9201181','{"jis": "17201", "kana": "ホクリクダイガク ヤクガクブ", "name": "北陸大学　薬学部", "prefecture": "石川県", "city": "金沢市", "neighborhood": "金川町", "banchi": "ホ3", "postal_code": "9201181", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カナガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201397','{"jis": "17201", "kana": "イシカワケンリツ タツミガオカコウトウガツコウ", "name": "石川県立　辰巳丘高等学校", "prefecture": "石川県", "city": "金沢市", "neighborhood": "末町", "banchi": "ニ18", "postal_code": "9201397", "old_code": "92013", "post_office": "犀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "スエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201392','{"jis": "17201", "kana": "カナザワガクインダイガク", "name": "金沢学院大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "末町", "banchi": "10-5-1", "postal_code": "9201392", "old_code": "92013", "post_office": "犀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "スエマチ", "alternates": []}');
@@ -132518,17 +132453,17 @@
 INSERT INTO office_data VALUES('4092193','{"jis": "19366", "kana": "ジエイエイフジカワ トミザワシテン", "name": "ＪＡふじかわ　富沢支店", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "福士", "banchi": "2705-3", "postal_code": "4092193", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "フクシ", "alternates": []}');
 INSERT INTO office_data VALUES('4092195','{"jis": "19366", "kana": "ズイエンカントリ-クラブ センチユリ-フジコ-ス", "name": "随縁カントリー倶楽部　センチュリー富士コース", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "万沢", "banchi": "7079-1", "postal_code": "4092195", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "マンザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4092196','{"jis": "19366", "kana": "チユウオウカガク (カブ) ヤマナシコウジヨウ ダイニジギヨウシヨ", "name": "中央化学　（株）　山梨工場　第二事業所", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "福士", "banchi": "28505-4", "postal_code": "4092196", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "フクシ", "alternates": []}');
 INSERT INTO office_data VALUES('4092192','{"jis": "19366", "kana": "ナンブチヨウヤクバ", "name": "南部町役場", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "福士", "banchi": "28505-2", "postal_code": "4092192", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "フクシ", "alternates": []}');
 INSERT INTO office_data VALUES('4092194','{"jis": "19366", "kana": "フジロイヤルカントリ-クラブ", "name": "富士ロイヤルカントリークラブ", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "万沢", "banchi": "7483", "postal_code": "4092194", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "マンザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4092398','{"jis": "19366", "kana": "ナンブチヨウヤクバ ナンブブンチヨウシヤ", "name": "南部町役場　南部分庁舎", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "内船", "banchi": "4473-1", "postal_code": "4092398", "old_code": "40923", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "ウツブナ", "alternates": []}');
 INSERT INTO office_data VALUES('4000598','{"jis": "19368", "kana": "カブシキガイシヤ ハクバク", "name": "株式会社　はくばく", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "最勝寺", "banchi": "1351", "postal_code": "4000598", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "サイショウジ", "alternates": []}');
-INSERT INTO office_data VALUES('4000593','{"jis": "19368", "kana": "キヤノンフアインテツクニスカ カブシキガイシヤ", "name": "キャノンファインテックニスカ　株式会社", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "小林", "banchi": "430番地1", "postal_code": "4000593", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "コバヤシ", "alternates": []}');
+INSERT INTO office_data VALUES('4000593','{"jis": "19368", "kana": "キヤノンフアインテツクニスカ カブシキガイシヤ", "name": "キャノンファインテックニスカ　株式会社", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "小林", "banchi": "430番地1", "postal_code": "4000593", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "コバヤシ", "alternates": []}');
 INSERT INTO office_data VALUES('4000592','{"jis": "19368", "kana": "フジカワチヨウヤクバ", "name": "富士川町役場", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "天神中條", "banchi": "1134番地", "postal_code": "4000592", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "テンジンナカジョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4000693','{"jis": "19368", "kana": "カジカザワゼイムシヨ", "name": "鰍沢税務署", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "1760番地1富士川地方合同庁舎3階", "postal_code": "4000693", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
+INSERT INTO office_data VALUES('4000693','{"jis": "19368", "kana": "カジカザワゼイムシヨ", "name": "鰍沢税務署", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "1760番地1富士川地方合同庁舎3階", "postal_code": "4000693", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4000695','{"jis": "19368", "kana": "フジカワチヨウヤクバ ブンチヨウシヤ", "name": "富士川町役場　分庁舎", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "1599番地5", "postal_code": "4000695", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4000692','{"jis": "19368", "kana": "ヤマナシケン キヨウナンチイキケンミンセンタ-", "name": "山梨県　峡南地域県民センター", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "771-2", "postal_code": "4000692", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4093897','{"jis": "19384", "kana": "カブシキガイシヤ アピオ", "name": "株式会社　アピオ", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "西条", "banchi": "3600", "postal_code": "4093897", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "サイジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4093880','{"jis": "19384", "kana": "シヨウワチヨウヤクバ", "name": "昭和町役場", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "押越", "banchi": "542-2", "postal_code": "4093880", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "オシコシ", "alternates": []}');
 INSERT INTO office_data VALUES('4093883','{"jis": "19384", "kana": "スミトモデンコウデバイス・イノベ-シヨン カブシキガイシヤ", "name": "住友電工デバイス・イノベーション　株式会社", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "紙漉阿原", "banchi": "1000番地", "postal_code": "4093883", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "カミスキアワラ", "alternates": []}');
 INSERT INTO office_data VALUES('4093895','{"jis": "19384", "kana": "パナソニツクフアクトリ-ソリユ-シヨンズ カブシキガイシヤ", "name": "パナソニックファクトリーソリューションズ　株式会社", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "紙漉阿原", "banchi": "1375", "postal_code": "4093895", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "カミスキアワラ", "alternates": []}');
 INSERT INTO office_data VALUES('4010592','{"jis": "19424", "kana": "オシノムラヤクバ", "name": "忍野村役場", "prefecture": "山梨県", "city": "南都留郡忍野村", "neighborhood": "忍草", "banchi": "1514", "postal_code": "4010592", "old_code": "40105", "post_office": "山中湖", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミツルグンオシノムラ", "neighborhood_kana": "シボクサ", "alternates": []}');
@@ -132775,27 +132710,27 @@
 INSERT INTO office_data VALUES('3868551','{"jis": "20203", "kana": "カブシキガイシヤ ニイムラ", "name": "株式会社　新村", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字秋和", "banchi": "199-4", "postal_code": "3868551", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868710','{"jis": "20203", "kana": "カブシキガイシヤ ハチジユウニギンコウ ウエダシテン", "name": "株式会社　八十二銀行　上田支店", "prefecture": "長野県", "city": "上田市", "neighborhood": "中央", "banchi": "2丁目2-12(上田郵便局私書箱第1号)", "postal_code": "3868710", "old_code": "386  ", "post_office": "上田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3868638','{"jis": "20203", "kana": "カブシキガイシヤ ミツバセイサクジヨ", "name": "株式会社　三葉製作所", "prefecture": "長野県", "city": "上田市", "neighborhood": "中央東", "banchi": "5-14", "postal_code": "3868638", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "チュウオウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3868634','{"jis": "20203", "kana": "サンヨウデンキ カブシキガイシヤ ウエダジギヨウシヨ カンガワコウジヨウ", "name": "山洋電気　株式会社　上田事業所　神川工場", "prefecture": "長野県", "city": "上田市", "neighborhood": "殿城", "banchi": "5-4", "postal_code": "3868634", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トノシロ", "alternates": []}');
 INSERT INTO office_data VALUES('3868668','{"jis": "20203", "kana": "シンシユウウエダ ノウギヨウキヨウドウクミアイ", "name": "信州うえだ　農業協同組合", "prefecture": "長野県", "city": "上田市", "neighborhood": "大手", "banchi": "2丁目7-10", "postal_code": "3868668", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオテ", "alternates": []}');
 INSERT INTO office_data VALUES('3868567','{"jis": "20203", "kana": "シンシユウダイガク センイガクブ", "name": "信州大学　繊維学部", "prefecture": "長野県", "city": "上田市", "neighborhood": "常田", "banchi": "3丁目15-1", "postal_code": "3868567", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トキダ", "alternates": []}');
 INSERT INTO office_data VALUES('3868686','{"jis": "20203", "kana": "シンシユウハム カブシキガイシヤ", "name": "信州ハム　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字下塩尻", "banchi": "950", "postal_code": "3868686", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3868666','{"jis": "20203", "kana": "シンワアドヴアンス カブシキガイシヤ", "name": "シンワアドヴァンス　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "住吉", "banchi": "21番地5", "postal_code": "3868666", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "スミヨシ", "alternates": []}');
+INSERT INTO office_data VALUES('3868666','{"jis": "20203", "kana": "シンワアドヴアンス カブシキガイシヤ", "name": "シンワアドヴァンス　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "住吉", "banchi": "21番地5", "postal_code": "3868666", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "スミヨシ", "alternates": []}');
 INSERT INTO office_data VALUES('3868705','{"jis": "20203", "kana": "チユウブデンリヨクパワ-グリツド カブシキガイシヤ ウエダエイギヨウシヨ", "name": "中部電力パワーグリッド　株式会社　上田営業所", "prefecture": "長野県", "city": "上田市", "neighborhood": "中央", "banchi": "1-7-22", "postal_code": "3868705", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3868610','{"jis": "20203", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ シンシユウウエダイリヨウセンター", "name": "独立行政法人　国立病院機構　信州上田医療センター", "prefecture": "長野県", "city": "上田市", "neighborhood": "緑が丘", "banchi": "1-27-21", "postal_code": "3868610", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ミドリガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3868588','{"jis": "20203", "kana": "ナガイプラスチツク コウギヨウカブシキガイシヤ", "name": "永井プラスチック工業　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "国分", "banchi": "1丁目3-37", "postal_code": "3868588", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "コクブ", "alternates": []}');
 INSERT INTO office_data VALUES('3868501','{"jis": "20203", "kana": "ナガノケイキ カブシキガイシヤ", "name": "長野計器　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字秋和", "banchi": "1150", "postal_code": "3868501", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868715','{"jis": "20203", "kana": "ナガノケン ウエダコウトウガツコウ", "name": "長野県　上田高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "大手", "banchi": "1-4-32", "postal_code": "3868715", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオテ", "alternates": []}');
 INSERT INTO office_data VALUES('3868555','{"jis": "20203", "kana": "ナガノケン ウエダゴウドウチヨウシヤ", "name": "長野県　上田合同庁舎", "prefecture": "長野県", "city": "上田市", "neighborhood": "材木町", "banchi": "1丁目2-6", "postal_code": "3868555", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ザイモクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3868685','{"jis": "20203", "kana": "ナガノケン ウエダソメヤオカコウトウガツコウ", "name": "長野県　上田染谷丘高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "", "banchi": "西丘1710", "postal_code": "3868685", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868585','{"jis": "20203", "kana": "ナガノケン ウエダチクマコウトウガツコウ", "name": "長野県　上田千曲高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字中之条", "banchi": "626", "postal_code": "3868585", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868683','{"jis": "20203", "kana": "ナガノケン ウエダヒガシコウトウガツコウ", "name": "長野県　上田東高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "常田", "banchi": "3丁目5-68", "postal_code": "3868683", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トキダ", "alternates": []}');
 INSERT INTO office_data VALUES('3868553','{"jis": "20203", "kana": "ナベリン カブシキガイシヤ ウエダシテン", "name": "鍋林　株式会社　上田支店", "prefecture": "長野県", "city": "上田市", "neighborhood": "常入", "banchi": "1丁目14-67", "postal_code": "3868553", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トキイリ", "alternates": []}');
 INSERT INTO office_data VALUES('3868609','{"jis": "20203", "kana": "ハロ-ワ-クウエダ(ウエダコウキヨウシヨクギヨウアンテイジヨ)", "name": "ハローワーク上田（上田公共職業安定所）", "prefecture": "長野県", "city": "上田市", "neighborhood": "天神", "banchi": "2丁目4-70", "postal_code": "3868609", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "テンジン", "alternates": []}');
-INSERT INTO office_data VALUES('3860192','{"jis": "20203", "kana": "カブシキガイシヤ トウトク", "name": "株式会社　ＴＯＴＯＫＵ", "prefecture": "長野県", "city": "上田市", "neighborhood": "大屋", "banchi": "300番地", "postal_code": "3860192", "old_code": "38601", "post_office": "上田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオヤ", "alternates": []}');
+INSERT INTO office_data VALUES('3860192','{"jis": "20203", "kana": "カブシキガイシヤ トウトク", "name": "株式会社　ＴＯＴＯＫＵ", "prefecture": "長野県", "city": "上田市", "neighborhood": "大屋", "banchi": "300番地", "postal_code": "3860192", "old_code": "38601", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオヤ", "alternates": []}');
 INSERT INTO office_data VALUES('3868505','{"jis": "20203", "kana": "ニツシンコウギヨウ カブシキガイシヤ", "name": "日信工業　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字国分", "banchi": "840", "postal_code": "3868505", "old_code": "38601", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3860396','{"jis": "20203", "kana": "カケユビヨウイン", "name": "鹿教湯病院", "prefecture": "長野県", "city": "上田市", "neighborhood": "鹿教湯温泉", "banchi": "1308", "postal_code": "3860396", "old_code": "38603", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カケユオンセン", "alternates": []}');
 INSERT INTO office_data VALUES('3860393','{"jis": "20203", "kana": "ミサヤマビヨウイン", "name": "三才山病院", "prefecture": "長野県", "city": "上田市", "neighborhood": "鹿教湯温泉", "banchi": "1777", "postal_code": "3860393", "old_code": "38603", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カケユオンセン", "alternates": []}');
 INSERT INTO office_data VALUES('3860493','{"jis": "20203", "kana": "イリヨウホウジン マルヤマカイ マルコチユウオウソウゴウビヨウイン", "name": "医療法人　丸山会　丸子中央総合病院", "prefecture": "長野県", "city": "上田市", "neighborhood": "上丸子", "banchi": "335-3(丸子郵便局私書箱第10号)", "postal_code": "3860493", "old_code": "38604", "post_office": "丸子", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カミマルコ", "alternates": []}');
 INSERT INTO office_data VALUES('3860492','{"jis": "20203", "kana": "ウエダシヤクシヨ マルコチイキジチセンタ-", "name": "上田市役所　丸子地域自治センター", "prefecture": "長野県", "city": "上田市", "neighborhood": "上丸子", "banchi": "1612", "postal_code": "3860492", "old_code": "38604", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カミマルコ", "alternates": []}');
 INSERT INTO office_data VALUES('3860498','{"jis": "20203", "kana": "シナノケンシ カブシキカイシヤ", "name": "シナノケンシ　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "上丸子", "banchi": "1078", "postal_code": "3860498", "old_code": "38604", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カミマルコ", "alternates": []}');
 INSERT INTO office_data VALUES('3860495','{"jis": "20203", "kana": "ニホンデンサンセイミツ カブシキガイシヤ", "name": "日本電産セイミツ　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "中丸子", "banchi": "1771", "postal_code": "3860495", "old_code": "38604", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ナカマルコ", "alternates": []}');
@@ -133040,15 +132975,15 @@
 INSERT INTO office_data VALUES('3938511','{"jis": "20361", "kana": "ニホンデンサンサンキヨ- カブシキガイシヤ", "name": "日本電産サンキョー　株式会社", "prefecture": "長野県", "city": "諏訪郡下諏訪町", "neighborhood": "", "banchi": "5329", "postal_code": "3938511", "old_code": "393  ", "post_office": "下諏訪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "スワグンシモスワマチ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3938503','{"jis": "20361", "kana": "ニホンデンサンサンキヨ-オルゴ-ルキネンカン スワノネ", "name": "日本電産サンキョーオルゴール記念館　すわのね", "prefecture": "長野県", "city": "諏訪郡下諏訪町", "neighborhood": "", "banchi": "5805", "postal_code": "3938503", "old_code": "393  ", "post_office": "下諏訪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "スワグンシモスワマチ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3990295','{"jis": "20362", "kana": "セイコ-エプソン カブシキガイシヤ スワミナミジギヨウシヨ", "name": "セイコーエプソン　株式会社　諏訪南事業所", "prefecture": "長野県", "city": "諏訪郡富士見町", "neighborhood": "富士見", "banchi": "1010", "postal_code": "3990295", "old_code": "39902", "post_office": "富士見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "スワグンフジミマチ", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('3990293','{"jis": "20362", "kana": "セイコ-エプソン カブシキガイシヤ フジミジギヨウシヨ", "name": "セイコーエプソン　株式会社　富士見事業所", "prefecture": "長野県", "city": "諏訪郡富士見町", "neighborhood": "富士見", "banchi": "281", "postal_code": "3990293", "old_code": "39902", "post_office": "富士見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "スワグンフジミマチ", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('3990292','{"jis": "20362", "kana": "フジミマチヤクバ", "name": "富士見町役場", "prefecture": "長野県", "city": "諏訪郡富士見町", "neighborhood": "落合", "banchi": "10777", "postal_code": "3990292", "old_code": "39902", "post_office": "富士見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "スワグンフジミマチ", "neighborhood_kana": "オチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('3910192','{"jis": "20363", "kana": "ハラムラヤクバ", "name": "原村役場", "prefecture": "長野県", "city": "諏訪郡原村", "neighborhood": "払沢", "banchi": "6549-1", "postal_code": "3910192", "old_code": "39101", "post_office": "原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "スワグンハラムラ", "neighborhood_kana": "ハライザワ", "alternates": []}');
 INSERT INTO office_data VALUES('3990492','{"jis": "20382", "kana": "イシカワジマハンヨウキカイ カブシキガイシヤ", "name": "石川島汎用機械　株式会社", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "大字伊那富", "banchi": "3934", "postal_code": "3990492", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3990495','{"jis": "20382", "kana": "オリンパス カブシキガイシヤ タツノジギヨウジヨウ", "name": "オリンパス　株式会社　辰野事業場", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "大字伊那富", "banchi": "6666", "postal_code": "3990495", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('3990495','{"jis": "20382", "kana": "カブシキガイシヤ エビデント ナガノジギヨウジヨウ", "name": "株式会社　エビデント　長野事業場", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "大字伊那富", "banchi": "6666番地", "postal_code": "3990495", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3990497','{"jis": "20382", "kana": "カブシキガイシヤ マブチ・エスアンドテイ-", "name": "株式会社　マブチ・エスアンドティー", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "大字樋口", "banchi": "1365番地", "postal_code": "3990497", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3990498','{"jis": "20382", "kana": "シンシユウホウナンタンキダイガク", "name": "信州豊南短期大学", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "中山", "banchi": "72番地", "postal_code": "3990498", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3990493','{"jis": "20382", "kana": "タツノマチヤクバ", "name": "辰野町役場", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "中央", "banchi": "1", "postal_code": "3990493", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "カミイナグンタツノマチ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3990496','{"jis": "20382", "kana": "チヨウリツ タツノビヨウイン", "name": "町立　辰野病院", "prefecture": "長野県", "city": "上伊那郡辰野町", "neighborhood": "大字辰野", "banchi": "1445番地5", "postal_code": "3990496", "old_code": "39904", "post_office": "辰野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3994692','{"jis": "20383", "kana": "カブシキカイシヤ シンコウセイサクシヨ", "name": "株式会社　伸光製作所", "prefecture": "長野県", "city": "上伊那郡箕輪町", "neighborhood": "大字中箕輪", "banchi": "12238", "postal_code": "3994692", "old_code": "39946", "post_office": "箕輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3994697','{"jis": "20383", "kana": "コ-ア カブシキガイシヤ ア-スウイング", "name": "ＫＯＡ　株式会社　アースウイング", "prefecture": "長野県", "city": "上伊那郡箕輪町", "neighborhood": "大字中箕輪", "banchi": "14016", "postal_code": "3994697", "old_code": "39946", "post_office": "箕輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3994696','{"jis": "20383", "kana": "セイコ-エプソン カブシキガイシヤ イナジギヨウシヨ", "name": "セイコーエプソン　株式会社　伊那事業所", "prefecture": "長野県", "city": "上伊那郡箕輪町", "neighborhood": "大字中箕輪", "banchi": "8548", "postal_code": "3994696", "old_code": "39946", "post_office": "箕輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -133277,14 +133212,15 @@
 INSERT INTO office_data VALUES('5038559','{"jis": "21202", "kana": "イビデン カブシキガイシヤ カワマコウジヨウ", "name": "イビデン　株式会社　河間工場", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "河間町", "banchi": "3丁目200", "postal_code": "5038559", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ガマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038560','{"jis": "21202", "kana": "イビデングリ-ンテツク カブシキガイシヤ", "name": "イビデングリーンテック　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "河間町", "banchi": "3丁目55", "postal_code": "5038560", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ガマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038566','{"jis": "21202", "kana": "エヌテイ-テイ- オオガキエイギヨウシヨ", "name": "ＮＴＴ　大垣営業所", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "丸の内", "banchi": "1丁目18", "postal_code": "5038566", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038564','{"jis": "21202", "kana": "オ-ミケンシ カブシキガイシヤ オオガキコウジヨウ", "name": "オーミケンシ　株式会社　大垣工場", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "林町", "banchi": "6丁目80", "postal_code": "5038564", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ハヤシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038513','{"jis": "21202", "kana": "オオガキキコウ", "name": "大垣機工", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "神田町", "banchi": "1丁目25", "postal_code": "5038513", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カンダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038521','{"jis": "21202", "kana": "オオガキコウギヨウコウトウガツコウ", "name": "大垣工業高等学校", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "南若森町", "banchi": "301-1", "postal_code": "5038521", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ミナミワカモリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038502','{"jis": "21202", "kana": "オオガキシミンビヨウイン", "name": "大垣市民病院", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "南頬町", "banchi": "4丁目86", "postal_code": "5038502", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ミナミノカワチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5038601','{"jis": "21202", "kana": "オオガキシヤクシヨ", "name": "大垣市役所", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "丸の内", "banchi": "2丁目29", "postal_code": "5038601", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038565','{"jis": "21202", "kana": "オオガキシヨウコウカイギシヨ", "name": "大垣商工会議所", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "小野", "banchi": "4丁目35番地の10", "postal_code": "5038565", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "コノ", "alternates": []}');
 INSERT INTO office_data VALUES('5038554','{"jis": "21202", "kana": "オオガキジヨシタンキダイガク", "name": "大垣女子短期大学", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "西之川町", "banchi": "1丁目109", "postal_code": "5038554", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ニシノカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038568','{"jis": "21202", "kana": "オオガキステ-シヨンビル アピオ", "name": "大垣ステーションビル　アピオ", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "高屋町", "banchi": "1丁目145", "postal_code": "5038568", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タカヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038556','{"jis": "21202", "kana": "オオガキゼイムシヨ", "name": "大垣税務署", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "丸の内", "banchi": "2丁目30", "postal_code": "5038556", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038520','{"jis": "21202", "kana": "オオガキニシコウトウガツコウ", "name": "大垣西高等学校", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "中曽根町", "banchi": "147-1", "postal_code": "5038520", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ナカゾネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038507','{"jis": "21202", "kana": "オオガキフソウボウセキ カブシキガイシヤ", "name": "大垣扶桑紡績　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "美和町", "banchi": "1688", "postal_code": "5038507", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ミワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038522','{"jis": "21202", "kana": "オオガキミナミコウトウガツコウ", "name": "大垣南高等学校", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "浅中", "banchi": "2丁目69", "postal_code": "5038522", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "アサナカ", "alternates": []}');
@@ -133295,30 +133231,29 @@
 INSERT INTO office_data VALUES('5038514','{"jis": "21202", "kana": "カブシキガイシヤ カワグチヤス-パ-チエン", "name": "株式会社　川口屋スーパーチェン", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "河間町", "banchi": "1丁目65番地", "postal_code": "5038514", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ガマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038509','{"jis": "21202", "kana": "カブシキガイシヤ セイノ-シヨウジ", "name": "株式会社　セイノー商事", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "田口町", "banchi": "1", "postal_code": "5038509", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タグチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5031696','{"jis": "21202", "kana": "カブシキガイシヤ マルジユン", "name": "株式会社　丸順", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "上石津町乙坂", "banchi": "130-1", "postal_code": "5031696", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カミイシヅチョウオツサカ", "alternates": []}');
 INSERT INTO office_data VALUES('5038550','{"jis": "21202", "kana": "ギフケイザイダイガク", "name": "岐阜経済大学", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "北方町", "banchi": "5丁目50", "postal_code": "5038550", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "キタガタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038569','{"jis": "21202", "kana": "コウエキザイダンホウジン ソフトピアジヤパン", "name": "公益財団法人　ソフトピアジャパン", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "加賀野", "banchi": "4丁目1番地の7", "postal_code": "5038569", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カガノ", "alternates": []}');
 INSERT INTO office_data VALUES('5038518','{"jis": "21202", "kana": "サンメツセ カブシキガイシヤ", "name": "サンメッセ　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "久瀬川町", "banchi": "7丁目5-1", "postal_code": "5038518", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "クゼガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038505','{"jis": "21202", "kana": "シンコウゾウキ", "name": "神鋼造機", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "本今町", "banchi": "1682-2", "postal_code": "5038505", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "モトイマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5038553','{"jis": "21202", "kana": "ジエイエイゼンノウミ-トフ-ズ カブシキガイシヤ チユウブエイギヨウホンブ ヨシダハムシテン", "name": "ＪＡ全農ミートフーズ　株式会社　中部営業本部　吉田ハム支店", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "寿町", "banchi": "1番地の1", "postal_code": "5038553", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5038553','{"jis": "21202", "kana": "ジエイエイゼンノウミ-トフ-ズ カブシキガイシヤ チユウブエイギヨウホンブ ヨシダハムシテン", "name": "ＪＡ全農ミートフーズ　株式会社　中部営業本部　吉田ハム支店", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "寿町", "banchi": "1番地の1", "postal_code": "5038553", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038567','{"jis": "21202", "kana": "スイトピアセンタ-", "name": "スイトピアセンター", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "室本町", "banchi": "5丁目51", "postal_code": "5038567", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ムロホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038512','{"jis": "21202", "kana": "セイノ-ジヨウホウサ-ビス", "name": "セイノー情報サービス", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "田口町", "banchi": "1", "postal_code": "5038512", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タグチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038501','{"jis": "21202", "kana": "セイノウウンユ カブシキガイシヤ", "name": "西濃運輸　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "田口町", "banchi": "1", "postal_code": "5038501", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タグチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038519','{"jis": "21202", "kana": "タイヘイヨウセイコウ", "name": "太平洋精工", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "久瀬川町", "banchi": "7丁目5-8", "postal_code": "5038519", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "クゼガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038515','{"jis": "21202", "kana": "ダイマルマツシタシヨクヒン カブシキガイシヤ", "name": "大丸松下食品　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "本今", "banchi": "5丁目141", "postal_code": "5038515", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "モトイマ", "alternates": []}');
 INSERT INTO office_data VALUES('5038557','{"jis": "21202", "kana": "ニチデンセイミツコウギヨウ カブシキガイシヤ", "name": "日電精密工業　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "三塚町", "banchi": "336", "postal_code": "5038557", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ミツヅカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038504','{"jis": "21202", "kana": "ニツポンゴウセイ", "name": "日本合成", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "神田町", "banchi": "2丁目35", "postal_code": "5038504", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カンダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038511','{"jis": "21202", "kana": "ニホンゴウセイカガクコウギヨウ カブシキガイシヤ オオガキジギヨウシヨ オオガキフイルムコウジヨウ", "name": "日本合成化学工業（株）大垣事業所大垣フイルム工場", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "上屋", "banchi": "2丁目80", "postal_code": "5038511", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カミヤ", "alternates": []}');
 INSERT INTO office_data VALUES('5038506','{"jis": "21202", "kana": "ニホンタイサンビンコウギヨウ カブシキガイシヤ", "name": "日本耐酸壜工業　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "中曽根町", "banchi": "610", "postal_code": "5038506", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ナカゾネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038558','{"jis": "21202", "kana": "ヤナゲン", "name": "ヤナゲン", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "高屋町", "banchi": "1丁目56", "postal_code": "5038558", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タカヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038571','{"jis": "21202", "kana": "ユニ- カブシキガイシヤ アクアウオ-クオオガキ", "name": "ユニー　株式会社　アクアウォーク大垣", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "林町", "banchi": "6丁目80番21", "postal_code": "5038571", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ハヤシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038570','{"jis": "21202", "kana": "ユニ- カブシキガイシヤ アピタオオガキテン", "name": "ユニー　株式会社　アピタ大垣店", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "林町", "banchi": "6丁目80番21", "postal_code": "5038570", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ハヤシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5030192','{"jis": "21202", "kana": "オオガキシ スノマタチイキジムシヨ", "name": "大垣市　墨俣地域事務所", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "墨俣町上宿", "banchi": "473-1", "postal_code": "5030192", "old_code": "50301", "post_office": "墨俣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "スノマタチョウカミジュク", "alternates": []}');
 INSERT INTO office_data VALUES('5038604','{"jis": "21202", "kana": "イビデン カブシキガイシヤ", "name": "イビデン　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "神田町", "banchi": "2丁目1(大垣郵便局私書箱第5号)", "postal_code": "5038604", "old_code": "50391", "post_office": "大垣", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カンダチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5038601','{"jis": "21202", "kana": "オオガキシヤクシヨ", "name": "大垣市役所", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "丸の内", "banchi": "2丁目29(大垣郵便局私書箱第37号)", "postal_code": "5038601", "old_code": "50391", "post_office": "大垣", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038603','{"jis": "21202", "kana": "タイヘイヨウコウギヨウ カブシキガイシヤ", "name": "太平洋工業　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "久徳町", "banchi": "100(大垣郵便局私書箱第24号)", "postal_code": "5038603", "old_code": "50391", "post_office": "大垣", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "キュウトクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5015492','{"jis": "21203", "kana": "タカヤマシ シヨウカワシシヨ", "name": "高山市　荘川支所", "prefecture": "岐阜県", "city": "高山市", "neighborhood": "荘川町新渕", "banchi": "550番地", "postal_code": "5015492", "old_code": "50154", "post_office": "荘川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タカヤマシ", "neighborhood_kana": "ショウカワチョウアラブチ", "alternates": []}');
 INSERT INTO office_data VALUES('5068585','{"jis": "21203", "kana": "カシワモツコウ カブシキガイシヤ", "name": "柏木工　株式会社", "prefecture": "岐阜県", "city": "高山市", "neighborhood": "上岡本町", "banchi": "1丁目260", "postal_code": "5068585", "old_code": "506  ", "post_office": "高山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タカヤマシ", "neighborhood_kana": "カミオカモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5068690','{"jis": "21203", "kana": "カブシキガイシヤ タカヤマシミンジホウシヤ ザ・チヤンス", "name": "株式会社　高山市民時報社　ザ・チャンス", "prefecture": "岐阜県", "city": "高山市", "neighborhood": "桐生町", "banchi": "3丁目122-1", "postal_code": "5068690", "old_code": "506  ", "post_office": "高山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タカヤマシ", "neighborhood_kana": "キリウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5068502','{"jis": "21203", "kana": "クミアイ コウセイビヨウイン", "name": "久美愛　厚生病院", "prefecture": "岐阜県", "city": "高山市", "neighborhood": "中切町", "banchi": "1番地1", "postal_code": "5068502", "old_code": "506  ", "post_office": "高山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タカヤマシ", "neighborhood_kana": "ナカギリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5068555','{"jis": "21203", "kana": "タカヤマシヤクシヨ", "name": "高山市役所", "prefecture": "岐阜県", "city": "高山市", "neighborhood": "花岡町", "banchi": "2丁目18", "postal_code": "5068555", "old_code": "506  ", "post_office": "高山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タカヤマシ", "neighborhood_kana": "ハナオカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5068678','{"jis": "21203", "kana": "タカヤマシヨウコウカイギシヨ", "name": "高山商工会議所", "prefecture": "岐阜県", "city": "高山市", "neighborhood": "天満町", "banchi": "5丁目1(高山郵便局私書箱第35号)", "postal_code": "5068678", "old_code": "506  ", "post_office": "高山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タカヤマシ", "neighborhood_kana": "テンマンマチ", "alternates": []}');
@@ -134498,15 +134433,14 @@
 INSERT INTO office_data VALUES('4506133','{"jis": "23105", "kana": "ジエイア-ルセントラルビル カブシキガイシヤ", "name": "ジェイアールセントラルビル　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "1-1-4JRセントラルタワーズ33F", "postal_code": "4506133", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508615','{"jis": "23105", "kana": "スミトモセイメイホケン ソウゴガイシヤ ナゴヤシシヤ", "name": "住友生命保険　相互会社　名古屋支社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅南", "banchi": "2丁目14-19", "postal_code": "4508615", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('4506363','{"jis": "23105", "kana": "ゼンコクケンコウホケンキヨウカイ アイチシブ", "name": "全国健康保険協会　愛知支部", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "一丁目1番1号JPタワー名古屋", "postal_code": "4506363", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508640','{"jis": "23105", "kana": "ダイコクデンキ カブシキガイシヤ", "name": "ダイコク電機　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "那古野", "banchi": "1丁目43番5号", "postal_code": "4508640", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ナゴノ", "alternates": []}');
 INSERT INTO office_data VALUES('4508614','{"jis": "23105", "kana": "トウヨウソウコ カブシキガイシヤ", "name": "東陽倉庫　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅南", "banchi": "2丁目6-17", "postal_code": "4508614", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('4508711','{"jis": "23105", "kana": "トヨタジドウシヤ カブシキガイシヤ ナゴヤオフイス", "name": "トヨタ自動車　株式会社　名古屋オフィス", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "4丁目7番1号", "postal_code": "4508711", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508575','{"jis": "23105", "kana": "トヨタツウシヨウ カブシキガイシヤ", "name": "豊田通商　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "4丁目9-8", "postal_code": "4508575", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
-INSERT INTO office_data VALUES('4508626','{"jis": "23105", "kana": "ナゴヤシ ササシマシゼイジムシヨ", "name": "名古屋市　ささしま市税事務所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅南", "banchi": "1丁目27番2号日本生命笹島ビル8階", "postal_code": "4508626", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('4506660','{"jis": "23105", "kana": "ナゴヤジエイア-ルゲ-トタワ-ホテル", "name": "名古屋ＪＲゲートタワーホテル", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "1-1-3", "postal_code": "4506660", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508501','{"jis": "23105", "kana": "ナゴヤテツドウ カブシキガイシヤ", "name": "名古屋鉄道　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "1丁目2-4", "postal_code": "4508501", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508601','{"jis": "23105", "kana": "ニツテツシヨウジ カブシキガイシヤ ナゴヤシテン", "name": "日鉄商事　株式会社　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅南", "banchi": "2丁目13番18号NSビル5階", "postal_code": "4508601", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('4508997','{"jis": "23105", "kana": "ニツポンユウセイ カブシキガイシヤ チユウブシセツセンタ-", "name": "日本郵政　株式会社　中部施設センター", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "一丁目1番1号JPタワー名古屋", "postal_code": "4508997", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508996','{"jis": "23105", "kana": "ニツポンユウセイ カブシキガイシヤ トウカイユウセイケンコウカンリセンタ-", "name": "日本郵政　株式会社　東海郵政健康管理センター", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "一丁目1番1号JPタワー名古屋", "postal_code": "4508996", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4698797','{"jis": "23105", "kana": "ニツポンユウビン カブシキガイシヤ トウカイシシヤ", "name": "日本郵便　株式会社　東海支社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "一丁目1番1号JPタワー名古屋", "postal_code": "4698797", "old_code": "450  ", "post_office": "名古屋神宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4508611','{"jis": "23105", "kana": "パナソニツク カブシキガイシヤ", "name": "パナソニック　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅南", "banchi": "二丁目7番55号パナソニック名古屋中村ビル", "postal_code": "4508611", "old_code": "450  ", "post_office": "名古屋西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキミナミ", "alternates": []}');
@@ -134542,19 +134476,19 @@
 INSERT INTO office_data VALUES('4538570','{"jis": "23105", "kana": "ダイワハウスコウギヨウ カブシキカイシヤ ナゴヤシシヤ", "name": "大和ハウス工業　株式会社　名古屋支社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60番地9", "postal_code": "4538570", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538704','{"jis": "23105", "kana": "チユウキヨウテレビホウソウ カブシキガイシヤ", "name": "中京テレビ放送　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60-11", "postal_code": "4538704", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538601','{"jis": "23105", "kana": "チユウブデンリヨクパワ-グリツド カブシキガイシヤ ナカムラエイギヨウシヨ", "name": "中部電力パワーグリッド　株式会社　中村営業所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤通", "banchi": "7丁目32", "postal_code": "4538601", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4538501','{"jis": "23105", "kana": "ナカムラクヤクシヨ", "name": "中村区役所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "松原町", "banchi": "1丁目23番地1", "postal_code": "4538501", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "マツバラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538505','{"jis": "23105", "kana": "ナカムラケンゼイジムシヨ", "name": "中村県税事務所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤", "banchi": "1丁目20-10", "postal_code": "4538505", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538626','{"jis": "23105", "kana": "ナゴヤシホンジンシゼイジムシヨ", "name": "名古屋市本陣市税事務所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "松原町", "banchi": "1丁目23番地の1", "postal_code": "4538626", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "マツバラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538511','{"jis": "23105", "kana": "ナゴヤダイイチセキジユウジビヨウイン", "name": "名古屋第一赤十字病院", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "道下町", "banchi": "3丁目35", "postal_code": "4538511", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ミチシタチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4538686','{"jis": "23105", "kana": "ナゴヤナカムラゼイムシヨ", "name": "名古屋中村税務署", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤", "banchi": "3丁目4-1", "postal_code": "4538686", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538580','{"jis": "23105", "kana": "メイジデンキコウギヨウ カブシキガイシヤ", "name": "明治電機工業　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "亀島", "banchi": "2丁目13-8", "postal_code": "4538580", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カメジマ", "alternates": []}');
 INSERT INTO office_data VALUES('4538522','{"jis": "23105", "kana": "ヤマダコウギヨウ カブシキガイシヤ", "name": "山田工業　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "竹橋町", "banchi": "9-9", "postal_code": "4538522", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タケバシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538777','{"jis": "23105", "kana": "ガツコウホウジン アイチダイガク ナゴヤコウシヤ", "name": "学校法人　愛知大学　名古屋校舎", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60番地6", "postal_code": "4538777", "old_code": "45308", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538662','{"jis": "23105", "kana": "トウカイデキストリン カブシキガイシヤ", "name": "東海デキストリン　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤通", "banchi": "6丁目88(中村郵便局私書箱第62号)", "postal_code": "4538662", "old_code": "45391", "post_office": "中村", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウトオリ", "alternates": []}');
-INSERT INTO office_data VALUES('4538686','{"jis": "23105", "kana": "ナゴヤナカムラゼイムシヨ", "name": "名古屋中村税務署", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤", "banchi": "3丁目4-1(中村郵便局私書箱第20号)", "postal_code": "4538686", "old_code": "45391", "post_office": "中村", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウ", "alternates": []}');
 INSERT INTO office_data VALUES('4608672','{"jis": "23106", "kana": "アイオイソンガイホケン カブシキガイシヤ", "name": "あいおい損害保険　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "千代田", "banchi": "5丁目7番5号(名古屋中郵便局私書箱第158号)", "postal_code": "4608672", "old_code": "460  ", "post_office": "名古屋中", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "チヨダ", "alternates": []}');
 INSERT INTO office_data VALUES('4608450','{"jis": "23106", "kana": "アイオイソンガイホケン カブシキガイシヤ ナゴヤサカエビル", "name": "あいおい損害保険　株式会社　名古屋栄ビル", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "栄", "banchi": "5丁目15番18号", "postal_code": "4608450", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サカエ", "alternates": []}');
 INSERT INTO office_data VALUES('4608512','{"jis": "23106", "kana": "アイチケン オワリジムシヨ", "name": "愛知県　尾張事務所", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "三の丸", "banchi": "2丁目6番1号", "postal_code": "4608512", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サンノマル", "alternates": []}');
 INSERT INTO office_data VALUES('4608566','{"jis": "23106", "kana": "アイチケン ジユウタクキヨウキユウコウシヤ", "name": "愛知県　住宅供給公社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "丸の内", "banchi": "3丁目19-30", "postal_code": "4608566", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('4608483','{"jis": "23106", "kana": "アイチケン ナゴヤトウブケンゼイジムシヨ", "name": "愛知県　名古屋東部県税事務所", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "新栄町", "banchi": "2丁目9番地", "postal_code": "4608483", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "シンサカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4608534','{"jis": "23106", "kana": "アイチケンキヨウイクイインカイ", "name": "愛知県教育委員会", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "三の丸", "banchi": "3丁目1番2号", "postal_code": "4608534", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サンノマル", "alternates": []}');
 INSERT INTO office_data VALUES('4608507','{"jis": "23106", "kana": "アイチロウドウキジユンキヨク", "name": "愛知労働基準局", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "三の丸", "banchi": "2丁目5-1名古屋合同庁舎第2号館", "postal_code": "4608507", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サンノマル", "alternates": []}');
@@ -134723,14 +134657,16 @@
 INSERT INTO office_data VALUES('4608708','{"jis": "23106", "kana": "ニツポンギンコウ ナゴヤシテン", "name": "日本銀行　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "2丁目1-1(名古屋中郵便局私書箱第111号)", "postal_code": "4608708", "old_code": "46091", "post_office": "名古屋中", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608689','{"jis": "23106", "kana": "ノムラシヨウケン カブシキガイシヤ ナゴヤシテン", "name": "野村證券　株式会社　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "2丁目19-22(名古屋中郵便局私書箱第58号)", "postal_code": "4608689", "old_code": "46091", "post_office": "名古屋中", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608679','{"jis": "23106", "kana": "モリリン カブシキガイシヤ ナゴヤシテン", "name": "モリリン　株式会社　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "2丁目4-14(名古屋中郵便局私書箱第62号)", "postal_code": "4608679", "old_code": "46091", "post_office": "名古屋中", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4668660','{"jis": "23107", "kana": "(カブ) ジヨツトインタ-ナシヨナル ナゴヤシテン", "name": "（株）　ジョットインターナショナル　名古屋支店", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "山手通", "banchi": "3丁目21ワイワイプラザ", "postal_code": "4668660", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ヤマノテトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4668558','{"jis": "23107", "kana": "アイチケン ジドウシヤカイカン", "name": "愛知県　自動車会館", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "滝子町", "banchi": "30番16号", "postal_code": "4668558", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タキコチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668501','{"jis": "23107", "kana": "アイチケンナゴヤナンブケンゼイジムシヨ タカツジカンゼイカ", "name": "愛知県名古屋南部県税事務所　高辻間税課", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "円上町", "banchi": "26番15号", "postal_code": "4668501", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "エンジョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668655','{"jis": "23107", "kana": "アイチケンホケンイキヨウカイ", "name": "愛知県保険医協会", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "妙見町", "banchi": "19-2", "postal_code": "4668655", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ミョウケンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4668688','{"jis": "23107", "kana": "アイチトヨタイ-スト カブシキガイシヤ", "name": "愛知トヨタＥＡＳＴ　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668688", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4668701','{"jis": "23107", "kana": "アイチトヨタウエスト カブシキガイシヤ", "name": "愛知トヨタＷＥＳＴ　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668701", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668554','{"jis": "23107", "kana": "アジノモト カブシキガイシヤ ナゴヤシシヤ", "name": "味の素　株式会社　名古屋支社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "阿由知通", "banchi": "2丁目3", "postal_code": "4668554", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "アユチトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4668515','{"jis": "23107", "kana": "アンドウ カブシキガイシヤ", "name": "安藤　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "白金", "banchi": "1丁目16-7", "postal_code": "4668515", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "シラカネ", "alternates": []}');
 INSERT INTO office_data VALUES('4668580','{"jis": "23107", "kana": "イツパンシヤダンホウジン ニホンジドウシヤレンメイ アイチシブ", "name": "一般社団法人　日本自動車連盟　愛知支部", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "福江", "banchi": "3丁目7番56号", "postal_code": "4668580", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "フクエ", "alternates": []}');
 INSERT INTO office_data VALUES('4668565','{"jis": "23107", "kana": "イツパンシヤダンホウジン ニホンジドウシヤレンメイ チユウブホンブ", "name": "一般社団法人　日本自動車連盟　中部本部", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "福江", "banchi": "3丁目7番56号", "postal_code": "4668565", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "フクエ", "alternates": []}');
 INSERT INTO office_data VALUES('4668539','{"jis": "23107", "kana": "カブシキガイシヤ イツコウ ナゴヤシテン", "name": "株式会社　一光　名古屋支店", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "福江", "banchi": "1丁目19-23", "postal_code": "4668539", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "フクエ", "alternates": []}');
 INSERT INTO office_data VALUES('4668636','{"jis": "23107", "kana": "カブシキガイシヤ エイテイビジネス", "name": "株式会社　ＡＴビジネス", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668636", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668507','{"jis": "23107", "kana": "カブシキガイシヤ キソジ", "name": "株式会社　木曽路", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "白金", "banchi": "3丁目18-13", "postal_code": "4668507", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "シラカネ", "alternates": []}');
@@ -134744,30 +134680,26 @@
 INSERT INTO office_data VALUES('4668512','{"jis": "23107", "kana": "タケダインサツ カブシキガイシヤ", "name": "竹田印刷　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "白金", "banchi": "1丁目11-10", "postal_code": "4668512", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "シラカネ", "alternates": []}');
 INSERT INTO office_data VALUES('4668711','{"jis": "23107", "kana": "タツミヤコウギヨウ カブシキガイシヤ", "name": "辰巳屋興業　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "白金", "banchi": "3丁目20-15", "postal_code": "4668711", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "シラカネ", "alternates": []}');
 INSERT INTO office_data VALUES('4668657','{"jis": "23107", "kana": "ダイガクセイキヨウ トウカイカイカン", "name": "大学生協　東海会館", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "山手通", "banchi": "2丁目16-1", "postal_code": "4668657", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ヤマノテトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4668511','{"jis": "23107", "kana": "チユウオウコウキ カブシキガイシヤ", "name": "中央工機　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "4-3", "postal_code": "4668511", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668666','{"jis": "23107", "kana": "チユウキヨウダイガク", "name": "中京大学", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "八事本町", "banchi": "101-2", "postal_code": "4668666", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ヤゴトホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4668525','{"jis": "23107", "kana": "チユウキヨウダイガクフゾク チユウキヨウコウトウガツコウ", "name": "中京大学附属　中京高等学校", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "川名山町", "banchi": "122", "postal_code": "4668525", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "カワナヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668502','{"jis": "23107", "kana": "トヨタエルアンドエフチユウブ カブシキガイシヤ", "name": "トヨタＬ＆Ｆ中部　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668502", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4668508','{"jis": "23107", "kana": "トヨタカロ-ラアイホウ カブシキガイシヤ", "name": "トヨタカローラ愛豊　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668508", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668555','{"jis": "23107", "kana": "ナゴヤコウギヨウダイガク", "name": "名古屋工業大学", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "御器所町", "banchi": "", "postal_code": "4668555", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ゴキソチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668585','{"jis": "23107", "kana": "ナゴヤシシヨウワクヤクシヨ", "name": "名古屋市昭和区役所", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "阿由知通", "banchi": "3丁目19", "postal_code": "4668585", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "アユチトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4668550','{"jis": "23107", "kana": "ナゴヤダイガク イガクブ", "name": "名古屋大学　医学部", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "鶴舞町", "banchi": "65", "postal_code": "4668550", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ツルマイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668560','{"jis": "23107", "kana": "ナゴヤダイガク イガクブ フゾクビヨウイン", "name": "名古屋大学　医学部　附属病院", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "鶴舞町", "banchi": "65", "postal_code": "4668560", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ツルマイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668650','{"jis": "23107", "kana": "ナゴヤダイニセキジユウジビヨウイン", "name": "名古屋第二赤十字病院", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "妙見町", "banchi": "2-9", "postal_code": "4668650", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ミョウケンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668673','{"jis": "23107", "kana": "ナンザンダイガク", "name": "南山大学", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "山里町", "banchi": "18", "postal_code": "4668673", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ヤマザトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668567','{"jis": "23107", "kana": "ニツポンネンキンキコウ シヨウワネンキンジムシヨ", "name": "日本年金機構　昭和年金事務所", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "桜山町", "banchi": "5丁目99番地6", "postal_code": "4668567", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "サクラヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668522','{"jis": "23107", "kana": "ニツポンペイントハンバイ カブシキガイシヤ チユウブシテン", "name": "日本ペイント販売　株式会社　中部支社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "白金", "banchi": "3丁目18-26", "postal_code": "4668522", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "シラカネ", "alternates": []}');
-INSERT INTO office_data VALUES('4668610','{"jis": "23107", "kana": "ネツツトヨタアイチ カブシキガイシヤ", "name": "ネッツトヨタ愛知　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668610", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4668688','{"jis": "23107", "kana": "ネツツトヨタトウカイ カブシキガイシヤ", "name": "ネッツトヨタ東海　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6番8号", "postal_code": "4668688", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668588','{"jis": "23107", "kana": "パイロツトインキ カブシキガイシヤ", "name": "パイロットインキ　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "緑町", "banchi": "3丁目17", "postal_code": "4668588", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ミドリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668506','{"jis": "23107", "kana": "ミヤキチガラス カブシキガイシヤ", "name": "宮吉硝子　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "福江", "banchi": "3丁目7-2", "postal_code": "4668506", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "フクエ", "alternates": []}');
 INSERT INTO office_data VALUES('4668656','{"jis": "23107", "kana": "ヤザキソウギヨウ カブシキガイシヤ ナゴヤシテン", "name": "矢崎総業　株式会社　名古屋支店", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "山手通", "banchi": "3丁目21", "postal_code": "4668656", "old_code": "466  ", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "ヤマノテトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4668635','{"jis": "23107", "kana": "チユウキヨウテレビホウソウ カブシキガイシヤ", "name": "中京テレビ放送　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高峯町", "banchi": "154", "postal_code": "4668635", "old_code": "46635", "post_office": "昭和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカミネチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4668701','{"jis": "23107", "kana": "アイチトヨタジドウシヤ カブシキガイシヤ", "name": "愛知トヨタ自動車　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高辻町", "banchi": "6-8(昭和郵便局私書箱第39号)", "postal_code": "4668701", "old_code": "46691", "post_office": "昭和", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカツジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4668707','{"jis": "23107", "kana": "チユウキヨウテレビホウソウ カブシキガイシヤ", "name": "中京テレビ放送　株式会社", "prefecture": "愛知県", "city": "名古屋市昭和区", "neighborhood": "高峯町", "banchi": "154(昭和郵便局私書箱第123号)", "postal_code": "4668707", "old_code": "46691", "post_office": "昭和", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシショウワク", "neighborhood_kana": "タカミネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4678633','{"jis": "23108", "kana": "(イ)シンセイカイ シンセイカイ・ダイイチビヨウイン", "name": "（医）新生会　新生会・第一病院", "prefecture": "愛知県", "city": "名古屋市瑞穂区", "neighborhood": "玉水町", "banchi": "1丁目3-2", "postal_code": "4678633", "old_code": "467  ", "post_office": "瑞穂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシミズホク", "neighborhood_kana": "タマミズチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4678639','{"jis": "23108", "kana": "アイチケンリツシヨウワコウコウ", "name": "愛知県立昭和高校", "prefecture": "愛知県", "city": "名古屋市瑞穂区", "neighborhood": "玉水町", "banchi": "1丁目18", "postal_code": "4678639", "old_code": "467  ", "post_office": "瑞穂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシミズホク", "neighborhood_kana": "タマミズチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4678588','{"jis": "23108", "kana": "アイチヒノジドウシヤ カブシキガイシヤ", "name": "愛知日野自動車　株式会社", "prefecture": "愛知県", "city": "名古屋市瑞穂区", "neighborhood": "神穂町", "banchi": "7-1", "postal_code": "4678588", "old_code": "467  ", "post_office": "瑞穂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシミズホク", "neighborhood_kana": "カミホチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4678580','{"jis": "23108", "kana": "アミテツク カブシキガイシヤ", "name": "アミテック　株式会社", "prefecture": "愛知県", "city": "名古屋市瑞穂区", "neighborhood": "内浜町", "banchi": "31-25", "postal_code": "4678580", "old_code": "467  ", "post_office": "瑞穂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシミズホク", "neighborhood_kana": "ウチハマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4678571','{"jis": "23108", "kana": "イシハラシヨウジ カブシキガイシヤ", "name": "石原商事　株式会社", "prefecture": "愛知県", "city": "名古屋市瑞穂区", "neighborhood": "塩入町", "banchi": "19-12", "postal_code": "4678571", "old_code": "467  ", "post_office": "瑞穂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシミズホク", "neighborhood_kana": "シオイリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4678555','{"jis": "23108", "kana": "イツパンシヤダンホウジン アイチケントラツクキヨウカイ", "name": "一般社団法人　愛知県トラック協会", "prefecture": "愛知県", "city": "名古屋市瑞穂区", "neighborhood": "新開町", "banchi": "12-6", "postal_code": "4678555", "old_code": "467  ", "post_office": "瑞穂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシミズホク", "neighborhood_kana": "シンカイチョウ", "alternates": []}');
@@ -135515,29 +135447,30 @@
 INSERT INTO office_data VALUES('4848502','{"jis": "23215", "kana": "ムラタキカイ カブシキガイシヤ イヌヤマコウジヨウ", "name": "村田機械　株式会社　犬山工場", "prefecture": "愛知県", "city": "犬山市", "neighborhood": "大字橋爪", "banchi": "字中島2", "postal_code": "4848502", "old_code": "484  ", "post_office": "犬山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4798601','{"jis": "23216", "kana": "アイチチタ ノウギヨウキヨウドウクミアイ", "name": "あいち知多　農業協同組合", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "多屋", "banchi": "字茨廻間1番地111(常滑郵便局私書箱第5号)", "postal_code": "4798601", "old_code": "479  ", "post_office": "常滑", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "タヤ", "alternates": []}');
 INSERT INTO office_data VALUES('4798586','{"jis": "23216", "kana": "イナツクスライブミユ-ジアム", "name": "ＩＮＡＸライブミュージアム", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "奥栄町", "banchi": "1丁目130番地", "postal_code": "4798586", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "オクエイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798511','{"jis": "23216", "kana": "カブシキガイシヤ デンソ-ダイシン", "name": "株式会社　デンソーダイシン", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "久米", "banchi": "字御林200番地", "postal_code": "4798511", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "クメ", "alternates": []}');
 INSERT INTO office_data VALUES('4798623','{"jis": "23216", "kana": "カブシキガイシヤ マキノ", "name": "株式会社　マキノ", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "大曽町", "banchi": "3丁目1番地", "postal_code": "4798623", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "オオソチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798588','{"jis": "23216", "kana": "カブシキガイシヤ リクシル エノキドコウジヨウ", "name": "株式会社　ＬＩＸＩＬ　榎戸工場", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "港町", "banchi": "3丁目77番地", "postal_code": "4798588", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "ミナトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798589','{"jis": "23216", "kana": "カブシキガイシヤ リクシル オオタニコウジヨウ", "name": "株式会社　ＬＩＸＩＬ　大谷工場", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "大谷", "banchi": "字坂森50番地", "postal_code": "4798589", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "オオタニ", "alternates": []}');
+INSERT INTO office_data VALUES('4798587','{"jis": "23216", "kana": "カブシキガイシヤ リクシル トコナメヒガシコウジヨウ", "name": "株式会社　ＬＩＸＩＬ　常滑東工場", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "奥栄町", "banchi": "1丁目47番地", "postal_code": "4798587", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "オクエイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798585','{"jis": "23216", "kana": "カブシキガイシヤ リクシル トコナメホンシヤ", "name": "株式会社　ＬＩＸＩＬ　常滑本社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "鯉江本町", "banchi": "5丁目1番地", "postal_code": "4798585", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "コイエホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4798787','{"jis": "23216", "kana": "コクドコウツウシヨウオオサカコウクウキヨク チユウブクウコウジムシヨ", "name": "国土交通省大阪航空局中部空港事務所", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "1丁目1番", "postal_code": "4798787", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798577','{"jis": "23216", "kana": "ジヤニスコウギヨウ カブシキガイシヤ", "name": "ジャニス工業　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "唐崎町", "banchi": "2丁目88", "postal_code": "4798577", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "カラサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798555','{"jis": "23216", "kana": "チタハントウケ-ブルネツトワ-ク カブシキガイシヤ", "name": "知多半島ケーブルネットワーク　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "かじま台", "banchi": "一丁目161", "postal_code": "4798555", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "カジマダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4798701','{"jis": "23216", "kana": "チユウブコクサイクウコウ カブシキガイシヤ", "name": "中部国際空港　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "一丁目1番地第1セントレアビル6F", "postal_code": "4798701", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798712','{"jis": "23216", "kana": "チユウブコクサイクウコウ カブシキガイシヤ コウクウエイギヨウブカモツエイギヨウグル-プ", "name": "中部国際空港　株式会社　航空営業部貨物営業グループ", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "一丁目2番地貨物地区貨物事務棟2F", "postal_code": "4798712", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798711','{"jis": "23216", "kana": "チユウブコクサイクウコウ カブシキガイシヤ ソウムブジンジグル-プシンソツサイヨウタントウ", "name": "中部国際空港　株式会社　総務部人事グループ新卒採用担当", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "1丁目1番地第1セントレアビル6F", "postal_code": "4798711", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798705','{"jis": "23216", "kana": "チユウブコクサイクウコウエネルギ-キヨウキユウ カブシキガイシヤ", "name": "中部国際空港エネルギー供給　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "1丁目1エネルギーセンター", "postal_code": "4798705", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798706','{"jis": "23216", "kana": "チユウブコクサイクウコウキユウユシセツ カブシキガイシヤ", "name": "中部国際空港給油施設　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "5丁目4中部国際空港航空機給油施設内", "postal_code": "4798706", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798703','{"jis": "23216", "kana": "チユウブコクサイクウコウシセツサ-ビス カブシキガイシヤ", "name": "中部国際空港施設サービス　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "一丁目1番地第1セントレアビル4階", "postal_code": "4798703", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798702','{"jis": "23216", "kana": "チユウブコクサイクウコウジヨウホウツウシン カブシキガイシヤ", "name": "中部国際空港情報通信　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "一丁目1番地第1セントレアビル2階", "postal_code": "4798702", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798704','{"jis": "23216", "kana": "チユウブコクサイクウコウリヨキヤクサ-ビス カブシキガイシヤ", "name": "中部国際空港旅客サービス　株式会社", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "一丁目1番地第2セントレアビル3階", "postal_code": "4798704", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798501','{"jis": "23216", "kana": "トコナメシボ-トレ-スジギヨウキヨク", "name": "常滑市ボートレース事業局", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "新開町", "banchi": "4丁目111番地", "postal_code": "4798501", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "シンカイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798510','{"jis": "23216", "kana": "トコナメシミンビヨウイン", "name": "常滑市民病院", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "飛香台", "banchi": "3丁目3番地の3", "postal_code": "4798510", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "アスカダイ", "alternates": []}');
-INSERT INTO office_data VALUES('4798610','{"jis": "23216", "kana": "トコナメシヤクシヨ", "name": "常滑市役所", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "新開町", "banchi": "4丁目1(常滑郵便局私書箱第1号)", "postal_code": "4798610", "old_code": "479  ", "post_office": "常滑", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "シンカイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4798610','{"jis": "23216", "kana": "トコナメシヤクシヨ", "name": "常滑市役所", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "飛香台", "banchi": "3丁目3番地の5(常滑郵便局私書箱第1号)", "postal_code": "4798610", "old_code": "479  ", "post_office": "常滑", "type": "box", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "アスカダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4798668','{"jis": "23216", "kana": "トコナメシヨウコウカイギシヨ", "name": "常滑商工会議所", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "新開町", "banchi": "5丁目58(常滑郵便局私書箱第4号)", "postal_code": "4798668", "old_code": "479  ", "post_office": "常滑", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "シンカイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4798708','{"jis": "23216", "kana": "ナゴヤゼカンチユウブクウコウゼイカンシシヨ(チユウブクウコウゴウドウチヨウシヤ)", "name": "名古屋税関中部空港税関支署（中部空港合同庁舎）", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "1丁目1番中部空港合同庁舎内", "postal_code": "4798708", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798707','{"jis": "23216", "kana": "ナゴヤゼカンチユウブクウコウゼイカンシシヨ(チユウブクウコウCIQチヨウシヤ)", "name": "名古屋税関中部空港税関支署（中部空港ＣＩＱ庁舎）", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "セントレア", "banchi": "1丁目1番中部空港CIQ庁舎内", "postal_code": "4798707", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "セントレア", "alternates": []}');
 INSERT INTO office_data VALUES('4798518','{"jis": "23216", "kana": "マルモコウギヨウ カブシキガイシヤ", "name": "丸茂工業", "prefecture": "愛知県", "city": "常滑市", "neighborhood": "小林町", "banchi": "1丁目30", "postal_code": "4798518", "old_code": "479  ", "post_office": "常滑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トコナメシ", "neighborhood_kana": "コバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4838704','{"jis": "23217", "kana": "アイチケンコウセイノウギヨウキヨウドウクミアイレンゴウカイ コウナンコウセイビヨウイン", "name": "愛知県厚生農業協同組合連合会　江南厚生病院", "prefecture": "愛知県", "city": "江南市", "neighborhood": "高屋町大松原", "banchi": "137番地", "postal_code": "4838704", "old_code": "483  ", "post_office": "江南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "コウナンシ", "neighborhood_kana": "タカヤチョウオオマツバラ", "alternates": []}');
 INSERT INTO office_data VALUES('4838507','{"jis": "23217", "kana": "アピタ コウナンテン", "name": "アピタ　江南店", "prefecture": "愛知県", "city": "江南市", "neighborhood": "村久野町瀬頭", "banchi": "163", "postal_code": "4838507", "old_code": "483  ", "post_office": "江南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "コウナンシ", "neighborhood_kana": "ムラクノチョウセガシラ", "alternates": []}');
 INSERT INTO office_data VALUES('4838502','{"jis": "23217", "kana": "カブシキガイシヤ ミサワテクノ", "name": "株式会社　ミサワテクノ", "prefecture": "愛知県", "city": "江南市", "neighborhood": "前野町東", "banchi": "2番地の1", "postal_code": "4838502", "old_code": "483  ", "post_office": "江南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "コウナンシ", "neighborhood_kana": "マエノチョウヒガシ", "alternates": []}');
@@ -135609,15 +135542,15 @@
 INSERT INTO office_data VALUES('4958505','{"jis": "23220", "kana": "アイチケンリツ キヨウワコウトウガツコウ", "name": "愛知県立　杏和高等学校", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町二俣", "banchi": "宮西1番地1", "postal_code": "4958505", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウフタマタ", "alternates": []}');
 INSERT INTO office_data VALUES('4958511','{"jis": "23220", "kana": "イナザワシ ソブエシシヨ", "name": "稲沢市　祖父江支所", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町山崎", "banchi": "鶴塚275番地1", "postal_code": "4958511", "old_code": "495  ", "post_office": "一宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウヤマザキ", "alternates": []}');
 INSERT INTO office_data VALUES('4958601','{"jis": "23220", "kana": "オウジマテリア カブシキガイシヤ ソブエコウジヨウ", "name": "王子マテリア　株式会社　祖父江工場", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町祖父江", "banchi": "外平150番地", "postal_code": "4958601", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウソブエ", "alternates": []}');
 INSERT INTO office_data VALUES('4958517','{"jis": "23220", "kana": "カブシキガイシヤ コメツトカトウ", "name": "株式会社　コメットカトウ", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町甲新田", "banchi": "イ九-65", "postal_code": "4958517", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウカブトシンデン", "alternates": []}');
 INSERT INTO office_data VALUES('4958510','{"jis": "23220", "kana": "テイジンテクロス カブシキガイシヤ", "name": "帝人テクロス　株式会社", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町四貫", "banchi": "堤外22番地", "postal_code": "4958510", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウヨツノキ", "alternates": []}');
 INSERT INTO office_data VALUES('4411392','{"jis": "23221", "kana": "シンシロシヤクシヨ", "name": "新城市役所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "字東入船", "banchi": "115番地", "postal_code": "4411392", "old_code": "44113", "post_office": "新城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4411492','{"jis": "23221", "kana": "シンシロシ ツクデソウゴウシシヨ", "name": "新城市　作手総合支所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "作手高里", "banchi": "字縄手上32番地", "postal_code": "4411492", "old_code": "44114", "post_office": "作手", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "シンシロシ", "neighborhood_kana": "ツクデタカサト", "alternates": []}');
-INSERT INTO office_data VALUES('4411692','{"jis": "23221", "kana": "シンシロシ ホウライソウゴウシシヨ", "name": "新城市　鳳来総合支所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "長篠", "banchi": "字仲野16番地11", "postal_code": "4411692", "old_code": "44116", "post_office": "長篠", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "シンシロシ", "neighborhood_kana": "ナガシノ", "alternates": []}');
+INSERT INTO office_data VALUES('4411692','{"jis": "23221", "kana": "シンシロシ ホウライソウゴウシシヨ", "name": "新城市　鳳来総合支所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "長篠", "banchi": "字仲野16番地11", "postal_code": "4411692", "old_code": "44116", "post_office": "長篠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "シンシロシ", "neighborhood_kana": "ナガシノ", "alternates": []}');
 INSERT INTO office_data VALUES('4768666','{"jis": "23222", "kana": "アイチセイコウ カブシキガイシヤ", "name": "愛知製鋼　株式会社", "prefecture": "愛知県", "city": "東海市", "neighborhood": "荒尾町", "banchi": "ワノ割1(東海北郵便局私書箱第3号)", "postal_code": "4768666", "old_code": "476  ", "post_office": "東海北", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "アラオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768585','{"jis": "23222", "kana": "カゴメ カブシキガイシヤ ウエノコウジヨウ", "name": "カゴメ　株式会社　上野工場", "prefecture": "愛知県", "city": "東海市", "neighborhood": "荒尾町", "banchi": "東屋敷108", "postal_code": "4768585", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "アラオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768577','{"jis": "23222", "kana": "カブシキガイシヤ バンカク ソウホンポ", "name": "株式会社　坂角　総本舗", "prefecture": "愛知県", "city": "東海市", "neighborhood": "荒尾町", "banchi": "甚造15-1", "postal_code": "4768577", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "アラオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768588','{"jis": "23222", "kana": "ガツコウホウジン ナゴヤイシダガクエン セイジヨウダイガク", "name": "学校法人　名古屋石田学園　星城大学", "prefecture": "愛知県", "city": "東海市", "neighborhood": "富貴ノ台", "banchi": "2丁目172", "postal_code": "4768588", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "フキノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4768510','{"jis": "23222", "kana": "キヨウエイコウギヨウカブシキガイシヤ.キヨウエイコウキカブシキガイシヤ.キヨウエイウンユカブシキガイシヤ.キヨウエイコウアツガスカブシキガイシヤ", "name": "協栄興業株式会社、協栄工機株式会社、協栄運輸株式会社、協栄高圧ガス株式会社", "prefecture": "愛知県", "city": "東海市", "neighborhood": "南柴田町", "banchi": "ルノ割426-4", "postal_code": "4768510", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "ミナミシバタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768686','{"jis": "23222", "kana": "シンニホンセイテツ カブシキガイシヤ ナゴヤセイテツシヨ", "name": "新日本製鐵　株式會社　名古屋製鐵所", "prefecture": "愛知県", "city": "東海市", "neighborhood": "東海町", "banchi": "5丁目3番地1(東海北郵便局私書箱第1号)", "postal_code": "4768686", "old_code": "476  ", "post_office": "東海北", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "トウカイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768503','{"jis": "23222", "kana": "タイヨウプラスチツク", "name": "大洋プラスチック", "prefecture": "愛知県", "city": "東海市", "neighborhood": "富木島町伏見", "banchi": "4丁目1-8", "postal_code": "4768503", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "フキシママチフシミ", "alternates": []}');
@@ -135638,14 +135571,15 @@
 INSERT INTO office_data VALUES('4748710','{"jis": "23223", "kana": "アイチシヨウニホケンイリヨウソウゴウセンタ-", "name": "あいち小児保健医療総合センター", "prefecture": "愛知県", "city": "大府市", "neighborhood": "森岡町", "banchi": "尾坂田1番2", "postal_code": "4748710", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "モリオカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748510','{"jis": "23223", "kana": "イヅミコウギヨウ カブシキガイシヤ", "name": "イヅミ工業　株式会社", "prefecture": "愛知県", "city": "大府市", "neighborhood": "北崎町", "banchi": "清水1-3", "postal_code": "4748510", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キタサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748503','{"jis": "23223", "kana": "オオブシヨウコウカイギシヨ", "name": "大府商工会議所", "prefecture": "愛知県", "city": "大府市", "neighborhood": "中央町", "banchi": "5丁目70番地", "postal_code": "4748503", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748585','{"jis": "23223", "kana": "カブシキガイシヤ アペツクス", "name": "株式会社　アペックス", "prefecture": "愛知県", "city": "大府市", "neighborhood": "大府町", "banchi": "柊山11", "postal_code": "4748585", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "オオブマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4748581','{"jis": "23223", "kana": "カブシキガイシヤ アンセイ", "name": "株式会社　アンセイ", "prefecture": "愛知県", "city": "大府市", "neighborhood": "北崎町", "banchi": "大島30", "postal_code": "4748581", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キタサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748558','{"jis": "23223", "kana": "カブシキガイシヤ トウカイリキセイサクジヨ ナガネコウジヨウ", "name": "株式会社　東海理機製作所　長根工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "長根町", "banchi": "2丁目290", "postal_code": "4748558", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "ナガネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748611','{"jis": "23223", "kana": "カブシキガイシヤ トミシンジユウタクセツビ", "name": "株式会社　富新住宅設備", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共栄町", "banchi": "9丁目1-4", "postal_code": "4748611", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウエイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4748668','{"jis": "23223", "kana": "カブシキガイシヤ トヨタジドウシヨツキ オオブコウジヨウ", "name": "株式会社　豊田自動織機　大府工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "江端町", "banchi": "一丁目一番地", "postal_code": "4748668", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "エバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748601','{"jis": "23223", "kana": "カブシキガイシヤ トヨタジドウシヨツキセイサクシヨ キヨウワコウジヨウ", "name": "株式会社　豊田自動織機製作所　共和工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共和町", "banchi": "茶屋8", "postal_code": "4748601", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748502','{"jis": "23223", "kana": "カブシキガイシヤ ニイハマテツコウジヨ ナゴヤコウジヨウ", "name": "株式会社　新居浜鐵工所　名古屋工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "横根町", "banchi": "惣作208", "postal_code": "4748502", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "ヨコネマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4748584','{"jis": "23223", "kana": "カブシキガイシヤ ハツシン", "name": "株式会社　八神", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共和町", "banchi": "3-8-9", "postal_code": "4748584", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748610','{"jis": "23223", "kana": "カブシキガイシヤ フジプレス", "name": "株式会社　富士プレス", "prefecture": "愛知県", "city": "大府市", "neighborhood": "北崎町", "banchi": "井田118", "postal_code": "4748610", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キタサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748543','{"jis": "23223", "kana": "カブシキガイシヤ メイナンセイサクジヨ", "name": "株式会社　名南製作所", "prefecture": "愛知県", "city": "大府市", "neighborhood": "梶田町", "banchi": "3丁目130", "postal_code": "4748543", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "カジタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748511','{"jis": "23223", "kana": "コクリツケンキユウカイハツホウジン コクリツチヨウジユイリヨウケンキユウセンタ-", "name": "国立研究開発法人　国立長寿医療研究センター", "prefecture": "愛知県", "city": "大府市", "neighborhood": "森岡町", "banchi": "7-430", "postal_code": "4748511", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "モリオカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748651','{"jis": "23223", "kana": "シガツカンダイガク", "name": "至学館大学", "prefecture": "愛知県", "city": "大府市", "neighborhood": "横根町", "banchi": "名高山55番地", "postal_code": "4748651", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "ヨコネマチ", "alternates": []}');
@@ -135757,15 +135691,15 @@
 INSERT INTO office_data VALUES('4818502','{"jis": "23234", "kana": "ナゴヤジユウガクイン", "name": "名古屋自由学院", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "熊之庄", "banchi": "古井281", "postal_code": "4818502", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "クマノショウ", "alternates": []}');
 INSERT INTO office_data VALUES('4818504','{"jis": "23234", "kana": "ナゴヤジユウガクイン タンキダイガク", "name": "名古屋自由学院　短期大学", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "熊之庄", "banchi": "古井281", "postal_code": "4818504", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "クマノショウ", "alternates": []}');
 INSERT INTO office_data VALUES('4818508','{"jis": "23234", "kana": "ニツシンデンキ カブシキガイシヤ", "name": "日進電気　株式会社", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "六ツ師", "banchi": "女夫越5", "postal_code": "4818508", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "ムツシ", "alternates": []}');
 INSERT INTO office_data VALUES('4988502','{"jis": "23235", "kana": "アイチケンコウセイノウギヨウキヨウドウクミアイレンゴウカイ カイナンビヨウイン", "name": "愛知県厚生農業協同組合連合会　海南病院", "prefecture": "愛知県", "city": "弥富市", "neighborhood": "前ケ須町", "banchi": "南本田396", "postal_code": "4988502", "old_code": "498  ", "post_office": "弥富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヤトミシ", "neighborhood_kana": "マエガスチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4988505','{"jis": "23235", "kana": "カブシキガイシヤ カワスミ", "name": "株式会社　川スミ", "prefecture": "愛知県", "city": "弥富市", "neighborhood": "鯏浦町", "banchi": "南前新田215", "postal_code": "4988505", "old_code": "498  ", "post_office": "弥富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヤトミシ", "neighborhood_kana": "ウグイウラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4988501','{"jis": "23235", "kana": "ヤトミシヤクシヨ", "name": "弥富市役所", "prefecture": "愛知県", "city": "弥富市", "neighborhood": "前ケ須町", "banchi": "南本田335", "postal_code": "4988501", "old_code": "498  ", "post_office": "弥富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヤトミシ", "neighborhood_kana": "マエガスチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4700292','{"jis": "23236", "kana": "エヌシ-エ-", "name": "ＮＣＡ", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "莇生町", "banchi": "下永井田20", "postal_code": "4700292", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "アザブチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4700297','{"jis": "23236", "kana": "カブシキカイシヤ コウソク チユウキヨウエイギヨウブ", "name": "株式会社　高速　中京営業部", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "根浦町", "banchi": "七丁目2番地1", "postal_code": "4700297", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ネウラマチ", "alternates": []}');
+INSERT INTO office_data VALUES('4700297','{"jis": "23236", "kana": "カブシキカイシヤ コウソク チユウキヨウエイギヨウブ", "name": "株式会社　高速　中京営業部", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "根浦町", "banchi": "七丁目2番地1", "postal_code": "4700297", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ネウラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4700294','{"jis": "23236", "kana": "カブシキガイシヤ サンゴ", "name": "株式会社　三五", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "福田町", "banchi": "宮下1番1", "postal_code": "4700294", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "フクタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4700293','{"jis": "23236", "kana": "ノリタケカンパニ-", "name": "ノリタケカンパニー", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "三好町", "banchi": "東山300", "postal_code": "4700293", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ミヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4700295','{"jis": "23236", "kana": "ミヨシシヤクシヨ", "name": "みよし市役所", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "三好町", "banchi": "小坂50", "postal_code": "4700295", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ミヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4901198','{"jis": "23237", "kana": "アマシヤクシヨ ジモクジチヨウシヤ", "name": "あま市役所　甚目寺庁舎", "prefecture": "愛知県", "city": "あま市", "neighborhood": "甚目寺", "banchi": "二伴田76番地", "postal_code": "4901198", "old_code": "49011", "post_office": "甚目寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "ジモクジ", "alternates": []}');
 INSERT INTO office_data VALUES('4901194','{"jis": "23237", "kana": "カブシキガイシヤ カマクラハム", "name": "株式会社　鎌倉ハム", "prefecture": "愛知県", "city": "あま市", "neighborhood": "中萱津", "banchi": "紺屋田30", "postal_code": "4901194", "old_code": "49011", "post_office": "甚目寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "ナカカヤヅ", "alternates": []}');
 INSERT INTO office_data VALUES('4901193','{"jis": "23237", "kana": "カブシキガイシヤ コ-ワ", "name": "株式会社　コーワ", "prefecture": "愛知県", "city": "あま市", "neighborhood": "西今宿", "banchi": "平割一22", "postal_code": "4901193", "old_code": "49011", "post_office": "甚目寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "ニシイマジュク", "alternates": []}');
 INSERT INTO office_data VALUES('4901296','{"jis": "23237", "kana": "アサヒチユウブシザイ カブシキカイシヤ", "name": "旭中部資材　株式会社", "prefecture": "愛知県", "city": "あま市", "neighborhood": "乙之子", "banchi": "八反田12", "postal_code": "4901296", "old_code": "49012", "post_office": "美和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "オトノコ", "alternates": []}');
@@ -136672,15 +136606,15 @@
 INSERT INTO office_data VALUES('5338555','{"jis": "27114", "kana": "カブシキガイシヤ キ-エンス", "name": "株式会社　キーエンス", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "東中島", "banchi": "1丁目3-14", "postal_code": "5338555", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ヒガシナカジマ", "alternates": []}');
 INSERT INTO office_data VALUES('5338585','{"jis": "27114", "kana": "カブシキガイシヤ ダイヤモンドプレス", "name": "株式会社　ダイヤモンドプレス", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "豊新", "banchi": "4丁目21-1", "postal_code": "5338585", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ホウシン", "alternates": []}');
 INSERT INTO office_data VALUES('5338651','{"jis": "27114", "kana": "サンテンセイヤク カブシキガイシヤ", "name": "参天製薬　株式会社", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "下新庄", "banchi": "3丁目9番31号", "postal_code": "5338651", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "シモシンジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5338502','{"jis": "27114", "kana": "スギモトシヨウジ カブシキガイシヤ ホンシヤ", "name": "杉本商事　株式会社　本社", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "豊新", "banchi": "5-6-27", "postal_code": "5338502", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ホウシン", "alternates": []}');
 INSERT INTO office_data VALUES('5338501','{"jis": "27114", "kana": "ヒガシヨドガワクヤクシヨ", "name": "東淀川区役所", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "豊新", "banchi": "2丁目1-4", "postal_code": "5338501", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ホウシン", "alternates": []}');
 INSERT INTO office_data VALUES('5338558','{"jis": "27114", "kana": "ライフコ-ポレ-シヨン", "name": "ライフコーポレーション", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "東中島", "banchi": "1丁目19-4", "postal_code": "5338558", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ヒガシナカジマ", "alternates": []}');
 INSERT INTO office_data VALUES('5378686','{"jis": "27115", "kana": "コクヨ カブシキガイシヤ", "name": "コクヨ　（株）", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "大今里南", "banchi": "6丁目1-1(東成郵便局私書箱第5号)", "postal_code": "5378686", "old_code": "537  ", "post_office": "東成", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "オオイマザトミナミ", "alternates": []}');
-INSERT INTO office_data VALUES('5378911','{"jis": "27115", "kana": "ザ・パツク カブシキガイシヤ", "name": "ザ・パック　株式会社", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "東小橋", "banchi": "2丁目9番3号", "postal_code": "5378911", "old_code": "537  ", "post_office": "東成", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "ヒガシオバセ", "alternates": []}');
+INSERT INTO office_data VALUES('5378911','{"jis": "27115", "kana": "ザ・パツク カブシキガイシヤ", "name": "ザ・パック　株式会社", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "東小橋", "banchi": "2丁目9番3号", "postal_code": "5378911", "old_code": "537  ", "post_office": "東成", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "ヒガシオバセ", "alternates": []}');
 INSERT INTO office_data VALUES('5378501','{"jis": "27115", "kana": "ヒガシナリクヤクシヨ", "name": "東成区役所", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "大今里西", "banchi": "2丁目8-4", "postal_code": "5378501", "old_code": "537  ", "post_office": "東成", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "オオイマザトニシ", "alternates": []}');
 INSERT INTO office_data VALUES('5448501','{"jis": "27116", "kana": "イクノクヤクシヨ", "name": "生野区役所", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "勝山南", "banchi": "3丁目1-19", "postal_code": "5448501", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "カツヤマミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('5448555','{"jis": "27116", "kana": "イクノゼイムシヨ", "name": "生野税務署", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "勝山北", "banchi": "5丁目22-14", "postal_code": "5448555", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "カツヤマキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5448585','{"jis": "27116", "kana": "カブシキガイシヤ モリタホ-ルデイングス", "name": "株式会社　モリタホールディングス", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "小路東", "banchi": "5丁目5番20号", "postal_code": "5448585", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "ショウジヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5448686','{"jis": "27116", "kana": "シヨウエイインサツ カブシキガイシヤ", "name": "昌栄印刷　株式会社", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "桃谷", "banchi": "1丁目3番23号", "postal_code": "5448686", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "モモダニ", "alternates": []}');
 INSERT INTO office_data VALUES('5448666','{"jis": "27116", "kana": "ロ-トセイヤク カブシキガイシヤ", "name": "ロート製薬　株式会社", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "巽西", "banchi": "1丁目8-1(生野郵便局私書箱第1号)", "postal_code": "5448666", "old_code": "544  ", "post_office": "生野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "タツミニシ", "alternates": []}');
 INSERT INTO office_data VALUES('5358555','{"jis": "27117", "kana": "アサヒ ゼイムシヨ", "name": "旭　税務署", "prefecture": "大阪府", "city": "大阪市旭区", "neighborhood": "大宮", "banchi": "1丁目1-25", "postal_code": "5358555", "old_code": "535  ", "post_office": "大阪旭", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシアサヒク", "neighborhood_kana": "オオミヤ", "alternates": []}');
@@ -136975,27 +136909,27 @@
 INSERT INTO office_data VALUES('5418572','{"jis": "27128", "kana": "エスエムビ-シ-フアイナンスサ-ビス (カ", "name": "ＳＭＢＣファイナンスサービス　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "4丁目5番15号", "postal_code": "5418572", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418540','{"jis": "27128", "kana": "エヌアイテイジンシヨウジ カブシキガイシヤ", "name": "ＮＩ帝人商事　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南本町", "banchi": "1丁目6-7", "postal_code": "5418540", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418765','{"jis": "27128", "kana": "エレコム カブシキガイシヤ", "name": "エレコム　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "4丁目1番1号明治安田生命大阪御堂筋ビル9階", "postal_code": "5418765", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418541','{"jis": "27128", "kana": "オ-ミケンシ カブシキカイシヤ", "name": "オーミケンシ　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南本町", "banchi": "4-1-1", "postal_code": "5418541", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418567','{"jis": "27128", "kana": "オオサカコクサイガンセンタ-", "name": "大阪国際がんセンター", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "3丁目1番69号", "postal_code": "5418567", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5418531','{"jis": "27128", "kana": "オオサカシシヨクインロウドウクミアイ", "name": "大阪市職員労働組合", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "2丁目4番7号新瓦町ビル7階", "postal_code": "5418531", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418518','{"jis": "27128", "kana": "オオサカシチユウオウクヤクジヨ", "name": "大阪市中央区役所", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "1丁目2-27", "postal_code": "5418518", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5418589','{"jis": "27128", "kana": "オザツクス カブシキガイシヤ", "name": "オザックス　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜", "banchi": "3丁目5番29号-13階", "postal_code": "5418589", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマ", "alternates": []}');
+INSERT INTO office_data VALUES('5418589','{"jis": "27128", "kana": "オザツクス カブシキガイシヤ", "name": "オザックス　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜", "banchi": "3丁目5番29号-13階", "postal_code": "5418589", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマ", "alternates": []}');
 INSERT INTO office_data VALUES('5418526','{"jis": "27128", "kana": "オノヤクヒンコウギヨウ カブシキガイシヤ", "name": "小野薬品工業　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "道修町", "banchi": "2丁目1-5", "postal_code": "5418526", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ドショウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418560','{"jis": "27128", "kana": "カネマツ カブシキガイシヤ オオサカシシヤ", "name": "兼松　株式会社　大阪支社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "淡路町", "banchi": "3-1-9", "postal_code": "5418560", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "アワジマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5418528','{"jis": "27128", "kana": "カブシキカイシヤ ニツケンセツケイ", "name": "株式会社　日建設計", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "3-6-5", "postal_code": "5418528", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
+INSERT INTO office_data VALUES('5418528','{"jis": "27128", "kana": "カブシキカイシヤ ニツケンセツケイ", "name": "株式会社　日建設計", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "3-6-5", "postal_code": "5418528", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5416666','{"jis": "27128", "kana": "カブシキガイシヤ オオニシ", "name": "株式会社　大西", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "3-4-12", "postal_code": "5416666", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418630','{"jis": "27128", "kana": "カブシキガイシヤ オオバヤシグミ", "name": "株式会社　大林組", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜", "banchi": "三丁目5番29号", "postal_code": "5418630", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマ", "alternates": []}');
 INSERT INTO office_data VALUES('5418561','{"jis": "27128", "kana": "カブシキガイシヤ サンケイリビングシンブンシヤ", "name": "株式会社　サンケイリビング新聞社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "2丁目6番6号", "postal_code": "5418561", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418515','{"jis": "27128", "kana": "カブシキガイシヤ ニホンケイザイシンブンシヤ オオサカホンシヤ", "name": "株式会社　日本経済新聞社　大阪本社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "高麗橋", "banchi": "1丁目4番2号", "postal_code": "5418515", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "コウライバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418503','{"jis": "27128", "kana": "カブシキガイシヤ プロル-トマルコウ", "name": "株式会社　プロルート丸光", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "2丁目1-5", "postal_code": "5418503", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5408630','{"jis": "27128", "kana": "カブシキガイシヤ ミズホギンコウ オオサカシテン", "name": "株式会社　みずほ銀行　大阪支店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "4丁目2-1(大阪東郵便局私書箱第145号)", "postal_code": "5408630", "old_code": "541  ", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418535','{"jis": "27128", "kana": "カブシキガイシヤ ミツビシトウキヨウユ-エフジエイギンコウ オオサカチユウオウシテン", "name": "株式会社　三菱東京ＵＦＪ銀行　大阪中央支店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "3丁目5-6", "postal_code": "5418535", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418530','{"jis": "27128", "kana": "カブシキガイシヤ ミツビシユ-エフジエイギンコウ", "name": "株式会社　三菱ＵＦＪ銀行", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "3-5-6", "postal_code": "5418530", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5418575','{"jis": "27128", "kana": "カブシキガイシヤ メイセイシヨウカイ", "name": "株式会社　明成商会", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "2丁目4番10号淀屋橋北浜センタービル2階", "postal_code": "5418575", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
+INSERT INTO office_data VALUES('5418575','{"jis": "27128", "kana": "カブシキガイシヤ メイセイシヨウカイ", "name": "株式会社　明成商会", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "2丁目4番10号淀屋橋北浜センタービル2階", "postal_code": "5418575", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418517','{"jis": "27128", "kana": "カブシキガイシヤ モリモトグミ", "name": "株式会社　森本組", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南本町", "banchi": "2-6-12サンマリオンNBFタワー", "postal_code": "5418517", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418523','{"jis": "27128", "kana": "カンサイペイント カブシキガイシヤ", "name": "関西ペイント　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "2丁目6-14", "postal_code": "5418523", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418513','{"jis": "27128", "kana": "キスコ カブシキガイシヤ オオサカホンシヤ", "name": "ＫＩＳＣＯ　株式会社　大阪本社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "三丁目3番7号", "postal_code": "5418513", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418519','{"jis": "27128", "kana": "キヨクトウカイハツコウギヨウ カブシキカイシヤ", "name": "極東開発工業　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "淡路町", "banchi": "二丁目5番11号", "postal_code": "5418519", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "アワジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418563','{"jis": "27128", "kana": "キヨクヨウ カブシキガイシヤ", "name": "旭洋　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "3-1-15", "postal_code": "5418563", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418506','{"jis": "27128", "kana": "キヨハラ カブシキガイシヤ", "name": "清原　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南久宝寺町", "banchi": "4丁目5-2", "postal_code": "5418506", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミキュウホウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418581','{"jis": "27128", "kana": "クラシキボウセキ カブシキガイシヤ", "name": "倉敷紡績　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "2丁目4-31", "postal_code": "5418581", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
@@ -137256,15 +137190,15 @@
 INSERT INTO office_data VALUES('5678520','{"jis": "27211", "kana": "マルカキカイ カブシキガイシヤ", "name": "マルカキカイ　株式会社", "prefecture": "大阪府", "city": "茨木市", "neighborhood": "五日市緑町", "banchi": "2-28", "postal_code": "5678520", "old_code": "567  ", "post_office": "茨木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イバラキシ", "neighborhood_kana": "イツカイチミドリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5678570','{"jis": "27211", "kana": "リツメイカンダイガク オオサカイバラキキヤンパス", "name": "立命館大学　大阪いばらきキャンパス", "prefecture": "大阪府", "city": "茨木市", "neighborhood": "岩倉町", "banchi": "2-150", "postal_code": "5678570", "old_code": "567  ", "post_office": "茨木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イバラキシ", "neighborhood_kana": "イワクラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818511','{"jis": "27212", "kana": "オオサカケイザイホウカダイガク", "name": "大阪経済法科大学", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "楽音寺", "banchi": "6-10", "postal_code": "5818511", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ガクオンジ", "alternates": []}');
 INSERT INTO office_data VALUES('5818686','{"jis": "27212", "kana": "カブシキカイシヤ クボタ キユウホウジジギヨウセンタ-", "name": "株式会社　クボタ　久宝寺事業センター", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "神武町", "banchi": "2番35号", "postal_code": "5818686", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ジンムチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818558','{"jis": "27212", "kana": "カブシキガイシヤ ミキハウス", "name": "株式会社　ミキハウス", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "若林町", "banchi": "1丁目76-2", "postal_code": "5818558", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ワカバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818539','{"jis": "27212", "kana": "カブシキガイシヤ ヤラカスカン プロダクトセンタ-", "name": "（株）　ヤラカス舘　プロダクトセンター", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "若林町", "banchi": "2丁目119", "postal_code": "5818539", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ワカバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818585','{"jis": "27212", "kana": "シヤ-プ カブシキガイシヤ スマ-トアプライアンスアンドソリユ-シヨンジギヨウホンブ", "name": "シャープ　株式会社　Ｓｍａｒｔ　Ａｐｐｌｉａｎｃｅｓ＆Ｓｏｌｕｔｉｏｎｓ事業本部", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "北亀井町", "banchi": "3丁目1番72号", "postal_code": "5818585", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "キタカメイチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5818502','{"jis": "27212", "kana": "ジエイピ-ラクテンロジステイクス カブシキガイシヤ ラクテンフルフイルメントセンタ-ヤオ", "name": "ＪＰ楽天ロジスティクス　株式会社　楽天フルフィルメントセンター八尾", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "郡川", "banchi": "一丁目557GLP八尾Ⅰ", "postal_code": "5818502", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "コオリガワ", "alternates": []}');
+INSERT INTO office_data VALUES('5818502','{"jis": "27212", "kana": "ジエイピ-ラクテンロジステイクス カブシキガイシヤ ラクテンフルフイルメントセンタ-ヤオ", "name": "ＪＰ楽天ロジスティクス　株式会社　楽天フルフィルメントセンター八尾", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "郡川", "banchi": "一丁目557GLP八尾Ⅰ", "postal_code": "5818502", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "コオリガワ", "alternates": []}');
 INSERT INTO office_data VALUES('5818505','{"jis": "27212", "kana": "ミキシヨウコウ カブシキガイシヤ", "name": "三起商行　株式会社", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "若林町", "banchi": "1丁目76-2", "postal_code": "5818505", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ワカバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5498522','{"jis": "27213", "kana": "キタカウンタ- カンサイクウコウタ-ミナル 4エフコクサイセンシユツパツロビ-・1エフコクサイセントウチヤクロビ-", "name": "北カウンター　関西空港ターミナル　４Ｆ国際線出発ロビー・１Ｆ国際線到着ロビー", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "泉州空港北", "banchi": "1番地", "postal_code": "5498522", "old_code": "549  ", "post_office": "大阪国際", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "センシュウクウコウキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5988503','{"jis": "27213", "kana": "イズミサノ ゼイムシヨ", "name": "泉佐野　税務署", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "日根野", "banchi": "3683-1", "postal_code": "5988503", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "ヒネノ", "alternates": []}');
 INSERT INTO office_data VALUES('5988550','{"jis": "27213", "kana": "イズミサノシヤクシヨ", "name": "泉佐野市役所", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "市場東", "banchi": "1丁目295-3", "postal_code": "5988550", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "イチバヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5988560','{"jis": "27213", "kana": "オオサカフリツ サノコウギヨウコウトウガツコウ", "name": "大阪府立　佐野工業高等学校", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "高松東", "banchi": "1丁目3-50", "postal_code": "5988560", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "タカマツヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5988531','{"jis": "27213", "kana": "オオサカフリツダイガク リンクウキヤンパス", "name": "大阪府立大学　りんくうキャンパス", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "りんくう往来北", "banchi": "1-58", "postal_code": "5988531", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "リンクウオウライキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5988522','{"jis": "27213", "kana": "カンサイエアポ-トワシントンホテル", "name": "関西エアポートワシントンホテル", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "りんくう往来北", "banchi": "1-7", "postal_code": "5988522", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "リンクウオウライキタ", "alternates": []}');
@@ -138297,15 +138231,15 @@
 INSERT INTO office_data VALUES('6892395','{"jis": "31371", "kana": "トウハクチヨウノウギヨウ キヨウドウクミアイ", "name": "東伯町農業　協同組合", "prefecture": "鳥取県", "city": "東伯郡琴浦町", "neighborhood": "大字徳万", "banchi": "558-1", "postal_code": "6892395", "old_code": "68923", "post_office": "東伯", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6892293','{"jis": "31372", "kana": "カブシキガイシヤ サンセキ", "name": "株式会社　サンセキ", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "東園", "banchi": "323-1", "postal_code": "6892293", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ヒガシソノ", "alternates": []}');
 INSERT INTO office_data VALUES('6892298','{"jis": "31372", "kana": "ジエイエイトツトリチユウオウ ダイエイシシヨ", "name": "ＪＡ鳥取中央　大栄支所", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "由良宿", "banchi": "561", "postal_code": "6892298", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ユラシュク", "alternates": []}');
 INSERT INTO office_data VALUES('6892295','{"jis": "31372", "kana": "トツトリケンリツ トツトリチユウオウイクエイコウトウガツコウ", "name": "鳥取県立　鳥取中央育英高等学校", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "由良宿", "banchi": "291-1", "postal_code": "6892295", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ユラシュク", "alternates": []}');
 INSERT INTO office_data VALUES('6892292','{"jis": "31372", "kana": "ホクエイチヨウヤクバ ダイエイチヨウシヤ", "name": "北栄町役場　大栄庁舎", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "由良宿", "banchi": "423-1", "postal_code": "6892292", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ユラシュク", "alternates": []}');
 INSERT INTO office_data VALUES('6894292','{"jis": "31390", "kana": "ホウキチヨウヤクバ ミゾグチブンチヨウシヤ", "name": "伯耆町役場　溝口分庁舎", "prefecture": "鳥取県", "city": "西伯郡伯耆町", "neighborhood": "溝口", "banchi": "647", "postal_code": "6894292", "old_code": "68942", "post_office": "米子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "サイハクグンホウキチョウ", "neighborhood_kana": "ミゾクチ", "alternates": []}');
 INSERT INTO office_data VALUES('6895292','{"jis": "31401", "kana": "ニチナンチヨウヤクバ", "name": "日南町役場", "prefecture": "鳥取県", "city": "日野郡日南町", "neighborhood": "霞", "banchi": "800", "postal_code": "6895292", "old_code": "68952", "post_office": "日南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "ヒノグンニチナンチョウ", "neighborhood_kana": "カスミ", "alternates": []}');
-INSERT INTO office_data VALUES('6908601','{"jis": "32201", "kana": "エヌエイチケイ マツエホウソウキヨク", "name": "ＮＨＫ　松江放送局", "prefecture": "島根県", "city": "松江市", "neighborhood": "灘町", "banchi": "101-6(松江中央郵便局私書箱第7号)", "postal_code": "6908601", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ナダマチ", "alternates": []}');
+INSERT INTO office_data VALUES('6908601','{"jis": "32201", "kana": "エヌエイチケイ マツエホウソウキヨク", "name": "ＮＨＫ　松江放送局", "prefecture": "島根県", "city": "松江市", "neighborhood": "灘町", "banchi": "101-6(松江中央郵便局私書箱第7号)", "postal_code": "6908601", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ナダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908550','{"jis": "32201", "kana": "カナツギケンコウギヨウ カブシキガイシヤ", "name": "カナツ技建工業　株式会社", "prefecture": "島根県", "city": "松江市", "neighborhood": "春日町", "banchi": "636", "postal_code": "6908550", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "カスガチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908555','{"jis": "32201", "kana": "カブシキガイシヤ イチバタヒヤツカテン", "name": "株式会社　一畑百貨店", "prefecture": "島根県", "city": "松江市", "neighborhood": "朝日町", "banchi": "661", "postal_code": "6908555", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908508','{"jis": "32201", "kana": "カブシキガイシヤ エフエムサンイン", "name": "株式会社　エフエム山陰", "prefecture": "島根県", "city": "松江市", "neighborhood": "学園南", "banchi": "1丁目2番1号くにびきメッセ西棟2階", "postal_code": "6908508", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ガクエンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('6908539','{"jis": "32201", "kana": "カブシキガイシヤ サンインゴウドウギンコウ クレジツトカ-ドセンタ-", "name": "株式会社　山陰合同銀行　クレジットカードセンター", "prefecture": "島根県", "city": "松江市", "neighborhood": "", "banchi": "白潟本町23(松江中央郵便局私書箱第62号)", "postal_code": "6908539", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6908580','{"jis": "32201", "kana": "カブシキガイシヤ サンインゴウドウギンコウ ジムセンタ-", "name": "株式会社　山陰合同銀行　事務センター", "prefecture": "島根県", "city": "松江市", "neighborhood": "袖師町", "banchi": "6-10(松江中央郵便局私書箱第20号)", "postal_code": "6908580", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ソデシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908530','{"jis": "32201", "kana": "カブシキガイシヤ マイカルマツエサテイ", "name": "株式会社　マイカル松江サティ", "prefecture": "島根県", "city": "松江市", "neighborhood": "東朝日町", "banchi": "151", "postal_code": "6908530", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシアサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908558','{"jis": "32201", "kana": "カブシキガイシヤ ユニコン", "name": "株式会社　ユニコン", "prefecture": "島根県", "city": "松江市", "neighborhood": "東朝日町", "banchi": "29", "postal_code": "6908558", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシアサヒマチ", "alternates": []}');
@@ -138317,17 +138251,17 @@
 INSERT INTO office_data VALUES('6908519','{"jis": "32201", "kana": "ケンリツマツエミナミコウトウガツコウ", "name": "県立松江南高等学校", "prefecture": "島根県", "city": "松江市", "neighborhood": "八雲台", "banchi": "1丁目1-1", "postal_code": "6908519", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヤクモダイ", "alternates": []}');
 INSERT INTO office_data VALUES('6908556','{"jis": "32201", "kana": "コクリツリヨウヨウシヨ マツエビヨウイン", "name": "国立療養所　松江病院", "prefecture": "島根県", "city": "松江市", "neighborhood": "上乃木", "banchi": "5丁目8-31", "postal_code": "6908556", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "アゲノギ", "alternates": []}');
 INSERT INTO office_data VALUES('6908677','{"jis": "32201", "kana": "ゴウギンリ-ス カブシキガイシヤ", "name": "ごうぎんリース　株式会社", "prefecture": "島根県", "city": "松江市", "neighborhood": "白潟本町", "banchi": "63番地", "postal_code": "6908677", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6908666','{"jis": "32201", "kana": "サンインチユウオウテレビジヨンホウソウ カブシキガイシヤ", "name": "山陰中央テレビジョン放送　株式会社", "prefecture": "島根県", "city": "松江市", "neighborhood": "向島町", "banchi": "140-1(松江中央郵便局私書箱第17号)", "postal_code": "6908666", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ムコウジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908502','{"jis": "32201", "kana": "シマネケン キヨウイクイインカイ", "name": "島根県　教育委員会", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "1", "postal_code": "6908502", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908510','{"jis": "32201", "kana": "シマネケン ケイサツホンブ", "name": "島根県　警察本部", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "8-1", "postal_code": "6908510", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908533','{"jis": "32201", "kana": "シマネケン シヤカイホケンシンリヨウホウシユウシハライキキン", "name": "島根県　社会保険診療報酬支払基金", "prefecture": "島根県", "city": "松江市", "neighborhood": "北田町", "banchi": "33-1", "postal_code": "6908533", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "キタタマチ", "alternates": []}');
-INSERT INTO office_data VALUES('6908503','{"jis": "32201", "kana": "シマネケン シンヨウホシヨウキヨウカイ", "name": "島根県　信用保証協会", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "105", "postal_code": "6908503", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908551','{"jis": "32201", "kana": "シマネケン トウブケンミンセンタ-", "name": "島根県　東部県民センター", "prefecture": "島根県", "city": "松江市", "neighborhood": "東津田町", "banchi": "1741-1", "postal_code": "6908551", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシツダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908535','{"jis": "32201", "kana": "シマネケンイシカイ", "name": "島根県医師会", "prefecture": "島根県", "city": "松江市", "neighborhood": "袖師町", "banchi": "1-31", "postal_code": "6908535", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ソデシチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('6908503','{"jis": "32201", "kana": "シマネケンシンヨウホシヨウキヨウカイ", "name": "島根県信用保証協会", "prefecture": "島根県", "city": "松江市", "neighborhood": "灘町", "banchi": "1番地7", "postal_code": "6908503", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ナダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908501','{"jis": "32201", "kana": "シマネケンチヨウ", "name": "島根県庁", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "1", "postal_code": "6908501", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908504','{"jis": "32201", "kana": "シマネダイガク", "name": "島根大学", "prefecture": "島根県", "city": "松江市", "neighborhood": "西川津町", "banchi": "1060", "postal_code": "6908504", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ニシカワツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908794','{"jis": "32201", "kana": "シマネチイキセンタ-", "name": "島根地域センター", "prefecture": "島根県", "city": "松江市", "neighborhood": "御手船場町", "banchi": "549-1損保ジャパン松江ビル3F", "postal_code": "6908794", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "オテセンバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908531','{"jis": "32201", "kana": "ゼンコクケンコウホケンキヨウカイ シマネシブ", "name": "全国健康保険協会　島根支部", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "383山陰中央ビル2階", "postal_code": "6908531", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908560','{"jis": "32201", "kana": "ゼンロウサイシマネケンホンブ", "name": "全労済島根県本部", "prefecture": "島根県", "city": "松江市", "neighborhood": "伊勢宮町", "banchi": "543-3", "postal_code": "6908560", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "イセミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908532','{"jis": "32201", "kana": "チユウゴクデンリヨク カブシキガイシヤ サンインデンリヨクシヨ", "name": "中国電力　株式会社　山陰電力所", "prefecture": "島根県", "city": "松江市", "neighborhood": "母衣町", "banchi": "115番地", "postal_code": "6908532", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ホロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908514','{"jis": "32201", "kana": "チユウゴクデンリヨク カブシキガイシヤ シマネシシヤ", "name": "中国電力　株式会社　島根支社", "prefecture": "島根県", "city": "松江市", "neighborhood": "母衣町", "banchi": "115", "postal_code": "6908514", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ホロマチ", "alternates": []}');
@@ -138399,15 +138333,15 @@
 INSERT INTO office_data VALUES('6990588','{"jis": "32203", "kana": "イツパンシヤダンホウジン ニホンアマチユアムセンレンメイ ジエイエ-ア-ルエル キユ-エスエルビユ-ロ-", "name": "一般社団法人　日本アマチュア無線連盟　ＪＡＲＬ　ＱＳＬビューロー", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町神庭", "banchi": "1324-3", "postal_code": "6990588", "old_code": "69905", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウカンバ", "alternates": []}');
 INSERT INTO office_data VALUES('6990593','{"jis": "32203", "kana": "シマネケンノウギヨウキヨウドウクミアイ ヒカワチクホンブ", "name": "島根県農業協同組合　斐川地区本部", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町荘原", "banchi": "2172番地3", "postal_code": "6990593", "old_code": "69905", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウショウバラ", "alternates": []}');
 INSERT INTO office_data VALUES('6990696','{"jis": "32203", "kana": "カブシキガイシヤ イズモムラタセイサクシヨ", "name": "株式会社　出雲村田製作所", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町上直江", "banchi": "2308", "postal_code": "6990696", "old_code": "69906", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウカミナオエ", "alternates": []}');
 INSERT INTO office_data VALUES('6990697','{"jis": "32203", "kana": "ジエイエイゼンノウ シマネケンホンブ", "name": "ＪＡ全農　島根県本部", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町直江", "banchi": "5030", "postal_code": "6990697", "old_code": "69906", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウナオエ", "alternates": []}');
 INSERT INTO office_data VALUES('6990792','{"jis": "32203", "kana": "イズモシヤクシヨ タイシヤシシヨ", "name": "出雲市役所　大社支所", "prefecture": "島根県", "city": "出雲市", "neighborhood": "大社町杵築南", "banchi": "1395", "postal_code": "6990792", "old_code": "69907", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "タイシャチョウキヅキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('6988504','{"jis": "32204", "kana": "カブシキカイシヤ イズミユメタウンマスダ", "name": "株式会社　イズミゆめタウン益田", "prefecture": "島根県", "city": "益田市", "neighborhood": "高津", "banchi": "7丁目21-12", "postal_code": "6988504", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "タカツ", "alternates": []}');
 INSERT INTO office_data VALUES('6988503','{"jis": "32204", "kana": "カブシキカイシヤ キヌヤ", "name": "株式会社　キヌヤ", "prefecture": "島根県", "city": "益田市", "neighborhood": "常盤町", "banchi": "4番38号", "postal_code": "6988503", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "トキワチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('6988506','{"jis": "32204", "kana": "ソニ-ネツトワ-クコミユニケ-シヨンズ カブシキガイシヤ", "name": "ソニーネットワークコミュニケーションズ　株式会社", "prefecture": "島根県", "city": "益田市", "neighborhood": "駅前町", "banchi": "17-1益田駅前ビルEAGA3F", "postal_code": "6988506", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "エキマエチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('6988506','{"jis": "32204", "kana": "ソニ-ネツトワ-クコミユニケ-シヨンズ カブシキガイシヤ", "name": "ソニーネットワークコミュニケーションズ　株式会社", "prefecture": "島根県", "city": "益田市", "neighborhood": "駅前町", "banchi": "17-1益田駅前ビルEAGA3F", "postal_code": "6988506", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "エキマエチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988651','{"jis": "32204", "kana": "マスダ ゼイムシヨ", "name": "益田　税務署", "prefecture": "島根県", "city": "益田市", "neighborhood": "元町", "banchi": "12-11(益田郵便局私書箱第5号)", "postal_code": "6988651", "old_code": "698  ", "post_office": "益田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "モトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6988505','{"jis": "32204", "kana": "マスダサテイ", "name": "益田サティ", "prefecture": "島根県", "city": "益田市", "neighborhood": "乙吉町", "banchi": "イ95-10", "postal_code": "6988505", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "オトヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988650','{"jis": "32204", "kana": "マスダシヤクシヨ", "name": "益田市役所", "prefecture": "島根県", "city": "益田市", "neighborhood": "常盤町", "banchi": "1-1(益田郵便局私書箱第4号)", "postal_code": "6988650", "old_code": "698  ", "post_office": "益田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "トキワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988501','{"jis": "32204", "kana": "マスダセキジユウジビヨウイン", "name": "益田赤十字病院", "prefecture": "島根県", "city": "益田市", "neighborhood": "乙吉町", "banchi": "イ103-1", "postal_code": "6988501", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "オトヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6980292','{"jis": "32204", "kana": "マスダシヤクシヨミトソウゴウシシヨ", "name": "益田市役所美都総合支所", "prefecture": "島根県", "city": "益田市", "neighborhood": "美都町都茂", "banchi": "1803-1", "postal_code": "6980292", "old_code": "69802", "post_office": "美都", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "ミトチョウツモ", "alternates": []}');
 INSERT INTO office_data VALUES('6948501','{"jis": "32205", "kana": "イワミオオダゼイムシヨ", "name": "石見大田税務署", "prefecture": "島根県", "city": "大田市", "neighborhood": "大田町大田", "banchi": "イ289-2", "postal_code": "6948501", "old_code": "694  ", "post_office": "石見大田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "オオダチョウオオダ", "alternates": []}');
 INSERT INTO office_data VALUES('6948502','{"jis": "32205", "kana": "オオダシヤクシヨ", "name": "大田市役所", "prefecture": "島根県", "city": "大田市", "neighborhood": "大田町大田", "banchi": "ロ1111番地", "postal_code": "6948502", "old_code": "694  ", "post_office": "石見大田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "オオダチョウオオダ", "alternates": []}');
@@ -138700,15 +138634,15 @@
 INSERT INTO office_data VALUES('7128525','{"jis": "33202", "kana": "ミツビシガスカガク カブシキガイシヤ ミズシマコウジヨウ", "name": "三菱ガス化学　株式会社　水島工場", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "水島海岸通", "banchi": "3丁目10", "postal_code": "7128525", "old_code": "712  ", "post_office": "水島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "ミズシマカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7128501','{"jis": "33202", "kana": "ミツビシジドウシヤコウギヨウ カブシキガイシヤ セイサン・ブツリユウホンブ ミズシマセイサクシヨ", "name": "三菱自動車工業　株式会社　生産・物流本部　水島製作所", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "水島海岸通", "banchi": "1丁目1番地", "postal_code": "7128501", "old_code": "712  ", "post_office": "水島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "ミズシマカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7138713','{"jis": "33202", "kana": "アカザワヤ カブシキガイシヤ", "name": "赤澤屋　株式会社", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "1丁目4-11(玉島郵便局私書箱第5号)", "postal_code": "7138713", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138668','{"jis": "33202", "kana": "オカヤマケンリツ タマシマコウトウガツコウ", "name": "岡山県立　玉島高等学校", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "3丁目1-1(玉島郵便局私書箱第4号)", "postal_code": "7138668", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138550','{"jis": "33202", "kana": "カブシキガイシヤ クラレ クラシキジギヨウシヨ (タマシマ)", "name": "株式会社　クラレ　倉敷事業所　（玉島）", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島乙島", "banchi": "7471", "postal_code": "7138550", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマオトシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138666','{"jis": "33202", "kana": "カブシキガイシヤ タイソウ", "name": "株式会社　鯛惣", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島勇崎", "banchi": "1292(玉島郵便局私書箱第6号)", "postal_code": "7138666", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマユウザキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138565','{"jis": "33202", "kana": "クラシキシ タマシマシシヨ", "name": "倉敷市　玉島支所", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "1丁目1-1", "postal_code": "7138565", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
-INSERT INTO office_data VALUES('7138588','{"jis": "33202", "kana": "サクヨウガクエンコウトウガツコウ", "name": "作陽学園高等学校", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島八島", "banchi": "1541番1", "postal_code": "7138588", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマヤシマ", "alternates": []}');
+INSERT INTO office_data VALUES('7138588','{"jis": "33202", "kana": "サクヨウガクエンコウトウガツコウ", "name": "作陽学園高等学校", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島八島", "banchi": "1541番1", "postal_code": "7138588", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマヤシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138501','{"jis": "33202", "kana": "スミトモジユウキカイコウギヨウ カブシキカイシヤ オカヤマセイゾウシヨ", "name": "住友重機械工業　株式会社　岡山製造所", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島乙島", "banchi": "8230", "postal_code": "7138501", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマオトシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138577','{"jis": "33202", "kana": "タチバナヨウキ カブシキガイシヤ", "name": "立花容器　株式会社", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島柏島", "banchi": "7047", "postal_code": "7138577", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマカシワジマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138601','{"jis": "33202", "kana": "タマシマ ゼイムシヨ", "name": "玉島　税務署", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "2丁目1-50(玉島郵便局私書箱第14号)", "postal_code": "7138601", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138686','{"jis": "33202", "kana": "タマシマシンヨウキンコ", "name": "玉島信用金庫", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島", "banchi": "1438(玉島郵便局私書箱第7号)", "postal_code": "7138686", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7088520','{"jis": "33203", "kana": "アルネ・ツヤマ", "name": "アルネ・津山", "prefecture": "岡山県", "city": "津山市", "neighborhood": "新魚町", "banchi": "17", "postal_code": "7088520", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "シンウオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7088515','{"jis": "33203", "kana": "イズミツヤマテン", "name": "イズミ津山店", "prefecture": "岡山県", "city": "津山市", "neighborhood": "伏見町", "banchi": "50", "postal_code": "7088515", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "フシミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7088506','{"jis": "33203", "kana": "オカヤマケン ミマサカケンミンキヨク", "name": "岡山県美作県民局", "prefecture": "岡山県", "city": "津山市", "neighborhood": "山下", "banchi": "53", "postal_code": "7088506", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "サンゲ", "alternates": []}');
@@ -138783,15 +138717,15 @@
 INSERT INTO office_data VALUES('7058501','{"jis": "33211", "kana": "シリツビゼンビヨウイン", "name": "市立備前病院", "prefecture": "岡山県", "city": "備前市", "neighborhood": "伊部", "banchi": "2245", "postal_code": "7058501", "old_code": "705  ", "post_office": "備前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ビゼンシ", "neighborhood_kana": "インベ", "alternates": []}');
 INSERT INTO office_data VALUES('7058585','{"jis": "33211", "kana": "パナソニツク カブシキガイシヤ オ-トモ-テイブアンドインダストリアルシステムズシヤ セミコンダクタ-ジギヨウブ オカヤマコウジヨウ", "name": "パナソニック　株式会社　オートモーティブ＆インダストリアルシステムズ社　セミコンダクター事業部　岡山工場", "prefecture": "岡山県", "city": "備前市", "neighborhood": "友延", "banchi": "700番地", "postal_code": "7058585", "old_code": "705  ", "post_office": "備前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ビゼンシ", "neighborhood_kana": "トモノブ", "alternates": []}');
 INSERT INTO office_data VALUES('7058588','{"jis": "33211", "kana": "ヒナセウンユ カブシキガイシヤ", "name": "日生運輸　株式会社", "prefecture": "岡山県", "city": "備前市", "neighborhood": "穂浪", "banchi": "3651-6", "postal_code": "7058588", "old_code": "705  ", "post_office": "備前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ビゼンシ", "neighborhood_kana": "ホナミ", "alternates": []}');
 INSERT INTO office_data VALUES('7058602','{"jis": "33211", "kana": "ビゼンシヤクシヨ", "name": "備前市役所", "prefecture": "岡山県", "city": "備前市", "neighborhood": "東片上", "banchi": "126(備前郵便局私書箱第2号)", "postal_code": "7058602", "old_code": "705  ", "post_office": "備前", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ビゼンシ", "neighborhood_kana": "ヒガシカタカミ", "alternates": []}');
 INSERT INTO office_data VALUES('7058558','{"jis": "33211", "kana": "ビゼンシヨウコウカイギシヨ", "name": "備前商工会議所", "prefecture": "岡山県", "city": "備前市", "neighborhood": "東片上", "banchi": "230", "postal_code": "7058558", "old_code": "705  ", "post_office": "備前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ビゼンシ", "neighborhood_kana": "ヒガシカタカミ", "alternates": []}');
 INSERT INTO office_data VALUES('7058603','{"jis": "33211", "kana": "ビゼンシンヨウキンコ", "name": "備前信用金庫", "prefecture": "岡山県", "city": "備前市", "neighborhood": "伊部", "banchi": "1660-7(備前郵便局私書箱第3号)", "postal_code": "7058603", "old_code": "705  ", "post_office": "備前", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ビゼンシ", "neighborhood_kana": "インベ", "alternates": []}');
 INSERT INTO office_data VALUES('7014292','{"jis": "33212", "kana": "セトウチシヤクシヨ", "name": "瀬戸内市役所", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "邑久町尾張", "banchi": "300番地1", "postal_code": "7014292", "old_code": "70142", "post_office": "邑久", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "オクチョウオワリ", "alternates": []}');
-INSERT INTO office_data VALUES('7014293','{"jis": "33212", "kana": "セトウチシヤクシヨ オサフネシシヨ", "name": "瀬戸内市役所　長船支所", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "長船町土師", "banchi": "291", "postal_code": "7014293", "old_code": "70142", "post_office": "邑久", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "オサフネチョウハジ", "alternates": []}');
+INSERT INTO office_data VALUES('7014293','{"jis": "33212", "kana": "セトウチシヤクシヨ オサフネシシヨ", "name": "瀬戸内市役所　長船支所", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "長船町土師", "banchi": "288番地1", "postal_code": "7014293", "old_code": "70142", "post_office": "邑久", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "オサフネチョウハジ", "alternates": []}');
 INSERT INTO office_data VALUES('7014398','{"jis": "33212", "kana": "カブシキガイシヤ モトハマグミ", "name": "株式会社　元浜組", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "牛窓町牛窓", "banchi": "6410(牛窓郵便局私書箱第8号)", "postal_code": "7014398", "old_code": "70143", "post_office": "牛窓", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "ウシマドチョウウシマド", "alternates": []}');
 INSERT INTO office_data VALUES('7014392','{"jis": "33212", "kana": "セトウチシヤクシヨ ウシマドシシヨ", "name": "瀬戸内市役所　牛窓支所", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "牛窓町牛窓", "banchi": "4911", "postal_code": "7014392", "old_code": "70143", "post_office": "牛窓", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "ウシマドチョウウシマド", "alternates": []}');
 INSERT INTO office_data VALUES('7014394','{"jis": "33212", "kana": "ニツポンオリ-ブ カブシキガイシヤ", "name": "日本オリーブ　株式会社", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "牛窓町牛窓", "banchi": "3911-10(牛窓郵便局私書箱第4号)", "postal_code": "7014394", "old_code": "70143", "post_office": "牛窓", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "ウシマドチョウウシマド", "alternates": []}');
 INSERT INTO office_data VALUES('7014593','{"jis": "33212", "kana": "コクリツリヨウヨウシヨ オクコウミヨウエン", "name": "国立療養所　邑久光明園", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "邑久町虫明", "banchi": "6253", "postal_code": "7014593", "old_code": "70145", "post_office": "虫明", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "オクチョウムシアゲ", "alternates": []}');
 INSERT INTO office_data VALUES('7014592','{"jis": "33212", "kana": "コクリツリヨウヨウシヨ ナガシマアイセイエン", "name": "国立療養所　長島愛生園", "prefecture": "岡山県", "city": "瀬戸内市", "neighborhood": "邑久町虫明", "banchi": "6539", "postal_code": "7014592", "old_code": "70145", "post_office": "虫明", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "セトウチシ", "neighborhood_kana": "オクチョウムシアゲ", "alternates": []}');
 INSERT INTO office_data VALUES('7012292','{"jis": "33213", "kana": "アカイワシ アカサカシシヨ", "name": "赤磐市　赤坂支所", "prefecture": "岡山県", "city": "赤磐市", "neighborhood": "町苅田", "banchi": "516", "postal_code": "7012292", "old_code": "70122", "post_office": "備前瀬戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "アカイワシ", "neighborhood_kana": "マチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('7012595','{"jis": "33213", "kana": "アカイワシ ヨシイシシヨ", "name": "赤磐市　吉井支所", "prefecture": "岡山県", "city": "赤磐市", "neighborhood": "周匝", "banchi": "136", "postal_code": "7012595", "old_code": "70125", "post_office": "周匝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "アカイワシ", "neighborhood_kana": "スサイ", "alternates": []}');
@@ -140866,15 +140800,15 @@
 INSERT INTO office_data VALUES('8108557','{"jis": "40133", "kana": "カブシキガイシヤ リクル-ト キユウシユウシシヤ", "name": "株式会社　リクルート　九州支社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "舞鶴", "banchi": "1丁目1-3", "postal_code": "8108557", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "マイヅル", "alternates": []}');
 INSERT INTO office_data VALUES('8108512','{"jis": "40133", "kana": "カブシキガイシヤカミグミフクオカシテン", "name": "株式会社　上組福岡支店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "那の津", "banchi": "3丁目2-10", "postal_code": "8108512", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナノツ", "alternates": []}');
 INSERT INTO office_data VALUES('8108565','{"jis": "40133", "kana": "カブシキガイシヤキユウシユウコクサイエフエム(LOVE FM76.1)", "name": "株式会社九州国際エフエム（ＬＯＶＥ　ＦＭ７６．１）", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "2丁目5-35NTT-Tビル7階", "postal_code": "8108565", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108631','{"jis": "40133", "kana": "カブシキガイシヤトウシヨク フクオカシテン", "name": "株式会社東食　福岡支店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目14-16三栄ビル5階", "postal_code": "8108631", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108619','{"jis": "40133", "kana": "ガツコウホウジン カワイジユク フクオカコウ", "name": "学校法人　河合塾　福岡校", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "渡辺通", "banchi": "4丁目2-11", "postal_code": "8108619", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ワタナベドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8108588','{"jis": "40133", "kana": "キユ-サイ カブシキカイシヤ", "name": "キューサイ　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "薬院", "banchi": "1-1-1", "postal_code": "8108588", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ヤクイン", "alternates": []}');
 INSERT INTO office_data VALUES('8108606','{"jis": "40133", "kana": "キユ-サイ カブシキガイシヤ", "name": "キューサイ　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "草香江", "banchi": "1丁目7-16", "postal_code": "8108606", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "クサガエ", "alternates": []}');
-INSERT INTO office_data VALUES('8108571','{"jis": "40133", "kana": "キユウシユウアサヒホウソウ カブシキガイシヤ", "name": "九州朝日放送　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": [{"jis": "40133", "kana": "ケ-ビ-シ-グル-プホ-ルデイングス カブシキガイシヤ", "name": "ＫＢＣグループホールディングス　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": []}]}');
+INSERT INTO office_data VALUES('8108571','{"jis": "40133", "kana": "キユウシユウアサヒホウソウ カブシキガイシヤ", "name": "九州朝日放送　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": [{"jis": "40133", "kana": "ケ-ビ-シ-グル-プホ-ルデイングス カブシキガイシヤ", "name": "ＫＢＣグループホールディングス　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": []}]}');
 INSERT INTO office_data VALUES('8108560','{"jis": "40133", "kana": "キユウシユウダイガク ロツポンマツチクブキヨク(ダイガクキヨウイクケンキユウセンタ-.ダイガクインヒカクシヤカイブンカケンキユウカ.ゲンゴブンカブ)", "name": "九州大学　六本松地区部局（大学教育研究センター、大学院比較社会文化研究科、言語文化部）", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "六本松", "banchi": "4丁目2-1", "postal_code": "8108560", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ロッポンマツ", "alternates": []}');
 INSERT INTO office_data VALUES('8108617','{"jis": "40133", "kana": "キユウシユウツウシンネツトワ-ク カブシキガイシヤ", "name": "九州通信ネットワーク　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目12-20-8F", "postal_code": "8108617", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108705','{"jis": "40133", "kana": "キユウシユウデンリヨクソウハイデン カブシキガイシヤ ホンテン", "name": "九州電力送配電　株式会社　本店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "渡辺通", "banchi": "二丁目1番82号(福岡中央郵便局私書箱第94号)", "postal_code": "8108705", "old_code": "810  ", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ワタナベドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8108636','{"jis": "40133", "kana": "キユウシユウミツビシジドウシヤハンバイ カブシキガイシヤ", "name": "九州三菱自動車販売　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "薬院", "banchi": "3丁目2-23", "postal_code": "8108636", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ヤクイン", "alternates": []}');
 INSERT INTO office_data VALUES('8108509','{"jis": "40133", "kana": "キユウシユウロウドウキンコ", "name": "九州労働金庫", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "大手門", "banchi": "3丁目3-3", "postal_code": "8108509", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "オオテモン", "alternates": []}');
 INSERT INTO office_data VALUES('8108532','{"jis": "40133", "kana": "キリンビ-ル カブシキガイシヤ キユウシユウシシヤ", "name": "キリンビール　株式会社　九州支社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "2丁目14-8FTCビル15F", "postal_code": "8108532", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108601','{"jis": "40133", "kana": "ゲツカンウルトラマンボウ カブシキガイシヤ ア-トライン", "name": "月刊うるとらマンボウ　株式会社　アートライン", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "4丁目9-15文化ビル1F", "postal_code": "8108601", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
@@ -141216,15 +141150,15 @@
 INSERT INTO office_data VALUES('8191392','{"jis": "40230", "kana": "イトシマシヤクシヨ シマチヨウシヤ", "name": "糸島市役所　志摩庁舎", "prefecture": "福岡県", "city": "糸島市", "neighborhood": "志摩初", "banchi": "30", "postal_code": "8191392", "old_code": "81913", "post_office": "前原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "イトシマシ", "neighborhood_kana": "シマハツ", "alternates": []}');
 INSERT INTO office_data VALUES('8191692','{"jis": "40230", "kana": "イトシマシヤクシヨ ニジヨウチヨウシヤ", "name": "糸島市役所　二丈庁舎", "prefecture": "福岡県", "city": "糸島市", "neighborhood": "二丈深江", "banchi": "1360", "postal_code": "8191692", "old_code": "81916", "post_office": "前原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "イトシマシ", "neighborhood_kana": "ニジョウフカエ", "alternates": []}');
 INSERT INTO office_data VALUES('8111292','{"jis": "40231", "kana": "ナカガワシヤクシヨ", "name": "那珂川市役所", "prefecture": "福岡県", "city": "那珂川市", "neighborhood": "西隈", "banchi": "1丁目1番1号", "postal_code": "8111292", "old_code": "81112", "post_office": "筑紫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ナカガワシ", "neighborhood_kana": "ニシグマ", "alternates": []}');
 INSERT INTO office_data VALUES('8112192','{"jis": "40341", "kana": "ウミマチヤクバ", "name": "宇美町役場", "prefecture": "福岡県", "city": "糟屋郡宇美町", "neighborhood": "宇美", "banchi": "5丁目1-1", "postal_code": "8112192", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンウミマチ", "neighborhood_kana": "ウミ", "alternates": []}');
 INSERT INTO office_data VALUES('8112195','{"jis": "40341", "kana": "サンドラツグ フクオカブツリユウセンタ-", "name": "サンドラッグ　福岡物流センター", "prefecture": "福岡県", "city": "糟屋郡宇美町", "neighborhood": "大字井野", "banchi": "字稲木369-8-10", "postal_code": "8112195", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112194','{"jis": "40341", "kana": "ダイレツクスフクオカマザ-センタ-", "name": "ダイレックス福岡マザーセンター", "prefecture": "福岡県", "city": "糟屋郡宇美町", "neighborhood": "大字井野", "banchi": "字稲木369-8-10", "postal_code": "8112194", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112495','{"jis": "40342", "kana": "エフコ-プ セイカツキヨウドウクミアイ", "name": "エフコープ　生活協同組合", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "大字篠栗", "banchi": "4826-1", "postal_code": "8112495", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('8112498','{"jis": "40342", "kana": "カブシキガイシヤ ヤマヤコミユニケ-シヨンズ", "name": "株式会社　やまやコミュニケーションズ", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "彩り台", "banchi": "1番1号", "postal_code": "8112498", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンササグリマチ", "neighborhood_kana": "イロドリダイ", "alternates": []}');
+INSERT INTO office_data VALUES('8112498','{"jis": "40342", "kana": "カブシキガイシヤ ヤマヤコミユニケ-シヨンズ", "name": "株式会社　やまやコミュニケーションズ", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "彩り台", "banchi": "1番1号", "postal_code": "8112498", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンササグリマチ", "neighborhood_kana": "イロドリダイ", "alternates": []}');
 INSERT INTO office_data VALUES('8112492','{"jis": "40342", "kana": "ササグリマチヤクバ", "name": "篠栗町役場", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "大字篠栗", "banchi": "4855-5", "postal_code": "8112492", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112496','{"jis": "40342", "kana": "セイカツキヨウドウクミアイレンゴウカイ コ-プキユウシユウジギヨウレンゴウ", "name": "生活協同組合連合会　コープ九州事業連合", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "大字篠栗", "banchi": "4826-1", "postal_code": "8112496", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112294','{"jis": "40343", "kana": "カブシキガイシヤ サカグチ", "name": "株式会社　サカグチ", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免", "banchi": "4丁目1-24", "postal_code": "8112294", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメ", "alternates": []}');
 INSERT INTO office_data VALUES('8112293','{"jis": "40343", "kana": "カブシキガイシヤ セイユウ シメテン", "name": "株式会社　西友　志免店", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免中央", "banchi": "3丁目4-1", "postal_code": "8112293", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('8112295','{"jis": "40343", "kana": "ギケンコウギヨウ カブシキガイシヤ", "name": "技研工業　株式会社", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免", "banchi": "3丁目14-1", "postal_code": "8112295", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメ", "alternates": []}');
 INSERT INTO office_data VALUES('8112292','{"jis": "40343", "kana": "シメマチヤクバ", "name": "志免町役場", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免中央", "banchi": "1丁目1-1", "postal_code": "8112292", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('8112196','{"jis": "40344", "kana": "サガワグロ-バルロジステイクス カブシキガイシヤ キユウシユウシテン スエエイギヨウシヨ", "name": "佐川グローバルロジスティクス　株式会社　九州支店　須恵営業所", "prefecture": "福岡県", "city": "糟屋郡須惠町", "neighborhood": "大字新原", "banchi": "16-10", "postal_code": "8112196", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -141619,15 +141553,15 @@
 INSERT INTO office_data VALUES('8570392','{"jis": "42391", "kana": "サザチヨウヤクバ", "name": "佐々町役場", "prefecture": "長崎県", "city": "北松浦郡佐々町", "neighborhood": "本田原免", "banchi": "168-2", "postal_code": "8570392", "old_code": "85703", "post_office": "佐々", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "キタマツウラグンサザチョウ", "neighborhood_kana": "ホンタバルメン", "alternates": []}');
 INSERT INTO office_data VALUES('8532392','{"jis": "42411", "kana": "シンカミゴトウチヨウヤクバ ワカマツシシヨ", "name": "新上五島町役場　若松支所", "prefecture": "長崎県", "city": "南松浦郡新上五島町", "neighborhood": "若松郷", "banchi": "277-7", "postal_code": "8532392", "old_code": "85323", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ミナミマツウラグンシンカミゴトウチョウ", "neighborhood_kana": "ワカマツゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('8574495','{"jis": "42411", "kana": "シンカミゴトウチヨウヤクバ", "name": "新上五島町役場", "prefecture": "長崎県", "city": "南松浦郡新上五島町", "neighborhood": "青方郷", "banchi": "1585-1", "postal_code": "8574495", "old_code": "85744", "post_office": "青方", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ミナミマツウラグンシンカミゴトウチョウ", "neighborhood_kana": "アオカタゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('8574592','{"jis": "42411", "kana": "シンカミゴトウチヨウヤクバ シンウオノメシシヨ", "name": "新上五島町役場　新魚目支所", "prefecture": "長崎県", "city": "南松浦郡新上五島町", "neighborhood": "榎津郷", "banchi": "491", "postal_code": "8574592", "old_code": "85745", "post_office": "青方", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ミナミマツウラグンシンカミゴトウチョウ", "neighborhood_kana": "エノキヅゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608543','{"jis": "43101", "kana": "エヌ・テイ・テイフアイナンス カブシキガイシヤ ミナミキユウシユウシテン", "name": "ＮＴＴファイナンス　株式会社　南九州支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "4-1太陽生命熊本第2ビル7F", "postal_code": "8608543", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608519','{"jis": "43101", "kana": "エヌテイテイニシニホン クマモトシテン", "name": "ＮＴＴ西日本　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "桜町", "banchi": "3-1", "postal_code": "8608519", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "サクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608536','{"jis": "43101", "kana": "カブシキカイシヤ クマニチカイカン", "name": "株式会社　熊日会館", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "上通町", "banchi": "2番33号", "postal_code": "8608536", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カミトオリチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('8608506','{"jis": "43101", "kana": "カブシキカイシヤ クマモトニチニチシンブンシヤ", "name": "株式会社　熊本日日新聞社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安", "banchi": "1丁目5番1号", "postal_code": "8608506", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤス", "alternates": []}');
+INSERT INTO office_data VALUES('8608506','{"jis": "43101", "kana": "カブシキカイシヤ クマモトニチニチシンブンシヤ", "name": "株式会社　熊本日日新聞社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安", "banchi": "1丁目5番1号", "postal_code": "8608506", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤス", "alternates": []}');
 INSERT INTO office_data VALUES('8608539','{"jis": "43101", "kana": "カブシキカイシヤ トリニテイ", "name": "株式会社　トリニティ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "妙体寺町", "banchi": "5番4号", "postal_code": "8608539", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ミョウタイジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608797','{"jis": "43101", "kana": "カブシキカイシヤ ユウチヨギンコウ クマモトシテン", "name": "株式会社　ゆうちょ銀行　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1番1号", "postal_code": "8608797", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": [{"jis": "43101", "kana": "カブシキガイシヤ カンポセイメイ クマモトシテン", "name": "株式会社　かんぽ生命　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1番1号", "postal_code": "8608797", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}, {"jis": "43101", "kana": "ニホンユウビン カブシキガイシヤ キユウシユウシシヤ", "name": "日本郵便　株式会社　九州支社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1-1", "postal_code": "8608797", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}]}');
 INSERT INTO office_data VALUES('8608525','{"jis": "43101", "kana": "カブシキガイシヤ アステム クマモトエイギヨウブ", "name": "株式会社　アステム　熊本営業部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "八王寺町", "banchi": "33-57", "postal_code": "8608525", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハチオウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608509','{"jis": "43101", "kana": "カブシキガイシヤ カミヒロ", "name": "株式会社　紙弘", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安町", "banchi": "378-4", "postal_code": "8608509", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤスマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608588','{"jis": "43101", "kana": "カブシキガイシヤ カリ-ノ", "name": "株式会社　カリーノ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "安政町", "banchi": "1番2号", "postal_code": "8608588", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "アンセイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608619','{"jis": "43101", "kana": "カブシキガイシヤ キユウシユウシンキンクレジツトサ-ビス", "name": "株式会社　九州しんきんクレジットサービス", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "草葉町", "banchi": "4番20号熊本富士火災熊本ビル(熊本中央郵便局私書箱第129号)", "postal_code": "8608619", "old_code": "860  ", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "クサバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608501','{"jis": "43101", "kana": "カブシキガイシヤ クマモトギンコウ チユウオウシテン", "name": "株式会社　熊本銀行　中央支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "山崎町", "banchi": "44", "postal_code": "8608501", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヤマサキマチ", "alternates": []}');
```

### Comparing `posuto-2023.5.0/posuto/posuto.py` & `posuto-2023.6.0/posuto/posuto.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/posuto/prep.py` & `posuto-2023.6.0/posuto/prep.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/posuto/tests/test_basic.py` & `posuto-2023.6.0/posuto/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.5.0/posuto.egg-info/PKG-INFO` & `posuto-2023.6.0/posuto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `posuto-2023.5.0/setup.cfg` & `posuto-2023.6.0/setup.cfg`

 * *Files identical despite different names*

