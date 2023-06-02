# Comparing `tmp/resoto-plugin-k8s-3.5.0.tar.gz` & `tmp/resoto-plugin-k8s-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.5.0.tar", last modified: Fri May 26 18:24:23 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.5.1.tar", last modified: Fri Jun  2 14:56:25 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.5.0.tar` & `resoto-plugin-k8s-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:23.407046 resoto-plugin-k8s-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-26 18:24:23.407046 resoto-plugin-k8s-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:23.403046 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   104090 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:23.407046 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 18:24:23.000000 resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 18:24:23.407046 resoto-plugin-k8s-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 18:21:39.000000 resoto-plugin-k8s-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:25.028645 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106215 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:47.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/setup.cfg
```

### Comparing `resoto-plugin-k8s-3.5.0/PKG-INFO` & `resoto-plugin-k8s-3.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Kubernetes Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/k8s
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-k8s
 
 Kubernetes plugin for Resoto.
 See [Getting Started](https://resoto.com/docs/getting-started) for more information.
```

### Comparing `resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.0/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from threading import Lock
 
 from attrs import define, field
 from datetime import datetime
-from typing import ClassVar, Optional, Dict, Type, List, Any, Union, Tuple
+from typing import ClassVar, Optional, Dict, Type, List, Any, Union, Tuple, Set
+from collections import defaultdict
 
 from jsons import set_deserializer
 from resoto_plugin_k8s.base import KubernetesResource, SortTransitionTime
 from resotolib.baseresources import (
     BaseAccount,
     BaseInstance,
     BaseRegion,
@@ -16,15 +17,15 @@
     BaseQuota,
     BaseLoadBalancer,
     EdgeType,
     VolumeStatus,
     ModelReference,
 )
 from resotolib.graph import Graph
-from resotolib.json_bender import StringToUnitNumber, CPUCoresToNumber, Bend, S, K, bend, ForallBend, Bender, MapEnum
+from resotolib.json_bender import StringToUnitNumber, CPUCoresToNumber, Bend, F, S, K, bend, ForallBend, Bender, MapEnum
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.k8s")
 
 
 class GraphBuilder:
     def __init__(self, graph: Graph):
@@ -1017,14 +1018,15 @@
         "load_balancer_class": S("loadBalancerClass"),
         "load_balancer_ip": S("loadBalancerIP"),
         "load_balancer_source_ranges": S("loadBalancerSourceRanges", default=[]),
         "ports": S("ports", default=[]) >> ForallBend(KubernetesServicePort.mapping),
         "publish_not_ready_addresses": S("publishNotReadyAddresses"),
         "session_affinity": S("sessionAffinity"),
         "type": S("type"),
+        "selector": S("selector", default={}),
     }
     allocate_load_balancer_node_ports: Optional[bool] = field(default=None)
     cluster_ip: Optional[str] = field(default=None)
     cluster_ips: List[str] = field(factory=list)
     external_ips: List[str] = field(factory=list)
     external_name: Optional[str] = field(default=None)
     external_traffic_policy: Optional[str] = field(default=None)
@@ -1035,14 +1037,15 @@
     load_balancer_class: Optional[str] = field(default=None)
     load_balancer_ip: Optional[str] = field(default=None)
     load_balancer_source_ranges: List[str] = field(factory=list)
     ports: List[KubernetesServicePort] = field(factory=list)
     publish_not_ready_addresses: Optional[bool] = field(default=None)
     session_affinity: Optional[str] = field(default=None)
     type: Optional[str] = field(default=None)
+    selector: Optional[Dict[str, str]] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class KubernetesService(KubernetesResource):
     kind: ClassVar[str] = "kubernetes_service"
     mapping: ClassVar[Dict[str, Bender]] = KubernetesResource.mapping | {
         "service_status": S("status") >> Bend(KubernetesServiceStatus.mapping),
@@ -2225,26 +2228,83 @@
         "tls": S("tls", default=[]) >> ForallBend(KubernetesIngressTLS.mapping),
     }
     ingress_class_name: Optional[str] = field(default=None)
     rules: List[KubernetesIngressRule] = field(factory=list)
     tls: List[KubernetesIngressTLS] = field(factory=list)
 
 
+def get_backend_service_names(json: Json) -> List[str]:
+    default_services: Optional[str] = bend(
+        S(
+            "spec",
+            "defaultBackend",
+            "service",
+            "name",
+        ),
+        json,
+    )
+    services_from_rules: List[str] = bend(
+        S("spec", "rules", default=[])
+        >> ForallBend(S("http", "paths", default=[]) >> ForallBend(S("backend", "service", "name")))
+        >> F(lambda outer: [elem for inner in outer for elem in inner if elem]),
+        json,
+    )
+
+    if default_services:
+        services_from_rules.append(default_services)
+
+    return services_from_rules
+
+
 @define(eq=False, slots=False)
 class KubernetesIngress(KubernetesResource, BaseLoadBalancer):
     kind: ClassVar[str] = "kubernetes_ingress"
     mapping: ClassVar[Dict[str, Bender]] = KubernetesResource.mapping | {
         "ingress_status": S("status") >> Bend(KubernetesIngressStatus.mapping),
         "public_ip_address": S("status", "loadBalancer", "ingress", default=[])[0]["ip"],
         # take the public ip of the first load balancer
         "ingress_spec": S("spec") >> Bend(KubernetesIngressSpec.mapping),
+        # temporary values, they will be replaced in connect_in_graph call with pod ids
+        "backends": F(get_backend_service_names),
     }
     ingress_status: Optional[KubernetesIngressStatus] = field(default=None)
     ingress_spec: Optional[KubernetesIngressSpec] = field(default=None)
 
+    def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
+        super().connect_in_graph(builder, source)
+
+        pods = [
+            ((key, val), pod)
+            for pod in builder.graph.nodes
+            if isinstance(pod, KubernetesPod)
+            for key, val in pod.labels.items()
+        ]
+        pods_by_labels = defaultdict(list)
+        for (key, val), pod in pods:
+            pods_by_labels[(key, val)].append(pod)
+
+        resolved_backends: Set[str] = set()
+
+        for backend in self.backends:
+            for service in builder.graph.searchall({"kind": KubernetesService.kind, "name": backend}):
+                if not isinstance(service, KubernetesService):
+                    continue
+
+                builder.add_edge(self, edge_type=EdgeType.default, node=service)
+
+                selector = service.service_spec.selector if service.service_spec else {}
+                if not selector:
+                    continue
+
+                for key, value in selector.items():
+                    for pod in pods_by_labels.get((key, value), []):
+                        resolved_backends.add(pod.name or pod.id)
+
+        self.backends = list(resolved_backends)
+
 
 @define(eq=False, slots=False)
 class KubernetesIngressClass(KubernetesResource):
     kind: ClassVar[str] = "kubernetes_ingress_class"
     mapping: ClassVar[Dict[str, Bender]] = KubernetesResource.mapping | {}
```

### Comparing `resoto-plugin-k8s-3.5.0/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Kubernetes Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/k8s
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-k8s
 
 Kubernetes plugin for Resoto.
 See [Getting Started](https://resoto.com/docs/getting-started) for more information.
```

### Comparing `resoto-plugin-k8s-3.5.0/setup.py` & `resoto-plugin-k8s-3.5.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-import os
-import pkg_resources
-from setuptools import setup, find_packages
-
-
-def read(file_name: str) -> str:
-    with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
-        return of.read()
-
-
-setup(
-    name="resoto-plugin-k8s",
-    version="3.5.0",
-    description="Resoto Kubernetes Collector Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={"resoto.plugins": ["k8s_collector = resoto_plugin_k8s:KubernetesCollectorPlugin"]},
-    include_package_data=True,
-    zip_safe=False,
-    install_requires=[str(requirement) for requirement in pkg_resources.parse_requirements(read("requirements.txt"))],
-    setup_requires=["pytest-runner"],
-    tests_require=["pytest"],
-    classifiers=[
-        # Current project status
-        "Development Status :: 4 - Beta",
-        # Audience
-        "Intended Audience :: System Administrators",
-        "Intended Audience :: Information Technology",
-        # License information
-        "License :: OSI Approved :: Apache Software License",
-        # Supported python versions
-        "Programming Language :: Python :: 3.9",
-        # Supported OS's
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        # Extra metadata
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Security",
-        "Topic :: Utilities",
-    ],
-    keywords="cloud security",
-    url="https://github.com/someengineering/resoto/tree/main/plugins/k8s",
-)
+[project]
+name = "resoto-plugin-k8s"
+description = "Resoto Kubernetes Collector Plugin"
+version = "3.5.1"
+authors = [{name="Some Engineering Inc."}]
+license = {file="LICENSE"}
+requires-python = ">=3.9"
+classifiers = [
+    # Current project status
+    "Development Status :: 4 - Beta",
+    # Audience
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Information Technology",
+    # License information
+    "License :: OSI Approved :: Apache Software License",
+    # Supported python versions
+    "Programming Language :: Python :: 3.9",
+    # Supported OS's
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
+    # Extra metadata
+    "Environment :: Console",
+    "Natural Language :: English",
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
+readme = {file="README.md", content-type="text/markdown"}
+
+dependencies = [
+    "resotolib==3.5.1",
+    "kubernetes",
+]
+
+[project.entry-points."resoto.plugins"]
+k8s_collector = "resoto_plugin_k8s:KubernetesCollectorPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/k8s"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

