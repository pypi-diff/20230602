# Comparing `tmp/code_qa-0.2.1.tar.gz` & `tmp/code_qa-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_qa-0.2.1.tar", max compression
+gzip compressed data, was "code_qa-0.3.1.tar", max compression
```

## Comparing `code_qa-0.2.1.tar` & `code_qa-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11356 2023-06-01 11:29:07.858435 code_qa-0.2.1/LICENSE
--rw-r--r--   0        0        0     2148 2023-06-02 04:27:10.766067 code_qa-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-01 11:28:22.025812 code_qa-0.2.1/code_qa/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-01 13:30:54.044136 code_qa-0.2.1/code_qa/cli.py
--rw-r--r--   0        0        0      167 2023-06-01 11:57:41.557031 code_qa-0.2.1/code_qa/logger.py
--rw-r--r--   0        0        0     1149 2023-06-02 02:24:31.211012 code_qa-0.2.1/code_qa/utils.py
--rw-r--r--   0        0        0      583 2023-06-02 04:27:16.934517 code_qa-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 code_qa-0.2.1/setup.py
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 code_qa-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-01 11:29:07.858435 code_qa-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2176 2023-06-02 04:31:58.721152 code_qa-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 11:28:22.025812 code_qa-0.3.1/code_qa/__init__.py
+-rw-r--r--   0        0        0     1876 2023-06-02 04:29:15.347651 code_qa-0.3.1/code_qa/cli.py
+-rw-r--r--   0        0        0      167 2023-06-01 11:57:41.557031 code_qa-0.3.1/code_qa/logger.py
+-rw-r--r--   0        0        0     1149 2023-06-02 02:24:31.211012 code_qa-0.3.1/code_qa/utils.py
+-rw-r--r--   0        0        0      583 2023-06-02 04:29:31.411214 code_qa-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 code_qa-0.3.1/setup.py
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 code_qa-0.3.1/PKG-INFO
```

### Comparing `code_qa-0.2.1/LICENSE` & `code_qa-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_qa-0.2.1/README.md` & `code_qa-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # CodeQA
 
-CodeQA is a powerful command-line tool designed to help developers understand and navigate their codebase more efficiently. By asking questions directly about your project, you can gain insights and deepen your understanding of the codebase without the need for extensive manual exploration. CodeQA is built on top of LangChain, leveraging its capabilities to provide accurate and insightful responses.
+**CodeQA** is a **powerful command-line tool** designed to help **developers understand and navigate their codebase**
+more efficiently. **By asking questions** directly about your project, you can **gain insights and deepen your
+understanding of the codebase** without the need for extensive manual exploration. CodeQA is built on top of LangChain,
+leveraging its capabilities to provide accurate and insightful responses.
 
-Besides code, CodeQA is engineered to be universally applicable across various text documents. It enables you to effortlessly navigate through:
+**Besides code,** CodeQA is engineered to be **universally applicable across various text documents**. It enables you to
+effortlessly navigate through:
 
 - PDF documents
 - Markdown files
 - And any other form of text-based documents.
 
 ## Getting Started
 
@@ -14,41 +18,45 @@
 
 1. **Install CodeQA**: Use pip to install CodeQA. Run the following command in your terminal:
 
     ```bash
     pip install code-qa
     ```
 
-2. **Set up OpenAI Token**: CodeQA uses OpenAI's API to generate responses. You need to add your OpenAI token to your virtual environment. Replace `YOUR_TOKEN` with your actual OpenAI token:
+2. **Set up OpenAI Token**: CodeQA uses OpenAI's API to generate responses. You need to add your OpenAI token to your
+   virtual environment. Replace `YOUR_TOKEN` with your actual OpenAI token:
 
     ```bash
     export OPENAI_TOKEN=YOUR_TOKEN
     ```
 
 3. **Navigate to your project folder**: Use the `cd` command to navigate to your project's directory:
 
     ```bash
     cd PATH/TO/MY/PROJECT
     ```
 
-4. **Initialize CodeQA Index**: This will generate a `.code_qa_data` folder within your project. The folder contains your project embeddings stored as parquet files. Run the following command:
+4. **Initialize CodeQA Index**: This will generate a `.code_qa` folder within your project. The folder contains your
+   project embeddings stored as parquet files. Run the following command:
 
     ```bash
     code_qa init
     ```
 
 ## Usage
 
-With CodeQA, you can ask questions directly about your code. For example, if you want to know how to test a particular part of your code, you can ask:
+With CodeQA, you can ask questions directly about your code. For example, if you want to know how to test a particular
+part of your code, you can ask:
 
 ```bash
 code_qa query "How can I test this?"
 ```
 
 ## Ignoring Files
 
-If there are certain files or directories that you want CodeQA to ignore, you can specify them in a `.codeqaignore` file. This file follows the same syntax and rules as the `.gitignore` file. Simply create a `.codeqaignore` file in your project's root directory and list the files or directories you want to ignore.
-
+If there are certain files or directories that you want CodeQA to ignore, you can specify them in a `.codeqaignore`
+file. This file follows the same syntax and rules as the `.gitignore` file. Simply create a `.codeqaignore` file in your
+project's root directory and list the files or directories you want to ignore.
 
 ## License
 
 CodeQA is licensed under the Apache License Version 2.0. For more details, see the [LICENSE](LICENSE) file.
```

### Comparing `code_qa-0.2.1/code_qa/cli.py` & `code_qa-0.3.1/code_qa/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from langchain.vectorstores import Chroma
 
 from code_qa.logger import logger
 from code_qa.utils import load_files, load_openai_token
 
 
 class CodeQA:
-    CODE_QA_FOLDER = "./.code_qa_data"
+    CODE_QA_FOLDER = "./.code_qa"
 
     def init(self, project_path="./"):
         token = load_openai_token()
 
         logger.info("Start loading project")
         raw_docs = load_files(project_path)
         text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
```

### Comparing `code_qa-0.2.1/code_qa/utils.py` & `code_qa-0.3.1/code_qa/utils.py`

 * *Files identical despite different names*

### Comparing `code_qa-0.2.1/pyproject.toml` & `code_qa-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "code-qa"
-version = "0.2.1"
+version = "0.3.1"
 description = "CodeQA: Unleash the power of AI in your codebase. Ask questions & get insights from your document."
 authors = ["Steven Mi <steven.mi@getyourguide.com>"]
 readme = "README.md"
 packages = [{include = "code_qa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `code_qa-0.2.1/setup.py` & `code_qa-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'tiktoken>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['code_qa = code_qa.cli:main']}
 
 setup_kwargs = {
     'name': 'code-qa',
-    'version': '0.2.1',
+    'version': '0.3.1',
     'description': 'CodeQA: Unleash the power of AI in your codebase. Ask questions & get insights from your document.',
-    'long_description': '# CodeQA\n\nCodeQA is a powerful command-line tool designed to help developers understand and navigate their codebase more efficiently. By asking questions directly about your project, you can gain insights and deepen your understanding of the codebase without the need for extensive manual exploration. CodeQA is built on top of LangChain, leveraging its capabilities to provide accurate and insightful responses.\n\nBesides code, CodeQA is engineered to be universally applicable across various text documents. It enables you to effortlessly navigate through:\n\n- PDF documents\n- Markdown files\n- And any other form of text-based documents.\n\n## Getting Started\n\nFollow these steps to install and set up CodeQA:\n\n1. **Install CodeQA**: Use pip to install CodeQA. Run the following command in your terminal:\n\n    ```bash\n    pip install code-qa\n    ```\n\n2. **Set up OpenAI Token**: CodeQA uses OpenAI\'s API to generate responses. You need to add your OpenAI token to your virtual environment. Replace `YOUR_TOKEN` with your actual OpenAI token:\n\n    ```bash\n    export OPENAI_TOKEN=YOUR_TOKEN\n    ```\n\n3. **Navigate to your project folder**: Use the `cd` command to navigate to your project\'s directory:\n\n    ```bash\n    cd PATH/TO/MY/PROJECT\n    ```\n\n4. **Initialize CodeQA Index**: This will generate a `.code_qa_data` folder within your project. The folder contains your project embeddings stored as parquet files. Run the following command:\n\n    ```bash\n    code_qa init\n    ```\n\n## Usage\n\nWith CodeQA, you can ask questions directly about your code. For example, if you want to know how to test a particular part of your code, you can ask:\n\n```bash\ncode_qa query "How can I test this?"\n```\n\n## Ignoring Files\n\nIf there are certain files or directories that you want CodeQA to ignore, you can specify them in a `.codeqaignore` file. This file follows the same syntax and rules as the `.gitignore` file. Simply create a `.codeqaignore` file in your project\'s root directory and list the files or directories you want to ignore.\n\n\n## License\n\nCodeQA is licensed under the Apache License Version 2.0. For more details, see the [LICENSE](LICENSE) file.\n',
+    'long_description': '# CodeQA\n\n**CodeQA** is a **powerful command-line tool** designed to help **developers understand and navigate their codebase**\nmore efficiently. **By asking questions** directly about your project, you can **gain insights and deepen your\nunderstanding of the codebase** without the need for extensive manual exploration. CodeQA is built on top of LangChain,\nleveraging its capabilities to provide accurate and insightful responses.\n\n**Besides code,** CodeQA is engineered to be **universally applicable across various text documents**. It enables you to\neffortlessly navigate through:\n\n- PDF documents\n- Markdown files\n- And any other form of text-based documents.\n\n## Getting Started\n\nFollow these steps to install and set up CodeQA:\n\n1. **Install CodeQA**: Use pip to install CodeQA. Run the following command in your terminal:\n\n    ```bash\n    pip install code-qa\n    ```\n\n2. **Set up OpenAI Token**: CodeQA uses OpenAI\'s API to generate responses. You need to add your OpenAI token to your\n   virtual environment. Replace `YOUR_TOKEN` with your actual OpenAI token:\n\n    ```bash\n    export OPENAI_TOKEN=YOUR_TOKEN\n    ```\n\n3. **Navigate to your project folder**: Use the `cd` command to navigate to your project\'s directory:\n\n    ```bash\n    cd PATH/TO/MY/PROJECT\n    ```\n\n4. **Initialize CodeQA Index**: This will generate a `.code_qa` folder within your project. The folder contains your\n   project embeddings stored as parquet files. Run the following command:\n\n    ```bash\n    code_qa init\n    ```\n\n## Usage\n\nWith CodeQA, you can ask questions directly about your code. For example, if you want to know how to test a particular\npart of your code, you can ask:\n\n```bash\ncode_qa query "How can I test this?"\n```\n\n## Ignoring Files\n\nIf there are certain files or directories that you want CodeQA to ignore, you can specify them in a `.codeqaignore`\nfile. This file follows the same syntax and rules as the `.gitignore` file. Simply create a `.codeqaignore` file in your\nproject\'s root directory and list the files or directories you want to ignore.\n\n## License\n\nCodeQA is licensed under the Apache License Version 2.0. For more details, see the [LICENSE](LICENSE) file.\n',
     'author': 'Steven Mi',
     'author_email': 'steven.mi@getyourguide.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `code_qa-0.2.1/PKG-INFO` & `code_qa-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-qa
-Version: 0.2.1
+Version: 0.3.1
 Summary: CodeQA: Unleash the power of AI in your codebase. Ask questions & get insights from your document.
 Author: Steven Mi
 Author-email: steven.mi@getyourguide.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,17 +15,21 @@
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # CodeQA
 
-CodeQA is a powerful command-line tool designed to help developers understand and navigate their codebase more efficiently. By asking questions directly about your project, you can gain insights and deepen your understanding of the codebase without the need for extensive manual exploration. CodeQA is built on top of LangChain, leveraging its capabilities to provide accurate and insightful responses.
+**CodeQA** is a **powerful command-line tool** designed to help **developers understand and navigate their codebase**
+more efficiently. **By asking questions** directly about your project, you can **gain insights and deepen your
+understanding of the codebase** without the need for extensive manual exploration. CodeQA is built on top of LangChain,
+leveraging its capabilities to provide accurate and insightful responses.
 
-Besides code, CodeQA is engineered to be universally applicable across various text documents. It enables you to effortlessly navigate through:
+**Besides code,** CodeQA is engineered to be **universally applicable across various text documents**. It enables you to
+effortlessly navigate through:
 
 - PDF documents
 - Markdown files
 - And any other form of text-based documents.
 
 ## Getting Started
 
@@ -33,42 +37,46 @@
 
 1. **Install CodeQA**: Use pip to install CodeQA. Run the following command in your terminal:
 
     ```bash
     pip install code-qa
     ```
 
-2. **Set up OpenAI Token**: CodeQA uses OpenAI's API to generate responses. You need to add your OpenAI token to your virtual environment. Replace `YOUR_TOKEN` with your actual OpenAI token:
+2. **Set up OpenAI Token**: CodeQA uses OpenAI's API to generate responses. You need to add your OpenAI token to your
+   virtual environment. Replace `YOUR_TOKEN` with your actual OpenAI token:
 
     ```bash
     export OPENAI_TOKEN=YOUR_TOKEN
     ```
 
 3. **Navigate to your project folder**: Use the `cd` command to navigate to your project's directory:
 
     ```bash
     cd PATH/TO/MY/PROJECT
     ```
 
-4. **Initialize CodeQA Index**: This will generate a `.code_qa_data` folder within your project. The folder contains your project embeddings stored as parquet files. Run the following command:
+4. **Initialize CodeQA Index**: This will generate a `.code_qa` folder within your project. The folder contains your
+   project embeddings stored as parquet files. Run the following command:
 
     ```bash
     code_qa init
     ```
 
 ## Usage
 
-With CodeQA, you can ask questions directly about your code. For example, if you want to know how to test a particular part of your code, you can ask:
+With CodeQA, you can ask questions directly about your code. For example, if you want to know how to test a particular
+part of your code, you can ask:
 
 ```bash
 code_qa query "How can I test this?"
 ```
 
 ## Ignoring Files
 
-If there are certain files or directories that you want CodeQA to ignore, you can specify them in a `.codeqaignore` file. This file follows the same syntax and rules as the `.gitignore` file. Simply create a `.codeqaignore` file in your project's root directory and list the files or directories you want to ignore.
-
+If there are certain files or directories that you want CodeQA to ignore, you can specify them in a `.codeqaignore`
+file. This file follows the same syntax and rules as the `.gitignore` file. Simply create a `.codeqaignore` file in your
+project's root directory and list the files or directories you want to ignore.
 
 ## License
 
 CodeQA is licensed under the Apache License Version 2.0. For more details, see the [LICENSE](LICENSE) file.
```

