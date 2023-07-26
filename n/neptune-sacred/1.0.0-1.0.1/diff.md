# Comparing `tmp/neptune_sacred-1.0.0.tar.gz` & `tmp/neptune_sacred-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_sacred-1.0.0.tar", max compression
+gzip compressed data, was "neptune_sacred-1.0.1.tar", max compression
```

## Comparing `neptune_sacred-1.0.0.tar` & `neptune_sacred-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1671 2023-03-28 14:05:40.737403 neptune_sacred-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-03-28 14:05:40.737403 neptune_sacred-1.0.0/LICENSE
--rw-r--r--   0        0        0     2546 2023-03-28 14:05:40.737403 neptune_sacred-1.0.0/README.md
--rw-r--r--   0        0        0     2537 2023-03-28 14:05:53.765652 neptune_sacred-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      727 2023-03-28 14:05:40.741404 neptune_sacred-1.0.0/src/neptune_sacred/__init__.py
--rw-r--r--   0        0        0     5578 2023-03-28 14:05:40.741404 neptune_sacred-1.0.0/src/neptune_sacred/impl/__init__.py
--rw-r--r--   0        0        0      241 2023-03-28 14:05:40.741404 neptune_sacred-1.0.0/src/neptune_sacred/impl/utils.py
--rw-r--r--   0        0        0      737 2023-03-28 14:05:40.741404 neptune_sacred-1.0.0/src/neptune_sacred/impl/version.py
--rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 neptune_sacred-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1833 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2395 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/README.md
+-rw-r--r--   0        0        0     2537 2023-07-26 11:25:03.879711 neptune_sacred-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      727 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/src/neptune_sacred/__init__.py
+-rw-r--r--   0        0        0     5521 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/src/neptune_sacred/impl/__init__.py
+-rw-r--r--   0        0        0      241 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/src/neptune_sacred/impl/utils.py
+-rw-r--r--   0        0        0      737 2023-07-26 11:24:49.659302 neptune_sacred-1.0.1/src/neptune_sacred/impl/version.py
+-rw-r--r--   0        0        0     4336 1970-01-01 00:00:00.000000 neptune_sacred-1.0.1/PKG-INFO
```

### Comparing `neptune_sacred-1.0.0/CHANGELOG.md` & `neptune_sacred-1.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune-sacred 1.0.1
+
+### Fixes
+- Fixed file upload if full path is used and file is not in CWD ([#25](https://github.com/neptune-ai/neptune-sacred/pull/25))
+
 ## neptune-sacred 1.0.0
 
 ### Changes
 - Updated integration to be compatible with `neptune` `1.0.0`. ([#20](https://github.com/neptune-ai/neptune-sacred/pull/20))
 - Removed `neptune` and `neptune-client` from base requirements  ([#20](https://github.com/neptune-ai/neptune-sacred/pull/20))
 - Only files are now uploaded instead of a catch-all `object` ([#20](https://github.com/neptune-ai/neptune-sacred/pull/20))
```

### Comparing `neptune_sacred-1.0.0/LICENSE` & `neptune_sacred-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_sacred-1.0.0/README.md` & `neptune_sacred-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,56 +6,59 @@
 
 * Log, display, organize, and compare ML experiments in a single place
 * Version, store, manage, and query trained models, and model building metadata
 * Record and monitor model training, evaluation, or production runs live
 
 ## What will be logged to Neptune?
 
-* Hyper-parameters
-* Losses & metrics
-* Training code(Python scripts or Jupyter notebooks) and git information
+* Hyperparameters
+* Losses and metrics
+* Training code (Python scripts or Jupyter notebooks) and Git information
 * Dataset version
-* Model Configuration
-* [Other metadata](https://docs.neptune.ai/you-should-know/what-can-you-log-and-display)
+* Model configuration
+* [Other metadata](https://docs.neptune.ai/logging/what_you_can_log)
 
 ![image](https://user-images.githubusercontent.com/97611089/160633857-48aa87ac-fcab-4225-8172-05aba159feaf.png)
-*Example custom dashboard in the Neptune UI*
-
+*Example custom dashboard in the Neptune app*
 
 ## Resources
 
-* [Documentation](https://docs.neptune.ai/integrations-and-supported-tools/experiment-tracking/sacred)
+* [Documentation](https://docs.neptune.ai/integrations/sacred)
 * [Code example on GitHub](https://github.com/neptune-ai/examples/tree/main/integrations-and-supported-tools/sacred/scripts)
-* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/sacred-integration/e/SAC-11/dashboard/Sacred-Dashboard-6741ab33-825c-4b25-8ebb-bb95c11ca3f4)
+* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/sacred-integration/e/SAC-1341/dashboard/Sacred-Dashboard-6741ab33-825c-4b25-8ebb-bb95c11ca3f4)
 * [Run example in Google Colab](https://colab.research.google.com/github/neptune-ai/examples/blob/main/integrations-and-supported-tools/sacred/notebooks/Neptune_Sacred.ipynb)
 
 ## Example
 
-```python
-# On the command line:
-pip install neptune-client[sacred] sacred torch torchvision
+On the command line:
+
 ```
-```python
-# In Python:
-import neptune.new as neptune
+pip install neptune-sacred
+```
+
+In Python:
 
+```python
+import neptune
 
 # Start a run
-run = neptune.init(project = "common/sacred-integration",
-                   api_token = "ANONYMOUS")
+run = neptune.init_run(
+    project = "common/sacred-integration",
+    api_token = neptune.ANONYMOUS_API_TOKEN,
+)
 
-# Create a sacred experiment
+# Create a Sacred experiment
 experiment = Experiment("image_classification", interactive=True)
 
 # Add NeptuneObserver and run the experiment
-experiment.observers.append(NeptuneObserver(run=neptune_run))
+experiment.observers.append(NeptuneObserver(run=run))
 experiment.run()
 ```
 
 ## Support
 
 If you got stuck or simply want to talk to us, here are your options:
 
-* Check our [FAQ page](https://docs.neptune.ai/getting-started/getting-help#frequently-asked-questions)
+* Check our [FAQ page](https://docs.neptune.ai/getting_help)
 * You can submit bug reports, feature requests, or contributions directly to the repository.
 * Chat! When in the Neptune application click on the blue message icon in the bottom-right corner and send a message. A real person will talk to you ASAP (typically very ASAP),
 * You can just shoot us an email at support@neptune.ai
```

### Comparing `neptune_sacred-1.0.0/pyproject.toml` & `neptune_sacred-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 repository = "https://github.com/neptune-ai/neptune-sacred"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations/sacred/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-sacred"
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_sacred-1.0.0/src/neptune_sacred/__init__.py` & `neptune_sacred-1.0.1/src/neptune_sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_sacred-1.0.0/src/neptune_sacred/impl/__init__.py` & `neptune_sacred-1.0.1/src/neptune_sacred/impl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
 import json
-import os
 import warnings
 
 try:
     from neptune import Run
     from neptune.handler import Handler
     from neptune.integrations.utils import expect_not_an_experiment
     from neptune.types import File
@@ -127,15 +126,14 @@
     def interrupted_event(self, interrupt_time, status):
         pass
 
     def failed_event(self, fail_time, fail_trace):
         pass
 
     def artifact_event(self, name, filename, metadata=None, content_type=None):
-        filename = os.path.split(filename)[-1]
         self._run[self.base_namespace][f"io_files/artifacts/{name}"].upload(filename)
 
     def resource_event(self, filename):
         if filename not in self.resources:
             md5 = get_digest(filename)
             self.resources[filename] = md5
```

### Comparing `neptune_sacred-1.0.0/src/neptune_sacred/impl/version.py` & `neptune_sacred-1.0.1/src/neptune_sacred/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_sacred-1.0.0/PKG-INFO` & `neptune_sacred-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-sacred
-Version: 1.0.0
+Version: 1.0.1
 Summary: Neptune.ai sacred integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -50,57 +50,60 @@
 
 * Log, display, organize, and compare ML experiments in a single place
 * Version, store, manage, and query trained models, and model building metadata
 * Record and monitor model training, evaluation, or production runs live
 
 ## What will be logged to Neptune?
 
-* Hyper-parameters
-* Losses & metrics
-* Training code(Python scripts or Jupyter notebooks) and git information
+* Hyperparameters
+* Losses and metrics
+* Training code (Python scripts or Jupyter notebooks) and Git information
 * Dataset version
-* Model Configuration
-* [Other metadata](https://docs.neptune.ai/you-should-know/what-can-you-log-and-display)
+* Model configuration
+* [Other metadata](https://docs.neptune.ai/logging/what_you_can_log)
 
 ![image](https://user-images.githubusercontent.com/97611089/160633857-48aa87ac-fcab-4225-8172-05aba159feaf.png)
-*Example custom dashboard in the Neptune UI*
-
+*Example custom dashboard in the Neptune app*
 
 ## Resources
 
-* [Documentation](https://docs.neptune.ai/integrations-and-supported-tools/experiment-tracking/sacred)
+* [Documentation](https://docs.neptune.ai/integrations/sacred)
 * [Code example on GitHub](https://github.com/neptune-ai/examples/tree/main/integrations-and-supported-tools/sacred/scripts)
-* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/sacred-integration/e/SAC-11/dashboard/Sacred-Dashboard-6741ab33-825c-4b25-8ebb-bb95c11ca3f4)
+* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/sacred-integration/e/SAC-1341/dashboard/Sacred-Dashboard-6741ab33-825c-4b25-8ebb-bb95c11ca3f4)
 * [Run example in Google Colab](https://colab.research.google.com/github/neptune-ai/examples/blob/main/integrations-and-supported-tools/sacred/notebooks/Neptune_Sacred.ipynb)
 
 ## Example
 
-```python
-# On the command line:
-pip install neptune-client[sacred] sacred torch torchvision
+On the command line:
+
 ```
-```python
-# In Python:
-import neptune.new as neptune
+pip install neptune-sacred
+```
+
+In Python:
 
+```python
+import neptune
 
 # Start a run
-run = neptune.init(project = "common/sacred-integration",
-                   api_token = "ANONYMOUS")
+run = neptune.init_run(
+    project = "common/sacred-integration",
+    api_token = neptune.ANONYMOUS_API_TOKEN,
+)
 
-# Create a sacred experiment
+# Create a Sacred experiment
 experiment = Experiment("image_classification", interactive=True)
 
 # Add NeptuneObserver and run the experiment
-experiment.observers.append(NeptuneObserver(run=neptune_run))
+experiment.observers.append(NeptuneObserver(run=run))
 experiment.run()
 ```
 
 ## Support
 
 If you got stuck or simply want to talk to us, here are your options:
 
-* Check our [FAQ page](https://docs.neptune.ai/getting-started/getting-help#frequently-asked-questions)
+* Check our [FAQ page](https://docs.neptune.ai/getting_help)
 * You can submit bug reports, feature requests, or contributions directly to the repository.
 * Chat! When in the Neptune application click on the blue message icon in the bottom-right corner and send a message. A real person will talk to you ASAP (typically very ASAP),
 * You can just shoot us an email at support@neptune.ai
```

