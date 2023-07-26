# Comparing `tmp/pydlmeta-1.0.1.tar.gz` & `tmp/pydlmeta-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlmeta-1.0.1.tar", last modified: Thu Jul 13 03:27:14 2023, max compression
+gzip compressed data, was "pydlmeta-1.0.2.tar", last modified: Wed Jul 26 09:58:40 2023, max compression
```

## Comparing `pydlmeta-1.0.1.tar` & `pydlmeta-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      904 2023-07-13 03:25:48.000000 pydlmeta-1.0.1/README.md
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/pydlmeta/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:40:59.000000 pydlmeta-1.0.1/pydlmeta/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      234 2023-07-12 03:15:30.000000 pydlmeta-1.0.1/pydlmeta/config.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4619 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/dtype_map.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/pydlmeta/identifier/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:49:38.000000 pydlmeta-1.0.1/pydlmeta/identifier/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     7418 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/identifier/dataset.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    10974 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/identifier/model.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2018 2023-07-11 03:49:38.000000 pydlmeta-1.0.1/pydlmeta/identifier/types.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    16534 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/meta.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      567 2023-07-12 03:15:30.000000 pydlmeta-1.0.1/pydlmeta/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/pydlmeta.egg-info/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      413 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/SOURCES.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/dependency_links.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       80 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/requires.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        9 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/setup.cfg
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1253 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.881665 pydlmeta-1.0.2/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      904 2023-07-13 03:25:48.000000 pydlmeta-1.0.2/README.md
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/pydlmeta/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:40:59.000000 pydlmeta-1.0.2/pydlmeta/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      234 2023-07-12 03:15:30.000000 pydlmeta-1.0.2/pydlmeta/config.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4619 2023-07-12 03:13:09.000000 pydlmeta-1.0.2/pydlmeta/dtype_map.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/pydlmeta/identifier/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:49:38.000000 pydlmeta-1.0.2/pydlmeta/identifier/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7418 2023-07-12 03:13:09.000000 pydlmeta-1.0.2/pydlmeta/identifier/dataset.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    10974 2023-07-12 03:13:09.000000 pydlmeta-1.0.2/pydlmeta/identifier/model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2010 2023-07-26 08:02:17.000000 pydlmeta-1.0.2/pydlmeta/identifier/types.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    16607 2023-07-26 08:00:04.000000 pydlmeta-1.0.2/pydlmeta/meta.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      567 2023-07-12 03:15:30.000000 pydlmeta-1.0.2/pydlmeta/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/pydlmeta.egg-info/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      413 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/SOURCES.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/dependency_links.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       80 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/requires.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        9 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-26 09:58:40.881665 pydlmeta-1.0.2/setup.cfg
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1253 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/setup.py
```

### Comparing `pydlmeta-1.0.1/PKG-INFO` & `pydlmeta-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlmeta
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # PyDLmeta
```

### Comparing `pydlmeta-1.0.1/README.md` & `pydlmeta-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.1/pydlmeta/dtype_map.py` & `pydlmeta-1.0.2/pydlmeta/dtype_map.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.1/pydlmeta/identifier/dataset.py` & `pydlmeta-1.0.2/pydlmeta/identifier/dataset.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.1/pydlmeta/identifier/model.py` & `pydlmeta-1.0.2/pydlmeta/identifier/model.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.1/pydlmeta/identifier/types.py` & `pydlmeta-1.0.2/pydlmeta/identifier/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,44 +26,36 @@
     elif path.is_file():
         return SrcType.FILE
     else:
         return None
 
 
 class ModelFormat(Enum):
+    CAFFE_DIR = auto()
+    CKPT = auto()
+    GRAPHDEF = auto()
+    H5 = auto()
+    KERAS_MODEL = auto()
+    MLIR = auto()
     NON_SPECIFIED = auto()
-
+    ONNX = auto()
+    OPENVINO_IRDIR = auto()
+    PB = auto()
     PT_NN_MODULE = auto()
+    PTH = auto()
+    RELAYIR = auto()
+    SAVED_MODEL = auto()
     TF_KERAS_MODEL = auto()
-    KERAS_MODEL = auto()
     TF_SESSION = auto()
-
-    H5 = auto()
-    SAVED_MODEL = auto()
-    PB = auto()
-    ZIPPED_SAVED_MODEL = auto()
     TFLITE = auto()
-
-    PTH = auto()
-    ONNX = auto()
     TORCH_TRACED = auto()
-
-    CKPT = auto()
-
     TRT_PLAN = auto()
-    OPENVINO_IRDIR = auto()
-    ZIPPED_OPENVINO_IRDIR = auto()
-
-    CAFFE_DIR = auto()
     ZIPPED_CAFFE_DIR = auto()
-    GRAPHDEF = auto()
-
-    RELAYIR = auto()
-
-    MLIR = auto()
+    ZIPPED_OPENVINO_IRDIR = auto()
+    ZIPPED_SAVED_MODEL = auto()
 
 
 TF_MODEL_FORMATS = [
     ModelFormat.TF_KERAS_MODEL, ModelFormat.KERAS_MODEL, ModelFormat.H5,
     ModelFormat.SAVED_MODEL, ModelFormat.PB, ModelFormat.TFLITE,
     ModelFormat.CKPT
 ]
```

### Comparing `pydlmeta-1.0.1/pydlmeta/meta.py` & `pydlmeta-1.0.2/pydlmeta/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,19 @@
         if name != "MetadataRetriver":
             cls.REGISTRY.append(new_cls)
         return new_cls
 
 
 class ModelMeta:
 
-    def __init__(self, inputs: List[TensorMeta], outputs: List[TensorMeta]):
+    def __init__(self, inputs: List[TensorMeta], outputs: List[TensorMeta],
+                format):
         self.inputs = inputs
         self.outputs = outputs
+        self.format = format
 
 
 class MetadataRetriver(metaclass=MetadataRetriverRegistry):
 
     FORMAT: ModelFormat = ModelFormat.NON_SPECIFIED
 
     @classmethod
@@ -61,15 +63,15 @@
         raise NotImplementedError("`retrieve_outputs` has to be implemented")
 
     def retrieve(self, model_path) -> ModelMeta:
         inputs = self.retrieve_inputs(model_path)
         logger.debug(f"Inputs: {inputs}")
         outputs = self.retrieve_outputs(model_path)
         logger.debug(f"Outputs: {outputs}")
-        return ModelMeta(inputs=inputs, outputs=outputs)
+        return ModelMeta(inputs=inputs, outputs=outputs, format=self.FORMAT)
 
 
 def retrieve_model_metadata(model_path) -> ModelMeta:
     for metadataretriever in MetadataRetriver.REGISTRY:
         if metadataretriever.is_me(model_path):
             return metadataretriever().retrieve(model_path)
```

### Comparing `pydlmeta-1.0.1/pydlmeta/utils.py` & `pydlmeta-1.0.2/pydlmeta/utils.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.1/pydlmeta.egg-info/PKG-INFO` & `pydlmeta-1.0.2/pydlmeta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlmeta
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # PyDLmeta
```

### Comparing `pydlmeta-1.0.1/setup.py` & `pydlmeta-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="pydlmeta",
-    version="1.0.1",
+    version="1.0.2",
     license="Apache License 2.0",
     long_description=README, # without this pypi upload will raise warning
     long_description_content_type="text/markdown",  # without this pypi upload will raise warning
     packages=find_packages(),
     package_data={"pydlmeta": ["*"]},
     dependency_links=[
         "https://download.pytorch.org/whl/torch_stable.html",
```

