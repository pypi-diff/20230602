# Comparing `tmp/deklinacija-1.0.3.tar.gz` & `tmp/deklinacija-1.0.4.tar.gz`

## Comparing `deklinacija-1.0.3.tar` & `deklinacija-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 deklinacija-1.0.3/main.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/__init__.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/module.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.3/LICENSE
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 deklinacija-1.0.3/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 deklinacija-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/__init__.py
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/module.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 deklinacija-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 deklinacija-1.0.4/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 deklinacija-1.0.4/PKG-INFO
```

### Comparing `deklinacija-1.0.3/.github/workflows/python-package.yml` & `deklinacija-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.3/deklinacija/utils.py` & `deklinacija-1.0.4/deklinacija/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     'а': 'a', 'б': 'b', 'ц': 'c', 'ч': 'č', 'ћ': 'ć', 'д': 'd', 'ђ': 'đ', 'е': 'e', 'ф': 'f', 'г': 'g',
     'х': 'h', 'и': 'i', 'ј': 'j', 'к': 'k', 'л': 'l', 'љ': 'lj', 'м': 'm', 'н': 'n', 'њ': 'nj', 'о': 'o',
     'п': 'p', 'р': 'r', 'с': 's', 'ш': 'š', 'т': 't', 'у': 'u', 'в': 'v', 'з': 'z', 'ж': 'ž', 'џ': 'dž'}
 
 latExceptions = []
 
 def isLatin(word):
-    if word[-1] in alphabet:
+    if word[-1].lower() in alphabet:
         return True
-    elif word[-1] in alphabet_latin:
+    elif word[-1].lower() in alphabet_latin:
         return False
     else:
         raise ValueError("word contains illegal characters")
 
 def toCyrillic(word):
 
     wordArray = []
@@ -91,16 +91,16 @@
 
         else:
             word[n] = i
         n += 1
     
     return "".join(word)
 
-def check(name,gender,latin):
-    if type(name) != str or type(name) != str or type(gender) != str or type(latin) != bool:
+def check(name,gender):
+    if type(name) != str or type(name) != str or type(gender) != str:
         raise TypeError("name and gender params must be a string, param latin must be a boolean")
     
     gender = gender.strip()
     name = name.strip()
 
     if gender.lower() not in ["male","female"]:
         raise ValueError('gender param must be either "male" or "female"')
@@ -145,15 +145,23 @@
 #     for (k,v) in reader.items():
 #         kConverted = toCyrillic(k)
 #         vConverted = toCyrillic(v)
 #         text = text + kConverted + "," + vConverted + "\n"
     
 #     f.truncate(0)
 #     f.write(text)
-
+def formatName(word):
+    word = list(word)
+    word[0] = word[0].upper()
+    n = 1
+    while n < len(word):
+        word[n] = word[n].lower()
+        n += 1
+    return "".join(word)
+        
 module_path = os.path.abspath(__file__)
 
 module_directory = os.path.dirname(module_path)
 
 csv_file_path = os.path.join(module_directory, 'vokativ_database.csv')
 
 with open(csv_file_path,"r",encoding="utf-8") as file:
```

### Comparing `deklinacija-1.0.3/deklinacija/vokativ_database.csv` & `deklinacija-1.0.4/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.3/LICENSE` & `deklinacija-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.3/README.md` & `deklinacija-1.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # deklinacija
-A Python library for declension of personal names in Serbian. The  grammatical rules utlized in this library also apply to Croatian and Bosnian.
+A Python library for declension of personal names in Serbian, with support for both Cyrillic and Latin scripts.
 
 ## Installation
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
 The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
 ```
-**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in the Cyrillic or Latin script. **Currently, only the Latin script is supported.**
+**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below).
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
 genitiv = dek.genitiv("Velja","male") #Velje
-dativ = dek.dativ("Petar","male") #Petru
+dativ = dek.dativ("Петар","male") #Петру
 akuzativ = dek.akuzativ("Jana","female") #Janu
 vokativ = dek.vokativ("Predrag","male") #Predraže
+vokativ2 = dek.vokativ("PREDRAG","male") #PREDRAŽE
 instrumental = dek.instrumental("Uroš","male") #Urošem
-instrumental2 = dek.instrumental("Vuk","male") #Vukom
+instrumental2 = dek.instrumental("Вук","male") #Вуком
 lokativ = dek.lokativ("Lana","female") #Lani
 
 print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
 #Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje.
 #Translation: Hello Predrag! You have received a friend request from Velja.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
-The `declineAll()` function returns a `dictionary`.
+The `declineAll()` function returns a `dictionary`, where keys are the grammatical cases.
 
 ```python
 import deklinacija as dek
 
 Nikola = dek.declineAll("Nikola","male") 
 #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
 #'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
@@ -47,12 +48,13 @@
 print("Dali ste poklon",Nikola['dativ']) 
 #Dali ste poklon Nikoli
 #Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
-- Support for both Latin and Cyrillic scripts
 - Declension of last names
+- Possessive forms
+
 
 ## Attribution
 [Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
```

### Comparing `deklinacija-1.0.3/pyproject.toml` & `deklinacija-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.0.3/PKG-INFO` & `deklinacija-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # deklinacija
-A Python library for declension of personal names in Serbian. The  grammatical rules utlized in this library also apply to Croatian and Bosnian.
+A Python library for declension of personal names in Serbian, with support for both Cyrillic and Latin scripts.
 
 ## Installation
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
 The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
 ```
-**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in the Cyrillic or Latin script. **Currently, only the Latin script is supported.**
+**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below).
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
 genitiv = dek.genitiv("Velja","male") #Velje
-dativ = dek.dativ("Petar","male") #Petru
+dativ = dek.dativ("Петар","male") #Петру
 akuzativ = dek.akuzativ("Jana","female") #Janu
 vokativ = dek.vokativ("Predrag","male") #Predraže
+vokativ2 = dek.vokativ("PREDRAG","male") #PREDRAŽE
 instrumental = dek.instrumental("Uroš","male") #Urošem
-instrumental2 = dek.instrumental("Vuk","male") #Vukom
+instrumental2 = dek.instrumental("Вук","male") #Вуком
 lokativ = dek.lokativ("Lana","female") #Lani
 
 print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
 #Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje.
 #Translation: Hello Predrag! You have received a friend request from Velja.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
-The `declineAll()` function returns a `dictionary`.
+The `declineAll()` function returns a `dictionary`, where keys are the grammatical cases.
 
 ```python
 import deklinacija as dek
 
 Nikola = dek.declineAll("Nikola","male") 
 #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
 #'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
@@ -61,12 +62,13 @@
 print("Dali ste poklon",Nikola['dativ']) 
 #Dali ste poklon Nikoli
 #Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
-- Support for both Latin and Cyrillic scripts
 - Declension of last names
+- Possessive forms
+
 
 ## Attribution
 [Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
```

