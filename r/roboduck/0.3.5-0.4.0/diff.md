# Comparing `tmp/roboduck-0.3.5.tar.gz` & `tmp/roboduck-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roboduck-0.3.5.tar", last modified: Sat May 27 04:33:43 2023, max compression
+gzip compressed data, was "roboduck-0.4.0.tar", last modified: Fri Jun  2 06:26:35 2023, max compression
```

## Comparing `roboduck-0.3.5.tar` & `roboduck-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.5/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)    10575 2023-05-27 04:33:43.000000 roboduck-0.3.5/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)    10346 2023-05-27 04:23:03.000000 roboduck-0.3.5/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.5/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-05-27 04:33:21.000000 roboduck-0.3.5/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.5/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.5/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.3.5/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    20180 2023-05-26 05:12:05.000000 roboduck-0.3.5/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.5/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.5/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.3.5/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.5/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.5/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.5/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.5/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.5/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6016 2023-05-25 04:05:13.000000 roboduck-0.3.5/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.5/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.5/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.3.5/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.3.5/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.3.5/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.3.5/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.5/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.5/roboduck/shell.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.5/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)    10575 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-27 04:33:43.000000 roboduck-0.3.5/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)     1181 2023-05-27 04:33:17.000000 roboduck-0.3.5/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.524701 roboduck-0.4.0/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.4.0/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)    11529 2023-06-02 06:26:35.524312 roboduck-0.4.0/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    11300 2023-05-29 21:50:53.000000 roboduck-0.4.0/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.4.0/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.517135 roboduck-0.4.0/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-02 06:25:16.000000 roboduck-0.4.0/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.519882 roboduck-0.4.0/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.4.0/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.4.0/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.4.0/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.4.0/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.4.0/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.4.0/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.4.0/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.521304 roboduck-0.4.0/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.4.0/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.4.0/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.4.0/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.4.0/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.4.0/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.4.0/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.521893 roboduck-0.4.0/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.4.0/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.523867 roboduck-0.4.0/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.4.0/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.4.0/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.4.0/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.4.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.4.0/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.4.0/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.4.0/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.519401 roboduck-0.4.0/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)    11529 2023-06-02 06:26:34.000000 roboduck-0.4.0/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-02 06:26:34.000000 roboduck-0.4.0/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-02 06:26:35.524871 roboduck-0.4.0/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)     1181 2023-05-27 04:33:17.000000 roboduck-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `roboduck-0.3.5/PKG-INFO` & `roboduck-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.3.5
+Version: 0.4.0
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -143,15 +143,15 @@
 
 To rebuild the docs locally:
 ```
 make docs
 ```
 
 ---
-Start of auto-generated file data.<br/>Last updated: 2023-04-23 20:52:09
+Start of auto-generated file data.<br/>Last updated: 2023-05-29 14:50:53
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th>File</th>
       <th>Summary</th>
       <th>Line Count</th>
@@ -159,58 +159,72 @@
       <th>Size</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>__init__.py</td>
       <td>_</td>
-      <td>5</td>
-      <td>2023-04-16 21:46:51</td>
-      <td>142.00 b</td>
+      <td>17</td>
+      <td>2023-05-26 21:33:35</td>
+      <td>548.00 b</td>
+    </tr>
+    <tr>
+      <td>config.py</td>
+      <td>Allow us to easily read from and write to roboduck's config file.<br/><br/>Roboduck creates a config file at `~/.roboduck/config.yaml`. This currently<br/>supports only two fields:<br/><br/>- `openai_api_key`: See the [Quickstart](https://hdmamin.github.io/roboduck/)<br/>for setup help.<br/><br/>- `model_name` (optional): Roboduck is configured to use gpt-3.5-turbo by<br/>default. This field lets you change that (e.g. to gpt-4). If present in the<br/>config file, this will take priority over any model_name field specified in a<br/>chat template<br/>(e.g. our [default debug prompt template](https://github.com/hdmamin/roboduck/blob/7ff904972921fd3f82b8b9fd862c4ffc7b61aee4/lib/roboduck/prompts/chat/debug.yaml#L2)).<br/>You can view valid options with `roboduck.available_models()`.<br/>You can still override the config default by manually passing a value into a<br/>function, e.g. `duck(model_name='gpt-4-32k')`.<br/><br/>You can manually edit your config file or use a command like<br/>`roboduck.update_config(model_name='gpt-4')`. Passing in a value of None<br/>(e.g. `roboduck.update_config(model_name=None)`) will delete that field from<br/>your config file.</td>
+      <td>181</td>
+      <td>2023-05-23 22:09:40</td>
+      <td>7.41 kb</td>
     </tr>
     <tr>
       <td>debug.py</td>
-      <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/># Our replacement for python's `breakpoint`.<br/>from roboduck.debug import duck<br/><br/># Broken version of bubble sort. Notice the duck() call on the second to last<br/># line.<br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums)):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1], nums[j] = nums[j], nums[j + 1]<br/>                duck()<br/>    return nums</td>
-      <td>424</td>
-      <td>2023-04-16 21:52:28</td>
-      <td>18.17 kb</td>
+      <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/>Here's a broken version of bubble sort that places a `duck()` call on the<br/>second to last line where you might normally call `breakpoint()`.<br/><br/>```<br/>from roboduck import duck<br/><br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums) - 1):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1] = nums[j]<br/>                nums[j] = nums[j + 1]<br/>                duck()   # &lt;--------------------------- instead of breakpoint()<br/>    return nums<br/><br/>nums = [3, 1, 9, 2, 1]<br/>bubble_sort(nums)<br/>```</td>
+      <td>486</td>
+      <td>2023-05-25 22:14:45</td>
+      <td>20.18 kb</td>
+    </tr>
+    <tr>
+      <td>decorators.py</td>
+      <td>Miscellaneous decorators used throughout the library.</td>
+      <td>287</td>
+      <td>2023-05-21 22:59:59</td>
+      <td>10.26 kb</td>
     </tr>
     <tr>
       <td>errors.py</td>
-      <td>Errors that explain themselves! Or more precisely, that are explained to you<br/>by a gpt-esque model. Simply importing this module will change python's default<br/>behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/># After this import, error explanations are automatically enabled.<br/>from roboduck import errors<br/><br/># Go back to python's regular behavior on errors.<br/>errors.disable()<br/><br/># You can use `enable` to change settings or manually re-enable gpt<br/># explanations. By default, we ask the user if they want an explanation after<br/># each error (y/n). Setting auto=True skips this step and always explains<br/># errors (not recommended in most cases, but it's an option).<br/>errors.enable(auto=True)</td>
-      <td>225</td>
-      <td>2023-04-12 21:48:03</td>
-      <td>9.27 kb</td>
+      <td>Errors that explain themselves! Or more precisely, errors that are explained<br/>to you by a gpt-esque model. Simply importing this module will change python's<br/>default behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/>Importing the errors module automatically enables optional error explanations.<br/>`disable()` reverts to python's regular behavior on errors. `enable()` can be<br/>used to re-enable error explanations or to change settings. For example,<br/>setting auto=True automatically explains all errors rather than asking the user<br/>if they want an explanation (y/n) when an error occurs.<br/>```<br/>from roboduck import errors<br/><br/>data = {'x': 0}<br/>y = data.x<br/><br/>errors.disable()<br/>y = data.x<br/><br/>errors.enable(auto=True)<br/>y = data.x<br/>```</td>
+      <td>276</td>
+      <td>2023-05-28 21:41:30</td>
+      <td>11.35 kb</td>
     </tr>
     <tr>
-      <td>logging.py</td>
-      <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>from roboduck import logging<br/><br/>logger = logging.getLogger()</td>
-      <td>118</td>
-      <td>2023-04-14 21:55:16</td>
-      <td>4.75 kb</td>
+      <td>ipy_utils.py</td>
+      <td>Functions related to loading, saving, or otherwise working with ipython<br/>sessions or jupyter notebooks.</td>
+      <td>186</td>
+      <td>2023-05-24 21:37:48</td>
+      <td>5.70 kb</td>
     </tr>
     <tr>
-      <td>magic.py</td>
-      <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/># cell 1<br/>from roboduck import magic<br/><br/># cell 2<br/>nums = [1, 2, 3]<br/>nums.add(4)<br/><br/># cell 3<br/>%duck</td>
-      <td>134</td>
-      <td>2023-04-13 22:05:19</td>
-      <td>5.46 kb</td>
+      <td>logging.py</td>
+      <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>```<br/>from roboduck import logging<br/><br/>logger = logging.getLogger(path='/tmp/log.txt')<br/>data = {'x': 0}<br/>try:<br/>    x = data.x<br/>except Exception as e:<br/>    logger.error(e)<br/>```</td>
+      <td>157</td>
+      <td>2023-05-18 22:25:48</td>
+      <td>6.28 kb</td>
     </tr>
     <tr>
-      <td>shell.py</td>
-      <td>This module allows our roboduck `%duck` magic to work in ipython. Ipython<br/>uses a TerminalInteractiveShell class which makes its debugger_cls attribute<br/>read only. We provide a drop-in replacement that allows our magic class to<br/>set that attribute when necessary. Note that you'd need to start an ipython<br/>session with the command:<br/><br/>```<br/>ipython --TerminalIPythonApp.interactive_shell_class=roboduck.shell.RoboDuckTerminalInteractiveShell<br/>```<br/><br/>for this to work. You'll still need to run `from roboduck import magic` inside<br/>your session to make it avaialble.<br/><br/>Alternatively, you can make it available automatically for all ipython<br/>sessions by adding the following lines to your ipython config (usually found at<br/>~/.ipython/profile_default/ipython_config.py):<br/><br/>```<br/>cfg = get_config()<br/>cfg.TerminalIPythonApp.interactive_shell_class = roboduck.shell.RoboDuckTerminalInteractiveShell<br/>cfg.InteractiveShellApp.exec_lines = ["from roboduck import magic"]<br/>```</td>
-      <td>34</td>
-      <td>2023-03-20 21:20:45</td>
-      <td>1.31 kb</td>
+      <td>magic.py</td>
+      <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/>```<br/># cell 1<br/>from roboduck import magic<br/><br/>nums = [1, 2, 3]<br/>nums.add(4)<br/>```<br/><br/>```<br/># cell 2<br/>%duck<br/>```</td>
+      <td>126</td>
+      <td>2023-05-28 21:41:30</td>
+      <td>5.11 kb</td>
     </tr>
     <tr>
       <td>utils.py</td>
       <td>Utility functions used by other roboduck modules.</td>
-      <td>599</td>
-      <td>2023-04-21 23:15:17</td>
-      <td>21.12 kb</td>
+      <td>420</td>
+      <td>2023-05-27 21:32:29</td>
+      <td>15.14 kb</td>
     </tr>
   </tbody>
 </table>
 <br/>End of auto-generated file data. Do not add anything below this.
```

### Comparing `roboduck-0.3.5/README.md` & `roboduck-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 To rebuild the docs locally:
 ```
 make docs
 ```
 
 ---
-Start of auto-generated file data.<br/>Last updated: 2023-04-23 20:52:09
+Start of auto-generated file data.<br/>Last updated: 2023-05-29 14:50:53
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th>File</th>
       <th>Summary</th>
       <th>Line Count</th>
@@ -149,56 +149,70 @@
       <th>Size</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>__init__.py</td>
       <td>_</td>
-      <td>5</td>
-      <td>2023-04-16 21:46:51</td>
-      <td>142.00 b</td>
+      <td>17</td>
+      <td>2023-05-26 21:33:35</td>
+      <td>548.00 b</td>
+    </tr>
+    <tr>
+      <td>config.py</td>
+      <td>Allow us to easily read from and write to roboduck's config file.<br/><br/>Roboduck creates a config file at `~/.roboduck/config.yaml`. This currently<br/>supports only two fields:<br/><br/>- `openai_api_key`: See the [Quickstart](https://hdmamin.github.io/roboduck/)<br/>for setup help.<br/><br/>- `model_name` (optional): Roboduck is configured to use gpt-3.5-turbo by<br/>default. This field lets you change that (e.g. to gpt-4). If present in the<br/>config file, this will take priority over any model_name field specified in a<br/>chat template<br/>(e.g. our [default debug prompt template](https://github.com/hdmamin/roboduck/blob/7ff904972921fd3f82b8b9fd862c4ffc7b61aee4/lib/roboduck/prompts/chat/debug.yaml#L2)).<br/>You can view valid options with `roboduck.available_models()`.<br/>You can still override the config default by manually passing a value into a<br/>function, e.g. `duck(model_name='gpt-4-32k')`.<br/><br/>You can manually edit your config file or use a command like<br/>`roboduck.update_config(model_name='gpt-4')`. Passing in a value of None<br/>(e.g. `roboduck.update_config(model_name=None)`) will delete that field from<br/>your config file.</td>
+      <td>181</td>
+      <td>2023-05-23 22:09:40</td>
+      <td>7.41 kb</td>
     </tr>
     <tr>
       <td>debug.py</td>
-      <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/># Our replacement for python's `breakpoint`.<br/>from roboduck.debug import duck<br/><br/># Broken version of bubble sort. Notice the duck() call on the second to last<br/># line.<br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums)):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1], nums[j] = nums[j], nums[j + 1]<br/>                duck()<br/>    return nums</td>
-      <td>424</td>
-      <td>2023-04-16 21:52:28</td>
-      <td>18.17 kb</td>
+      <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/>Here's a broken version of bubble sort that places a `duck()` call on the<br/>second to last line where you might normally call `breakpoint()`.<br/><br/>```<br/>from roboduck import duck<br/><br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums) - 1):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1] = nums[j]<br/>                nums[j] = nums[j + 1]<br/>                duck()   # &lt;--------------------------- instead of breakpoint()<br/>    return nums<br/><br/>nums = [3, 1, 9, 2, 1]<br/>bubble_sort(nums)<br/>```</td>
+      <td>486</td>
+      <td>2023-05-25 22:14:45</td>
+      <td>20.18 kb</td>
+    </tr>
+    <tr>
+      <td>decorators.py</td>
+      <td>Miscellaneous decorators used throughout the library.</td>
+      <td>287</td>
+      <td>2023-05-21 22:59:59</td>
+      <td>10.26 kb</td>
     </tr>
     <tr>
       <td>errors.py</td>
-      <td>Errors that explain themselves! Or more precisely, that are explained to you<br/>by a gpt-esque model. Simply importing this module will change python's default<br/>behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/># After this import, error explanations are automatically enabled.<br/>from roboduck import errors<br/><br/># Go back to python's regular behavior on errors.<br/>errors.disable()<br/><br/># You can use `enable` to change settings or manually re-enable gpt<br/># explanations. By default, we ask the user if they want an explanation after<br/># each error (y/n). Setting auto=True skips this step and always explains<br/># errors (not recommended in most cases, but it's an option).<br/>errors.enable(auto=True)</td>
-      <td>225</td>
-      <td>2023-04-12 21:48:03</td>
-      <td>9.27 kb</td>
+      <td>Errors that explain themselves! Or more precisely, errors that are explained<br/>to you by a gpt-esque model. Simply importing this module will change python's<br/>default behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/>Importing the errors module automatically enables optional error explanations.<br/>`disable()` reverts to python's regular behavior on errors. `enable()` can be<br/>used to re-enable error explanations or to change settings. For example,<br/>setting auto=True automatically explains all errors rather than asking the user<br/>if they want an explanation (y/n) when an error occurs.<br/>```<br/>from roboduck import errors<br/><br/>data = {'x': 0}<br/>y = data.x<br/><br/>errors.disable()<br/>y = data.x<br/><br/>errors.enable(auto=True)<br/>y = data.x<br/>```</td>
+      <td>276</td>
+      <td>2023-05-28 21:41:30</td>
+      <td>11.35 kb</td>
     </tr>
     <tr>
-      <td>logging.py</td>
-      <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>from roboduck import logging<br/><br/>logger = logging.getLogger()</td>
-      <td>118</td>
-      <td>2023-04-14 21:55:16</td>
-      <td>4.75 kb</td>
+      <td>ipy_utils.py</td>
+      <td>Functions related to loading, saving, or otherwise working with ipython<br/>sessions or jupyter notebooks.</td>
+      <td>186</td>
+      <td>2023-05-24 21:37:48</td>
+      <td>5.70 kb</td>
     </tr>
     <tr>
-      <td>magic.py</td>
-      <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/># cell 1<br/>from roboduck import magic<br/><br/># cell 2<br/>nums = [1, 2, 3]<br/>nums.add(4)<br/><br/># cell 3<br/>%duck</td>
-      <td>134</td>
-      <td>2023-04-13 22:05:19</td>
-      <td>5.46 kb</td>
+      <td>logging.py</td>
+      <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>```<br/>from roboduck import logging<br/><br/>logger = logging.getLogger(path='/tmp/log.txt')<br/>data = {'x': 0}<br/>try:<br/>    x = data.x<br/>except Exception as e:<br/>    logger.error(e)<br/>```</td>
+      <td>157</td>
+      <td>2023-05-18 22:25:48</td>
+      <td>6.28 kb</td>
     </tr>
     <tr>
-      <td>shell.py</td>
-      <td>This module allows our roboduck `%duck` magic to work in ipython. Ipython<br/>uses a TerminalInteractiveShell class which makes its debugger_cls attribute<br/>read only. We provide a drop-in replacement that allows our magic class to<br/>set that attribute when necessary. Note that you'd need to start an ipython<br/>session with the command:<br/><br/>```<br/>ipython --TerminalIPythonApp.interactive_shell_class=roboduck.shell.RoboDuckTerminalInteractiveShell<br/>```<br/><br/>for this to work. You'll still need to run `from roboduck import magic` inside<br/>your session to make it avaialble.<br/><br/>Alternatively, you can make it available automatically for all ipython<br/>sessions by adding the following lines to your ipython config (usually found at<br/>~/.ipython/profile_default/ipython_config.py):<br/><br/>```<br/>cfg = get_config()<br/>cfg.TerminalIPythonApp.interactive_shell_class = roboduck.shell.RoboDuckTerminalInteractiveShell<br/>cfg.InteractiveShellApp.exec_lines = ["from roboduck import magic"]<br/>```</td>
-      <td>34</td>
-      <td>2023-03-20 21:20:45</td>
-      <td>1.31 kb</td>
+      <td>magic.py</td>
+      <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/>```<br/># cell 1<br/>from roboduck import magic<br/><br/>nums = [1, 2, 3]<br/>nums.add(4)<br/>```<br/><br/>```<br/># cell 2<br/>%duck<br/>```</td>
+      <td>126</td>
+      <td>2023-05-28 21:41:30</td>
+      <td>5.11 kb</td>
     </tr>
     <tr>
       <td>utils.py</td>
       <td>Utility functions used by other roboduck modules.</td>
-      <td>599</td>
-      <td>2023-04-21 23:15:17</td>
-      <td>21.12 kb</td>
+      <td>420</td>
+      <td>2023-05-27 21:32:29</td>
+      <td>15.14 kb</td>
     </tr>
   </tbody>
 </table>
 <br/>End of auto-generated file data. Do not add anything below this.
```

### Comparing `roboduck-0.3.5/roboduck/__init__.py` & `roboduck-0.4.0/roboduck/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roboduck.debug import duck, DuckDB, CodeCompletionCache
 from roboduck.langchain.chat import Chat, DummyChatModel
 from roboduck.config import update_config, load_config, set_openai_api_key
 from roboduck.ipy_utils import is_colab
 from roboduck.utils import available_models
 
 
-__version__ = '0.3.5'
+__version__ = '0.4.0'
 set_openai_api_key()
 if is_colab():
     warnings.warn(
         'It looks like you\'re using Google Colab, which may make your '
         'roboduck experience slightly sub-optimal (e.g. typing can be a bit '
         'laggy).'
     )
```

### Comparing `roboduck-0.3.5/roboduck/cli/cli.py` & `roboduck-0.4.0/roboduck/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,38 +5,15 @@
 import error caused by logging.py name collision with standard library.
 """
 import argparse
 import ast
 from pathlib import Path
 import subprocess
 
-
-def make_import_statement(cls_name):
-    """Given a class name like 'roboduck.debug.DuckDB', construct the import
-    statement (str) that should likely be used to import that class (in this
-    case 'from roboduck.debug import DuckDB'.
-
-    Parameters
-    ----------
-    cls_name : str
-        Class name including module (essentially __qualname__?), e.g.
-        roboduck.DuckDB. (Note that this would need to be roboduck.debug.DuckDB
-        if we didn't include DuckDB in roboduck's __init__.py.)
-
-    Returns
-    -------
-    str
-        E.g. "from roboduck import DuckDB"
-    """
-    parts = cls_name.split('.')
-    if len(parts) == 1:
-        return f'import {parts[0]}'
-    else:
-        lib = '.'.join(parts[:-1])
-        return f'from {lib} import {parts[-1]}'
+from roboduck.utils import make_import_statement
 
 
 def run():
     """Execute a python script with auto error mode enabled.
 
     Run a python script with roboduck's errors mode
     automatically enabled.
@@ -44,15 +21,15 @@
     Examples
     --------
     Make sure to include the equals sign between option name and value.
     If using a custom chat_class, the full name must be provided.
 
     ```
     duck my_script.py
-    duck my_script.py --chat_class=roboduck.DummyChatClass
+    duck my_script.py --chat_class=roboduck.DummyChatModel
     duck my_script.py --auto=True --prompt_name=~/my_custom_prompt.yaml
     ```
     """
     parser = argparse.ArgumentParser(
         description=run.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter
     )
```

### Comparing `roboduck-0.3.5/roboduck/config.py` & `roboduck-0.4.0/roboduck/config.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/debug.py` & `roboduck-0.4.0/roboduck/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,23 @@
     return nums
 
 nums = [3, 1, 9, 2, 1]
 bubble_sort(nums)
 ```
 """
 import cmd
+from contextlib import contextmanager, redirect_stdout
 from functools import partial
+import io
 import inspect
 import ipynbname
 from langchain.callbacks.base import CallbackManager
 from pdb import Pdb
 import sys
+import uuid
 import warnings
 
 from roboduck.langchain.chat import Chat
 from roboduck.langchain.callbacks import LiveTypingCallbackHandler
 from roboduck.utils import type_annotated_dict_str, colored, truncated_repr, \
     colordiff_new_str, \
     parse_completion
@@ -50,25 +53,83 @@
     b. allows us to easily reset all defaults
 
     The magic only needs to access it in Paste mode (-p flag) to insert
     the fixed code snippet into a new code cell.
     """
 
     # LLM full completion.
-    last_completion = ''
+    last_completion = []
     # LLM natural language explanation.
-    last_explanation = ''
+    last_explanation = []
     # User code snippet.
-    last_code = ''
+    last_code = []
     # LLM generated code.
-    last_new_code = ''
+    last_new_code = []
     # LLM generated code with new bits highlighted (print to render correctly).
-    last_code_diff = ''
-    # Allows storing extra values when passing a custom parse_func to DuckDB.
-    last_extra = {}
+    last_code_diff = []
+    # Technically tied to the DuckDB instance, but in roboduck a new instance
+    # is created for each session. We only store one value here rather than a
+    # list because it will be the same for every turn in the session.
+    last_session_id = ''
+    # List of dicts. Allows storing extra values when passing a
+    # custom parse_func to DuckDB.
+    last_extra = []
+
+    @classmethod
+    def update_cache(cls, **kwargs):
+        for k, v in kwargs.items():
+            cache = getattr(cls, k)
+            if isinstance(cache, list):
+                cache.append(v)
+            elif isinstance(cache, str):
+                setattr(cls, k, v)
+            else:
+                raise ValueError(
+                    'Roboduck encountered an unexpected value in '
+                    f'CodeCompletionCache: attr {k} has type {type(cache)},'
+                    f'expected str or list.'
+                )
+
+    @classmethod
+    def get(cls, name, newest=True):
+        """Get the first/last truthy value of a given attribute if one exists,
+        e.g. the most recent code completion.
+
+        Parameters
+        ----------
+        name : str
+            Attribute name. Should be a class attribute like 'last_code'.
+        newest : bool
+            Determines whether to get the first (newest=False) or last
+            (newest=True) truthy value.
+
+        Returns
+        -------
+        any
+            The first/last truthy value of the requested class attribute. If
+            no truthy values are found, we return None.
+
+        Examples
+        --------
+        ```
+        # Get the most recent LLM response.
+        CodeCompletionCache.get('last_completion')
+        ```
+        """
+        if not hasattr(cls, name):
+            raise AttributeError(f'{cls.__name__} has no attribute {name}.')
+
+        items = getattr(cls, name)
+        if isinstance(items, (list, tuple)):
+            if newest:
+                items = items[::-1]
+            for val in items:
+                if val:
+                    return val
+        return items or None
 
 
 class DuckDB(Pdb):
     """Conversational debugger powered by LLM (e.g. gpt-3.5-turbo or gpt-4).
     Once you're in a debugging session, regular pdb commands will work as usual
     but any user command containing a question mark will be interpreted as a
     question for the lLM. Prefixing your question with "[dev]" will print out
@@ -151,14 +212,18 @@
         self.full_context = 'full_code' in self.field_names()
         self.prompt_name = prompt_name
         self.repr_func = partial(truncated_repr, max_len=max_len_per_var)
         self.silent = silent
         self.parse_func = parse_func
         # This gets updated every time the user asks a question.
         self.prev_kwargs_hash = None
+        # This can generally be treated as a session ID since roboduck always
+        # creates a new debugger object for each session. It lets us know when
+        # to clear the CodeCompletionCache.
+        self.uuid = str(uuid.uuid1())
 
     def _chat_prompt_keys(self):
         """Retrieve default and backup user reply prompt keys (names) from
         self.chat object. If the prompt template has only one reply type,
         the backup key will equal the default key.
         """
         keys = list(self.chat.user_templates)
@@ -172,14 +237,31 @@
                     'user replies. This is not recommended because it\'s '
                     'not clear how to determine which reply type to use. We '
                     'arbitrarily choose the first non-default key as the '
                     f'backup reply type ("{backup}").'
                 )
         return default, backup
 
+    def error(self, line):
+        """Add a hint when displaying errors that roboduck only responds to
+        *questions* in natural language.
+
+        Parameters
+        ----------
+        line : str
+        """
+        super().error(line)
+        if any(term in line for term in ('SyntaxError', 'NameError')):
+            print(
+                '*** If you meant to respond to Duck in natural language, '
+                'remember that it only provides English responses to '
+                'questions. Statements are evaluated as Pdb commands.',
+                file=self.stdout
+            )
+
     def field_names(self, key=''):
         """Get names of variables that are expected to be passed into default
         user prompt template.
 
         Parameters
         ----------
         key : str
@@ -412,29 +494,32 @@
             # This is intentionally nested in if statement because if answer is
             # truthy, we will have already printed it via our callback if not
             # in silent mode.
             if not self.silent:
                 print(colored(answer, self.color))
 
         parsed_kwargs = self.parse_func(answer)
-        # When using the `duck` jupyter magic in "insert" mode, we reference
-        # the CodeCompletionCache to populate the new code cell.
-        CodeCompletionCache.last_completion = answer
-        CodeCompletionCache.last_explanation = parsed_kwargs['explanation']
+        if CodeCompletionCache.last_session_id != self.uuid:
+            CodeCompletionCache.reset_class_vars()
+
         # Built-in prompts always ask for a fixed version of the relevant
         # snippet, not the whole code, so that's what we store here and use for
-        # the diff operation.
-        # Contextless prompt has no `code` key.
+        # the diff operation. Contextless prompt has no `code` key, hence the
+        # `get` usage.
         old_code = prompt_kwargs.get('code', '')
         new_code = parsed_kwargs['code']
-        CodeCompletionCache.last_code_diff = colordiff_new_str(old_code,
-                                                               new_code)
-        CodeCompletionCache.last_code = old_code
-        CodeCompletionCache.last_new_code = new_code
-        CodeCompletionCache.last_extra = parsed_kwargs.get('extra', {})
+        CodeCompletionCache.update_cache(
+            last_completion=answer,
+            last_explanation=parsed_kwargs['explanation'],
+            last_code_diff=colordiff_new_str(old_code, new_code),
+            last_code=old_code,
+            last_new_code=new_code,
+            last_extra=parsed_kwargs.get('extra', {}),
+            last_session_id=self.uuid
+        )
         self.prev_kwargs_hash = kwargs_hash
 
     def precmd(self, line):
         """We need to define this to make our errors module work. Our
         post_mortem function sometimes places a tuple in our debugger's
         cmdqueue and precmd is called as part of the default cmdloop method.
         Technically it calls postcmd too but we don't need to override that
```

### Comparing `roboduck-0.3.5/roboduck/decorators.py` & `roboduck-0.4.0/roboduck/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Miscellaneous decorators used throughout the library."""
-import warnings
+from copy import deepcopy
 from functools import partial, wraps
-from inspect import signature, Parameter
+from inspect import signature, Parameter, getmembers, isroutine
+import warnings
 
 
 def typecheck(func_=None, **types):
     """Decorator to enforce type checking for a function or method. There are
     two ways to call this: either explicitly passing argument types to the
     decorator, or letting it infer them using type annotations in the function
     that will be decorated. We allow both usage methods since older
@@ -183,18 +184,33 @@
         # because otherwise we could provide no kwargs and _func wouldn't
         # complain. Just use generic type because we only care that a value is
         # provided.
         wrapper = typecheck(wrapper, **{f: object for f in fields})
     return wrapper
 
 
+def _classvars(cls):
+    """Get class variable nnames and values for a given class.
+
+    Parameters
+    ----------
+    cls : type
+
+    Returns
+    -------
+    dict[str, any]
+    """
+    return dict(getmembers(cls, lambda x: not(isroutine(x))))
+
+
 def store_class_defaults(cls=None, attr_filter=None):
     """Class decorator that stores default values of class attributes (can be
     all or a subset). Default here refers to the value at class definition
-    time.
+    time. Mutable defaults should be okay since we deepcopy them, but are
+    probably still riskier to use than immutable defaults.
 
     Examples
     --------
     ```
     @store_class_defaults(attr_filter=lambda x: x.startswith('last_'))
     class Foo:
         last_bar = 3
@@ -220,19 +236,21 @@
             f'cls arg in store_class_defaults decorator has type {type(cls)} '
             f'but expected type `type`, i.e. a class. You may be passing in '
             f'an attr_filter as a positional arg which is not allowed - it '
             f'must be a named arg if provided.'
         )
     if not attr_filter:
         def attr_filter(x):
-            return True
+            # Usually returns True, just False for some magic methods that are
+            # not easily filtered out otherwise.
+            return not (x.startswith('__') and x.endswith('__'))
     defaults = {}
-    for k, v in vars(cls).items():
+    for k, v in _classvars(cls).items():
         if attr_filter(k):
-            defaults[k] = v
+            defaults[k] = deepcopy(v)
 
     name = '_class_defaults'
     if hasattr(cls, name):
         raise AttributeError(
             f'Class {cls} already has attribute {name}. store_class_defaults '
             'decorator would overwrite that. Exiting.'
         )
```

### Comparing `roboduck-0.3.5/roboduck/errors.py` & `roboduck-0.4.0/roboduck/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         'debug' and will warn if it doesn't.
     colordiff : bool
         If True, the new code snippet in the exception will print new
         parts in green.
     interactive : bool
         If False, LLM will just explain the error and exit. If True, user
         instead will be thrown into an interactive debugging session where
-        they can ask followup questions.
+        they can ask followup questions (the first LLM response will still be
+        automatic though).
     kwargs : any
         Additional kwargs to pass to debugger class constructor. The docstring
         of the default class is included below for reference.
     """
     if t is None:
         t = sys.exc_info()[2]
         assert t is not None, "post_mortem outside of exception context"
@@ -98,19 +99,22 @@
     else:
         p.cmdqueue.insert(1, 'q')
     p.interaction(None, t)
 
     # Make gpt explanation available as part of last error message,
     # accessible via sys.last_value.
     last_value = getattr(sys, 'last_value', None)
-    if CodeCompletionCache.last_completion and last_value:
-        code_name = 'last_code_diff' if colordiff else 'last_new_code'
+    last_completion = CodeCompletionCache.get('last_completion')
+    if last_completion and last_value:
+        # Logging often eschews code-diffing because it doesn't render in file.
+        last_code = CodeCompletionCache.get(
+            'last_code_diff' if colordiff else 'last_new_code'
+        )
         last_value.args = tuple(
-            arg if i else f'{arg}\n\n{CodeCompletionCache.last_explanation}'
-                          f'\n\n{getattr(CodeCompletionCache, code_name)}'
+            arg if i else f'{arg}\n\n{last_completion}\n\n{last_code}'
             for i, arg in enumerate(last_value.args)
         )
 
 
 def print_exception(etype, value, tb, limit=None, file=None, chain=True):
     """Replacement for traceback.print_exception() that returns the
     whole stack trace as a single string. Used in roboduck's custom excepthook
```

### Comparing `roboduck-0.3.5/roboduck/ipy_utils.py` & `roboduck-0.4.0/roboduck/ipy_utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/langchain/callbacks.py` & `roboduck-0.4.0/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/langchain/chat.py` & `roboduck-0.4.0/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/langchain/utils.py` & `roboduck-0.4.0/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/logging.py` & `roboduck-0.4.0/roboduck/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         ----------
         name : str
             Same as base logger name arg.
         colordiff : bool
             Another kwarg to pass to our excepthook function. This is separate
             from the others because we want to use a different default than the
             function has since we often log to a file, in which case
-            colordiff=True may be undesirable.
+            colordiff=True may be undesirable since color is only visible when
+            printed.
         fmt : str
             Defines logging format. The default format produces output like
             this when an error is logged:
             2023-03-08 19:20:52,514 [ERROR]: list indices must be integers or
             slices, not tuple
         stdout : bool
             If True, logged items will appear in stdout. You are free to log
```

### Comparing `roboduck-0.3.5/roboduck/magic.py` & `roboduck-0.4.0/roboduck/magic.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 
 ```
 # cell 2
 %duck
 ```
 """
 
-from functools import partial
 from IPython import get_ipython
 from IPython.core.magic import line_magic, magics_class, Magics
 from IPython.core.magic_arguments import argument, magic_arguments, \
     parse_argstring
 import sys
 import warnings
 
-from roboduck.debug import DuckDB, CodeCompletionCache
+from roboduck.debug import CodeCompletionCache
 from roboduck.ipy_utils import is_colab
 
 
 @magics_class
 class DebugMagic(Magics):
     """Enter a conversational debugging session after an error is thrown by a
     jupyter notebook code cell.
@@ -60,15 +59,20 @@
 
     %duck -ip
     """
 
     @magic_arguments()
     @argument('-p', action='store_true',
               help='Boolean flag: if provided, try to PASTE a solution into a '
-                   'new code cell below.')
+                   'new code cell below. If you also choose to use '
+                   'interactive mode and receive multiple replies containing '
+                   'code snippets, the last snippet to be generated will be '
+                   'the one that is pasted in (we make the assumption that '
+                   'users will prompt for increasingly correct code rather '
+                   'than the reverse).')
     @argument('-i', action='store_true',
               help='Boolean flag: if provided, use INTERACTIVE mode. Start a '
                    'conversational debugger session and allow the user to ask '
                    'custom questions, just as they would if using '
                    'roboduck.debug.duck(). The default mode, meanwhile, '
                    'simply asks gpt what caused the error that just '
                    'occurred and then exits, rather than lingering in a '
@@ -77,70 +81,47 @@
     @line_magic
     def duck(self, line=''):
         """Silence warnings for a cell. The -p flag can be used to make the
         change persist, at least until the user changes it again.
         """
         args = parse_argstring(self.duck, line)
         if args.prompt:
-            warnings.warn('Support for custom prompts is somewhat limited - '
-                          'your prompt must use the default parse_func '
-                          '(roboduck.utils.parse_completion).')
+            warnings.warn('Support for custom prompts is somewhat limited '
+                          'at the moment - your prompt must use the default '
+                          'parse_func (roboduck.utils.parse_completion).')
         if args.p and is_colab(self.shell):
             warnings.warn('Paste mode is unavailable in google colab, which '
                           'you appear to be using. Ignoring -p flag.')
-        if args.i:
-            old_cls = self.shell.debugger_cls
-            if args.prompt:
-                new_cls = partial(DuckDB, prompt=args.prompt)
-            else:
-                new_cls = DuckDB
-            try:
-                self.shell.debugger_cls = new_cls
-            except AttributeError:
-                print(
-                    'Roboduck is unavailable in your current ipython session. '
-                    'To use it, start a new session with the command:\n\n'
-                    'ipython --TerminalIPythonApp.interactive_shell_class='
-                    'roboduck.shell.RoboDuckTerminalInteractiveShell\n\n'
-                    '(You will also need to run `from roboduck import '
-                    'magic` in the session to make the magic available.) To '
-                    'make it available automatically for all '
-                    'ipython sessions by default, add the following lines to '
-                    'your ipython config (usually found at '
-                    '~/.ipython/profile_default/ipython_config.py):\n\n'
-                    'cfg = get_config()\ncfg.TerminalIPythonApp.interactive_'
-                    'shell_class = roboduck.shell.'
-                    'RoboDuckTerminalInteractiveShell'
-                    '\ncfg.InteractiveShellApp.exec_lines = '
-                    '["from roboduck import magic"]'
-                )
-                return
-            self.shell.InteractiveTB.debugger_cls = new_cls
-            self.shell.debugger(force=True)
-            self.shell.debugger_cls = self.shell.InteractiveTB.debugger_cls = old_cls
-        else:
-            # Confine this import to this if clause rather than keeping a top
-            # level import - importing this module overwrites sys.excepthook
-            # which we don't necessarily want in most cases.
-            # Note that this uses the `debug_stack_trace` prompt by default
-            # whereas interactive mode uses `debug` by default.
-            # UPDATE: we could probably use excepthook for both cases
-            # (args.i = True or False) now that
-            # I added interactive support in the errors module. However,
-            # everything is working nicely now and I don't see a compelling
-            # reason to change things at the moment.
+        try:
+            # Confine this import to this method rather than keeping a top
+            # level import because importing this module overwrites
+            # sys.excepthook which we don't necessarily want when
+            # importing this module.
+            # Note that this uses the `debug_stack_trace` prompt by default.
+            # This does NOT include a user question param in the contextful
+            # prompt, but in this setting we only use that method once (for our
+            # automatic question) because excepthook transports us to one
+            # step before the error. The user can ask followup questions but
+            # the code state will not progress because we can't step through
+            # any further, and thus the contextless method (which does include
+            # a user question) is used from that point forward.
+            # Color should be specified because errors module uses red
+            # by default (whereas debug module uses green).
             from roboduck import errors
-            kwargs = {'auto': True, 'color': 'green'}
+            kwargs = {'auto': True, 'interactive': args.i, 'color': 'green'}
             if args.prompt:
                 kwargs['prompt'] = args.prompt
             errors.excepthook(sys.last_type, sys.last_value,
                               sys.last_traceback, **kwargs)
+        except Exception as e:
+            pass
+        finally:
             errors.disable()
 
         # Insert suggested code into next cell.
-        if args.p and CodeCompletionCache.last_completion:
-            self.shell.set_next_input(CodeCompletionCache.last_new_code,
+        if args.p and CodeCompletionCache.get('last_completion'):
+            self.shell.set_next_input(CodeCompletionCache.get('last_new_code'),
                                       replace=False)
         CodeCompletionCache.reset_class_vars()
 
 
 get_ipython().register_magics(DebugMagic)
```

### Comparing `roboduck-0.3.5/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.4.0/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/prompts/chat/debug.yaml` & `roboduck-0.4.0/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.4.0/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.4.0/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.4.0/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/prompts/utils.py` & `roboduck-0.4.0/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.5/roboduck/utils.py` & `roboduck-0.4.0/roboduck/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -388,8 +388,33 @@
     res = {}
 
     # This logic may not always hold but as of April 2023, this returns
     # openai's available chat models.
     openai_res = openai.Model.list()
     res['openai'] = [row['id'] for row in openai_res['data']
                      if row['id'].startswith('gpt')]
-    return res
+    return res
+
+
+def make_import_statement(cls_name):
+    """Given a class name like 'roboduck.debug.DuckDB', construct the import
+    statement (str) that should likely be used to import that class (in this
+    case 'from roboduck.debug import DuckDB'.
+
+    Parameters
+    ----------
+    cls_name : str
+        Class name including module (essentially __qualname__?), e.g.
+        roboduck.DuckDB. (Note that this would need to be roboduck.debug.DuckDB
+        if we didn't include DuckDB in roboduck's __init__.py.)
+
+    Returns
+    -------
+    str
+        E.g. "from roboduck import DuckDB"
+    """
+    parts = cls_name.split('.')
+    if len(parts) == 1:
+        return f'import {parts[0]}'
+    else:
+        lib = '.'.join(parts[:-1])
+        return f'from {lib} import {parts[-1]}'
```

### Comparing `roboduck-0.3.5/roboduck.egg-info/PKG-INFO` & `roboduck-0.4.0/roboduck.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.3.5
+Version: 0.4.0
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -143,15 +143,15 @@
 
 To rebuild the docs locally:
 ```
 make docs
 ```
 
 ---
-Start of auto-generated file data.<br/>Last updated: 2023-04-23 20:52:09
+Start of auto-generated file data.<br/>Last updated: 2023-05-29 14:50:53
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th>File</th>
       <th>Summary</th>
       <th>Line Count</th>
@@ -159,58 +159,72 @@
       <th>Size</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>__init__.py</td>
       <td>_</td>
-      <td>5</td>
-      <td>2023-04-16 21:46:51</td>
-      <td>142.00 b</td>
+      <td>17</td>
+      <td>2023-05-26 21:33:35</td>
+      <td>548.00 b</td>
+    </tr>
+    <tr>
+      <td>config.py</td>
+      <td>Allow us to easily read from and write to roboduck's config file.<br/><br/>Roboduck creates a config file at `~/.roboduck/config.yaml`. This currently<br/>supports only two fields:<br/><br/>- `openai_api_key`: See the [Quickstart](https://hdmamin.github.io/roboduck/)<br/>for setup help.<br/><br/>- `model_name` (optional): Roboduck is configured to use gpt-3.5-turbo by<br/>default. This field lets you change that (e.g. to gpt-4). If present in the<br/>config file, this will take priority over any model_name field specified in a<br/>chat template<br/>(e.g. our [default debug prompt template](https://github.com/hdmamin/roboduck/blob/7ff904972921fd3f82b8b9fd862c4ffc7b61aee4/lib/roboduck/prompts/chat/debug.yaml#L2)).<br/>You can view valid options with `roboduck.available_models()`.<br/>You can still override the config default by manually passing a value into a<br/>function, e.g. `duck(model_name='gpt-4-32k')`.<br/><br/>You can manually edit your config file or use a command like<br/>`roboduck.update_config(model_name='gpt-4')`. Passing in a value of None<br/>(e.g. `roboduck.update_config(model_name=None)`) will delete that field from<br/>your config file.</td>
+      <td>181</td>
+      <td>2023-05-23 22:09:40</td>
+      <td>7.41 kb</td>
     </tr>
     <tr>
       <td>debug.py</td>
-      <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/># Our replacement for python's `breakpoint`.<br/>from roboduck.debug import duck<br/><br/># Broken version of bubble sort. Notice the duck() call on the second to last<br/># line.<br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums)):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1], nums[j] = nums[j], nums[j + 1]<br/>                duck()<br/>    return nums</td>
-      <td>424</td>
-      <td>2023-04-16 21:52:28</td>
-      <td>18.17 kb</td>
+      <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/>Here's a broken version of bubble sort that places a `duck()` call on the<br/>second to last line where you might normally call `breakpoint()`.<br/><br/>```<br/>from roboduck import duck<br/><br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums) - 1):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1] = nums[j]<br/>                nums[j] = nums[j + 1]<br/>                duck()   # &lt;--------------------------- instead of breakpoint()<br/>    return nums<br/><br/>nums = [3, 1, 9, 2, 1]<br/>bubble_sort(nums)<br/>```</td>
+      <td>486</td>
+      <td>2023-05-25 22:14:45</td>
+      <td>20.18 kb</td>
+    </tr>
+    <tr>
+      <td>decorators.py</td>
+      <td>Miscellaneous decorators used throughout the library.</td>
+      <td>287</td>
+      <td>2023-05-21 22:59:59</td>
+      <td>10.26 kb</td>
     </tr>
     <tr>
       <td>errors.py</td>
-      <td>Errors that explain themselves! Or more precisely, that are explained to you<br/>by a gpt-esque model. Simply importing this module will change python's default<br/>behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/># After this import, error explanations are automatically enabled.<br/>from roboduck import errors<br/><br/># Go back to python's regular behavior on errors.<br/>errors.disable()<br/><br/># You can use `enable` to change settings or manually re-enable gpt<br/># explanations. By default, we ask the user if they want an explanation after<br/># each error (y/n). Setting auto=True skips this step and always explains<br/># errors (not recommended in most cases, but it's an option).<br/>errors.enable(auto=True)</td>
-      <td>225</td>
-      <td>2023-04-12 21:48:03</td>
-      <td>9.27 kb</td>
+      <td>Errors that explain themselves! Or more precisely, errors that are explained<br/>to you by a gpt-esque model. Simply importing this module will change python's<br/>default behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/>Importing the errors module automatically enables optional error explanations.<br/>`disable()` reverts to python's regular behavior on errors. `enable()` can be<br/>used to re-enable error explanations or to change settings. For example,<br/>setting auto=True automatically explains all errors rather than asking the user<br/>if they want an explanation (y/n) when an error occurs.<br/>```<br/>from roboduck import errors<br/><br/>data = {'x': 0}<br/>y = data.x<br/><br/>errors.disable()<br/>y = data.x<br/><br/>errors.enable(auto=True)<br/>y = data.x<br/>```</td>
+      <td>276</td>
+      <td>2023-05-28 21:41:30</td>
+      <td>11.35 kb</td>
     </tr>
     <tr>
-      <td>logging.py</td>
-      <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>from roboduck import logging<br/><br/>logger = logging.getLogger()</td>
-      <td>118</td>
-      <td>2023-04-14 21:55:16</td>
-      <td>4.75 kb</td>
+      <td>ipy_utils.py</td>
+      <td>Functions related to loading, saving, or otherwise working with ipython<br/>sessions or jupyter notebooks.</td>
+      <td>186</td>
+      <td>2023-05-24 21:37:48</td>
+      <td>5.70 kb</td>
     </tr>
     <tr>
-      <td>magic.py</td>
-      <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/># cell 1<br/>from roboduck import magic<br/><br/># cell 2<br/>nums = [1, 2, 3]<br/>nums.add(4)<br/><br/># cell 3<br/>%duck</td>
-      <td>134</td>
-      <td>2023-04-13 22:05:19</td>
-      <td>5.46 kb</td>
+      <td>logging.py</td>
+      <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>```<br/>from roboduck import logging<br/><br/>logger = logging.getLogger(path='/tmp/log.txt')<br/>data = {'x': 0}<br/>try:<br/>    x = data.x<br/>except Exception as e:<br/>    logger.error(e)<br/>```</td>
+      <td>157</td>
+      <td>2023-05-18 22:25:48</td>
+      <td>6.28 kb</td>
     </tr>
     <tr>
-      <td>shell.py</td>
-      <td>This module allows our roboduck `%duck` magic to work in ipython. Ipython<br/>uses a TerminalInteractiveShell class which makes its debugger_cls attribute<br/>read only. We provide a drop-in replacement that allows our magic class to<br/>set that attribute when necessary. Note that you'd need to start an ipython<br/>session with the command:<br/><br/>```<br/>ipython --TerminalIPythonApp.interactive_shell_class=roboduck.shell.RoboDuckTerminalInteractiveShell<br/>```<br/><br/>for this to work. You'll still need to run `from roboduck import magic` inside<br/>your session to make it avaialble.<br/><br/>Alternatively, you can make it available automatically for all ipython<br/>sessions by adding the following lines to your ipython config (usually found at<br/>~/.ipython/profile_default/ipython_config.py):<br/><br/>```<br/>cfg = get_config()<br/>cfg.TerminalIPythonApp.interactive_shell_class = roboduck.shell.RoboDuckTerminalInteractiveShell<br/>cfg.InteractiveShellApp.exec_lines = ["from roboduck import magic"]<br/>```</td>
-      <td>34</td>
-      <td>2023-03-20 21:20:45</td>
-      <td>1.31 kb</td>
+      <td>magic.py</td>
+      <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/>```<br/># cell 1<br/>from roboduck import magic<br/><br/>nums = [1, 2, 3]<br/>nums.add(4)<br/>```<br/><br/>```<br/># cell 2<br/>%duck<br/>```</td>
+      <td>126</td>
+      <td>2023-05-28 21:41:30</td>
+      <td>5.11 kb</td>
     </tr>
     <tr>
       <td>utils.py</td>
       <td>Utility functions used by other roboduck modules.</td>
-      <td>599</td>
-      <td>2023-04-21 23:15:17</td>
-      <td>21.12 kb</td>
+      <td>420</td>
+      <td>2023-05-27 21:32:29</td>
+      <td>15.14 kb</td>
     </tr>
   </tbody>
 </table>
 <br/>End of auto-generated file data. Do not add anything below this.
```

### Comparing `roboduck-0.3.5/roboduck.egg-info/SOURCES.txt` & `roboduck-0.4.0/roboduck.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 roboduck/config.py
 roboduck/debug.py
 roboduck/decorators.py
 roboduck/errors.py
 roboduck/ipy_utils.py
 roboduck/logging.py
 roboduck/magic.py
-roboduck/shell.py
 roboduck/utils.py
 roboduck.egg-info/PKG-INFO
 roboduck.egg-info/SOURCES.txt
 roboduck.egg-info/dependency_links.txt
 roboduck.egg-info/entry_points.txt
 roboduck.egg-info/requires.txt
 roboduck.egg-info/top_level.txt
```

### Comparing `roboduck-0.3.5/setup.py` & `roboduck-0.4.0/setup.py`

 * *Files identical despite different names*

