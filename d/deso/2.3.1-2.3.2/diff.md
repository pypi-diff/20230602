# Comparing `tmp/deso-2.3.1.tar.gz` & `tmp/deso-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deso-2.3.1.tar", last modified: Tue Apr 25 05:14:25 2023, max compression
+gzip compressed data, was "deso-2.3.2.tar", last modified: Fri Jun  2 15:06:07 2023, max compression
```

## Comparing `deso-2.3.1.tar` & `deso-2.3.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 05:14:25.202108 deso-2.3.1/
--rw-rw-rw-   0        0        0     1085 2022-10-22 06:55:06.000000 deso-2.3.1/LICENSE
--rw-rw-rw-   0        0        0    20360 2023-04-25 05:14:25.201113 deso-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    19062 2023-02-08 08:09:20.000000 deso-2.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 05:14:25.177249 deso-2.3.1/deso/
--rw-rw-rw-   0        0        0     2262 2022-10-22 06:55:06.000000 deso-2.3.1/deso/Derived.py
--rw-rw-rw-   0        0        0     2838 2023-02-08 08:09:20.000000 deso-2.3.1/deso/Identity.py
--rw-rw-rw-   0        0        0     1032 2022-10-22 06:55:06.000000 deso-2.3.1/deso/Media.py
--rw-rw-rw-   0        0        0     1745 2022-10-22 06:55:06.000000 deso-2.3.1/deso/Metadata.py
--rw-rw-rw-   0        0        0     5422 2023-04-20 15:06:54.000000 deso-2.3.1/deso/Posts.py
--rw-rw-rw-   0        0        0     4441 2023-04-25 05:13:58.000000 deso-2.3.1/deso/Sign.py
--rw-rw-rw-   0        0        0    28489 2023-04-16 19:32:16.000000 deso-2.3.1/deso/Social.py
--rw-rw-rw-   0        0        0    15734 2022-10-22 06:55:06.000000 deso-2.3.1/deso/Trade.py
--rw-rw-rw-   0        0        0     7817 2023-02-08 08:09:20.000000 deso-2.3.1/deso/User.py
--rw-rw-rw-   0        0        0      256 2022-10-22 06:55:06.000000 deso-2.3.1/deso/__init__.py
--rw-rw-rw-   0        0        0     1634 2022-10-22 06:55:06.000000 deso-2.3.1/deso/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 05:14:25.197088 deso-2.3.1/deso.egg-info/
--rw-rw-rw-   0        0        0    20360 2023-04-25 05:14:24.000000 deso-2.3.1/deso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-25 05:14:24.000000 deso-2.3.1/deso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 05:14:24.000000 deso-2.3.1/deso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-25 05:14:24.000000 deso-2.3.1/deso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 05:14:24.000000 deso-2.3.1/deso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 05:14:25.203607 deso-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1425 2023-04-25 05:14:10.000000 deso-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:06:07.799801 deso-2.3.2/
+-rw-rw-rw-   0        0        0     1085 2022-07-14 19:21:22.000000 deso-2.3.2/LICENSE
+-rw-rw-rw-   0        0        0    21289 2023-06-02 15:06:07.798801 deso-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19951 2023-06-02 15:04:51.000000 deso-2.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 15:06:07.739788 deso-2.3.2/deso/
+-rw-rw-rw-   0        0        0    15297 2023-06-02 14:52:12.000000 deso-2.3.2/deso/Associations.py
+-rw-rw-rw-   0        0        0     2262 2022-07-14 19:21:22.000000 deso-2.3.2/deso/Derived.py
+-rw-rw-rw-   0        0        0     2838 2023-01-11 16:02:29.000000 deso-2.3.2/deso/Identity.py
+-rw-rw-rw-   0        0        0     1032 2022-07-14 19:21:22.000000 deso-2.3.2/deso/Media.py
+-rw-rw-rw-   0        0        0     1745 2022-07-14 19:21:22.000000 deso-2.3.2/deso/Metadata.py
+-rw-rw-rw-   0        0        0     5422 2023-05-01 06:22:38.000000 deso-2.3.2/deso/Posts.py
+-rw-rw-rw-   0        0        0     4441 2023-05-01 06:22:38.000000 deso-2.3.2/deso/Sign.py
+-rw-rw-rw-   0        0        0    28489 2023-04-08 09:19:16.000000 deso-2.3.2/deso/Social.py
+-rw-rw-rw-   0        0        0    15734 2022-07-14 19:21:22.000000 deso-2.3.2/deso/Trade.py
+-rw-rw-rw-   0        0        0     7817 2022-12-09 09:21:26.000000 deso-2.3.2/deso/User.py
+-rw-rw-rw-   0        0        0      300 2023-06-02 14:08:05.000000 deso-2.3.2/deso/__init__.py
+-rw-rw-rw-   0        0        0     1634 2022-07-14 19:21:22.000000 deso-2.3.2/deso/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:06:07.795800 deso-2.3.2/deso.egg-info/
+-rw-rw-rw-   0        0        0    21289 2023-06-02 15:06:07.000000 deso-2.3.2/deso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-02 15:06:07.000000 deso-2.3.2/deso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:06:07.000000 deso-2.3.2/deso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-02 15:06:07.000000 deso-2.3.2/deso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-02 15:06:07.000000 deso-2.3.2/deso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:06:07.799801 deso-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2023-06-02 15:05:25.000000 deso-2.3.2/setup.py
```

### Comparing `deso-2.3.1/LICENSE` & `deso-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/PKG-INFO` & `deso-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deso
-Version: 2.3.1
+Version: 2.3.2
 Summary: A python module for deso
 Author: ItsAditya (https://itsaditya.xyz)
 Author-email: <chaudharyaditya0005@gmail.com>
 Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation,decentralized social media
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,21 +23,42 @@
 by passing the argument `nodeURL` to any of the classes.
 
 For example:
 
 ```python
 import deso
 
-desoUser = deso.User(nodeURL="https://love4src.com/api/v0/")
+desoUser = deso.User(nodeURL="https://diamondapp.com/api/v0/")
 ```
 
 Developed by [ItsAditya](https://diamondapp.com/u/itsaditya)
 
+
 ## How to Use:
 
+To perform all the WRITE actions to DeSo Blockchain you need SEED_HEX and DESO Public Key.
+
+This is how you generate SEED_HEX using your 12 word mnemonic phrase.
+
+```python
+from deso import Identity
+SEED_PHRASE = 'YOUR 12 WORD DESO SEED PHRASE'
+SEED_HEX = Identity.getSeedHexFromSeedPhrase(SEED_PHRASE)
+print(SEED_HEX)
+```
+
+You can also generate brand new DeSo seed phrase using this code.
+
+```python
+from deso import Identity
+seedPhrase = Identity.generateDesoSeedPhrase()
+print(seedPhrase)
+```
+
+
 ### Metadata
 
 1. Getting Deso Price
 
 ```python
 import deso
 
@@ -299,32 +320,14 @@
 desoPosts = deso.Posts()
 postHashHex = "74d50e4d33b7512941a2ada91a947aecfc2f9fd179d67eb1e0008d4812597196"
 print(desoPosts.getNFTBidsForNFTPost(postHashHex).json())
 ```
 
 ### Social
 
-To perform all the WRITE actions to DeSo Blockchain you need SEED_HEX and DESO Public Key.
-
-This is how you generate SEED_HEX using your 12 word mnemonic phrase.
-
-```python
-from deso import Identity
-SEED_PHRASE = 'YOUR 12 WORD DESO SEED PHRASE'
-SEED_HEX = Identity.getSeedHexFromSeedPhrase(SEED_PHRASE)
-print(SEED_HEX)
-```
-
-You can also generate brand new DeSo seed phrase using this code.
-
-```python
-from deso import Identity
-seedPhrase = Identity.generateDesoSeedPhrase()
-print(seedPhrase)
-```
 
 1. Making post to deso blockchain
 
 ```python
 import deso
 
 SEED_HEX = 'YOUR SEED SEED_HEX'
@@ -674,7 +677,44 @@
         for Example, if you want to mint 15 DAO coin, set coinsToBurn to hex(int(15*1e18))'''
 desoTrade = deso.Trade(publicKey=PUBLIC_KEY, seedHex=SEED_HEX)
 coinsToMint = 1000000
 coinsToBurnInRequiredFormat = hex(int(coinsToMint * 1e18))
 mintStatus = desoTrade.mintDAOCoins(coinsToBurnInRequiredFormat)
 print(mintStatus)
 ```
+
+### Associations
+
+1. React on a deso post (create post association)
+
+```python
+import deso
+SEED_HEX = "YOUR SEED HEX"
+PUBLIC_KEY = "YOUR PUBLIC KEY"
+
+desoAssociation = deso.Associations(
+    publicKey=PUBLIC_KEY, seedHex=SEED_HEX, nodeURL="https://diamondapp.com/api/v0/")
+
+response = desoAssociation.createPostAssociation(
+    associationType="REACTION",
+    associationValue="LOVE",
+    postHashHex="a6db1ca8dedd90df367b556ec7898a9b1be55eff4926f62caeef9221d3c5bac7",
+
+)
+```
+
+2. Delete post reaction
+
+```python
+
+import deso
+
+SEED_HEX = "YOUR SEED HEX"
+PUBLIC_KEY = "YOUR PUBLIC KEY"
+
+desoAssociation = deso.Associations(
+    publicKey=PUBLIC_KEY, seedHex=SEED_HEX, nodeURL="https://diamondapp.com/api/v0/")
+
+
+res = desoAssociation.deletePostAssociation(
+    association_ID="892a296a4e0af04c8edb22a53ced1cb98a8358450605f6fa08a6a109c9e22f3b")
+
```

### Comparing `deso-2.3.1/README.md` & `deso-2.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,42 @@
 by passing the argument `nodeURL` to any of the classes.
 
 For example:
 
 ```python
 import deso
 
-desoUser = deso.User(nodeURL="https://love4src.com/api/v0/")
+desoUser = deso.User(nodeURL="https://diamondapp.com/api/v0/")
 ```
 
 Developed by [ItsAditya](https://diamondapp.com/u/itsaditya)
 
+
 ## How to Use:
 
+To perform all the WRITE actions to DeSo Blockchain you need SEED_HEX and DESO Public Key.
+
+This is how you generate SEED_HEX using your 12 word mnemonic phrase.
+
+```python
+from deso import Identity
+SEED_PHRASE = 'YOUR 12 WORD DESO SEED PHRASE'
+SEED_HEX = Identity.getSeedHexFromSeedPhrase(SEED_PHRASE)
+print(SEED_HEX)
+```
+
+You can also generate brand new DeSo seed phrase using this code.
+
+```python
+from deso import Identity
+seedPhrase = Identity.generateDesoSeedPhrase()
+print(seedPhrase)
+```
+
+
 ### Metadata
 
 1. Getting Deso Price
 
 ```python
 import deso
 
@@ -282,32 +303,14 @@
 desoPosts = deso.Posts()
 postHashHex = "74d50e4d33b7512941a2ada91a947aecfc2f9fd179d67eb1e0008d4812597196"
 print(desoPosts.getNFTBidsForNFTPost(postHashHex).json())
 ```
 
 ### Social
 
-To perform all the WRITE actions to DeSo Blockchain you need SEED_HEX and DESO Public Key.
-
-This is how you generate SEED_HEX using your 12 word mnemonic phrase.
-
-```python
-from deso import Identity
-SEED_PHRASE = 'YOUR 12 WORD DESO SEED PHRASE'
-SEED_HEX = Identity.getSeedHexFromSeedPhrase(SEED_PHRASE)
-print(SEED_HEX)
-```
-
-You can also generate brand new DeSo seed phrase using this code.
-
-```python
-from deso import Identity
-seedPhrase = Identity.generateDesoSeedPhrase()
-print(seedPhrase)
-```
 
 1. Making post to deso blockchain
 
 ```python
 import deso
 
 SEED_HEX = 'YOUR SEED SEED_HEX'
@@ -657,7 +660,44 @@
         for Example, if you want to mint 15 DAO coin, set coinsToBurn to hex(int(15*1e18))'''
 desoTrade = deso.Trade(publicKey=PUBLIC_KEY, seedHex=SEED_HEX)
 coinsToMint = 1000000
 coinsToBurnInRequiredFormat = hex(int(coinsToMint * 1e18))
 mintStatus = desoTrade.mintDAOCoins(coinsToBurnInRequiredFormat)
 print(mintStatus)
 ```
+
+### Associations
+
+1. React on a deso post (create post association)
+
+```python
+import deso
+SEED_HEX = "YOUR SEED HEX"
+PUBLIC_KEY = "YOUR PUBLIC KEY"
+
+desoAssociation = deso.Associations(
+    publicKey=PUBLIC_KEY, seedHex=SEED_HEX, nodeURL="https://diamondapp.com/api/v0/")
+
+response = desoAssociation.createPostAssociation(
+    associationType="REACTION",
+    associationValue="LOVE",
+    postHashHex="a6db1ca8dedd90df367b556ec7898a9b1be55eff4926f62caeef9221d3c5bac7",
+
+)
+```
+
+2. Delete post reaction
+
+```python
+
+import deso
+
+SEED_HEX = "YOUR SEED HEX"
+PUBLIC_KEY = "YOUR PUBLIC KEY"
+
+desoAssociation = deso.Associations(
+    publicKey=PUBLIC_KEY, seedHex=SEED_HEX, nodeURL="https://diamondapp.com/api/v0/")
+
+
+res = desoAssociation.deletePostAssociation(
+    association_ID="892a296a4e0af04c8edb22a53ced1cb98a8358450605f6fa08a6a109c9e22f3b")
+
```

### Comparing `deso-2.3.1/deso/Derived.py` & `deso-2.3.2/deso/Derived.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Identity.py` & `deso-2.3.2/deso/Identity.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Media.py` & `deso-2.3.2/deso/Media.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Metadata.py` & `deso-2.3.2/deso/Metadata.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Posts.py` & `deso-2.3.2/deso/Posts.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Sign.py` & `deso-2.3.2/deso/Sign.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Social.py` & `deso-2.3.2/deso/Social.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/Trade.py` & `deso-2.3.2/deso/Trade.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/User.py` & `deso-2.3.2/deso/User.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso/utils.py` & `deso-2.3.2/deso/utils.py`

 * *Files identical despite different names*

### Comparing `deso-2.3.1/deso.egg-info/PKG-INFO` & `deso-2.3.2/deso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deso
-Version: 2.3.1
+Version: 2.3.2
 Summary: A python module for deso
 Author: ItsAditya (https://itsaditya.xyz)
 Author-email: <chaudharyaditya0005@gmail.com>
 Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation,decentralized social media
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,21 +23,42 @@
 by passing the argument `nodeURL` to any of the classes.
 
 For example:
 
 ```python
 import deso
 
-desoUser = deso.User(nodeURL="https://love4src.com/api/v0/")
+desoUser = deso.User(nodeURL="https://diamondapp.com/api/v0/")
 ```
 
 Developed by [ItsAditya](https://diamondapp.com/u/itsaditya)
 
+
 ## How to Use:
 
+To perform all the WRITE actions to DeSo Blockchain you need SEED_HEX and DESO Public Key.
+
+This is how you generate SEED_HEX using your 12 word mnemonic phrase.
+
+```python
+from deso import Identity
+SEED_PHRASE = 'YOUR 12 WORD DESO SEED PHRASE'
+SEED_HEX = Identity.getSeedHexFromSeedPhrase(SEED_PHRASE)
+print(SEED_HEX)
+```
+
+You can also generate brand new DeSo seed phrase using this code.
+
+```python
+from deso import Identity
+seedPhrase = Identity.generateDesoSeedPhrase()
+print(seedPhrase)
+```
+
+
 ### Metadata
 
 1. Getting Deso Price
 
 ```python
 import deso
 
@@ -299,32 +320,14 @@
 desoPosts = deso.Posts()
 postHashHex = "74d50e4d33b7512941a2ada91a947aecfc2f9fd179d67eb1e0008d4812597196"
 print(desoPosts.getNFTBidsForNFTPost(postHashHex).json())
 ```
 
 ### Social
 
-To perform all the WRITE actions to DeSo Blockchain you need SEED_HEX and DESO Public Key.
-
-This is how you generate SEED_HEX using your 12 word mnemonic phrase.
-
-```python
-from deso import Identity
-SEED_PHRASE = 'YOUR 12 WORD DESO SEED PHRASE'
-SEED_HEX = Identity.getSeedHexFromSeedPhrase(SEED_PHRASE)
-print(SEED_HEX)
-```
-
-You can also generate brand new DeSo seed phrase using this code.
-
-```python
-from deso import Identity
-seedPhrase = Identity.generateDesoSeedPhrase()
-print(seedPhrase)
-```
 
 1. Making post to deso blockchain
 
 ```python
 import deso
 
 SEED_HEX = 'YOUR SEED SEED_HEX'
@@ -674,7 +677,44 @@
         for Example, if you want to mint 15 DAO coin, set coinsToBurn to hex(int(15*1e18))'''
 desoTrade = deso.Trade(publicKey=PUBLIC_KEY, seedHex=SEED_HEX)
 coinsToMint = 1000000
 coinsToBurnInRequiredFormat = hex(int(coinsToMint * 1e18))
 mintStatus = desoTrade.mintDAOCoins(coinsToBurnInRequiredFormat)
 print(mintStatus)
 ```
+
+### Associations
+
+1. React on a deso post (create post association)
+
+```python
+import deso
+SEED_HEX = "YOUR SEED HEX"
+PUBLIC_KEY = "YOUR PUBLIC KEY"
+
+desoAssociation = deso.Associations(
+    publicKey=PUBLIC_KEY, seedHex=SEED_HEX, nodeURL="https://diamondapp.com/api/v0/")
+
+response = desoAssociation.createPostAssociation(
+    associationType="REACTION",
+    associationValue="LOVE",
+    postHashHex="a6db1ca8dedd90df367b556ec7898a9b1be55eff4926f62caeef9221d3c5bac7",
+
+)
+```
+
+2. Delete post reaction
+
+```python
+
+import deso
+
+SEED_HEX = "YOUR SEED HEX"
+PUBLIC_KEY = "YOUR PUBLIC KEY"
+
+desoAssociation = deso.Associations(
+    publicKey=PUBLIC_KEY, seedHex=SEED_HEX, nodeURL="https://diamondapp.com/api/v0/")
+
+
+res = desoAssociation.deletePostAssociation(
+    association_ID="892a296a4e0af04c8edb22a53ced1cb98a8358450605f6fa08a6a109c9e22f3b")
+
```

### Comparing `deso-2.3.1/setup.py` & `deso-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "2.3.1"
+VERSION = "2.3.2"
 DESCRIPTION = "A python module for DeSo"
 LONG_DESCRIPTION = "DesoPy is a python module that enables devs to interact with DeSo Blockchain using node.deso.org node by default. Includes all functions to read from or write to DeSo Blockchain"
 # Setting up
 setup(
     name="deso",
     version=VERSION,
     author="ItsAditya (https://itsaditya.xyz)",
```

