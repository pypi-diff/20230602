# Comparing `tmp/pop-llm-0.0.4.tar.gz` & `tmp/pop-llm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-llm-0.0.4.tar", last modified: Fri Jun  2 05:25:21 2023, max compression
+gzip compressed data, was "pop-llm-0.0.5.tar", last modified: Fri Jun  2 09:49:57 2023, max compression
```

## Comparing `pop-llm-0.0.4.tar` & `pop-llm-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.946389 pop-llm-0.0.4/
--rw-r--r--   0 wyb       (1000) wyb       (1000)      205 2023-06-02 03:16:11.000000 pop-llm-0.0.4/.gitignore
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 03:16:11.000000 pop-llm-0.0.4/LICENSE
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1865 2023-06-02 05:25:21.946389 pop-llm-0.0.4/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1385 2023-06-02 03:16:11.000000 pop-llm-0.0.4/README.md
--rw-r--r--   0 wyb       (1000) wyb       (1000)     8844 2023-06-02 03:16:11.000000 pop-llm-0.0.4/demo.ipynb
--rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 05:23:39.000000 pop-llm-0.0.4/pyproject.toml
--rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-02 00:09:11.000000 pop-llm-0.0.4/requirement.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 05:25:21.946389 pop-llm-0.0.4/setup.cfg
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.943055 pop-llm-0.0.4/src/
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.943055 pop-llm-0.0.4/src/pop_llm/
--rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 03:16:11.000000 pop-llm-0.0.4/src/pop_llm/__init__.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)    12589 2023-06-02 05:21:45.000000 pop-llm-0.0.4/src/pop_llm/chat_agent.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     2682 2023-06-02 05:21:45.000000 pop-llm-0.0.4/src/pop_llm/pop.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 03:16:11.000000 pop-llm-0.0.4/src/pop_llm/prompts.py
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.946389 pop-llm-0.0.4/src/pop_llm.egg-info/
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1865 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/SOURCES.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/dependency_links.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/requires.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/top_level.txt
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.735896 pop-llm-0.0.5/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      214 2023-06-02 09:19:20.000000 pop-llm-0.0.5/.gitignore
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 07:40:05.000000 pop-llm-0.0.5/LICENSE
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 09:49:57.735896 pop-llm-0.0.5/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     2571 2023-06-02 09:19:20.000000 pop-llm-0.0.5/README.md
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    13272 2023-06-02 09:32:43.000000 pop-llm-0.0.5/demo.ipynb
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 09:49:25.000000 pop-llm-0.0.5/pyproject.toml
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-01 07:43:51.000000 pop-llm-0.0.5/requirement.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 09:49:57.735896 pop-llm-0.0.5/setup.cfg
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.732563 pop-llm-0.0.5/src/
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.735896 pop-llm-0.0.5/src/pop_llm/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 07:40:05.000000 pop-llm-0.0.5/src/pop_llm/__init__.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    12718 2023-06-02 09:19:20.000000 pop-llm-0.0.5/src/pop_llm/chat_agent.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3962 2023-06-02 09:19:20.000000 pop-llm-0.0.5/src/pop_llm/pop.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 07:40:05.000000 pop-llm-0.0.5/src/pop_llm/prompts.py
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.735896 pop-llm-0.0.5/src/pop_llm.egg-info/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/requires.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/top_level.txt
```

### Comparing `pop-llm-0.0.4/LICENSE` & `pop-llm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.4/PKG-INFO` & `pop-llm-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -26,14 +26,17 @@
 Saving the key to `openai_api_key.txt` is recommended if you are using Jupyter Notebook:
 
 ```bash
 echo $OPENAI_API_KEY > openai_api_key.txt
 ```
 
 ## Usage
+
+### Getting Started
+
 You can define a "function" using natural language. Simply define a `PopFunction` with three required parameters:
 
 ```python
 from pop_llm import PopFunction
 
 # Specify the input and output parameters, and a description
 add = PopFunction(["a", "b"], ["sum"], "Add the two numbers")
@@ -60,8 +63,43 @@
     description="Add two numbers.", # The description of the task
     name = "add", # A name for the function, default to "function"
     input_assert=lambda a, b: type(a) == int and type(b) == int, # A function to assert the input
     temperature=0 # Set to 0 for deterministic, 1 for the most randomness
 )
 ```
 
+### Allowing LLM to use external tools
+
+You can provide a list of external tools. Simply define some well documented functions and pass them to `PopFunction`.
+
+The LLM Agent will automatically use these tools to help it complete the task.
+
+For example, you have a secret function:
+
+```python
+def secret_function(a: int, b: int) -> int:
+    """
+    A secret function
+    Args:
+        a: The first string
+        b: The second string
+    Returns:
+        int: The result of the secret function
+    """
+    return a * 2 + b - 1
+
+secret_function_runner = PopFunction(
+    input_keys=["a", "b"],
+    output_keys=["output"],
+    description="Return the result of the secret function on input a and b.",
+    name = "secret_function",
+    input_assert=lambda a, b: type(a) == int and type(b) == int,
+    temperature=0,
+    tools=[secret_function]
+)
+```
+
+Be creative when defining your tools. This can be a web API, a database call, reading a file, etc.
+
+Note: Your function input should be able to be parsed from JSON. The output should be able to be converted to string without loosing information. (i.e. str(output) is not something like `<object at 0x7f9c2c0b4a90>`)
+
 For more examples, please refer to the [Demo Notebook](./demo.ipynb)
```

### Comparing `pop-llm-0.0.4/demo.ipynb` & `pop-llm-0.0.5/demo.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'cells'": "{insert: [(10, OrderedDict([('attachments', OrderedDict()), ('cell_type', "*

 * *            "'markdown'), ('metadata', OrderedDict()), ('source', ['## Use external tools'])])), "*

 * *            "(11, OrderedDict([('cell_type', 'code'), ('execution_count', 4), ('metadata', "*

 * *            "OrderedDict()), ('outputs', [OrderedDict([('name', 'stdout'), ('output_type', "*

 * *            "'stream'), ('text', ['\\n', 'You are a function that strictly takes inputs from the "*

 * *            "user and return a JSON for […]*

```diff
@@ -189,14 +189,129 @@
                 "\n",
                 "print(chatbot(\"Hello, how are you?\")[\"response\"])\n",
                 "print(chatbot(\"Remember my name is John.\")[\"response\"])\n",
                 "print(chatbot(\"What is my name?\")[\"response\"])\n",
                 "chatbot.reset_history()\n",
                 "print(chatbot(\"What is my name?\")[\"response\"])"
             ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Use external tools"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "You are a function that strictly takes inputs from the user and return a JSON formatted output.\n",
+                        "Think about this step by step:\n",
+                        "1. You will be given a task description.\n",
+                        "2. You will be given a list of input keys.\n",
+                        "3. You will be given a list of output keys.\n",
+                        "4. User will give you a JSON formatted input.\n",
+                        "5. You will follow the task description to process the input.\n",
+                        "6. You will return a JSON formatted output, which contains the output keys.\n",
+                        "\n",
+                        "Rules:\n",
+                        "1. Unless you are specifically asked to write code, you should directly process the inputs and return the outputs by yourself.\n",
+                        "2. You can ONLY reply with a JSON formatted string.\n",
+                        "3. You ONLY reply with the given output keys.\n",
+                        "Your name is: tldr.\n",
+                        "Your task is described as follows:\n",
+                        "    Generate a TL;DR summary of a text.\n",
+                        "Your input keys are: \n",
+                        "[\"text\"].\n",
+                        "Your output keys are: \n",
+                        "[\"summary\"].\n",
+                        "\n",
+                        "\n",
+                        "You can use tools to help you solve the task. However, YOU MUST ask the user for permission before using a tool.\n",
+                        "After you use a tool, system will provide you the output of the tool. You should observe the output and decide what to do next.\n",
+                        "System may also provide you with error messages of your tool. You should try to fix the error and run the tool again. Think about the number of arguments you provided.\n",
+                        "Remember: always use double quotes for strings in JSON.\n",
+                        "Sometimes you need to break the task into multiple steps. Use one tool each time and observe the output. Then decide what to do next.\n",
+                        "You have the following tools to help you:\n",
+                        "Name: read_file\n",
+                        "Description: \n",
+                        "    Read the content of a file.\n",
+                        "\n",
+                        "    Args:\n",
+                        "        path (str): path to the file\n",
+                        "\n",
+                        "    Returns:\n",
+                        "        str: file content\n",
+                        "    \n",
+                        "\n",
+                        "\n",
+                        "To use a tool, respond with a JSON string with the following keys. If you don't want to use a tool, leave the value as an empty string.\n",
+                        "tool: The name of the tool to use\n",
+                        "args: The arguments to pass to the tool\n",
+                        "For example:\n",
+                        "{\"tool\": \"tool_name\", \"args\": [\"arg1\", \"arg2\"]}\n",
+                        "\n",
+                        "Using tool: \"read_file\" with args: ['README.md']\n",
+                        "POP: Prompt Oriented Programming is a Python package that allows you to define a function using natural language. You can call the function and view the raw API response. You can also provide a list of external tools to help complete the task. For more examples, please refer to the Demo Notebook.\n"
+                    ]
+                }
+            ],
+            "source": [
+                "def read_file(path: str) -> str:\n",
+                "    \"\"\"\n",
+                "    Read the content of a file.\n",
+                "\n",
+                "    Args:\n",
+                "        path (str): path to the file\n",
+                "\n",
+                "    Returns:\n",
+                "        str: file content\n",
+                "    \"\"\"\n",
+                "    with open(path, \"r\") as f:\n",
+                "        return f.read()\n",
+                "\n",
+                "# Create a function similar to the tldr function above, but with tools.\n",
+                "tldr_with_tools = PopFunction(\n",
+                "    input_keys=[\"text\"],\n",
+                "    output_keys=[\"summary\"],\n",
+                "    description=\"Generate a TL;DR summary of a text.\",\n",
+                "    name = \"tldr\",\n",
+                "    input_assert=lambda text: type(text) == str,\n",
+                "    tools=[read_file]\n",
+                ")\n",
+                "\n",
+                "print(tldr_with_tools.system_prompt)\n",
+                "\n",
+                "print(tldr_with_tools(\"Summarize README.md\")[\"summary\"])"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Sometimes the stupid GPT-3.5 will try to use a non-existent tool to complete the task. It's okay because we correct it's mistakes by providing error feedback."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "tldr_with_tools.history"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "pop",
             "language": "python",
             "name": "python3"
```

### Comparing `pop-llm-0.0.4/pyproject.toml` & `pop-llm-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pop-llm"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Yibo Wei", email="david_wyb2001@outlook.com" },
 ]
 description = "A Python library for Prompt Oriented Programming with Large Language Models"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `pop-llm-0.0.4/src/pop_llm/chat_agent.py` & `pop-llm-0.0.5/src/pop_llm/chat_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,20 @@
         self.history = history
         self.max_tokens = max_tokens
         self.model = model
         self.temperature = temperature
         if not len(self.history):
             self.history.append(OpenAIMessage("system", self.system_prompt))
         self.tools = tools
+        # Validate tools
+        for tool in self.tools:
+            if not callable(tool):
+                raise ValueError("All tools must be callable.")
+            if not tool.__doc__:
+                raise ValueError("All tools must have a docstring.")
 
     def add_message(self, message: OpenAIMessage) -> None:
         """
         Add a new message to the chatbot's history
 
         Args:
             message (Message): The message to add.
@@ -165,15 +171,15 @@
         Returns:
             str: The response content from the chatbot.
         """
         prompt_of_time = f"current datetime: {datetime.now()}, today is {datetime.now().strftime('%A')}\n"
         if len(self.output_keys):
             output_key_str = str(self.output_keys).replace("'", '"')
             prompt_of_output_format = f"Your output should be a JSON string with the following keys: {output_key_str}\n"
-        prompt = "User: " + prompt
+        prompt = "Input: " + prompt
         logging.debug(
             "Running chatbot with prompt: %s",
             prompt_of_time + prompt_of_output_format + prompt,
         )
         self.add_message(
             OpenAIMessage(role, prompt_of_time + prompt_of_output_format + prompt)
         )
@@ -187,27 +193,21 @@
                 raise ValueError("Token usage exceeded maximum tokens.")
         response = self.send_history()
         # Parse output if output keys are specified
         parsed_content = self.parse_output(response.content)
 
         # Call the tool if the output contains a tool name
         args = None
-        if (
-            parsed_content.get("tool", None) is not None
-            and parsed_content.get("tool", None) != ""
-        ):
+        if (parsed_content.get("tool", None) not in {None, ""}):
             args = parsed_content.get("args", None)
-            # Make sure args are raw strings
-            if args is not None:
-                args = [str(arg) for arg in args]
             tool_output = self.use_tool(parsed_content["tool"], args)
-            tool_output = (
-                "Tool output: "
-                + tool_output
-                + "\nWith this output, you should be able to answer the previous question.\n"
+            tool_output = f"Tool output: {tool_output}\n"
+            tool_output += (
+                "\n Observe the output and continue the conversation."
+                + "\n Do not use the tool if you are ready to complete the task."
             )
             # Run with the tool output as the prompt
             return self.run(tool_output, "system")
         return parsed_content
 
     def rerun(self, prompt: str) -> str:
         """
@@ -265,15 +265,15 @@
                 return self.parse_output(output)
         except ValueError as e:
             return parsed_output
         for key in self.output_keys:
             parsed_output[key] = output_dict.get(key, None)
         return parsed_output
 
-    def use_tool(self, tool_name: str, args: List[str]) -> str:
+    def use_tool(self, tool_name: str, args: list) -> any:
         """
         Use a tool with the chatbot
 
         Args:
             tool (str): The name of the tool to use.
             args (List[str]): The arguments to pass to the tool.
 
@@ -289,15 +289,15 @@
             if t.__name__ == tool_name:
                 tool = t
                 break
         if tool is None:
             return f"Tool {tool_name} not found. Please try a valid tool."
         # Get args
         try:
-            if args is None:
+            if args is None or len(args) == 0:
                 return tool()
             else:
                 return tool(*args)
         except Exception as e:
             return f"Error using tool {tool_name}: {str(e)}"
 
     def save_history(self, path: str = "./history.json") -> None:
```

### Comparing `pop-llm-0.0.4/src/pop_llm/prompts.py` & `pop-llm-0.0.5/src/pop_llm/prompts.py`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.4/src/pop_llm.egg-info/PKG-INFO` & `pop-llm-0.0.5/src/pop_llm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -26,14 +26,17 @@
 Saving the key to `openai_api_key.txt` is recommended if you are using Jupyter Notebook:
 
 ```bash
 echo $OPENAI_API_KEY > openai_api_key.txt
 ```
 
 ## Usage
+
+### Getting Started
+
 You can define a "function" using natural language. Simply define a `PopFunction` with three required parameters:
 
 ```python
 from pop_llm import PopFunction
 
 # Specify the input and output parameters, and a description
 add = PopFunction(["a", "b"], ["sum"], "Add the two numbers")
@@ -60,8 +63,43 @@
     description="Add two numbers.", # The description of the task
     name = "add", # A name for the function, default to "function"
     input_assert=lambda a, b: type(a) == int and type(b) == int, # A function to assert the input
     temperature=0 # Set to 0 for deterministic, 1 for the most randomness
 )
 ```
 
+### Allowing LLM to use external tools
+
+You can provide a list of external tools. Simply define some well documented functions and pass them to `PopFunction`.
+
+The LLM Agent will automatically use these tools to help it complete the task.
+
+For example, you have a secret function:
+
+```python
+def secret_function(a: int, b: int) -> int:
+    """
+    A secret function
+    Args:
+        a: The first string
+        b: The second string
+    Returns:
+        int: The result of the secret function
+    """
+    return a * 2 + b - 1
+
+secret_function_runner = PopFunction(
+    input_keys=["a", "b"],
+    output_keys=["output"],
+    description="Return the result of the secret function on input a and b.",
+    name = "secret_function",
+    input_assert=lambda a, b: type(a) == int and type(b) == int,
+    temperature=0,
+    tools=[secret_function]
+)
+```
+
+Be creative when defining your tools. This can be a web API, a database call, reading a file, etc.
+
+Note: Your function input should be able to be parsed from JSON. The output should be able to be converted to string without loosing information. (i.e. str(output) is not something like `<object at 0x7f9c2c0b4a90>`)
+
 For more examples, please refer to the [Demo Notebook](./demo.ipynb)
```

