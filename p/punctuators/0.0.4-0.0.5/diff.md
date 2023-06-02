# Comparing `tmp/punctuators-0.0.4-py3-none-any.whl.zip` & `tmp/punctuators-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10075 bytes, number of entries: 13
+Zip file size: 10176 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 00:39 punctuators/__init__.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Mar-04 22:49 punctuators/collectors/__init__.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Mar-12 00:51 punctuators/collectors/pcs_collector.py
 -rw-r--r--  2.0 unx     1682 b- defN 23-Mar-04 23:07 punctuators/collectors/sbd_collector.py
 -rw-r--r--  2.0 unx      140 b- defN 23-Feb-28 23:53 punctuators/data/__init__.py
 -rw-r--r--  2.0 unx     4598 b- defN 23-Mar-01 23:45 punctuators/data/infer_dataset.py
 -rw-r--r--  2.0 unx      177 b- defN 23-Mar-04 22:53 punctuators/models/__init__.py
--rw-r--r--  2.0 unx     6529 b- defN 23-Mar-24 22:17 punctuators/models/punc_cap_seg_model.py
+-rw-r--r--  2.0 unx     6899 b- defN 23-May-29 21:39 punctuators/models/punc_cap_seg_model.py
 -rw-r--r--  2.0 unx     5630 b- defN 23-Mar-04 23:04 punctuators/models/sbd_model.py
--rw-r--r--  2.0 unx      322 b- defN 23-Apr-15 18:40 punctuators-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 18:40 punctuators-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-15 18:40 punctuators-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1117 b- defN 23-Apr-15 18:40 punctuators-0.0.4.dist-info/RECORD
-13 files, 24915 bytes uncompressed, 8183 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx      322 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/RECORD
+13 files, 25285 bytes uncompressed, 8284 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: punctuators/models/punc_cap_seg_model.py
 Comment: 
 
 Filename: punctuators/models/sbd_model.py
 Comment: 
 
-Filename: punctuators-0.0.4.dist-info/METADATA
+Filename: punctuators-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: punctuators-0.0.4.dist-info/WHEEL
+Filename: punctuators-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: punctuators-0.0.4.dist-info/top_level.txt
+Filename: punctuators-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: punctuators-0.0.4.dist-info/RECORD
+Filename: punctuators-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## punctuators/models/punc_cap_seg_model.py

```diff
@@ -18,16 +18,16 @@
     """ No abstraction yet, will be refactored """
 
     pass
 
 
 @dataclass
 class PunctCapSegConfigONNX(PunctCapSegConfig):
-    spe_filename: str
-    model_filename: str
+    spe_filename: str = "sp.model"
+    model_filename: str = "model.onnx"
     config_filename: str = "config.yaml"
     hf_repo_id: Optional[str] = None
     directory: Optional[str] = None
 
 
 class PunctCapSegModel:
     """ No abstraction yet, will be refactored """
@@ -77,20 +77,31 @@
                 model_filename="model.onnx",
             ),
         }
         return info
 
     @classmethod
     def from_pretrained(cls, pretrained_name: str) -> "PunctCapSegModelONNX":
-        available_models: Dict[str, PunctCapSegConfigONNX] = cls.pretrained_model_info()
-        if pretrained_name not in available_models:
-            raise ValueError(
-                f"Pretrained name '{pretrained_name}' not in available models: '{list(available_models.keys())}'"
-            )
-        return cls(cfg=available_models[pretrained_name])
+        """
+
+        Args:
+            pretrained_name: 
+        """
+        cfg: PunctCapSegConfigONNX
+        if "/" in pretrained_name:
+            # Assume this is a HuggingFace repository with default model names
+            cfg = PunctCapSegConfigONNX(hf_repo_id=pretrained_name)
+        else:
+            available_models: Dict[str, PunctCapSegConfigONNX] = cls.pretrained_model_info()
+            if pretrained_name not in available_models:
+                raise ValueError(
+                    f"Pretrained name '{pretrained_name}' not in available models: '{list(available_models.keys())}'"
+                )
+            cfg = available_models[pretrained_name]
+        return cls(cfg=cfg)
 
     @property
     def languages(self) -> List[str]:
         return self._languages
 
     def _setup_dataloader(
         self, texts: List[str], batch_size_tokens: int, overlap: int, num_workers: int = os.cpu_count() - 1
```

## Comparing `punctuators-0.0.4.dist-info/RECORD` & `punctuators-0.0.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 punctuators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 punctuators/collectors/__init__.py,sha256=kLlJ1RLmInnM2wHwvhYvHLmt1zm3mKoxst4RfIzIXBY,208
 punctuators/collectors/pcs_collector.py,sha256=aMS6QCqBxu7dBWarD2N6YeeQx9sB7Q05NI4Enn4aXJ4,4408
 punctuators/collectors/sbd_collector.py,sha256=2k_LQVHwFgsYuFEOYsmk7kficnLyjDhcldTWpMJ2Fx8,1682
 punctuators/data/__init__.py,sha256=PhY4MZZkqp4y8dmwQNq9YsV0PDBrevMCI662R57bpCM,140
 punctuators/data/infer_dataset.py,sha256=ZuTl9XzNo2snzbVLwR1q0lnYMbZZi6FmqTRPrFB-FZ0,4598
 punctuators/models/__init__.py,sha256=LGoYK3mX6zbuVpKgO18fl4KpNnYIJYUHjjXLTAuNmS0,177
-punctuators/models/punc_cap_seg_model.py,sha256=QeMA7rwpnosdG2kfPYjq1mg5htKyXO8gOStrtjF3DmM,6529
+punctuators/models/punc_cap_seg_model.py,sha256=GidKb3J3XGij0qjO4Vx9u2rdMh3SvlE9ICCJ4BkY3j8,6899
 punctuators/models/sbd_model.py,sha256=YbK1Mphxsa6Ayf16_qEpvRWUro2F8YskDTsC5ygYeUY,5630
-punctuators-0.0.4.dist-info/METADATA,sha256=A1_w7T8T6zEgdzzB8pbwkdHZp17mw1irVs48a_FqqlE,322
-punctuators-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-punctuators-0.0.4.dist-info/top_level.txt,sha256=Y6h2UBM8ZvPkmyZfr85YtuqiskQtKq-92_fwwvm9x3s,12
-punctuators-0.0.4.dist-info/RECORD,,
+punctuators-0.0.5.dist-info/METADATA,sha256=Jpt7tOAX_NcK77XBvSx-PJoDxq3llEuDQ_yMcQq7Gns,322
+punctuators-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+punctuators-0.0.5.dist-info/top_level.txt,sha256=Y6h2UBM8ZvPkmyZfr85YtuqiskQtKq-92_fwwvm9x3s,12
+punctuators-0.0.5.dist-info/RECORD,,
```

