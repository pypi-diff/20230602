# Comparing `tmp/phyloroot-0.0.2.tar.gz` & `tmp/phyloroot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phyloroot-0.0.2.tar", last modified: Fri Jun  2 14:22:14 2023, max compression
+gzip compressed data, was "phyloroot-0.1.0.tar", last modified: Fri Jun  2 20:43:26 2023, max compression
```

## Comparing `phyloroot-0.0.2.tar` & `phyloroot-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.995552 phyloroot-0.0.2/
--rw-rw-r--   0 remie     (1000) remie     (1000)     1072 2023-06-02 13:57:14.000000 phyloroot-0.0.2/LICENCE
--rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 14:22:14.995552 phyloroot-0.0.2/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)      152 2023-06-02 13:56:35.000000 phyloroot-0.0.2/README.md
--rw-rw-r--   0 remie     (1000) remie     (1000)      684 2023-06-02 14:21:09.000000 phyloroot-0.0.2/pyproject.toml
--rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-02 14:22:14.995552 phyloroot-0.0.2/setup.cfg
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.991552 phyloroot-0.0.2/src/
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.991552 phyloroot-0.0.2/src/phyloroot/
--rw-rw-r--   0 remie     (1000) remie     (1000)       23 2023-06-02 14:18:51.000000 phyloroot-0.0.2/src/phyloroot/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     5398 2023-06-02 14:09:13.000000 phyloroot-0.0.2/src/phyloroot/network_rootability.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    22349 2023-06-02 14:00:41.000000 phyloroot-0.0.2/src/phyloroot/rooting.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.995552 phyloroot-0.0.2/src/phyloroot.egg-info/
--rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)      268 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/SOURCES.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/dependency_links.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)       10 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/top_level.txt
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 20:43:26.337509 phyloroot-0.1.0/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     1072 2023-06-02 13:57:14.000000 phyloroot-0.1.0/LICENCE
+-rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 20:43:26.337509 phyloroot-0.1.0/PKG-INFO
+-rw-rw-r--   0 remie     (1000) remie     (1000)      152 2023-06-02 13:56:35.000000 phyloroot-0.1.0/README.md
+-rw-rw-r--   0 remie     (1000) remie     (1000)      741 2023-06-02 20:40:29.000000 phyloroot-0.1.0/pyproject.toml
+-rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-02 20:43:26.337509 phyloroot-0.1.0/setup.cfg
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 20:43:26.333507 phyloroot-0.1.0/src/
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 20:43:26.333507 phyloroot-0.1.0/src/phyloroot/
+-rw-rw-r--   0 remie     (1000) remie     (1000)       23 2023-06-02 14:18:51.000000 phyloroot-0.1.0/src/phyloroot/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     4254 2023-06-02 20:38:32.000000 phyloroot-0.1.0/src/phyloroot/main_cli.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)    22349 2023-06-02 14:00:41.000000 phyloroot-0.1.0/src/phyloroot/rooting.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 20:43:26.333507 phyloroot-0.1.0/src/phyloroot.egg-info/
+-rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 20:43:26.000000 phyloroot-0.1.0/src/phyloroot.egg-info/PKG-INFO
+-rw-rw-r--   0 remie     (1000) remie     (1000)      297 2023-06-02 20:43:26.000000 phyloroot-0.1.0/src/phyloroot.egg-info/SOURCES.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-02 20:43:26.000000 phyloroot-0.1.0/src/phyloroot.egg-info/dependency_links.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)       54 2023-06-02 20:43:26.000000 phyloroot-0.1.0/src/phyloroot.egg-info/entry_points.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)       10 2023-06-02 20:43:26.000000 phyloroot-0.1.0/src/phyloroot.egg-info/top_level.txt
```

### Comparing `phyloroot-0.0.2/LICENCE` & `phyloroot-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `phyloroot-0.0.2/PKG-INFO` & `phyloroot-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyloroot
-Version: 0.0.2
+Version: 0.1.0
 Summary: A package for orienting phylogenetic networks in several well-known classes.
 Author-email: Remie Janssen <remiejanssen92@gmail.com>
 Project-URL: Homepage, https://github.com/RemieJanssen/RootingNetworks
 Project-URL: Bug Tracker, https://github.com/RemieJanssen/RootingNetworks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phyloroot-0.0.2/pyproject.toml` & `phyloroot-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "networkx>=3.1",    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phyloroot"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Remie Janssen", email="remiejanssen92@gmail.com" },
 ]
 description = "A package for orienting phylogenetic networks in several well-known classes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,7 +19,10 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/RemieJanssen/RootingNetworks"
 "Bug Tracker" = "https://github.com/RemieJanssen/RootingNetworks/issues"
+
+[project.scripts]
+phyloroot = "phyloroot.main_cli:main"
```

### Comparing `phyloroot-0.0.2/src/phyloroot/network_rootability.py` & `phyloroot-0.1.0/src/phyloroot/main_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,125 @@
-from rooting import *
+from .rooting import *
 import networkx as nx
 import os
 import sys
 import csv
-
-errorInFile = False
-
-#####################################################################
-#####################################################################
-##############          Terminal arguments                ###########
-#####################################################################
-#####################################################################
-
-#Set default values
-option_out = False
-option_out_argument = ""
-option_file = False
-option_file_argument = ""
-option_class = False
-option_class_argument = ""
-option_simple = False
-option_help = False
-
-#Read the arguments
-i = 1
-while i < len(sys.argv):
-    arg= sys.argv[i]
-    if arg == "-f" or arg == "--file":
-        option_file = True
-        i+=1
-        option_file_argument = sys.argv[i]
-    if arg == "-o" or arg == "--output":
-        option_out = True
-        i+=1
-        option_out_argument = sys.argv[i]
-    if arg == "-c" or arg == "--class":
-        option_class = True
-        i+=1
-        option_class_argument = sys.argv[i]
-    if arg == "-s" or arg == "--simple":
-        option_simple = True
-    if arg == "-h" or arg == "--help":
-        option_help = True
-    i += 1
-
-
-
-#Set the class parameters corresponding to the option_class_argument
-nwClass = option_class_argument
-ClassChecker = ClassAllNetworks
-length = 1
-if nwClass == "TC":
-    ClassChecker = ClassTreeChild
-    length = 3
-elif nwClass == "SF":
-    ClassChecker = ClassStackFree
-    length = 3
-elif nwClass == "O":
-    ClassChecker = ClassOrchard
-    length = 3
-elif nwClass == "TB":
-    ClassChecker = ClassTreeBased
-    length = 2
-elif not option_class:
-    print("Error: have to choose a class!\n\n")
-    option_help = True    
-else:
-    print("Error: invalid class chosen!\n\n")
-    option_help = True
-
-
-
-#Output the help text to the terminal if no argument is given, or if the help option is chosen.
-if len(sys.argv)==1 or option_help:
-    print("Mandatory arguments:\n -f or --file followed by the input file with a list of edges. One edge per line, vertices are positive integers separated by a comma\n -c or -class followed by a class:\n   TC: tree-child\n   TB: tree-based\n   SF: stack-free\n   O: Orchard \n\nOptional arguments:\n -o or --output followed by the output file name\n -s or --simple for output only consisting of the root-edge and the reticulation nodes.")
-    sys.exit()
-
-
+import argparse
 
 
+def read_network_file(filename):
+    # Parse the network in <filename>
+    edges = []
+    with open(filename, "rt") as f:
+        reader = csv.reader(f, delimiter=",", quotechar="|")
+        for row in reader:
+            if len(row) == 2:
+                edges.append((int(row[0]), int(row[1])))
+
+    # Build the unrooted network to be oriented
+    network = nx.Graph()
+    network.add_edges_from(edges)
+    return network
+
+
+def get_class_checker_and_chain_length(nwClass):
+    """Set the class parameters corresponding to nwClass abbreviation"""
+    ClassChecker = ClassAllNetworks
+    length = 1
+    if nwClass == "TC":
+        ClassChecker = ClassTreeChild
+        length = 3
+    elif nwClass == "SF":
+        ClassChecker = ClassStackFree
+        length = 3
+    elif nwClass == "O":
+        ClassChecker = ClassOrchard
+        length = 3
+    elif nwClass == "TB":
+        ClassChecker = ClassTreeBased
+        length = 2
+    return ClassChecker, length
+
+
+def set_output(network, orientations, simple):
+    output = ""
+    if orientations:
+        rootableEdges = orientations.keys()
+        # print("rootable at: ", rootableEdges)
+        # print("not at: ", set(network.edges)-set(rootableEdges))
+        if not simple:
+            output += "The root edges, reticulations and orientations are:"
+        else:
+            output += "The orientations of the network consist of the following root edges and reticulations:\r\n"
+        for rootEdge, reticulations in orientations.items():
+            # compute the actual orientation, instead of only the retculations.
+            dinetwork = OrientationAlgorithmBinary(network, rootEdge, reticulations)
+            if not simple:
+                output += (
+                    "\r\n\r\nroot edge:\r\n   "
+                    + str(rootEdge)
+                    + "\r\nreticulations:\r\n   "
+                    + str(reticulations)
+                    + "\r\norientation:\r\n   "
+                    + str(dinetwork.edges)
+                )
+            else:
+                output += "\r\n" + str(rootEdge) + " " + str(reticulations)
+        if not simple:
+            output += "\r\n\r\nThe network cannot be rooted at the edges:"
+            for non_root in set(network.edges) - set(rootableEdges):
+                output += "\r\n" + str(non_root)
+    else:
+        output = "There is no orientation of the given network in the desired class."
+    return output
 
 
-#####################################################################
-#####################################################################
-##############             Read the input                 ###########
-#####################################################################
-#####################################################################
-
-
-
-
-#Read each line of the input file with name set by "option_file_argument"
-edges = []
-f = open("./"+option_file_argument, "rt")
-reader = csv.reader(f, delimiter=',', quotechar='|')
-for row in reader:
-    if len(row)==2:
-        edges.append((int(row[0]),int(row[1])))
-f.close()
-
-#Build the unrooted network to be oriented
-network = nx.Graph()
-network.add_edges_from(edges)
-
-
-
-#####################################################################
-#####################################################################
-##############            Find an orientation             ###########
-#####################################################################
-#####################################################################
-
-orientations = LevelStuff(network,length,ClassChecker)
-
-output = ""
-if orientations:
-    rootableEdges = orientations.keys()
-    #print("rootable at: ", rootableEdges)
-    #print("not at: ", set(network.edges)-set(rootableEdges))
-    if not option_simple:
-        output += "The root edges, reticulations and orientations are:"
+def cmd_parser():
+    parser = argparse.ArgumentParser(
+        description="finds the orientations of an undirected phylogenetic network that belong to a given class of directed networks."
+    )
+    parser.add_argument(
+        "-f",
+        "--file",
+        help="input file with an undirected phylogenetic network as a list of edges. One edge per line, vertices are positive integers separated by a comma",
+        required=True,
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        help="output file",
+    )
+    parser.add_argument(
+        "-c",
+        "--classname",
+        help="A class of networks, choose from: TC (tree-child) TB (tree-based), SF (stack-free), and O (Orchard). If not set, this will return all orientations.",
+    )
+    parser.add_argument(
+        "-s",
+        "--simple",
+        help="Use this option if you want output only consisting of the root-edge and the reticulation nodes for each orientation.",
+        action="store_true",
+    )
+    return parser.parse_args()
+
+
+def main():
+    cmd_args = cmd_parser()
+    network = read_network_file(cmd_args.file)
+    ClassChecker, length = get_class_checker_and_chain_length(cmd_args.classname)
+    orientations = LevelStuff(network, length, ClassChecker)
+    output = set_output(network, orientations, cmd_args.simple)
+
+    # write output to file or to the shell
+    if cmd_args.output:
+        with open(cmd_args.output, "w+") as f:
+            f.write("The input network was:\r\n")
+            f.write("  " + str(network.edges) + "\r\n")
+            f.write("The class is:\r\n")
+            f.write("  " + cmd_args.classname + "\r\n")
+            f.write(output)
     else:
-        output += "The orientations of the network consist of the following root edges and reticulations:\r\n"
-    for rootEdge, reticulations in orientations.items():
-        #compute the actual orientation, instead of only the retculations.
-        dinetwork = OrientationAlgorithmBinary(network,rootEdge,reticulations)
-        if not option_simple:
-            output += "\r\n\r\nroot edge:\r\n   "+str(rootEdge)+"\r\nreticulations:\r\n   "+str(reticulations)+"\r\norientation:\r\n   "+str(dinetwork.edges)
-        else:
-            output += "\r\n"+str(rootEdge)+" "+str(reticulations)
-    if not option_simple:
-        output+="\r\n\r\nThe network cannot be rooted at the edges:"
-        for non_root in set(network.edges)-set(rootableEdges):
-            output+="\r\n"+str(non_root)
-else:
-    output = "There is no orientation of the given network in the desired class."
-
-
-#####################################################################
-#####################################################################
-##############                   Output                   ###########
-#####################################################################
-#####################################################################
-
-
-#Open the output file for writing
-if option_out:
-    f= open(option_out_argument,"w+")
-    f.write("The input network was:\r\n")
-    f.write("  "+str(network.edges)+"\r\n")
-    f.write("The class is:\r\n")
-    f.write("  "+option_class_argument+"\r\n")    
-    f.write(output)
-    f.close()
-else:
-    print(output)
+        print(output)
+
 
+if __name__ == "__main__":
+    main()
```

### Comparing `phyloroot-0.0.2/src/phyloroot/rooting.py` & `phyloroot-0.1.0/src/phyloroot/rooting.py`

 * *Files identical despite different names*

### Comparing `phyloroot-0.0.2/src/phyloroot.egg-info/PKG-INFO` & `phyloroot-0.1.0/src/phyloroot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyloroot
-Version: 0.0.2
+Version: 0.1.0
 Summary: A package for orienting phylogenetic networks in several well-known classes.
 Author-email: Remie Janssen <remiejanssen92@gmail.com>
 Project-URL: Homepage, https://github.com/RemieJanssen/RootingNetworks
 Project-URL: Bug Tracker, https://github.com/RemieJanssen/RootingNetworks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

