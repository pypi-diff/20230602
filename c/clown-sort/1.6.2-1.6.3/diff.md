# Comparing `tmp/clown_sort-1.6.2.tar.gz` & `tmp/clown_sort-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.6.2.tar", max compression
+gzip compressed data, was "clown_sort-1.6.3.tar", max compression
```

## Comparing `clown_sort-1.6.2.tar` & `clown_sort-1.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2840 2023-05-28 21:14:51.544578 clown_sort-1.6.2/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.2/LICENSE
--rw-r--r--   0        0        0     8340 2023-05-28 21:13:57.663794 clown_sort-1.6.2/README.md
--rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.2/clown_sort/__init__.py
--rw-r--r--   0        0        0     7864 2023-05-28 21:12:17.679551 clown_sort-1.6.2/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.6.2/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.2/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     2199 2023-05-27 22:17:44.883449 clown_sort-1.6.2/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.6.2/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3276 2023-05-27 21:44:44.872765 clown_sort-1.6.2/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     9634 2023-05-27 21:44:44.873210 clown_sort-1.6.2/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.2/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.2/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.2/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.2/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.2/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.2/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.2/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-05-28 21:14:51.549471 clown_sort-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     9762 1970-01-01 00:00:00.000000 clown_sort-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2961 2023-06-02 21:09:30.892923 clown_sort-1.6.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.3/LICENSE
+-rw-r--r--   0        0        0     8659 2023-05-28 21:20:43.213283 clown_sort-1.6.3/README.md
+-rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.3/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7864 2023-05-28 21:12:17.679551 clown_sort-1.6.3/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.6.3/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.3/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     2199 2023-05-27 22:17:44.883449 clown_sort-1.6.3/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11399 2023-06-02 21:07:03.088714 clown_sort-1.6.3/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3310 2023-06-02 21:07:10.228823 clown_sort-1.6.3/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    10043 2023-06-02 07:17:50.864003 clown_sort-1.6.3/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.3/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.3/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.3/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.3/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.3/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.3/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.3/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-06-02 21:09:30.898473 clown_sort-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0    10081 1970-01-01 00:00:00.000000 clown_sort-1.6.3/PKG-INFO
```

### Comparing `clown_sort-1.6.2/CHANGELOG.md` & `clown_sort-1.6.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+### 1.6.3
+* Fix bug with manual folder selection
+* Refactor `move_to_processed_dir()` and call from `sort_selector.py`.
+
 ### 1.6.2
 * Add `--force` and `[gui,pdf]` to the `pipx` installation instructions
 
 ### 1.6.1
 * Make the brackets print in the optional package install instructions
 * Only check for `pymupdf` once
```

### Comparing `clown_sort-1.6.2/LICENSE` & `clown_sort-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/README.md` & `clown_sort-1.6.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -134,18 +134,17 @@
 Feel free to file issues or open pull requests.
 
 This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
 1. Install Poetry.
 1. `git clone` this repo.
 1. `cd clown_sort`
 1. `poetry install`
-1. Optional components can be install with `poetry install -E pdf -E gui`
+1. Optional components can be install with `poetry install --all-extras`
 
-Only requirement is that tests should pass before you open it, which you can check with
+Only requirement is that tests should pass before you open it which you can check by running `pytest`.
 
-```
-pytest
-```
+### Running Tests
+Test suite can be launched with `pytest`. If you do some development and something goes weird and you're continually running into errors about non-empty directories try clearing out the test suite's temp directory by deleting the contents of `tests/tmp/` (`rm -fr tests/tmp/*` on Linux or macOS etc.).
 
 [^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.
 
 [^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried's various scams as part of his commitment to "unrivaled transparency".
```

### Comparing `clown_sort-1.6.2/clown_sort/__init__.py` & `clown_sort-1.6.3/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/config.py` & `clown_sort-1.6.3/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/filename_extractor.py` & `clown_sort-1.6.3/clown_sort/filename_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 REVEDDIT_REGEX = re.compile('Reveddit Real.?Time')
 SUBREDDIT_REGEX = re.compile('/r/(?P<subreddit>\\w+)|\\sse(lf|ir)\\.(?P<subreddit2>\\w+)')
 DUNE_ANALYTICS_REGEX = re.compile('Query results (.*) @\\w+')
 RETWEETED_REGEX = re.compile('(.*) Retweeted')
 
 MAX_FILENAME_LENGTH = 225
 MIN_LENGTH_FOR_DUPE_CHECK = 9
-DEFAULT_LENGTH_FOR_LONG_FILENAMES = 150
+DEFAULT_LENGTH_FOR_LONG_FILENAMES = 190
 MIN_SIMILARITY_RATIO_TO_BE_SAME = 0.80
 
 
 class FilenameExtractor:
     def __init__(self, image_file: 'ImageFile') -> None:
         self.image_file = image_file
         self.text: Optional[str] = image_file.extracted_text()
```

### Comparing `clown_sort-1.6.2/clown_sort/files/image_file.py` & `clown_sort-1.6.3/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/files/pdf_file.py` & `clown_sort-1.6.3/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/files/sortable_file.py` & `clown_sort-1.6.3/clown_sort/files/sortable_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,18 @@
                 if not (Config.yes_overwrite or Confirm.ask(f"Overwrite?")):
                     console.print("Skipping...", style='dim')
                     continue
 
             self._paths_of_sorted_copies.append(destination_path)
             self.copy_file_to_sorted_dir(destination_path, match)
 
+        self.move_to_processed_dir()
+
+    def move_to_processed_dir(self) -> None:
+        """Finalize the file handling, either leaving, deleting, or moving to processed files dir."""
         if Config.leave_in_place:
             console.print(bullet_text(Text('Leaving in place...', style='dim')))
             return
 
         # Don't move the file to the processed_dir if it started in a sorted location
         if self.file_path in self._paths_of_sorted_copies:
             console.print(bullet_text(Text('Not moving original file to processed dir...', style='color(127)')))
```

### Comparing `clown_sort-1.6.2/clown_sort/sort_selector.py` & `clown_sort-1.6.3/clown_sort/sort_selector.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,16 +68,16 @@
             return
         elif event == EXIT:
             sys.exit()
         elif event == OK:
             break
 
     log.debug(f"All values: {values}")
-    chosen_filename = values[0]
-    new_subdir = values[1]
+    chosen_filename = values[1]
+    new_subdir = values[2]
     destination_dir = Config.sorted_screenshots_dir.joinpath(new_subdir)
 
     if is_empty(chosen_filename):
         raise ValueError("Filename can't be blank!")
 
     if not destination_dir.exists():
         result = psg.popup_yes_no(f"Subdir '{new_subdir}' doesn't exist. Create?",  title="Unknown Subdirectory")
@@ -89,7 +89,8 @@
             console.print(bullet_text(f"Directory not found. Skipping '{image.file_path}'..."))
             return
 
     new_filename = destination_dir.joinpath(chosen_filename)
     log.info(f"Chosen Filename: '{chosen_filename}'\nSubdir: '{new_subdir}'\nNew file: '{new_filename}'\nEvent: {event}\n")
     console.print(bullet_text(f"Moving '{image.file_path}' to '{new_filename}'..."))
     image.copy_file_to_sorted_dir(new_filename)
+    image.move_to_processed_dir()
```

### Comparing `clown_sort-1.6.2/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.6.3/clown_sort/sorting_rules/crypto.csv`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,156 @@
 folder,regex
-1mdb,1mdb|jho[-_\s]*low|Victor[-_\s]*Hoo
-3ac,3ac|Three[-_\s]*Arrows[-_\s]*Capital|su[-_\s]*zhu|zhu[-_\s]*su|kyle[-_\s]*davies|OPNX
-A16Z,a16z|andreessen|packym|arianna[-_\s1]*simpson
-Aave,aave
+1mdb,1mdb|jho[-_\s.]*low|Victor[-_\s.]*Hoo
+3ac,3ac|Three[-_\s.]*Arrows[-_\s.]*Capital|su[-_\s.]*zhu|zhu[-_\s.]*su|kyle[-_\s.]*davies|OPNX
+A16Z,a16z|Andreessen|Packym|Arianna[-_\s1]*Simpson
+Aave,\bAave
 AAX,\baax
 Algorand,\bAlgorand|\b[$#]ALGO\b
 Arbitrum,Arbitrum|[$#]ARB\b
-Amber Group,Amber[-_\s]*Group|\btiantian\b|\bkullander\b|\btony[-_\s]*he\b|\bbo[-_\s]*shen\b
+Amber Group,Amber[-_\s.]*Group|\btiantian\b|\bkullander\b|\btony[-_\s.]*he\b|\bbo[-_\s.]*shen\b
 Aptos,\bAptos\b
 Art,occult
-Avalanche,\bAvax|AVAX\b|avalanche|\bava[-_\s]*labs
-Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC|Commercium[-_\s]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s]*Bancshares|United[-_\s]*Texas|\bUTB\b|Craig[-_\s]*Sellars
-Bankless,Bankless|David[-_\s]*Hoffman
+Avalanche,\bAvax|AVAX\b|avalanche|\bava[-_\s.]*labs
+Banks,SEBA[^a-z]|Credit[-_\s.]*Suisse|SJMBT|Sygnum|Celtic[-_\s.]*Bank|\bMercury\b|Choice[-_\s.]*Financial[-_\s.]*Group|\$FRC|Commercium[-_\s.]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s.]*Bancshares|United[-_\s.]*Texas|\bUTB\b|Craig[-_\s.]*Sellars
+Bankless,Bankless|David[-_\s.]*Hoffman
 Biconomy,\bBiconomy|Omchain
-Binary Options,binary[-_\s]*options
-Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s]*(IO|Wallet)|\bkeyway|\bkey[-_\s]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s]*Ng|InvestByBit|Swyftx
+Binary Options,binary[-_\s.]*options
+Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s.]*(IO|Wallet)|\bkeyway|\bkey[-_\s.]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s.]*Ng|InvestByBit|Swyftx
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bithumb,\bbithumb
 Bitmain,Bitmain
 Bitstamp,Bitstamp
-Bittrex,Bittrex|Ritchie[-_\s]*Lai|Kiran[-_\s]*Raj|John[-_\s]*Roth\b|\bAquila\b
+Bittrex,Bittrex|Ritchie[-_\s.]*Lai|Kiran[-_\s.]*Raj|John[-_\s.]*Roth\b|\bAquila\b
 Bitzlato,Bitzlato
 Blockchain.com,\bblockchain\.com\b|@blockchain\b|@AskBlockchain\b
-Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna|KMSmithDC|Kristin[-_\s]*Smith\b|Warren[-_\s]*Davidson
-Blockchain Capital,Blockchain[-_\s]*Capital|\bbrock\b|brockpierce
-BlockFi,BlockFi|Zac[-_\s]*Prince|Brian[-_\s]*Oliver
+Blockchain8,Blockchain8|tom[-_\s.]*emmer|ritchie[-_\s.]*torres|repritchie|Warren[-_\s.]*Davidson|Byron[-_\s.]*Donalds|Ted[-_\s.]*Budd|Josh[-_\s.]*Gotheimer|Jake[-_\s.]*Auchincloss|Darren[-_\s.]*Soto|ro[-_\s.]*khanna|KMSmithDC|Kristin[-_\s.]*Smith\b|Warren[-_\s.]*Davidson
+Blockchain Capital,Blockchain[-_\s.]*Capital|\bbrock\b|brockpierce
+BlockFi,BlockFi|Zac[-_\s.]*Prince|Brian[-_\s.]*Oliver
 Blockstream,Blockstream
-Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s]*Paul\b|raoul(gmi|[-_\s]*pal)|mccormack
-Broettes,Nicole[-_\s]*Behnam|natbrunell
-Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit|TravelByBit
+Bored Ape Yacht Club,BAYC|Bored[-_\s.]*Ape|yuga[-_\s.]*labs
+Bros,cryptomanran|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang
+Broettes,Nicole[-_\s.]*Behnam|natbrunell
+Bybit,\bBybit\b|Ben[-_\s.]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
-Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)|\bIZRL
-Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|\bcelsian|Artur[-_\s]*Abreu|ronpaulbot
-China,fentanyl
-Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
-CMCC Global,CMCC[-_\s]*Global
-Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam|\bremitly\b|\$RELY\b
-Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd|Leslie[-_\s]*Lamb|dougpolkvids
+Cathie Wood,Cathie[-_\s.]*Wood|\bARK(F|G|K|[-_\s.]*Innovation|[-_\s.]*Invest)|\bIZRL
+Celsius,celsius|mashinsky|levity[-_\s.]*and[-_\s.]*love|\bcelsian|Artur[-_\s.]*Abreu|ronpaulbot
+China,fentanyl|chin(a|ese)
+Circle,[@#]circle|usdc|circle[-_\s.]*internet|disparte|\ballaire|jerallaire
+CMCC Global,CMCC[-_\s.]*Global
+Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
+Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
-Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv
+Cross River Bank,\bCRB|Cross[-_\s.]*River|Prestige[-_\s.]*Capital|\bbae[-_\s.]*communications|Zenfi\b|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv|\bKabbage|\bAFRM\b
 Cumberland,cumberland
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
-CUBI,\bCUBI\b|Customers[-_\s]*Ban(k|corp)
-Custodia,custodia\b|caitlin[-_\s]*long
-dalle,craiyon|midjourney|\bdall[-_\s]*e\b
-DCG,DCG|digital\s*currency\s*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b
-DeFi,\bdefi\b|decentralized[-_\s]*finance
-Dragonfly Capital,Dragonfly[-_\s]*Capital
-DWF,DWF|Andrey[-_\s]*Grachev|\bgrachev\b
-Effective Altruism,\bE\.?A\.?\b|effective[-_\s]*altruism
-El Salvador,El[-_\s]*Salvador|Bukele|Max[-_\s]*Keiser
+CUBI,\bCUBI\b|Customers[-_\s.]*Ban(k|corp)
+Custodia,custodia\b|caitlin[-_\s.]*long
+dalle,craiyon|midjourney|\bdall[-_\s.]*e\b
+DCG,DCG|digital[-_\s.]*currency[-_\s.]*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b
+DeFi,\bdefi\b|decentralized[-_\s.]*finance
+Dragonfly Capital,Dragonfly[-_\s.]*Capital
+DWF,DWF|Andrey[-_\s.]*Grachev|\bgrachev\b
+Effective Altruism,\bE\.?A\.?\b|effective[-_\s.]*altruism
+El Salvador,El[-_\s.]*Salvador|Bukele|Max[-_\s.]*Keiser
 Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Euler Finance,\beuler\b
 FalconX,falconx
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
-Friedlander Group,Friedlander|Agro[-_\s]*Bank|all\s*year\*m|\bbrock\b|brockpierce|litvishhocker
-FTX,FTX|\bFTT\b|\bSBF|Trabucco|\bBankman\b|\bEllison|\bNishad|\bAlameda|Moonstone|friedberg|autism\s*capital|\bryne\b|clifton[-_\s]*bay|\bZUBR\b
-Galaxy Digital,novogratz|Alex[-_\s]*Thorn
-Gelato Network,Gelato[-_\s]*Network|\bSorbet[-_\s]*Finance|@gitpusha|hilmar[-_\s]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s]*Finance|Dave[-_\s]*Leibowitz|Hilmar[-_\s]*Orth|joehquak
+Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker
+FTX,FTX|\bFTT\b|\bSBF|Trabucco|\bBankman\b|\bEllison|\bNishad|\bAlameda|Moonstone|friedberg|autism[-_\s.]*capital|\bryne\b|clifton[-_\s.]*bay|\bZUBR\b
+Galaxy Digital,novogratz|Alex[-_\s.]*Thorn
+Gelato Network,Gelato[-_\s.]*Network|\bSorbet[-_\s.]*Finance|@gitpusha|hilmar[-_\s.]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s.]*Finance|Dave[-_\s.]*Leibowitz|Hilmar[-_\s.]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
-Hamas,\bHamas\b|Al[-_\s]*Qassam
-Hex,\bHex\b|[#$]Hex|Pulsechain|Richard\s*Heart|Hexican
-Hoo,Hoo[-_\s]*(Research|Exchange)|[#$]Hoo\b|Rexy\s*(Hoo|Wang)|\bhoo\b
-Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s]*Li
+Hamas,\bHamas\b|Al[-_\s.]*Qassam
+Hex,\bHex\b|[#$]Hex|Pulsechain|Richard[-_\s.]*Heart|Hexican
+Hoo,Hoo[-_\s.]*(Research|Exchange)|[#$]Hoo\b|Rexy[-_\s.]*(Hoo|Wang)|\bhoo\b
+Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s.]*Li
 Iran,\bIran\b|\bIranian\b|Nobitex|\bCoinNik|\bWallex\b|Sarmayex|\bRabex\b
-Jump Trading,Jump[-_\s]*Trading|@jump_
-Justin Sun,justin[-_\s]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina
-Kazakhstan,\bkazakh|Freedom[-_\s]*Holding|\balmaty|Timor[-_\s]*Turlov|\bFFIN[-_\s]*brokerage
+Jump Trading,Jump[-_\s.]*Trading|@jump_
+Justin Sun,justin[-_\s.]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina
+Kazakhstan,\bkazakh|Freedom[-_\s.]*Holding|\balmaty|Timor[-_\s.]*Turlov|\bFFIN[-_\s.]*brokerage
 Kinesis,kinesis|\bKVT\b|\bABX\b|\bKAG\b
 Kraken,kraken|payward
 KuCoin,kucoin
+Lead Bank,\bLead[-_\s.]*Bank\b|Finzly
 LBRY,LBRY|\bLBC\b
-Lexpunk Army,lexpunk|gabriel[-_\s]*shapiro|_gabrielShapir0|\blex_node\b
-Lifeboat Foundation,Lifeboat[-_\s]*Foundation
-North Korea,lazarus|North\s*Korea|pyongyang|\bDPRK|puuurtbubv|@fast4release
+Lexpunk Army,lexpunk|gabriel[-_\s.]*shapiro|_gabrielShapir0|\blex_node\b
+Lifeboat Foundation,Lifeboat[-_\s.]*Foundation
+North Korea,lazarus|North[-_\s.]*Korea|pyongyang|\bDPRK|puuurtbubv|@fast4release
 Paul LeRoux,leroux
-Polygon Labs,polygon[-_\s]*labs|ryan[-_\s]*watt\b|@Fwiz|Rebecca[-_\s]*Rettig|[#$]DOT\b
+Polygon Labs,polygon[-_\s.]*labs|ryan[-_\s.]*watt\b|@Fwiz|Rebecca[-_\s.]*Rettig|[#$]DOT\b
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
-Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s]*International|Keystone[-_\s]*Capital[-_\s]*Partners
-Mario Nawfal,mario[-_\s]*nawfal
-Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
+Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s.]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s.]*International|Keystone[-_\s.]*Capital[-_\s.]*Partners
+Mario Nawfal,mario[-_\s.]*nawfal
+Messari,Ryan[-_\s.]*Selkis|twobitidiot|messari|@robustus|Dan[-_\s.]*McArdle
 Memes,\smeme
-Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart|\bHayner\b
-Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)|Mission[-_\s]*Gateway|Aryeh[-_\s]*Realty
-Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
-Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b|\bLi[-_\s]*You\b
-Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
+Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s.]*Stewart|\bHayner\b
+Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s.]*(Bank|Commercial)|Mission[-_\s.]*Gateway|Aryeh[-_\s.]*Realty
+Founders Bank,Michael[-_\s.]*Bianchi|Founders[-_\s.]*Bank
+Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s.]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s.]*seven|kin[-_\s.]*ming[-_\s.]*je|william[-_\s.]*je\b|\bHaoyun\b|\bLi[-_\s.]*You\b
+Miners,bitcoin[-_\s.]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s.]*Scientific|Iris[-_\s.]*Energy|Blockstream
 Moonpay,\bmoonpay
 MSTR,Saylor|MSTR
-MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s]*bot
-Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
-Nexo,\bNexo\b|Antoni[-_\s]*Trenchev|Georgi[-_\s]*Shulev|Lydia[-_\s]*Shuleva
-NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
-OKX,oke?[cx]|star[-_\s]*xu|\blennix[-_\s]*lai\b
+MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s.]*bot
+Near Protocol,NEAR[-_\s.]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s.]*Rettig
+Nexo,\bNexo\b|Antoni[-_\s.]*Trenchev|Georgi[-_\s.]*Shulev|Lydia[-_\s.]*Shuleva
+NFTs,crypto[-_\s.]*punk|pudgy[-_\s.]*penguin
+OKX,oke?[cx]|star[-_\s.]*xu|\blennix[-_\s.]*lai\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
-PAG,\bpag\b|Weijian[-_\s]*Shan
-Paradigm,Fred[-_\s]*Ehrsam|paradigm\b
-Paxful,paxful|Ray[-_\s]*(Youssef|Savant)|Artur[-_\s]*Schaback
+PAG,\bpag\b|Weijian[-_\s.]*Shan
+Paradigm,Fred[-_\s.]*Ehrsam|paradigm\b
+Paxful,paxful|Ray[-_\s.]*(Youssef|Savant)|Artur[-_\s.]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
-Pi,\$PI[^\w]|Pi[-_\s]*Network
+Pi,\$PI[^\w]|Pi[-_\s.]*Network
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
-Quadriga,Quadriga|Gerald[-_\s]*Cotten|0xsifu\b|michael[-_\s]*patryn|wonderland|daniele[-_\s]*sesta\b
+Quadriga,Quadriga|Gerald[-_\s.]*Cotten|0xsifu\b|michael[-_\s.]*patryn|wonderland|daniele[-_\s.]*sesta\b
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
 SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
-Signature Bank,SBNY|Signature[-_\s]*Bank|Signet|Scott[-_\s]*Shay\b|(Joseph|Joe)[-_\s]*DePaolo|\bKushner\b
-Silicon Valley Bank,si?vb|Silicon[-_\s]*Valley[-_\s]*Bank
-Silk Road,Silk[-_\s]*Road|\bulbricht|\bDPR\b
-Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s]*Rettig
+Signature Bank,SBNY|Signature[-_\s.]*Bank|Signet|Scott[-_\s.]*Shay\b|(Joseph|Joe)[-_\s.]*DePaolo|\bKushner\b
+Silicon Valley Bank,si?vb|Silicon[-_\s.]*Valley[-_\s.]*Bank
+Silk Road,Silk[-_\s.]*Road|\bulbricht|\bDPR\b
+Silvergate,\$SI|Silvergate|Alan[-_\s.]*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s.]*Rettig
 Skrill,\bskrill
 Solana,Solana|Serum
-Symbolic Capital,Symbolic[-_\s]*Capital|Lev[-_\s]Livnev
-TerraLuna,luna\b|do[-_\s]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s]*Foundation\b
-Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s]*pierce)?\b|Clearstone[-_\s]*Global|Capital[-_\s]*Union|Noblex|SJMBT|Global[-_\s]*Trad(ing|e)[-_\s]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s]*Potter|Stablehouse|Samson[-_\s]*Mow|Gabor[-_\s]*Grubacs|XBTO|Paul[-_\s]*Eisma|Philippe[-_\s]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s]*Collins|\bdevasini\b|phil(ip)?[-_\s]*potter\b|van[-_\s]*der[-_\s]*velde|Perpetual[-_\s]*Action[-_\s]*Group|\burwhatyouknow|global[-_\s]*trade[-_\s]*solutions|reginald[-_\s]*fowler|renrenbee\b|\bludovicus|Amos[-_\s]*Ltd|William[-_\s]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s]*payments|Five[-_\s]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s]*sukenik|R(ondell|[ho][ho]n)[-_\s]*(Clyde)?[-_\s]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec
-Tornado Cash,tornado\s*cash
+Symbolic Capital,Symbolic[-_\s.]*Capital|Lev[-_\s]Livnev
+TerraLuna,luna\b|do[-_\s.]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s.]*Foundation\b
+Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Grubacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners
+Tornado Cash,tornado[-_\s.]*cash
 Transactive Systems UAB,Transactive
-Tron,\btron\b|tron(block|\s*)?chain|trondao|TRX\b
+Tron,\btron\b|tron(block|[-_\s.]*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
-VCs,venture[-_\s]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s]*sacks|\bthiel\b|sequoia|founders[-_\s]*fund|Valar[-_\s]*Ventures|6th[-_\s]*Man[-_\s]*Ventures|Northzone|Warburg[-_\s]*Serres|Alan[-_\s]*Howard|Tiger[-_\s]*Global
+VCs,venture[-_\s.]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s.]*sacks|\bthiel\b|sequoia|founders[-_\s.]*fund|Valar[-_\s.]*Ventures|6th[-_\s.]*Man[-_\s.]*Ventures|Northzone|Warburg[-_\s.]*Serres|Alan[-_\s.]*Howard|Tiger[-_\s.]*Global
 Vitalik Buterin,\bvitalik\b
 Voyager,voyager
 Wallet Addresses BCH,bitcoincash:q.*\b
 Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0–9]{25,39}\b
 Wallet Addresses Cardano,\baddr1[a-z0–9]+\b
 Wallet Addresses Cosmos,\bcosmos[a-zA-Z0–9_.-]{10,}\b
 Wallet Addresses Dash,\bX[1–9A-HJ-NP-Za-km-z]{33}
 Wallet Addresses Doge,\bD[a-zA-Z0–9_.-]{33}
 Wallet Addresses Ethereum,\b0x[a-fA-F0–9]{40}
 Wallet Addresses Monero,\b[48][0–9AB][1–9A-HJ-NP-Za-km-z]{93}
 Wallet Addresses Polkadot,\b1[0–9a-zA-Z]{47}
 Wallet Addresses Ripple,\br[0–9a-zA-Z]{33}
 Wallet Addresses Stellar,\bG[0–9A-Z]{40,60}\b
-Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s]*ivanov|boris[-_\s]*titov|[$#]waves\b
+Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s.]*ivanov|boris[-_\s.]*titov|[$#]waves\b
 Wintermute,wintermute|\bbebop\b
 Wirecard,wirecard|\bmarsalek\b|\bBafin\b
-Wyre,\bwyre|sendwyre
+Wyre,\bwyre|sendwyre|\bLead[-_\s.]*Bank\b
```

### Comparing `clown_sort-1.6.2/clown_sort/util/argument_parser.py` & `clown_sort-1.6.3/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/util/constants.py` & `clown_sort-1.6.3/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/util/filesystem_helper.py` & `clown_sort-1.6.3/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/util/rich_helper.py` & `clown_sort-1.6.3/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/clown_sort/util/string_helper.py` & `clown_sort-1.6.3/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.2/pyproject.toml` & `clown_sort-1.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.6.2"
+version = "1.6.3"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.6.2/PKG-INFO` & `clown_sort-1.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.6.2
+Version: 1.6.3
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -167,19 +167,18 @@
 Feel free to file issues or open pull requests.
 
 This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
 1. Install Poetry.
 1. `git clone` this repo.
 1. `cd clown_sort`
 1. `poetry install`
-1. Optional components can be install with `poetry install -E pdf -E gui`
+1. Optional components can be install with `poetry install --all-extras`
 
-Only requirement is that tests should pass before you open it, which you can check with
+Only requirement is that tests should pass before you open it which you can check by running `pytest`.
 
-```
-pytest
-```
+### Running Tests
+Test suite can be launched with `pytest`. If you do some development and something goes weird and you're continually running into errors about non-empty directories try clearing out the test suite's temp directory by deleting the contents of `tests/tmp/` (`rm -fr tests/tmp/*` on Linux or macOS etc.).
 
 [^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.
 
 [^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried's various scams as part of his commitment to "unrivaled transparency".
```

