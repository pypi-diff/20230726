# Comparing `tmp/huggingface_tool-0.0.3.tar.gz` & `tmp/huggingface_tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huggingface_tool-0.0.3.tar", last modified: Thu Jul 20 03:28:08 2023, max compression
+gzip compressed data, was "huggingface_tool-0.0.4.tar", last modified: Wed Jul 26 09:19:27 2023, max compression
```

## Comparing `huggingface_tool-0.0.3.tar` & `huggingface_tool-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.129807 huggingface_tool-0.0.3/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-07-05 08:02:03.000000 huggingface_tool-0.0.3/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     2894 2023-07-20 03:28:08.129274 huggingface_tool-0.0.3/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     1797 2023-07-20 03:24:51.000000 huggingface_tool-0.0.3/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.119785 huggingface_tool-0.0.3/huggingface_tool/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1113 2023-07-12 05:32:35.000000 huggingface_tool-0.0.3/huggingface_tool/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.121816 huggingface_tool-0.0.3/huggingface_tool/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 huggingface_tool-0.0.3/huggingface_tool/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3900 2023-07-20 03:15:34.000000 huggingface_tool-0.0.3/huggingface_tool/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.124618 huggingface_tool-0.0.3/huggingface_tool/savers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-05 05:24:38.000000 huggingface_tool-0.0.3/huggingface_tool/savers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      961 2023-07-12 05:17:52.000000 huggingface_tool-0.0.3/huggingface_tool/savers/base_model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1277 2023-07-12 05:19:30.000000 huggingface_tool-0.0.3/huggingface_tool/savers/base_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1025 2023-07-05 07:49:11.000000 huggingface_tool-0.0.3/huggingface_tool/savers/dataset_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      931 2023-07-12 05:17:52.000000 huggingface_tool-0.0.3/huggingface_tool/savers/diffusion_model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1779 2023-07-12 05:23:51.000000 huggingface_tool-0.0.3/huggingface_tool/savers/model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      861 2023-07-12 05:18:18.000000 huggingface_tool-0.0.3/huggingface_tool/savers/tokenizer_saver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.126935 huggingface_tool-0.0.3/huggingface_tool/uploaders/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-20 03:03:53.000000 huggingface_tool-0.0.3/huggingface_tool/uploaders/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1320 2023-07-20 03:23:56.000000 huggingface_tool-0.0.3/huggingface_tool/uploaders/base_uploader.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1655 2023-07-20 03:23:27.000000 huggingface_tool-0.0.3/huggingface_tool/uploaders/dataset_uploader.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.128784 huggingface_tool-0.0.3/huggingface_tool/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 huggingface_tool-0.0.3/huggingface_tool/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1290 2023-07-05 05:32:09.000000 huggingface_tool-0.0.3/huggingface_tool/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1370 2023-07-05 05:21:26.000000 huggingface_tool-0.0.3/huggingface_tool/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-20 03:28:08.121283 huggingface_tool-0.0.3/huggingface_tool.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     2894 2023-07-20 03:28:08.000000 huggingface_tool-0.0.3/huggingface_tool.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      877 2023-07-20 03:28:08.000000 huggingface_tool-0.0.3/huggingface_tool.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-20 03:28:08.000000 huggingface_tool-0.0.3/huggingface_tool.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-07-20 03:28:08.000000 huggingface_tool-0.0.3/huggingface_tool.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      213 2023-07-20 03:28:08.000000 huggingface_tool-0.0.3/huggingface_tool.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       17 2023-07-20 03:28:08.000000 huggingface_tool-0.0.3/huggingface_tool.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-20 03:28:08.129862 huggingface_tool-0.0.3/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2978 2023-07-20 02:39:22.000000 huggingface_tool-0.0.3/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:27.001184 huggingface_tool-0.0.4/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-07-05 08:02:03.000000 huggingface_tool-0.0.4/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3053 2023-07-26 09:19:27.001043 huggingface_tool-0.0.4/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1956 2023-07-26 09:17:43.000000 huggingface_tool-0.0.4/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.995038 huggingface_tool-0.0.4/huggingface_tool/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1113 2023-07-20 03:29:40.000000 huggingface_tool-0.0.4/huggingface_tool/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.996324 huggingface_tool-0.0.4/huggingface_tool/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 huggingface_tool-0.0.4/huggingface_tool/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4249 2023-07-26 08:28:45.000000 huggingface_tool-0.0.4/huggingface_tool/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.998549 huggingface_tool-0.0.4/huggingface_tool/savers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-05 05:24:38.000000 huggingface_tool-0.0.4/huggingface_tool/savers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      961 2023-07-12 05:17:52.000000 huggingface_tool-0.0.4/huggingface_tool/savers/base_model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1277 2023-07-12 05:19:30.000000 huggingface_tool-0.0.4/huggingface_tool/savers/base_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1025 2023-07-05 07:49:11.000000 huggingface_tool-0.0.4/huggingface_tool/savers/dataset_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      931 2023-07-12 05:17:52.000000 huggingface_tool-0.0.4/huggingface_tool/savers/diffusion_model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1779 2023-07-12 05:23:51.000000 huggingface_tool-0.0.4/huggingface_tool/savers/model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      861 2023-07-12 05:18:18.000000 huggingface_tool-0.0.4/huggingface_tool/savers/tokenizer_saver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:27.000004 huggingface_tool-0.0.4/huggingface_tool/uploaders/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-20 03:03:53.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1320 2023-07-20 03:23:56.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/base_uploader.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1655 2023-07-20 03:23:27.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/dataset_uploader.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1949 2023-07-26 09:16:10.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/model_uploader.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1776 2023-07-26 09:15:26.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:27.000724 huggingface_tool-0.0.4/huggingface_tool/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 huggingface_tool-0.0.4/huggingface_tool/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1290 2023-07-05 05:32:09.000000 huggingface_tool-0.0.4/huggingface_tool/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1370 2023-07-05 05:21:26.000000 huggingface_tool-0.0.4/huggingface_tool/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.995837 huggingface_tool-0.0.4/huggingface_tool.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3053 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)      958 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      213 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       17 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-26 09:19:27.001226 huggingface_tool-0.0.4/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2978 2023-07-20 02:39:22.000000 huggingface_tool-0.0.4/setup.py
```

### Comparing `huggingface_tool-0.0.3/LICENSE` & `huggingface_tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/PKG-INFO` & `huggingface_tool-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huggingface_tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolkit for managing huggingface models and datasets
 Home-page: https://github.com/OpenRL-Lab/huggingface_tool
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/huggingface_tool
 Project-URL: Documentation, https://huggingface_tool.readthedocs.io/
 Keywords: huggingface toolkit
@@ -35,28 +35,31 @@
 
 ## Installation
 
 `pip install huggingface-tool`
 
 ## Usage
 
+Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
+
 - Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
   - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
   - For example: `htool save-dm google/ddpm-cat-256 ./google/`
 
-You can also use htool to upload datasets and models to huggingface. 
-Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
+You can also use htool to upload datasets and models to huggingface.
 
 - Upload dataset with: `htool upload-data <local_dataset_dir> <organization_or_username/dataset_name>`
   - For example: `htool upload-data ./daily_dialog OpenRL/daily_dialog`
+- Upload model with: `htool upload-model <local_model_dir> <organization_or_username/model_name>`
+  - For example: `htool upload-model ./tizero OpenRL/tizero`
 
 
 ## Citing huggingface_tool
 
 If our work has been helpful to you, please feel free to cite us:
 ```latex
 @misc{huggingface_tool2023,
```

### Comparing `huggingface_tool-0.0.3/README.md` & `huggingface_tool-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 
 ## Installation
 
 `pip install huggingface-tool`
 
 ## Usage
 
+Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
+
 - Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
   - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
   - For example: `htool save-dm google/ddpm-cat-256 ./google/`
 
-You can also use htool to upload datasets and models to huggingface. 
-Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
+You can also use htool to upload datasets and models to huggingface.
 
 - Upload dataset with: `htool upload-data <local_dataset_dir> <organization_or_username/dataset_name>`
   - For example: `htool upload-data ./daily_dialog OpenRL/daily_dialog`
+- Upload model with: `htool upload-model <local_model_dir> <organization_or_username/model_name>`
+  - For example: `htool upload-model ./tizero OpenRL/tizero`
 
 
 ## Citing huggingface_tool
 
 If our work has been helpful to you, please feel free to cite us:
 ```latex
 @misc{huggingface_tool2023,
```

### Comparing `huggingface_tool-0.0.3/huggingface_tool/__init__.py` & `huggingface_tool-0.0.4/huggingface_tool/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "huggingface_tool"
-__VERSION__ = "v0.0.3"
+__VERSION__ = "v0.0.4"
 __DESCRIPTION__ = "Toolkit for managing huggingface models and datasets"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `huggingface_tool-0.0.3/huggingface_tool/cli/__init__.py` & `huggingface_tool-0.0.4/huggingface_tool/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/cli/cli.py` & `huggingface_tool-0.0.4/huggingface_tool/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,7 +137,18 @@
 def upload_data(dataset_dir, dataset_name):
     from huggingface_tool.uploaders.dataset_uploader import DatasetUploader
     uploader = DatasetUploader(dataset_dir, dataset_name)
     if uploader.check():
         uploader.push()
     else:
         uploader.logger.info("Dataset not valid")
+
+@cli.command()
+@click.argument("model_dir")
+@click.argument("model_name")
+def upload_model(model_dir, model_name):
+    from huggingface_tool.uploaders.model_uploader import ModelUploader
+    uploader = ModelUploader(model_dir, model_name)
+    if uploader.check():
+        uploader.push()
+    else:
+        uploader.logger.info("Dataset not valid")
```

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/__init__.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/base_model_saver.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/base_model_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/base_saver.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/base_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/dataset_saver.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/dataset_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/diffusion_model_saver.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/diffusion_model_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/model_saver.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/model_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/savers/tokenizer_saver.py` & `huggingface_tool-0.0.4/huggingface_tool/savers/tokenizer_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/uploaders/__init__.py` & `huggingface_tool-0.0.4/huggingface_tool/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/uploaders/base_uploader.py` & `huggingface_tool-0.0.4/huggingface_tool/uploaders/base_uploader.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/uploaders/dataset_uploader.py` & `huggingface_tool-0.0.4/huggingface_tool/uploaders/dataset_uploader.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/utils/__init__.py` & `huggingface_tool-0.0.4/huggingface_tool/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/utils/logger.py` & `huggingface_tool-0.0.4/huggingface_tool/utils/logger.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool/utils/util.py` & `huggingface_tool-0.0.4/huggingface_tool/utils/util.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.3/huggingface_tool.egg-info/PKG-INFO` & `huggingface_tool-0.0.4/huggingface_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huggingface-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolkit for managing huggingface models and datasets
 Home-page: https://github.com/OpenRL-Lab/huggingface_tool
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/huggingface_tool
 Project-URL: Documentation, https://huggingface_tool.readthedocs.io/
 Keywords: huggingface toolkit
@@ -35,28 +35,31 @@
 
 ## Installation
 
 `pip install huggingface-tool`
 
 ## Usage
 
+Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
+
 - Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
   - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
   - For example: `htool save-dm google/ddpm-cat-256 ./google/`
 
-You can also use htool to upload datasets and models to huggingface. 
-Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
+You can also use htool to upload datasets and models to huggingface.
 
 - Upload dataset with: `htool upload-data <local_dataset_dir> <organization_or_username/dataset_name>`
   - For example: `htool upload-data ./daily_dialog OpenRL/daily_dialog`
+- Upload model with: `htool upload-model <local_model_dir> <organization_or_username/model_name>`
+  - For example: `htool upload-model ./tizero OpenRL/tizero`
 
 
 ## Citing huggingface_tool
 
 If our work has been helpful to you, please feel free to cite us:
 ```latex
 @misc{huggingface_tool2023,
```

### Comparing `huggingface_tool-0.0.3/huggingface_tool.egg-info/SOURCES.txt` & `huggingface_tool-0.0.4/huggingface_tool.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,10 +16,12 @@
 huggingface_tool/savers/dataset_saver.py
 huggingface_tool/savers/diffusion_model_saver.py
 huggingface_tool/savers/model_saver.py
 huggingface_tool/savers/tokenizer_saver.py
 huggingface_tool/uploaders/__init__.py
 huggingface_tool/uploaders/base_uploader.py
 huggingface_tool/uploaders/dataset_uploader.py
+huggingface_tool/uploaders/model_uploader.py
+huggingface_tool/uploaders/utils.py
 huggingface_tool/utils/__init__.py
 huggingface_tool/utils/logger.py
 huggingface_tool/utils/util.py
```

### Comparing `huggingface_tool-0.0.3/setup.py` & `huggingface_tool-0.0.4/setup.py`

 * *Files identical despite different names*

