# Comparing `tmp/corporate_reputation-0.7.1.tar.gz` & `tmp/corporate_reputation-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.7.1.tar", max compression
+gzip compressed data, was "corporate_reputation-0.8.0.tar", max compression
```

## Comparing `corporate_reputation-0.7.1.tar` & `corporate_reputation-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-07-25 00:30:01.415885 corporate_reputation-0.7.1/LICENSE
--rw-r--r--   0        0        0     3898 2023-07-25 00:30:01.415885 corporate_reputation-0.7.1/README.md
--rw-r--r--   0        0        0     3045 2023-07-25 00:30:44.408557 corporate_reputation-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      182 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/__cli__.py
--rw-r--r--   0        0        0      484 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-07-25 00:30:44.352556 corporate_reputation-0.7.1/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/absa/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/absa/agent.py
--rw-r--r--   0        0        0     4793 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/absa/config.py
--rw-r--r--   0        0        0        0 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      286 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/about/corprep.yaml
--rw-r--r--   0        0        0      259 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/absa/default.yaml
--rw-r--r--   0        0        0     2930 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/absa/prompts/default.yaml
--rw-r--r--   0        0        0      294 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/absa_agent_predict.yaml
--rw-r--r--   0        0        0      274 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/dataset_filter.yaml
--rw-r--r--   0        0        0      163 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/dataset_load_raw.yaml
--rw-r--r--   0        0        0      276 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/dataset_tokenize.yaml
--rw-r--r--   0        0        0      204 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/__init__.py
--rw-r--r--   0        0        0     1665 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/io.py
--rw-r--r--   0        0        0      617 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/sample.py
--rw-r--r--   0        0        0     1790 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/similarity.py
--rw-r--r--   0        0        0     1039 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/tokenize.py
--rw-r--r--   0        0        0        0 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/py.typed
--rw-r--r--   0        0        0  2355775 2023-07-25 00:30:01.435886 corporate_reputation-0.7.1/src/corprep/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0     4811 1970-01-01 00:00:00.000000 corporate_reputation-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-26 19:11:27.879430 corporate_reputation-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3898 2023-07-26 19:11:27.879430 corporate_reputation-0.8.0/README.md
+-rw-r--r--   0        0        0     3324 2023-07-26 19:12:03.036127 corporate_reputation-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      484 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-26 19:12:02.992127 corporate_reputation-0.8.0/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/absa/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/absa/agent.py
+-rw-r--r--   0        0        0     4793 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/absa/config.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/about/corprep.yaml
+-rw-r--r--   0        0        0      259 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/absa/default.yaml
+-rw-r--r--   0        0        0     2930 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/absa/prompts/default.yaml
+-rw-r--r--   0        0        0      113 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/pipe/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      156 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/pipe/dataset_filter.yaml
+-rw-r--r--   0        0        0      107 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/pipe/dataset_load_raw.yaml
+-rw-r--r--   0        0        0      230 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/run/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      171 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/run/filter_dataset.yaml
+-rw-r--r--   0        0        0      138 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/run/load_raw_dataset.yaml
+-rw-r--r--   0        0        0      204 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/io.py
+-rw-r--r--   0        0        0     1790 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/similarity.py
+-rw-r--r--   0        0        0     2606 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/tokenize.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/py.typed
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 corporate_reputation-0.8.0/PKG-INFO
```

### Comparing `corporate_reputation-0.7.1/LICENSE` & `corporate_reputation-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.1/README.md` & `corporate_reputation-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.1/pyproject.toml` & `corporate_reputation-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.7.1"
+version = "0.8.0"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
 
 [tool.poetry.scripts]
 corprep = 'corprep.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.9.3"
+hyfi = "^1.11.0"
 openai = "^0.27.8"
 backoff = "^2.2.1"
 scikit-learn = "^1.3.0"
-lexikanon = "^0.2.3"
+lexikanon = "^0.3.1"
+# lexikanon = { path = "../lexikanon", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
@@ -33,28 +34,64 @@
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe]
 include = [".tasks.toml", ".tasks-extra.toml"]
 
 [tool.black]
-exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+exclude = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.isort]
 profile = "black"
-skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+skip = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.flake8]
 ignore = ['F401', 'E501', 'W503']
-exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "_build",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
-exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "build",
+    "_build",
+    "dist",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = true
 disallow_any_expr = false
 disallow_any_decorated = false
 disallow_any_explicit = true
@@ -87,22 +124,21 @@
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/corprep/_version.py:__version__"
 version_source = "tag"
-commit_version_number = true # required for version_source = "tag"
+commit_version_number = true                                    # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-hvcs = "github" # hosting version control system, gitlab is also supported
+hvcs = "github"                                                 # hosting version control system, gitlab is also supported
 build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `corporate_reputation-0.7.1/src/corprep/absa/agent.py` & `corporate_reputation-0.8.0/src/corprep/absa/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 
 def predict(
     dataset: Dataset,
     tasks=None,
     absa_config_name: str = "default",
     text_col: str = "bodyText",
-    batch_size=2,
-    num_workers=1,
+    batch_size: int = 1000,
+    num_workers: int = 1,
     remove_columns: Optional[Union[List[str], str]] = None,
     load_from_cache_file=True,
     verbose=False,
 ) -> Dataset:
     if tasks is None:
         tasks = ["QUAD"]
     for task in tasks:
```

### Comparing `corporate_reputation-0.7.1/src/corprep/absa/config.py` & `corporate_reputation-0.8.0/src/corprep/absa/config.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.1/src/corprep/conf/absa/prompts/default.yaml` & `corporate_reputation-0.8.0/src/corprep/conf/absa/prompts/default.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.1/src/corprep/datasets/io.py` & `corporate_reputation-0.8.0/src/corprep/datasets/io.py`

 * *Files 27% similar despite different names*

```diff
@@ -30,38 +30,7 @@
     logger.info("Number of training samples: %s", len(ds_train))
     if verbose:
         print(ds_train[99])
         print(ds_train[-99])
         logger.info("Dataset features: %s", ds_train.features)
 
     return ds_train
-
-
-def save_dataset(
-    data: Dataset,
-    dataset_path: Union[str, Path],
-) -> Dataset:
-    """
-    Save a dataset.
-    """
-    data.save_to_disk(dataset_path)
-    logger.info("Dataset saved to %s.", dataset_path)
-
-    return data
-
-
-def load_dataset(
-    dataset_path: str,
-    verbose: bool = False,
-) -> Dataset:
-    """
-    Save a dataset.
-    """
-    data = Dataset.load_from_disk(dataset_path)
-    logger.info("Dataset loaded from %s.", dataset_path)
-    if verbose:
-        print(data[0])
-        print(data[-1])
-        logger.info("Dataset features: %s", data.features)
-        logger.info("Number of samples: %s", len(data))
-
-    return data
```

### Comparing `corporate_reputation-0.7.1/src/corprep/datasets/similarity.py` & `corporate_reputation-0.8.0/src/corprep/datasets/similarity.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.1/PKG-INFO` & `corporate_reputation-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.7.1
+Version: 0.8.0
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: hyfi (>=1.9.3,<2.0.0)
-Requires-Dist: lexikanon (>=0.2.3,<0.3.0)
+Requires-Dist: hyfi (>=1.11.0,<2.0.0)
+Requires-Dist: lexikanon (>=0.3.1,<0.4.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
```

