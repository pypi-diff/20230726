# Comparing `tmp/e2xauthoring-0.1.0.tar.gz` & `tmp/e2xauthoring-0.2.0.dev0.tar.gz`

## Comparing `e2xauthoring-0.1.0.tar` & `e2xauthoring-0.2.0.dev0.tar`

### file list

```diff
@@ -1,22 +1,63 @@
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/lerna.json
--rw-r--r--   0        0        0  1694405 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/package-lock.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/package.json
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/.github/workflows/sonarcloud.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/__version__.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/utils.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/app/__init__.py
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/app/apihandlers.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/app/authoring.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/app/handlers.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/assets/.gitignore
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/models/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/models/taskmodel.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/e2xauthoring/models/taskpoolmodel.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 e2xauthoring-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/MANIFEST.in
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/lerna.json
+-rw-r--r--   0        0        0  1694428 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/package-lock.json
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/package.json
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/.github/workflows/sonarcloud.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/__version__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/authoring.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/apihandlers.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/base.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/handlers.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/assets/.gitignore
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/converters/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/converters/converter.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/converters/generateexercise.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/assignmentmodel.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/basemodel.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/exercisemodel.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presetmodel.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskmodel.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskpoolmodel.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/templatemodel.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/dataclasses/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/dataclasses/message.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/dataclasses/template.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/lister.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/taskpoollister.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/templatelister.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/manager.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/taskmanager.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/taskpoolmanager.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/templatemanager.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/addtaskheader.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/copyfiles.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/copynotebooks.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/filltemplate.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/generatetaskids.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/makeexercise.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/removeexercise.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/utils/__init__.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/utils/gitutils.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/utils/notebookvariableextractor.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/LICENSE
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/PKG-INFO
```

### Comparing `e2xauthoring-0.1.0/package-lock.json` & `e2xauthoring-0.2.0.dev0/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.916659670885418%*

 * *Differences: {"'dependencies'": "{'@e2xauthoring/app': {'requires': {'@e2xauthoring/api': '0.2.0-dev0'}}}",*

 * * "'packages'": "{'': {'version': '0.2.0-dev0'}, 'packages/api': {'version': '0.2.0-dev0'}, "*

 * *               "'packages/app': {'version': '0.2.0-dev0', 'dependencies': {'@e2xauthoring/api': "*

 * *               "'0.2.0-dev0'}}}",*

 * * "'version'": "'0.2.0-dev0'"}*

```diff
@@ -1361,15 +1361,15 @@
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/api"
         },
         "@e2xauthoring/app": {
             "requires": {
-                "@e2xauthoring/api": "*",
+                "@e2xauthoring/api": "0.2.0-dev0",
                 "@emotion/react": "^11.10.0",
                 "@emotion/styled": "^11.10.0",
                 "@fontsource/roboto": "^4.5.8",
                 "@mui/icons-material": "^5.8.4",
                 "@mui/material": "^5.10.0",
                 "@mui/x-data-grid": "^5.15.2",
                 "@mui/x-date-pickers": "^5.0.0-beta.5",
@@ -17715,15 +17715,15 @@
             "devDependencies": {
                 "lerna": "^5.3.0",
                 "prettier": "^2.7.1"
             },
             "hasInstallScript": true,
             "license": "MIT",
             "name": "e2xauthoring",
-            "version": "0.1.0.dev0",
+            "version": "0.2.0-dev0",
             "workspaces": [
                 "packages/*"
             ]
         },
         "node_modules/@adobe/css-tools": {
             "integrity": "sha512-+u76oB43nOHrF4DDWRLWDCtci7f3QJoEBigemIdIeTi1ODqjx6Tad9NCVnPRwewWlKkVab5PlK8DCtPTyX7S8g==",
             "resolved": "https://registry.npmjs.org/@adobe/css-tools/-/css-tools-4.0.1.tgz",
@@ -42129,19 +42129,19 @@
         "packages/api": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xauthoring/api",
-            "version": "0.1.0.dev0"
+            "version": "0.2.0-dev0"
         },
         "packages/app": {
             "dependencies": {
-                "@e2xauthoring/api": "*",
+                "@e2xauthoring/api": "0.2.0-dev0",
                 "@emotion/react": "^11.10.0",
                 "@emotion/styled": "^11.10.0",
                 "@fontsource/roboto": "^4.5.8",
                 "@mui/icons-material": "^5.8.4",
                 "@mui/material": "^5.10.0",
                 "@mui/x-data-grid": "^5.15.2",
                 "@mui/x-date-pickers": "^5.0.0-beta.5",
@@ -42158,13 +42158,13 @@
                 "web-vitals": "^2.1.4",
                 "yup": "^0.32.11"
             },
             "devDependencies": {
                 "react-app-rewired": "^2.2.1"
             },
             "name": "@e2xauthoring/app",
-            "version": "0.1.0"
+            "version": "0.2.0-dev0"
         }
     },
     "requires": true,
-    "version": "0.1.0.dev0"
+    "version": "0.2.0-dev0"
 }
```

### Comparing `e2xauthoring-0.1.0/package.json` & `e2xauthoring-0.2.0.dev0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.0-dev0'"}*

```diff
@@ -25,12 +25,12 @@
     },
     "scripts": {
         "build": "lerna run build",
         "install": "lerna run bootstrap",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:files": "prettier --write"
     },
-    "version": "0.1.0.dev0",
+    "version": "0.2.0-dev0",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `e2xauthoring-0.1.0/.github/workflows/sonarcloud.yml` & `e2xauthoring-0.2.0.dev0/.github/workflows/sonarcloud.yml`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.1.0/e2xauthoring/utils.py` & `e2xauthoring-0.2.0.dev0/e2xauthoring/utils/gitutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,24 @@
         Repo(path, search_parent_directories=True)
         return True
     except InvalidGitRepositoryError:
         return False
 
 
 def vcs_status(path: str, relative: bool = False) -> Dict[str, Union[List[str], bool]]:
-
     """Get the version control status of a path
 
     Args:
         path (str): Path to check
-        relative (bool, optional): Turn paths into relative paths starting at path. Defaults to False.
+        relative (bool, optional): Turn paths into relative paths starting at path.
+                                   Defaults to False.
 
     Returns:
-        dict: A dictionary containing untracked files, unstaged files and staged files under the path
+        dict: A dictionary containing untracked files, unstaged files and staged files
+              under the path
     """
     if not is_version_controlled(path):
         return dict(repo=None)
     repo = Repo(path, search_parent_directories=True)
     # Get the general status of the repository
     status = dict(
         repo=repo,
@@ -86,15 +87,16 @@
     author: Actor = None,
 ) -> bool:
     """Commit all files in a given path
 
     Args:
         repo (Repo): A git repository instance
         path (str): The path to commit
-        add_if_untracked (bool, optional): If untracked files should be added before committing. Defaults to False.
+        add_if_untracked (bool, optional): If untracked files should be added before committing.
+        Defaults to False.
         message (str, optional): The commit message. Defaults to None.
         author (Actor, optional): An author object to specify the author of the commit.
                                   If not set the global git author will be used. Defaults to None.
 
     Returns:
         bool: status
     """
@@ -115,35 +117,37 @@
 
 def create_repository(path: str, exists_ok: bool = True, author: Actor = None) -> Repo:
     """Create a repository
     Intitializes the repository with a gitignore if it does not exists
 
     Args:
         path (str): The base path of the repository
-        exists_ok (bool, optional): If the repository already exists do not throw an exception. Defaults to True.
-        author (Actor, optional): author (Actor, optional): An author object to specify the author of the commit.
+        exists_ok (bool, optional): If the repository already exists do not throw an exception.
+                                    Defaults to True.
+        author (Actor, optional): An author object to specify the author of the commit.
                                   If not set the global git author will be used. Defaults to None.
 
     Returns:
         Repo: _description_
     """
     path = os.path.abspath(path)
     repo = None
     try:
         repo = Repo(path, search_parent_directories=True)
-        assert (
-            exists_ok
-        ), f"A repository already exists at {repo.working_tree_dir}. Run with option exists_ok=True to ignore."
+        assert exists_ok, (
+            f"A repository already exists at {repo.working_tree_dir}."
+            "Run with option exists_ok=True to ignore."
+        )
         return repo
     except InvalidGitRepositoryError:
         repo = Repo.init(path)
     here = os.path.dirname(__file__)
     gitignore = ".gitignore"
     shutil.copy(
-        os.path.join(here, "assets", gitignore),
+        os.path.join(here, "..", "assets", gitignore),
         os.path.join(repo.working_tree_dir, gitignore),
     )
     repo.git.add([gitignore])
     command = [f"-m 'Add {gitignore}'"]
     if author is not None:
         command.append(f"--author='{author.name} <{author.email}'")
     command.append(gitignore)
```

### Comparing `e2xauthoring-0.1.0/e2xauthoring/app/apihandlers.py` & `e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/apihandlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,75 @@
 import json
+import os
 
-from e2xgrader.converters import GenerateExercise
-from e2xgrader.models import AssignmentModel, TemplateModel
-from e2xgrader.server_extensions.grader.apps.authoring.apihandlers import (
-    BaseApiListHandler,
-    BaseApiManageHandler,
-    E2xApiHandler,
-    ExerciseModel,
-    KernelSpecHandler,
-    PresetHandler,
-    TemplateVariableHandler,
-    api_url,
-    assignment_regex,
-    name_regex,
-    pool_regex,
-)
-from e2xgrader.utils import urljoin
+from e2xcore.handlers import E2xApiHandler
+from e2xcore.utils import urljoin
+from jupyter_client.kernelspec import KernelSpecManager
 from nbgrader.server_extensions.formgrader.base import check_xsrf
 from tornado import web
 
-from e2xauthoring.utils import get_author, set_author
+from ...converters import GenerateExercise
+from ...models import (
+    AssignmentModel,
+    ExerciseModel,
+    PresetModel,
+    TaskModel,
+    TaskPoolModel,
+    TemplateModel,
+)
+from ...utils import NotebookVariableExtractor
+from ...utils.gitutils import get_author, set_author
+from .base import BaseApiListHandler, BaseApiManageHandler
+
+
+class PresetHandler(E2xApiHandler):
+    def initialize(self):
+        self.__model = PresetModel(self.coursedir)
+
+    def _list_template(self):
+        self.write(json.dumps(self.__model.list_template_presets()))
+
+    def _get_template(self):
+        name = self.get_argument("name")
+        self.write(json.dumps(self.__model.get_template_preset(name)))
+
+    def _list_question(self):
+        self.write(json.dumps(self.__model.list_question_presets()))
+
+    def _get_question(self):
+        name = self.get_argument("name")
+        self.write(json.dumps(self.__model.get_question_preset(name)))
+
+    @web.authenticated
+    @check_xsrf
+    def get(self):
+        action = self.get_argument("action")
+        preset_type = self.get_argument("type")
+        handler = getattr(self, "_{}_{}".format(action, preset_type))
+        handler()
+
+
+class TemplateVariableHandler(E2xApiHandler):
+    @web.authenticated
+    @check_xsrf
+    def get(self):
+        template = self.get_argument("template")
+        variables = NotebookVariableExtractor().extract(
+            os.path.join(
+                self.url_prefix, "templates", template, "{}.ipynb".format(template)
+            )
+        )
+        self.write(json.dumps(variables))
+
 
-from ..models import TaskModel, TaskPoolModel
+class KernelSpecHandler(E2xApiHandler):
+    @web.authenticated
+    @check_xsrf
+    def get(self):
+        self.write(json.dumps(KernelSpecManager().get_all_specs()))
 
 
 class ManagePoolsHandler(E2xApiHandler):
     def initialize(self) -> None:
         self.__poolmodel = TaskPoolModel(self.coursedir)
 
     @web.authenticated
@@ -181,14 +225,17 @@
     def post(self):
         data = self.get_json_body()
         name = data.get("name")
         email = data.get("email")
         self.write(json.dumps(set_author(name=name, email=email)))
 
 
+api_url = urljoin("e2x", "authoring", "api")
+name_regex = r"(?P<name>[^/]+)"
+assignment_regex = r"(?P<assignment>[^/]+)"
 pool_action_regex = r"(?P<action>new|list|remove|get|init_repo)"
 task_action_regex = r"(?P<action>new|list|list_all|remove|commit|get|diff)"
 template_action_regex = r"(?P<action>new|list|remove)"
 default_handlers = [
     (urljoin(api_url, "presets"), PresetHandler),
     (
         urljoin(api_url, "assignments", "?"),
```

### Comparing `e2xauthoring-0.1.0/e2xauthoring/app/authoring.py` & `e2xauthoring-0.2.0.dev0/e2xauthoring/app/authoring.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 
-from e2xgrader.server_extensions.grader.apps.base import BaseApp
+from e2xcore import BaseApp
 from nbgrader.apps.baseapp import NbGrader
 from tornado import web
 
-from .apihandlers import default_handlers
-from .handlers import default_handlers as handlers
+from .handlers.apihandlers import default_handlers
+from .handlers.handlers import default_handlers as handlers
 
 
 class AuthoringApp(NbGrader, BaseApp):
-
     template_path = os.path.join(os.path.dirname(__file__), "templates")
     static_path = os.path.join(template_path, "authoring", "static")
 
     def __init__(self, **kwargs) -> None:
         NbGrader.__init__(self, **kwargs)
         BaseApp.__init__(self, **kwargs)
```

### Comparing `e2xauthoring-0.1.0/e2xauthoring/app/handlers.py` & `e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import sys
-from email.policy import default
 
-from e2xgrader.server_extensions.grader.apps.authoring.handlers import app_url
-from e2xgrader.utils import urljoin
+from e2xcore.utils import urljoin
 from nbgrader.server_extensions.formgrader.base import (
     BaseHandler,
     check_notebook_dir,
     check_xsrf,
 )
 from tornado import web
 
+app_url = urljoin("e2x", "authoring", "app")
+
 
 class AuthoringHandler(BaseHandler):
     @web.authenticated
     @check_xsrf
     @check_notebook_dir
     def get(self):
         self.write(
```

### Comparing `e2xauthoring-0.1.0/e2xauthoring/assets/.gitignore` & `e2xauthoring-0.2.0.dev0/e2xauthoring/assets/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.1.0/e2xauthoring/models/taskpoolmodel.py` & `e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskpoolmodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,71 @@
 import os
+import shutil
 import traceback as tb
 from typing import Dict
 
-from e2xgrader.models import TaskPoolModel as E2xTaskPoolModel
+from traitlets import Unicode
 
-from ..utils import create_repository, is_version_controlled
+from ..utils.gitutils import create_repository, is_version_controlled
+from .basemodel import BaseModel
+
+
+class E2xTaskPoolModel(BaseModel):
+    directory = Unicode("pools", help="The directory where the task pools go.")
+
+    def new(self, **kwargs):
+        name = kwargs["name"]
+        if self.is_valid_name(name):
+            path = os.path.join(self.base_path(), name)
+            if os.path.exists(path):
+                return {
+                    "success": False,
+                    "error": f"A pool with the name {name} already exists!",
+                }
+            else:
+                os.makedirs(path, exist_ok=True)
+                return {"success": True, "path": path}
+        else:
+            return {"success": False, "error": "Invalid name"}
+
+    def remove(self, **kwargs):
+        name = kwargs["name"]
+        path = os.path.join(self.base_path(), name)
+        shutil.rmtree(path)
+
+    def get(self, **kwargs):
+        name = kwargs["name"]
+        tasks = self.__get_pool_info(name)
+        return {
+            "name": name,
+            "tasks": tasks,
+            "link": os.path.join("taskcreator", "pools", name),
+        }
+
+    def list(self, **kwargs):
+        if not os.path.isdir(self.base_path()):
+            os.makedirs(self.base_path(), exist_ok=True)
+        poolfolders = os.listdir(self.base_path())
+        pools = []
+        for poolfolder in poolfolders:
+            if poolfolder.startswith("."):
+                continue
+            tasks = self.__get_pool_info(poolfolder)
+            pools.append(
+                {
+                    "name": poolfolder,
+                    "tasks": tasks,
+                    "link": os.path.join("taskcreator", "pools", poolfolder),
+                }
+            )
+
+        return pools
+
+    def __get_pool_info(self, name):
+        return len(os.listdir(os.path.join(self.base_path(), name)))
 
 
 class TaskPoolModel(E2xTaskPoolModel):
     def new(self, **kwargs) -> Dict[str, str]:
         """Create a new task pool
 
         Returns:
```

### Comparing `e2xauthoring-0.1.0/.gitignore` & `e2xauthoring-0.2.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.1.0/LICENSE` & `e2xauthoring-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.1.0/PKG-INFO` & `e2xauthoring-0.2.0.dev0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: e2xauthoring
-Version: 0.1.0
+Version: 0.2.0.dev0
 Summary: Authoring app for e2xgrader
 Project-URL: Source, https://github.com/Digiklausur/e2xauthoring
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
-Requires-Dist: e2xgrader==0.1.*
+Requires-Dist: e2xcore==0.0.2
 Requires-Dist: gitpython
 Provides-Extra: dev
 Requires-Dist: hatchling; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: tbump; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # e2xauthoring
 
 ---
 
-This is an authoring component for e2xgrader
+This is an authoring component for e2xgrader
```

