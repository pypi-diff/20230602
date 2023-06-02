# Comparing `tmp/ngrad-1.0.1.tar.gz` & `tmp/ngrad-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngrad-1.0.1.tar", last modified: Tue May 30 18:37:22 2023, max compression
+gzip compressed data, was "ngrad-1.0.2.tar", last modified: Fri Jun  2 07:15:51 2023, max compression
```

## Comparing `ngrad-1.0.1.tar` & `ngrad-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1061 2023-05-30 18:26:38.000000 ngrad-1.0.1/LICENSE
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3933 2023-05-30 18:37:22.201923 ngrad-1.0.1/PKG-INFO
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3432 2023-05-30 18:26:38.000000 ngrad-1.0.1/README.md
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/ngrad/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:04:57.000000 ngrad-1.0.1/ngrad/__init__.py
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5211 2023-05-28 18:23:58.000000 ngrad-1.0.1/ngrad/engine.py
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1896 2023-05-29 09:29:42.000000 ngrad-1.0.1/ngrad/library.py
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/ngrad.egg-info/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3933 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/PKG-INFO
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      241 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/SOURCES.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        1 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/dependency_links.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/requires.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/top_level.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)       38 2023-05-30 18:37:22.201923 ngrad-1.0.1/setup.cfg
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      727 2023-05-30 18:35:42.000000 ngrad-1.0.1/setup.py
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/test/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5098 2023-05-30 18:04:58.000000 ngrad-1.0.1/test/test_engine.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.851438 ngrad-1.0.2/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1061 2023-05-30 18:26:38.000000 ngrad-1.0.2/LICENSE
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3963 2023-06-02 07:15:51.847439 ngrad-1.0.2/PKG-INFO
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3462 2023-06-01 16:52:46.000000 ngrad-1.0.2/README.md
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.835440 ngrad-1.0.2/ngrad/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:04:57.000000 ngrad-1.0.2/ngrad/__init__.py
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5054 2023-06-02 07:10:55.000000 ngrad-1.0.2/ngrad/engine.py
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1898 2023-06-02 07:10:35.000000 ngrad-1.0.2/ngrad/library.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.847439 ngrad-1.0.2/ngrad.egg-info/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3963 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/PKG-INFO
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      241 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        1 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/requires.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/top_level.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)       38 2023-06-02 07:15:51.851438 ngrad-1.0.2/setup.cfg
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      727 2023-06-02 07:12:23.000000 ngrad-1.0.2/setup.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.847439 ngrad-1.0.2/test/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5098 2023-05-30 18:04:58.000000 ngrad-1.0.2/test/test_engine.py
```

### Comparing `ngrad-1.0.1/LICENSE` & `ngrad-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngrad-1.0.1/PKG-INFO` & `ngrad-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: ngrad
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Autograd engine and a neural network library that handle an N-dimensional array.
 Home-page: https://github.com/x0axz/ngrad
 Author: Nooh
 Author-email: x0axz@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Autograd Engine
+# Autograd Engine & Neural Network Library
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
 Andrej Karaphy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
 
 ## Blog
 
-[Building an Autograd Engine: An Illustrative and Interactive Guide](https://x0axz.com/blog/autograd.html)
+[Building Autograd Engine & Neural Network Library: An Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
 
 ## Installation
 
 ```
 pip install ngrad
```

### Comparing `ngrad-1.0.1/README.md` & `ngrad-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Autograd Engine
+# Autograd Engine & Neural Network Library
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
 Andrej Karaphy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
 
 ## Blog
 
-[Building an Autograd Engine: An Illustrative and Interactive Guide](https://x0axz.com/blog/autograd.html)
+[Building Autograd Engine & Neural Network Library: An Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
 
 ## Installation
 
 ```
 pip install ngrad
```

### Comparing `ngrad-1.0.1/ngrad/engine.py` & `ngrad-1.0.2/ngrad/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     other = other if isinstance(other, Value) else Value(other)
     
     # Create a new Value instance representing the addition operation
     out = Value(self.data + other.data, (self, other), '+')
 
     def _backward():
       # Calculate the gradients using the chain rule and update the gradients of the operands
-      self.grad = self.grad + np.multiply(1.0, out.grad)
-      other.grad = other.grad + np.multiply(1.0, out.grad)
+      self.grad = self.grad + (1.0 * out.grad)
+      other.grad = other.grad + (1.0 * out.grad)
 
     # Assign the backward function to the new Value instance
     out._backward = _backward
     return out
 
 
   def __mul__(self, other):
@@ -47,96 +47,98 @@
     other = other if isinstance(other, Value) else Value(other)
     
     # Create a new Value instance representing the multiplication operation
     out = Value(self.data * other.data, (self, other), '*')
 
     def _backward():
       # Calculate the gradients using the chain rule and update the gradients of the operands
-      self.grad = self.grad + np.multiply(other.data, out.grad)
-      other.grad = other.grad + np.multiply(self.data, out.grad)
+      self.grad = self.grad + (other.data * out.grad)
+      other.grad = other.grad + (self.data * out.grad)
 
     # Assign the backward function to the new Value instance
     out._backward = _backward
     return out
 
 
   def __pow__(self, other):
     if isinstance(other, (int, float)):
       # If the exponent is a scalar, perform element-wise power operation
       out_data = np.power(self.data, other)
       out = Value(out_data, (self,), f'**{other}')
 
       def _backward():
         # Calculate the gradients using the chain rule and update the gradients of the operand
-        self.grad = self.grad + np.multiply(np.multiply(other, np.power(self.data, other - 1)), out.grad)
+        self.grad = self.grad + ((other * np.power(self.data, other - 1)) * out.grad)
 
       out._backward = _backward
       return out
     elif isinstance(other, Value):
       # If the exponent is a Value instance, perform element-wise power operation
       out_data = np.power(self.data, other.data)
       out = Value(out_data, (self, other), f'**')
 
       def _backward():
         # Calculate the gradients using the chain rule and update the gradients of the operands
-        self.grad = self.grad + np.multiply(np.multiply(other.data, np.power(self.data, other.data - 1)), out.grad)
-        other.grad = other.grad + np.multiply(np.log(self.data), out.grad)
+        self.grad = self.grad + ((other.data * np.power(self.data * other.data - 1)) * out.grad)
+        other.grad = other.grad + (np.log(self.data) * out.grad)
 
       out._backward = _backward
       return out
     else:
       raise TypeError("Unsupported operand type(s) for **: 'Value' and '{}'".format(type(other).__name__))
 
+
   def __radd__(self, other):
     # Perform right addition by the Value instance
-    return np.add(self, other)
+    return self + other
+
 
   def __rmul__(self, other):
     # Perform right multiplication by the Value instance
-    return np.multiply(self, other)
+    return self * other
 
 
   def __truediv__(self, other):
     # Perform true division by the Value instance
-    return np.multiply(self, other**-1)
+    return self * other**-1
 
 
   def __neg__(self):
     # Perform negation of the Value instance
-    return np.multiply(self, -1)
+    return self * -1
 
 
   def __sub__(self, other):
     # Perform subtraction of a Value instance
-    return np.add(self, (-other))
+    return self + (-other)
 
 
   def exp(self):
     # Compute the element-wise exponential of the Value instance
     x = self.data
     out = Value(np.exp(x), (self, ), 'exp')
 
     def _backward():
         # Calculate the gradients using the chain rule
-        self.grad = self.grad + np.multiply(out.data, out.grad)
+        self.grad = self.grad + (out.data * out.grad)
 
     # Assign the backward function to the new Value instance
     out._backward = _backward
     return out
 
 
   def tanh(self):
     # Compute the element-wise hyperbolic tangent of the Value instance
     x = self.data
     t = np.tanh(x)
     out = Value(t, (self, ), 'tanh')
 
     def _backward():
         # Calculate the gradients using the chain rule
-        self.grad = self.grad + np.multiply((1 - t**2), out.grad)
+        self.grad = self.grad + ((1 - t**2) * out.grad)
 
     # Assign the backward function to the new Value instance
     out._backward = _backward
     return out
 
 
   def backward(self):
```

### Comparing `ngrad-1.0.1/ngrad/library.py` & `ngrad-1.0.2/ngrad/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     out = act.tanh()
     # Return the output of the neuron
     return out
   
   def parameters(self):
     # Return the weights and bias of the neuron as parameters
     return self.w + [self.b]
+
   
 class Layer:
 
   def __init__(self, nin, nout):
     # Create a layer with a specified number of input and output neurons
     self.neurons = [Neuron(nin) for _ in range(nout)]
   
@@ -31,14 +32,15 @@
     outs = [n(x) for n in self.neurons]
     # If there is only one output neuron, return it directly; otherwise, return a list of outputs
     return outs[0] if len(outs) == 1 else outs
   
   def parameters(self):
     # Return the parameters of all neurons in the layer
     return [p for neuron in self.neurons for p in neuron.parameters()]
+
   
 class MLP:
 
   def __init__(self, nin, nouts):
     # Create a multi-layer perceptron (MLP) with the specified number of input and output neurons for each layer
     sz = [nin] + nouts
     self.layers = [Layer(sz[i], sz[i+1]) for i in range(len(nouts))]
```

### Comparing `ngrad-1.0.1/ngrad.egg-info/PKG-INFO` & `ngrad-1.0.2/ngrad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: ngrad
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Autograd engine and a neural network library that handle an N-dimensional array.
 Home-page: https://github.com/x0axz/ngrad
 Author: Nooh
 Author-email: x0axz@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Autograd Engine
+# Autograd Engine & Neural Network Library
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
 Andrej Karaphy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
 
 ## Blog
 
-[Building an Autograd Engine: An Illustrative and Interactive Guide](https://x0axz.com/blog/autograd.html)
+[Building Autograd Engine & Neural Network Library: An Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
 
 ## Installation
 
 ```
 pip install ngrad
```

### Comparing `ngrad-1.0.1/setup.py` & `ngrad-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ngrad",
-    version="1.0.1",
+    version="1.0.2",
     description="An Autograd engine and a neural network library that handle an N-dimensional array.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Nooh",
     author_email="x0axz@protonmail.com",
     url="https://github.com/x0axz/ngrad",
     packages=setuptools.find_packages(),
```

### Comparing `ngrad-1.0.1/test/test_engine.py` & `ngrad-1.0.2/test/test_engine.py`

 * *Files identical despite different names*

