# Comparing `tmp/gitease-0.0.8.tar.gz` & `tmp/gitease-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.8.tar", last modified: Thu Jun 29 07:11:00 2023, max compression
+gzip compressed data, was "gitease-0.0.9.tar", max compression
```

## Comparing `gitease-0.0.8.tar` & `gitease-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,10 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.244374 gitease-0.0.8/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.8/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4174 2023-06-28 15:37:04.000000 gitease-0.0.8/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      708 2023-06-27 15:09:45.000000 gitease-0.0.8/.readthedocs.yaml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1068 2023-06-27 15:09:45.000000 gitease-0.0.8/LICENSE
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4565 2023-06-29 07:11:00.243933 gitease-0.0.8/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3288 2023-06-28 15:51:28.000000 gitease-0.0.8/README.md
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.224067 gitease-0.0.8/docs/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      634 2023-06-19 19:56:47.000000 gitease-0.0.8/docs/Makefile
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1131 2023-06-29 07:10:17.000000 gitease-0.0.8/docs/conf.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.224333 gitease-0.0.8/docs/images/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)   154160 2023-06-28 15:51:00.000000 gitease-0.0.8/docs/images/logo.png
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2153 2023-06-27 15:17:54.000000 gitease-0.0.8/docs/index.rst
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      800 2023-06-19 19:56:47.000000 gitease-0.0.8/docs/make.bat
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.225576 gitease-0.0.8/docs/markdowns/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      261 2023-06-27 15:09:45.000000 gitease-0.0.8/docs/markdowns/quickstart.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)    10378 2023-06-28 15:37:04.000000 gitease-0.0.8/docs/markdowns/usage.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       90 2023-06-27 15:09:45.000000 gitease-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.226870 gitease-0.0.8/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.8/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     6146 2023-06-28 15:37:04.000000 gitease-0.0.8/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4420 2023-06-28 15:37:04.000000 gitease-0.0.8/gitease/git_helper.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2772 2023-06-28 15:37:04.000000 gitease-0.0.8/gitease/llm_helper.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.228701 gitease-0.0.8/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      956 2023-06-28 15:37:04.000000 gitease-0.0.8/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.8/gitease/prompts/undo_template.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.228234 gitease-0.0.8/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4565 2023-06-29 07:10:56.000000 gitease-0.0.8/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      703 2023-06-29 07:11:00.000000 gitease-0.0.8/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-29 07:10:56.000000 gitease-0.0.8/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-29 07:10:56.000000 gitease-0.0.8/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      111 2023-06-29 07:10:56.000000 gitease-0.0.8/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-29 07:10:56.000000 gitease-0.0.8/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1579 2023-06-29 07:10:17.000000 gitease-0.0.8/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.8/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-29 07:11:00.244460 gitease-0.0.8/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-29 07:11:00.230303 gitease-0.0.8/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.8/tests/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2505 2023-06-28 15:37:04.000000 gitease-0.0.8/tests/cli_test.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2478 2023-06-28 15:37:04.000000 gitease-0.0.8/tests/git_helper_test.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      754 2023-06-28 15:37:04.000000 gitease-0.0.8/tests/llm_helper_test.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      208 2023-06-28 15:37:04.000000 gitease-0.0.8/tests/util_tests.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      423 2023-06-28 15:37:04.000000 gitease-0.0.8/tests/utils.py
+-rw-r--r--   0        0        0     1068 2023-06-27 15:09:45.444353 gitease-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3415 2023-07-26 07:59:14.925092 gitease-0.0.9/README.md
+-rw-r--r--   0        0        0        2 2023-06-14 15:01:01.677790 gitease-0.0.9/gitease/__init__.py
+-rw-r--r--   0        0        0     6630 2023-07-26 07:59:14.926252 gitease-0.0.9/gitease/cli.py
+-rw-r--r--   0        0        0     4665 2023-07-26 07:59:14.926718 gitease-0.0.9/gitease/git_helper.py
+-rw-r--r--   0        0        0     2772 2023-06-28 15:37:04.142653 gitease-0.0.9/gitease/llm_helper.py
+-rw-r--r--   0        0        0      956 2023-06-28 15:37:04.143247 gitease-0.0.9/gitease/prompts/prompt_template.txt
+-rw-r--r--   0        0        0      157 2023-06-15 11:21:54.034848 gitease-0.0.9/gitease/prompts/undo_template.txt
+-rw-r--r--   0        0        0     1607 2023-07-26 08:32:32.353962 gitease-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 gitease-0.0.9/PKG-INFO
```

### Comparing `gitease-0.0.8/LICENSE` & `gitease-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gitease-0.0.8/PKG-INFO` & `gitease-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to simplfy git operations
-Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
-Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
+Author: Yonatan Alexander
+Author-email: yonatan@xethub.com
+Maintainer: XetHub
+Maintainer-email: contact@xethub.com
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Classifier: Topic :: System :: Filesystems
+Requires-Dist: gitpython (>=3.1.32,<4.0.0)
+Requires-Dist: langchain (>=0.0.242,<0.0.243)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 <p align="center">
    <img src="https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png" alt="logo" width="400" />
 </p>
 
 
 # GitEase
 [![Version](https://img.shields.io/pypi/v/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Python](https://img.shields.io/pypi/pyversions/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
-[![License](https://img.shields.io/github/license/xetdata/gitease?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
 [![Downloads](https://img.shields.io/pypi/dm/gitease?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Documentation Status](https://readthedocs.org/projects/gitease/badge/?version=latest)](https://gitease.readthedocs.io/en/latest/?badge=latest)
 
 
 A tool to simplify git usage with sprinkles of AI magic.
 
 Humans think in simpler terms than git operates in. This tool aims to bridge that gap by providing a simpler language to
@@ -106,15 +115,18 @@
 # Add multiple files
 ge save -a README.md -a gitease/cli.py
 
 # Add and commits everything without prompting for validation
 ge save -y
 
 # Add the README.md file and commit with a generated message
-ge share -a README.md -y 
+ge share -a README.md -y
+
+# Add and commit README.md file with "upload readme" message and merges to main
+ge share -a README.md -m "upload readme" --merge=main 
 
 # Pull recent changes from git
 ge load
 ```
 
 ```bash
 $ ge undo
```

### Comparing `gitease-0.0.8/README.md` & `gitease-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    <img src="https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png" alt="logo" width="400" />
 </p>
 
 
 # GitEase
 [![Version](https://img.shields.io/pypi/v/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Python](https://img.shields.io/pypi/pyversions/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
-[![License](https://img.shields.io/github/license/xetdata/gitease?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
 [![Downloads](https://img.shields.io/pypi/dm/gitease?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Documentation Status](https://readthedocs.org/projects/gitease/badge/?version=latest)](https://gitease.readthedocs.io/en/latest/?badge=latest)
 
 
 A tool to simplify git usage with sprinkles of AI magic.
 
 Humans think in simpler terms than git operates in. This tool aims to bridge that gap by providing a simpler language to
@@ -77,15 +77,18 @@
 # Add multiple files
 ge save -a README.md -a gitease/cli.py
 
 # Add and commits everything without prompting for validation
 ge save -y
 
 # Add the README.md file and commit with a generated message
-ge share -a README.md -y 
+ge share -a README.md -y
+
+# Add and commit README.md file with "upload readme" message and merges to main
+ge share -a README.md -m "upload readme" --merge=main 
 
 # Pull recent changes from git
 ge load
 ```
 
 ```bash
 $ ge undo
```

### Comparing `gitease-0.0.8/gitease/cli.py` & `gitease-0.0.9/gitease/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,19 +107,28 @@
         helper.stage(staged_at_start)
 
 
 @cli.command()
 def share(add: add_annotation = None,
           message: message_annotation = None,
           quiet: quiet_annotation = False,
-          y: y_annotation = False):
+          y: y_annotation = False,
+          merge: Annotated[str, typer.Option("--merge", help="A branch to merge after pushing")] = None):
     """Share to remote: add, commit and push to git"""
     save(add=add, message=message, quiet=quiet, y=y)
-    GitHelper(verbose=not quiet).push()
+    helper = GitHelper(verbose=not quiet)
+    helper.push()
     console.print("Pushed changes to the cloud", style=Style(color="green", blink=True, bold=True))
+    if merge:
+        branch = helper.get_current_branch()
+        helper.checkout(merge)
+        helper.merge(branch)
+        helper.push()
+        console.print(f"Merged {branch} into {merge}", style=Style(color="green", blink=True, bold=True))
+        console.print(f"You are now on branch {merge}", style=Style(color="yellow", blink=True, bold=True))
 
 
 @cli.command()
 def load():
     """Pull recent updates from git"""
     console.print(GitHelper().pull(), style=Style(color="yellow", blink=True, bold=True))
 
@@ -143,15 +152,15 @@
 
 @cli.command()
 def undo():
     """Undo last git action"""
     llm = LanguageModel()
     reflog = "\n".join(GitHelper().reflog().split("\n")[0])
     last_action = llm.get_git_undo(reflog)
-    console.print(f"Last git action is: [purple]{last_action.action}[/purple]", style=Style(color="yellow"))
+    console.print(f"The last git action is: [purple]{last_action.action}[/purple]", style=Style(color="yellow"))
     console.print(f"A revert command is: [red]{last_action.revert_command}[/red]", style=Style(color="yellow"))
     response = Prompt.ask("Shell I run the command for you?", choices=["y", "n"])
     if response == "y":
         console.print(f"Running: '{last_action.revert_command}'", style=Style(color="red"))
         os.system(last_action.revert_command)
     if response == "n":
         console.print("Ok, Bye!", style=Style(color="green"))
```

### Comparing `gitease-0.0.8/gitease/git_helper.py` & `gitease-0.0.9/gitease/git_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,29 +124,36 @@
             return diff
 
         return "Diff too long to summarize."
 
     def reflog(self):
         return self.repo.git.reflog('show')
 
-
-    def reset(self, hard: bool = False, commit:str=None ):
-        args =[]
+    def reset(self, hard: bool = False, commit: str = None):
+        args = []
         if hard:
             args.append('--hard')
         if commit:
             args.append(commit)
         return self.repo.git.reset(*args)
 
-    def remove(self, files: List[str] = None, commit:str=None):
+    def remove(self, files: List[str] = None, commit: str = None):
         """
         Removes the files.
          :param files: The files to remove.
          :param commit: The commit message.
         """
         if not files:
             return False
         commit = commit or f"Removed files - {files}"
         self.repo.index.remove(files)
         self.repo.index.commit(commit)
         return True
 
+    def get_current_branch(self):
+        return self.repo.active_branch.name
+
+    def checkout(self, branch: str):
+        return self.repo.git.checkout(branch)
+
+    def merge(self, branch: str):
+        return self.repo.git.merge(branch)
```

### Comparing `gitease-0.0.8/gitease/llm_helper.py` & `gitease-0.0.9/gitease/llm_helper.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.8/gitease/prompts/prompt_template.txt` & `gitease-0.0.9/gitease/prompts/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.8/pyproject.toml` & `gitease-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[project]
+[tool.poetry]
 name = "gitease"
-version = "0.0.8"
+version = "0.0.9"
 description = "A tool to simplfy git operations"
 readme = "README.md"
+packages = [{ include = "gitease" }]
+authors = ["Yonatan Alexander <yonatan@xethub.com>"]
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
     "git",
     "nlp",
 ]
-license = { text = "BSD-3-Clause" }
-maintainers = [{ name = "XetHub", email = "contact@xethub.com" }]
-requires-python = ">=3.7"
+license = "BSD-3-Clause"
+maintainers = ["XetHub <contact@xethub.com>"]
+
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -33,24 +35,24 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Filesystems",
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
-dependencies = [
-    "openai>=0.27.7",
-    "typer>=0.9.0",
-    "rich>=13.4.2",
-    "langchain>=0.0.191",
-    "GitPython>=3.1.31",
-    "tiktoken>=0.4.0",
-    "pyperclip>=1.8.2"
-]
+
+[tool.poetry.dependencies]
+python = "^3.8.1"
+openai = "^0.27.8"
+typer = "^0.9.0"
+rich = "^13.4.2"
+langchain = "^0.0.242"
+gitpython = "^3.1.32"
+tiktoken = "^0.4.0"
+pyperclip = "^1.8.2"
 
 [project.urls]
 Homepage = "https://xethub.com/xdssio/gitease"
 
 
 [project.scripts]
-ge = "gitease.cli:cli"
-
+ge = "gitease.cli:cli"
```

