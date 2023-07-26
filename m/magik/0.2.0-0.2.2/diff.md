# Comparing `tmp/magik-0.2.0.tar.gz` & `tmp/magik-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.2.0.tar", last modified: Thu Jul 20 20:10:31 2023, max compression
+gzip compressed data, was "magik-0.2.2.tar", last modified: Wed Jul 26 12:55:20 2023, max compression
```

## Comparing `magik-0.2.0.tar` & `magik-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.270813 magik-0.2.0/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-20 20:10:31.270652 magik-0.2.0/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     5580 2023-07-19 22:37:02.000000 magik-0.2.0/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.269606 magik-0.2.0/magik/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.2.0/magik/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1844 2023-07-20 17:04:56.000000 magik-0.2.0/magik/classifier.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2478 2023-07-19 22:36:56.000000 magik-0.2.0/magik/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-20 08:24:46.000000 magik-0.2.0/magik/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-18 19:22:52.000000 magik-0.2.0/magik/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      617 2023-07-19 22:36:56.000000 magik-0.2.0/magik/decorators.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1403 2023-07-19 22:36:56.000000 magik-0.2.0/magik/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)    12700 2023-07-20 19:58:37.000000 magik-0.2.0/magik/evaluators.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.270496 magik-0.2.0/magik/examples/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.2.0/magik/examples/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1295 2023-07-19 22:36:56.000000 magik-0.2.0/magik/examples/assertions.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1385 2023-07-19 22:36:56.000000 magik-0.2.0/magik/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-19 22:36:56.000000 magik-0.2.0/magik/initialize.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.2.0/magik/internal_logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      895 2023-07-20 20:01:05.000000 magik-0.2.0/magik/logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.2.0/magik/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1248 2023-07-20 12:39:03.000000 magik-0.2.0/magik/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     8190 2023-07-20 20:02:29.000000 magik-0.2.0/magik/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      897 2023-07-20 12:53:40.000000 magik-0.2.0/magik/similarity.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-19 22:36:56.000000 magik-0.2.0/magik/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1539 2023-07-19 22:36:56.000000 magik-0.2.0/magik/utils.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.270301 magik-0.2.0/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      578 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/top_level.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-20 20:10:31.270850 magik-0.2.0/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-20 20:08:26.000000 magik-0.2.0/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.832035 magik-0.2.2/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-26 12:55:20.831847 magik-0.2.2/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     5580 2023-07-19 22:37:02.000000 magik-0.2.2/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.830821 magik-0.2.2/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.2.2/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1844 2023-07-26 12:54:23.000000 magik-0.2.2/magik/classifier.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2622 2023-07-26 12:54:23.000000 magik-0.2.2/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-20 08:24:46.000000 magik-0.2.2/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      662 2023-07-26 12:54:23.000000 magik-0.2.2/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      617 2023-07-22 21:10:23.000000 magik-0.2.2/magik/decorators.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1867 2023-07-26 12:54:23.000000 magik-0.2.2/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)    12979 2023-07-26 12:54:23.000000 magik-0.2.2/magik/evaluators.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.831708 magik-0.2.2/magik/examples/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.2.2/magik/examples/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1295 2023-07-19 22:36:56.000000 magik-0.2.2/magik/examples/assertions.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1385 2023-07-19 22:36:56.000000 magik-0.2.2/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3007 2023-07-26 12:54:23.000000 magik-0.2.2/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-25 12:50:52.000000 magik-0.2.2/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1001 2023-07-26 12:54:23.000000 magik-0.2.2/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.2.2/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1248 2023-07-26 12:54:23.000000 magik-0.2.2/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     8900 2023-07-26 12:54:23.000000 magik-0.2.2/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      822 2023-07-26 12:54:23.000000 magik-0.2.2/magik/similarity.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-19 22:36:56.000000 magik-0.2.2/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1539 2023-07-19 22:36:56.000000 magik-0.2.2/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.831502 magik-0.2.2/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      578 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-26 12:55:20.832078 magik-0.2.2/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-26 12:54:23.000000 magik-0.2.2/setup.py
```

### Comparing `magik-0.2.0/PKG-INFO` & `magik-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.2.0
+Version: 0.2.2
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `magik-0.2.0/README.md` & `magik-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/classifier.py` & `magik-0.2.2/magik/classifier.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/cli.py` & `magik-0.2.2/magik/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import argparse
 from magik.initialize import initialize
 from magik.generate import generate_test
 from magik.deploy import deploy_test
 from magik.internal_logger import logger
+from magik.constants import TEST_DIR, TEST_RUNS_DIR
 from magik.run import Run
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="magik", description="Magik testing suite CLI tool"
     )
@@ -57,24 +58,24 @@
 
 
 def generate(args):
     generate_test(args.test_name)
 
 
 def run(args):
-    test_runner = Run()
+    test_runner = Run(test_dir=TEST_DIR, test_runs_dir=TEST_RUNS_DIR)
     test_runner.run_tests(args.test_name)
 
 
 def deploy(args):
     deploy_test(args.test_name)
 
 
 def run_prod(args):
-    test_runner = Run()
+    test_runner = Run(test_dir=TEST_DIR, test_runs_dir=TEST_RUNS_DIR)
     test_runner.run_tests_in_prod(
         start_date=args.start_date,
         end_date=args.end_date,
         prompt_slug=args.prompt_slug,
         test_slug=args.test_name,
     )
```

### Comparing `magik-0.2.0/magik/constants.py` & `magik-0.2.2/magik/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # API URLs
 API_BASE_URL = "https://api.magiklabs.app"
 DEPLOY_URL = f"{API_BASE_URL}/api/v1/testDeploy"
-RUN_URL = f"{API_BASE_URL}/api/v1/testRun/group"
+RUN_URL = f"{API_BASE_URL}/api/v1/testRun/trigger/byPromptSlug"
 
 # Directory paths
 TEST_DIR = "./magik_tests/tests"
-TESTRUNS_DIR = "./magik_tests/test_runs"
+TEST_RUNS_DIR = "./magik_tests/test_runs"
 CONFIG_FILE_PATH = f"./magik_tests/magik_config.json"
+SCHEDULE_CONFIG_FILE_PATH = f"./magik_tests/schedule.json"
 MAGIK_SDK_DIR = "./magik"  # TODO: This should come from the directory that one will have on running pip install magik
 EXAMPLES_DIR = f"{MAGIK_SDK_DIR}/examples"
 EXAMPLE_CONFIG_PATH = f"{EXAMPLES_DIR}/magik_config.example.json"
 
 # Open AI defaults
 OPEN_AI_DEFAULT_MODEL = "gpt-3.5-turbo"
```

### Comparing `magik-0.2.0/magik/decorators.py` & `magik-0.2.2/magik/decorators.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/deploy.py` & `magik-0.2.2/magik/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import json
 import os
 import requests
 from magik.internal_logger import logger
-from magik.constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR
+from magik.constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR, TEST_RUNS_DIR
+from magik.run import Run
 from magik.config import get_magik_api_key
 
 
 def deploy_test(test_name: str):
     api_key = get_magik_api_key()
     if api_key == None:
         logger.error(f"No API key found. Please add your API key to {CONFIG_FILE_PATH}")
@@ -19,20 +21,28 @@
         return
 
     # read file
     with open(file_path, "rb") as f:
         file_content = f.read()
 
     # prepare data for API request
+    test_runner = Run(test_dir=TEST_DIR, test_runs_dir=TEST_RUNS_DIR)
+    test_context = test_runner._load_context(test_name)
+    tests = test_runner._load_tests(test_name=test_name, test_context=test_context)
+    tests = list(map(lambda test: {**test, "eval": test["eval"].__name__}, tests))
+
     headers = {"magik-api-key": api_key}
-    data = {"testId": test_name}
-    files = {"file": ("assertions.py", file_content)}
+    data = {"test_slug": test_name, "test_data": tests}
+    files = {
+        "file": ("assertions.py", file_content, "application/octet-stream"),
+        "json": (None, json.dumps(data), "application/json"),
+    }
 
     # make a POST request to the API
-    response = requests.post(DEPLOY_URL, files=files, data=data, headers=headers)
+    response = requests.post(DEPLOY_URL, files=files, headers=headers)
 
     # check the response
     if response.status_code == 200:
         logger.info(f"Successfully uploaded {file_path}")
     else:
         logger.info(
             f"Failed to upload {file_path}. Status code: {response.status_code}"
```

### Comparing `magik-0.2.0/magik/evaluators.py` & `magik-0.2.2/magik/evaluators.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,14 @@
     """
     return grade_using_llm(sentiment_grading_prompt)(output_to_test)
 
 
 @magik_eval
 def contains_link(output_to_test=None):
     pattern = r"(?!.*@)(?:https?://)?(?:www\.)?\S+\.\S+"
-    print("output_to_test", output_to_test)
     result = bool(re.search(pattern, output_to_test))
     if result:
         return {"result": True, "reason": "Link found in output"}
     else:
         return {"result": False, "reason": "No link found in output"}
 
 
@@ -345,15 +344,14 @@
 def cosine_similarity_above_threshold(
     compare_against: str,
     threshold: float,
     model="text-embedding-ada-002",
     output_to_test=None,
 ):
     score = similarity_score(output_to_test, compare_against, model)
-    print(f"score is {score}")
     result = score > threshold
     return {
         "result": result,
         "reason": f"cosine similarity score is {score} and is above threshold {threshold}",
     }
 
 
@@ -361,15 +359,14 @@
 def cosine_similarity_below_threshold(
     compare_against: str,
     threshold: float,
     model="text-embedding-ada-002",
     output_to_test=None,
 ):
     score = similarity_score(output_to_test, compare_against, model)
-    print(f"score is {score}")
     result = score < threshold
     return {
         "result": result,
         "reason": f"cosine similarity score is {score} and is below threshold {threshold}",
     }
 
 
@@ -388,7 +385,25 @@
         output_to_test=output_to_test,
     )
     result = label == desired_classification_label
     return {
         "result": result,
         "reason": f"output is classified as {label} and desired classification is {desired_classification_label}",
     }
+
+
+@magik_eval
+def api_call(
+    url: str,
+    payload: dict,
+    headers: dict = None,
+    output_to_test=None,
+):
+    payload["output_to_test"] = output_to_test
+    response = requests.post(url, json=payload, headers=headers)
+    result = response.json().get("result")
+    reason = response.json().get("reason")
+
+    return {
+        "result": result,
+        "reason": reason,
+    }
```

### Comparing `magik-0.2.0/magik/examples/assertions.py` & `magik-0.2.2/magik/examples/assertions.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/generate.py` & `magik-0.2.2/magik/generate.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/initialize.py` & `magik-0.2.2/magik/initialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import os
 from magik.internal_logger import logger
 from magik.sys_exec import write_to_file
 from magik.constants import (
-    TESTRUNS_DIR,
+    TEST_RUNS_DIR,
     TEST_DIR,
     CONFIG_FILE_PATH,
+    SCHEDULE_CONFIG_FILE_PATH,
 )
-from magik.sys_exec import read_from_file
 
 
 # Create magik_tests directory
 # Create magik_test_runs directory
-# Create magik_config.json
+# Create magik_tests/magik_config.json
+# Create magik_tests/schedule.json
 def initialize():
     _create_magik_tests_dir()
     _create_magik_test_runs_dir()
     _create_magik_config_file()
-    _add_config_file_to_gitignore()
+    _create_schedule_config_file()
 
 
 def _create_magik_tests_dir():
     if not os.path.exists(TEST_DIR):
         os.makedirs(TEST_DIR, exist_ok=True)
         logger.info(f"✅ Created {TEST_DIR} directory")
     else:
         logger.info(f"{TEST_DIR} directory already exists")
 
 
 def _create_magik_test_runs_dir():
-    if not os.path.exists(TESTRUNS_DIR):
-        os.makedirs(TESTRUNS_DIR, exist_ok=True)
-        logger.info(f"✅ Created {TESTRUNS_DIR} directory")
+    if not os.path.exists(TEST_RUNS_DIR):
+        os.makedirs(TEST_RUNS_DIR, exist_ok=True)
+        logger.info(f"✅ Created {TEST_RUNS_DIR} directory")
     else:
-        logger.info(f"{TESTRUNS_DIR} directory already exists")
+        logger.info(f"{TEST_RUNS_DIR} directory already exists")
 
 
 def _create_magik_config_file():
     # Check if magik_config.json already exists
     if os.path.exists(CONFIG_FILE_PATH):
         logger.info(f"{CONFIG_FILE_PATH} already exists!")
         return
@@ -50,25 +51,61 @@
 }"""
     write_to_file(
         CONFIG_FILE_PATH,
         example_config_contents,
     )
 
     logger.info(f"✅ Created {CONFIG_FILE_PATH} (config file)")
+
+    # add config file to gitignore
+    _add_to_gitignore()
+
     logger.info("")
     logger.log_with_color(
         f"IMP: Please fill in the API keys in {CONFIG_FILE_PATH}", "yellow"
     )
     logger.info("")
 
 
-def _add_config_file_to_gitignore():
+def _create_schedule_config_file():
+    # Check if magik_config.json already exists
+    if os.path.exists(SCHEDULE_CONFIG_FILE_PATH):
+        logger.info(f"{SCHEDULE_CONFIG_FILE_PATH} already exists!")
+        return
+
+    # Create file magik_config.json
+    logger.debug("Creating schedule_config.json...")
+
+    example_schedule_config_contents = """[
+  {
+    "trigger_type": "by-slug",
+    "trigger_data": [
+      {
+        "prompt_slug": "*",
+        "test_slugs": "*"
+      }
+    ]
+  }
+]"""
+    write_to_file(
+        SCHEDULE_CONFIG_FILE_PATH,
+        example_schedule_config_contents,
+    )
+
+    logger.info(f"✅ Created {SCHEDULE_CONFIG_FILE_PATH} (schedule config)")
+    logger.info("")
+
+
+def _add_to_gitignore():
     gitignore_path = ".gitignore"
     if not os.path.exists(gitignore_path):
         logger.info(f"{gitignore_path} does not exist!")
-        logger.info(f"Make sure to add {CONFIG_FILE_PATH} to your gitignore file")
+        logger.info(
+            f"Make sure to add {CONFIG_FILE_PATH} to your gitignore file")
         return
 
     with open(gitignore_path, "a") as gitignore_file:
-        gitignore_file.write("\n# Magik config file\nmagik_config.json\n")
+        gitignore_file.write(
+            "\n# Magik config file\nmagik_config.json\nmagik_tests/test_runs/*\n"
+        )
 
     logger.info(f"✅ Added {CONFIG_FILE_PATH} to {gitignore_path}")
```

### Comparing `magik-0.2.0/magik/internal_logger.py` & `magik-0.2.2/magik/internal_logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/logger.py` & `magik-0.2.2/magik/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 
 # Log the request and response from OpenAI chat completion to Magik API
 #
 # prompt_slug: name of the prompt for analytics and grouping
 # messages: "messages" json array sent to OpenAI chat completion
 # model: string id of the language model used
 # chat_completion: "choices" json response from OpenAI chat completion
-def log_open_ai_chat_response(prompt_slug, messages, model, chat_completion):
+def log_open_ai_chat_response(
+    prompt_slug, messages, model, chat_completion, response_time, context
+):
     """
     Track the request and response.
     """
     requests.post(
         f"{API_BASE_URL}/api/v1/savePromptAndResponse",
         json={
             "prompt_slug": prompt_slug,
             "prompt_data": messages,
             "language_model_id": model,
             "completion": chat_completion,
+            "response_time": response_time,
+            "context": context,
         },
         headers={
             "magik-api-key": get_magik_api_key(),
         },
     )
```

### Comparing `magik-0.2.0/magik/openai_helper.py` & `magik-0.2.2/magik/openai_helper.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/run.py` & `magik-0.2.2/magik/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 import importlib.util
 from datetime import datetime
 from magik.internal_logger import logger
 from magik.utils import substitute_vars
 from magik.openai_helper import OpenAI
 from magik.sys_exec import read_from_file, create_file
 from magik.config import get_open_ai_default_model, get_magik_api_key
-from magik.constants import TESTRUNS_DIR, TEST_DIR, RUN_URL
+from magik.constants import RUN_URL
 
 
 class Run:
-    def __init__(self):
+    def __init__(self, test_dir, test_runs_dir):
         self.saved_prompt_response = ""
+        self.test_dir = test_dir
+        self.test_runs_dir = test_runs_dir
 
     def run_tests(self, test_name):
-        tests = self._load_tests(test_name)
+        test_context = self._load_context(test_name)
+        tests = self._load_tests(test_name, test_context=test_context)
         raw_prompt = self._load_prompt(test_name)
-        log_file_path = self._log_file_path(test_name)
+        log_file_path = self._log_file_path()
         self._run_tests_for_prompt(
-            test_name, tests, raw_prompt, log_file_path=log_file_path
+            tests=tests, raw_prompt=raw_prompt, log_file_path=log_file_path
         )
 
     def run_tests_in_prod(self, start_date, end_date, prompt_slug, test_slug):
         request_data = {
             "source": "CLI",
             "start_date": start_date,
             "end_date": end_date,
@@ -46,26 +49,26 @@
                 "magik-api-key": get_magik_api_key(),
             },
         )
         if response.status_code != 200:
             logger.error(f"ERROR: Failed to trigger test in prod: {response.text}")
             return
 
-    def _run_tests_for_prompt(self, test_name, tests, raw_prompt, log_file_path):
+    def _run_tests_for_prompt(self, tests, raw_prompt, log_file_path):
         self._log_to_file_and_console("---------------")
         self._log_to_file_and_console("TEST RESULTS")
         self._log_to_file_and_console("---------------")
         self._log_to_file_and_console("\n")
 
         num_tests_passed = 0
         for test in tests:
-            test_result = self._run_individual_test_for_prompt(
-                test_name, test, raw_prompt, log_file_path
+            test_result_obj = self._run_individual_test_for_prompt(
+                test=test, raw_prompt=raw_prompt, log_file_path=log_file_path
             )
-            if test_result:
+            if test_result_obj["test_result"]["result"]:
                 num_tests_passed += 1
 
         num_tests_failed = len(tests) - num_tests_passed
 
         logger.info("\n------------")
         if num_tests_passed == len(tests):
             logger.info("✅ All tests passed")
@@ -74,17 +77,15 @@
             logger.info(
                 f"""
     ✅ {num_tests_passed}/{len(tests)} tests passed
     ❌ {num_tests_failed}/{len(tests)} tests failed
             """
             )
 
-    def _run_individual_test_for_prompt(
-        self, test_name, test, raw_prompt, log_file_path
-    ):
+    def _run_individual_test_for_prompt(self, test, raw_prompt, log_file_path):
         openai = OpenAI()
         prompt_vars = test["prompt_vars"]
         model = get_open_ai_default_model()
         if len(prompt_vars) == 0:
             prompt = raw_prompt
             if len(self.saved_prompt_response) == 0:
                 self.saved_prompt_response = openai.openai_chat_completion_message(
@@ -94,66 +95,86 @@
         else:
             prompt = substitute_vars(raw_prompt, prompt_vars)
             prompt_response = openai.openai_chat_completion_message(
                 model=model, prompt=prompt
             )
 
         return self._run_individual_test_for_prompt_response(
-            test_name, test, prompt, prompt_response, log_file_path=log_file_path
+            test=test,
+            prompt=prompt,
+            prompt_response=prompt_response,
+            log_file_path=log_file_path,
         )
 
     def _run_individual_test_for_prompt_response(
-        self, test_name, test, prompt, prompt_response, log_file_path
+        self, test, prompt, prompt_response, log_file_path
     ):
         test_function_result_obj = test["eval"](prompt_response)
         result_obj = self._generate_result_object(
             test=test,
             test_result=test_function_result_obj,
             prompt=prompt,
             prompt_response=prompt_response,
         )
 
         self._log_results(
             result_obj,
             log_file_path=log_file_path,
         )
 
-        return result_obj["test_result"]["result"]
+        return result_obj
 
     def _load_prompt(self, test_name):
-        test_file_path = f"{TEST_DIR}/{test_name}/prompt.txt"
+        test_file_path = f"{self.test_dir}/{test_name}/prompt.txt"
         absolute_path = os.path.abspath(test_file_path)
         return read_from_file(absolute_path)
 
-    def _load_tests(self, test_name):
-        test_file_path = f"{TEST_DIR}/{test_name}/assertions.py"
+    def _load_attr_from_test_file(self, test_name, attr_name, default_value=None):
+        test_file_path = f"{self.test_dir}/{test_name}/assertions.py"
         # Get the absolute path by resolving against the current working directory
         absolute_path = os.path.abspath(test_file_path)
 
         # Get the directory path and module name from the absolute path
         directory, module_name = os.path.split(absolute_path)
         module_name = os.path.splitext(module_name)[0]
 
         # Load the module dynamically
         spec = importlib.util.spec_from_file_location(module_name, absolute_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
 
         # Access the `tests` array from the module
-        return getattr(module, "tests", [])
+        return getattr(module, attr_name, default_value)
+
+    def _load_define_tests_fn(self, test_name):
+        return self._load_attr_from_test_file(
+            test_name=test_name, attr_name="define_tests", default_value=lambda _: []
+        )
+
+    def _load_context(self, test_name):
+        return self._load_attr_from_test_file(
+            test_name=test_name, attr_name="test_context", default_value=None
+        )
+
+    def _load_tests(self, test_name, test_context):
+        define_tests_fn = self._load_define_tests_fn(test_name)
+        return define_tests_fn(test_context)
+
+    def _generate_test_object(self, test):
+        test_function_name = test["eval"].__name__
+        return {
+            **test,
+            "eval": test_function_name,
+        }
 
     def _generate_result_object(self, test, test_result, prompt, prompt_response):
         did_test_pass = test_result["result"]
         failure_labels = test["failure_labels"] if not did_test_pass else []
-        test_function_name = test["eval"].__name__
         return {
-            "test": {
-                **test,
-                "eval": test_function_name,
-            },
+            "test": self._generate_test_object(test),
             "test_result": test_result,
             "prompt": prompt,
             "prompt_response": prompt_response,
             "failure_labels": failure_labels,
         }
 
     def _log_results(self, result_obj, log_file_path=None):
@@ -197,12 +218,10 @@
         failure_labels = result_obj["failure_labels"]
 
         self._log_to_file_and_console(f"Test Result: {test_result_str}", log_file)
         self._log_to_file_and_console(f"Reason: {test_result_reason}", log_file)
         self._log_to_file_and_console(f"Failure Labels: {failure_labels}", log_file)
         self._log_to_file_and_console("\n", log_file)
 
-    def _log_file_path(self, test_name):
-        current_timestamp = datetime.now()
-        formatted_timestamp = current_timestamp.strftime("%Y-%m-%d_%H-%M-%S")
-        log_file_path = f"{TESTRUNS_DIR}/{test_name}/{formatted_timestamp}.txt"
+    def _log_file_path(self):
+        log_file_path = f"{self.test_runs_dir}/log.txt"
         return log_file_path
```

### Comparing `magik-0.2.0/magik/similarity.py` & `magik-0.2.2/magik/similarity.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,11 @@
     similarity = dot_product / (magnitude_v1 * magnitude_v2)
 
     return similarity
 
 
 def similarity_score(str1, str2, model):
     openai = OpenAI()
-    # print(f"str1: {str1}")
-    # print(f"str2: {str2}")
-    # return 0.6
     e1 = openai.get_embedding(str1, model=model)
     e2 = openai.get_embedding(str2, model=model)
     score = _cosine_similarity_from_embeddings(e1, e2)
     return score
```

### Comparing `magik-0.2.0/magik/sys_exec.py` & `magik-0.2.2/magik/sys_exec.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik/utils.py` & `magik-0.2.2/magik/utils.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/magik.egg-info/PKG-INFO` & `magik-0.2.2/magik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.2.0
+Version: 0.2.2
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `magik-0.2.0/magik.egg-info/SOURCES.txt` & `magik-0.2.2/magik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magik-0.2.0/setup.py` & `magik-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.2.0",
+    version="0.2.2",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

