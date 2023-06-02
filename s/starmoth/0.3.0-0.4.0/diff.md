# Comparing `tmp/starmoth-0.3.0.tar.gz` & `tmp/starmoth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.3.0.tar", last modified: Thu May 18 01:47:02 2023, max compression
+gzip compressed data, was "starmoth-0.4.0.tar", last modified: Fri Jun  2 16:09:42 2023, max compression
```

## Comparing `starmoth-0.3.0.tar` & `starmoth-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.166228 starmoth-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-05-18 01:47:02.166228 starmoth-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1288 2023-05-17 18:11:33.000000 starmoth-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.158228 starmoth-0.3.0/moth/
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-05-17 16:52:15.000000 starmoth-0.3.0/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.3.0/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-05-17 16:52:15.000000 starmoth-0.3.0/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-17 16:52:15.000000 starmoth-0.3.0/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.3.0/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     2967 2023-05-11 20:09:31.000000 starmoth-0.3.0/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 01:47:02.166228 starmoth-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.166228 starmoth-0.3.0/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.476009 starmoth-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-02 16:09:42.472009 starmoth-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2023-05-17 18:11:33.000000 starmoth-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.468009 starmoth-0.4.0/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     4042 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.468009 starmoth-0.4.0/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.4.0/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.468009 starmoth-0.4.0/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.472009 starmoth-0.4.0/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.4.0/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.472009 starmoth-0.4.0/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     5763 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 16:09:42.476009 starmoth-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.472009 starmoth-0.4.0/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.3.0/PKG-INFO` & `starmoth-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.3.0
+Version: 0.4.0
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `starmoth-0.3.0/README.md` & `starmoth-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `starmoth-0.3.0/moth/cli/__init__.py` & `starmoth-0.4.0/moth/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.3.0/moth/driver/__init__.py` & `starmoth-0.4.0/moth/driver/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import abc
 from PIL import Image, ImageOps
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
-from moth.message import ImagePromptMsg, ClassificationResultMsg
+from moth.message import ImagePromptMsg, ClassificationResultMsg, ObjectDetectionResultMsg
 
 
 class ModelDriver(abc.ABC):
     @abc.abstractmethod
-    def on_model_result(self):
+    def on_model_result(self, result: Union[ClassificationResultMsg, ObjectDetectionResultMsg]):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def next_model_prompt(self) -> Optional[ImagePromptMsg]:
         raise NotImplementedError()
```

### Comparing `starmoth-0.3.0/moth/message/__init__.py` & `starmoth-0.4.0/moth/message/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from moth.message.exceptions import FailedToParseMessage, UnknownMessageType
 
 
 class HandshakeTaskTypes(str, Enum):
     CLASSIFICATION = "classification"
     OBJECT_DETECTION = "object_detection"
 
+
 def parse_message(msg: bytes) -> Msg:
     try:
         envelope = msgpack.unpackb(msg)
         message_type = envelope["msgType"]
 
         if message_type not in _MESSAGE_CLASSES:
             raise UnknownMessageType(f"Cannot parse message of type: {message_type}")
@@ -130,76 +131,91 @@
         )
 
 
 class ObjectDetectionResult:
     """
     COCO-style bounding box annotation.
     """
-    def __init__(self, x: int, y: int, w: int, h: int, class_index: Optional[int] = None, class_name: Optional[str] = None, confidence: Optional[float] = None):
+
+    def __init__(
+        self,
+        x: int,
+        y: int,
+        w: int,
+        h: int,
+        class_index: Optional[int] = None,
+        class_name: Optional[str] = None,
+        confidence: Optional[float] = None,
+    ):
         self.x = x
         self.y = y
         self.w = w
         self.h = h
         self.class_index = class_index
         self.class_name = class_name
         self.confidence = confidence
-    
+
     def serialize(self):
         obj = {
             "x": self.x,
             "y": self.y,
             "w": self.w,
             "h": self.h,
             "classIndex": self.class_index,
             "className": self.class_name,
-            "confidence": self.confidence
+            "confidence": self.confidence,
         }
 
         return msgpack.packb(obj)
-    
+
     @staticmethod
     def deserialize(bytes) -> ObjectDetectionResult:
         obj = msgpack.unpackb(bytes)
         return ObjectDetectionResult(
             x=obj["x"],
             y=obj["y"],
             w=obj["w"],
             h=obj["h"],
             class_index=obj.get("classIndex"),
             class_name=obj.get("className"),
-            confidence=obj.get("confidence")
+            confidence=obj.get("confidence"),
         )
 
 
 class ObjectDetectionResultMsg(Msg):
     """
     Message for object detection results.
     A list of bounding boxes.
     """
 
-    def __init__(self, prompt_id: str, object_detection_results: List[ObjectDetectionResult]):
+    def __init__(
+        self, prompt_id: str, object_detection_results: List[ObjectDetectionResult]
+    ):
         self.prompt_id = prompt_id
         self.object_detection_results = object_detection_results
 
     def serialize(self):
         obj = {
             "promptId": self.prompt_id,
-            "results": [bb.serialize() for bb in self.object_detection_results]
+            "results": [bb.serialize() for bb in self.object_detection_results],
         }
 
         return msgpack.packb(obj)
 
     @staticmethod
     def deserialize(bytes) -> ObjectDetectionResultMsg:
         obj = msgpack.unpackb(bytes)
         return ObjectDetectionResultMsg(
             prompt_id=obj["promptId"],
-            object_detection_results=[ObjectDetectionResult.deserialize(bb) for bb in obj["results"]]
+            object_detection_results=[
+                ObjectDetectionResult.deserialize(bb) for bb in obj["results"]
+            ],
         )
 
+
 @dataclass
 class HandshakeMsg(Msg):
     name: str
     handshake_token: str
     version: str = "v0"
     task_type: HandshakeTaskTypes = HandshakeTaskTypes.CLASSIFICATION
 
@@ -212,18 +228,37 @@
         }
         return msgpack.packb(obj)
 
     @staticmethod
     def deserialize(data: bytes) -> HandshakeMsg:
         obj = msgpack.unpackb(data)
         return HandshakeMsg(
-            name=obj["name"], handshake_token=obj["token"], version=obj["version"], task_type=obj["taskType"]
+            name=obj["name"],
+            handshake_token=obj["token"],
+            version=obj["version"],
+            task_type=obj.get("taskType", HandshakeTaskTypes.CLASSIFICATION), # Ensure backwards compatibility
         )
 
+@dataclass
+class HandshakeResponseMsg(Msg):
+    def serialize(self) -> bytes:
+        return msgpack.packb({})
+
+    @staticmethod
+    def deserialize(data: bytes) -> HandshakeResponseMsg:
+        return HandshakeResponseMsg()
+
+
+
+class PromptResultMsg(Msg):
+    pass
+
 
 _MESSAGE_CLASSES: Dict[str, Type[Msg]] = {
     HandshakeMsg.msg_type_name(): HandshakeMsg,
     ImagePromptMsg.msg_type_name(): ImagePromptMsg,
     HeartbeatMsg.msg_type_name(): HeartbeatMsg,
+    PromptResultMsg.msg_type_name(): ClassificationResultMsg,  # Ensure backwards compatibility
     ClassificationResultMsg.msg_type_name(): ClassificationResultMsg,
-    ObjectDetectionResultMsg.msg_type_name(): ObjectDetectionResultMsg
+    ObjectDetectionResultMsg.msg_type_name(): ObjectDetectionResultMsg,
+    HandshakeResponseMsg.msg_type_name(): HandshakeResponseMsg,
 }
```

### Comparing `starmoth-0.3.0/setup.py` & `starmoth-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.3.0/starmoth.egg-info/PKG-INFO` & `starmoth-0.4.0/starmoth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.3.0
+Version: 0.4.0
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

