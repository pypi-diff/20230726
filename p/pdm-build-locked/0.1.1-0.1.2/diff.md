# Comparing `tmp/pdm_build_locked-0.1.1.tar.gz` & `tmp/pdm_build_locked-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_build_locked-0.1.1.tar", last modified: Mon Jul 24 21:57:06 2023, max compression
+gzip compressed data, was "pdm_build_locked-0.1.2.tar", last modified: Wed Jul 26 05:36:53 2023, max compression
```

## Comparing `pdm_build_locked-0.1.1.tar` & `pdm_build_locked-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/LICENSE
--rw-r--r--   0        0        0     1017 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/README.rst
--rw-r--r--   0        0        0     2052 2023-07-24 21:57:06.426361 pdm_build_locked-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      515 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/src/pdm_build_locked/__init__.py
--rw-r--r--   0        0        0     7678 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/src/pdm_build_locked/command.py
--rw-r--r--   0        0        0        0 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2176 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0      200 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/data/invalid/pyproject.toml
--rw-r--r--   0        0        0   117717 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/data/large/pdm.lock
--rw-r--r--   0        0        0     1896 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/data/large/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/data/large/src/large/__init__.py
--rw-r--r--   0        0        0      221 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/data/simple-optional/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/data/simple/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     7138 2023-07-24 21:56:45.678324 pdm_build_locked-0.1.1/tests/unit/test_build_locked.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 pdm_build_locked-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1017 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/README.rst
+-rw-r--r--   0        0        0     2052 2023-07-26 05:36:53.770502 pdm_build_locked-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      515 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/src/pdm_build_locked/__init__.py
+-rw-r--r--   0        0        0     6916 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/src/pdm_build_locked/command.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2176 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      200 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/tests/data/invalid/pyproject.toml
+-rw-r--r--   0        0        0   117717 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/large/pdm.lock
+-rw-r--r--   0        0        0     1896 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/large/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/large/src/large/__init__.py
+-rw-r--r--   0        0        0      221 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/simple-optional/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/simple/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     7138 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/unit/test_build_locked.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 pdm_build_locked-0.1.2/PKG-INFO
```

### Comparing `pdm_build_locked-0.1.1/LICENSE` & `pdm_build_locked-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/README.rst` & `pdm_build_locked-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/pyproject.toml` & `pdm_build_locked-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 authors = [
     { name = "sigma67", email = "sigma67.github@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
-version = "0.1.1"
+version = "0.1.2"
 
 [project.entry-points.pdm]
 pdm-build-locked = "pdm_build_locked:plugin"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `pdm_build_locked-0.1.1/src/pdm_build_locked/__init__.py` & `pdm_build_locked-0.1.2/src/pdm_build_locked/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/src/pdm_build_locked/command.py` & `pdm_build_locked-0.1.2/src/pdm_build_locked/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """pdm build --locked command"""
 import argparse
 import subprocess
 from contextlib import suppress
-from typing import Dict, List, Set, Tuple, Union
+from typing import Dict, List, Tuple, Union
 
 from pdm.cli import actions
 from pdm.cli.commands.build import Command as BaseCommand
 from pdm.exceptions import PdmException
 from pdm.models.candidates import Candidate
-from pdm.models.requirements import Requirement, parse_requirement
+from pdm.models.requirements import Requirement
 from pdm.project.core import Project
+from pdm.resolver import resolve
+from resolvelib import BaseReporter
 
 DependencyList = Dict[str, Union[List[str], Dict[str, List[str]]]]
 
 # copied from pdm.models.repository due to TYPECHECKING guard
 CandidateKey = Tuple[str, Union[str, None], Union[str, None], bool]
 
 
@@ -51,46 +53,41 @@
 
         ###################
         # update lockfile
         ###################
         self._update_lockfile(project)
 
         # retrieve locked dependencies and write to pyproject
-        optional_dependencies: Dict[str, Set[str]] = {}
+        optional_dependencies: Dict[str, List[str]] = {}
 
         ###############################
         # determine locked dependencies
         ###############################
         # performance optimization: we prepare the data structure here instead of searching inside the loop
         locked_package_version: Dict[str, Tuple[CandidateKey, Candidate]] = {}
         for package_key, package in project.locked_repository.packages.items():
             locked_package_version[str(package.name)] = (package_key, package)
 
         for group in groups:
-            group_name = self._get_locked_group_name(group)
-            optional_dependencies[group_name] = set()
+            locked_group_name = self._get_locked_group_name(group)
 
-            for dependency in project.all_dependencies[group].values():
-                locked_packages = self._get_locked_packages(project, locked_package_version, str(dependency.name))
-                optional_dependencies[group_name].update(locked_packages)
+            locked_packages = self._get_locked_packages(project, group)
+            optional_dependencies[locked_group_name] = locked_packages
 
         ####################
         # write to pyproject
         ####################
-        # transform sets to list for target project.pyproject.metadata
-        optional_dependencies_pyproject = dict((key, list(value)) for key, value in optional_dependencies.items())
-        optional_dependencies_pyproject.update(project.pyproject.metadata.get("optional-dependencies", {}))
 
         # get reference to optional-dependencies in project.pyproject, or create it if it doesn't exist
         optional = project.pyproject.metadata.get(
             "optional-dependencies", None
         ) or project.pyproject.metadata.setdefault("optional-dependencies", {})
 
         # update target
-        optional.update(optional_dependencies_pyproject)
+        optional.update(optional_dependencies)
         project.pyproject.write()
 
         # to prevent unclean scm status, we need to ignore pyproject.toml during build
         self._git_ignore_pyproject(project, True)
 
         ################
         # build project
@@ -137,49 +134,36 @@
         group_name = "locked"
         if group != "default":
             group_name = f"{group}-{group_name}"
 
         return group_name
 
     @staticmethod
-    def _get_locked_packages(
-        project: Project, locked_package_version: Dict[str, Tuple[CandidateKey, Candidate]], pkg: str
-    ) -> Set[str]:
+    def _get_locked_packages(project: Project, group: str) -> List[str]:
         """
-        Recursively determine locked dependency strings
-        For
-
-        Target: the locked optional-dependency groups in pyproject.toml
+        Determine locked dependency strings for direct and transitive dependencies
 
         Args:
             project: the pdm Project
-            locked_package_version: data structure based on current lockfile mapping package name to lockfile Candidate
-            pkg: package name
+            group: the group to get pinned dependencies for
 
         Returns:
             Set of locked packages
         """
-        locked_packages: Set[str] = set()
-        pkg = pkg.lower()
-
-        package_key, package = locked_package_version[pkg]
+        requirements: Dict[str, Requirement] = project.get_dependencies(group)
 
-        # lock self
-        locked_packages.add(str(package.req))  # pdm Requirement classes implement __repr__
-
-        # lock self requirements, if any
-        reqs, _, _ = project.locked_repository.candidate_info[package_key]
-        sub_dependencies: List[Requirement] = list(map(parse_requirement, reqs))
-        for sub_dependency in sub_dependencies:
-            # recursing into self for each sub-package
-            locked_packages.update(
-                BuildCommand._get_locked_packages(project, locked_package_version, str(sub_dependency.name))
-            )
+        # taken from pdm.actions.resolve_candidates_from_lockfile and adjusted so
+        # that environment markers are not evaluated
+        # -- we want to publish all requirements with markers
+        provider = project.get_provider(ignore_compatibility=True)
+        resolver = project.core.resolver_class(provider, BaseReporter())  # type: ignore
+        reqs = list(requirements.values())
+        candidates, *_ = resolve(resolver, reqs, project.environment.python_requires)
 
-        return locked_packages
+        return [str(c.req) for c in candidates.values()]
 
     @staticmethod
     def _git_ignore_pyproject(project: Project, ignore: bool = True) -> None:
         """
         set the git index status of pyproject.toml if the project uses scm-based versioning
         Note: currently only git is supported - will crash if git repo is not present
```

### Comparing `pdm_build_locked-0.1.1/tests/conftest.py` & `pdm_build_locked-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/tests/data/large/pdm.lock` & `pdm_build_locked-0.1.2/tests/data/large/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/tests/data/large/pyproject.toml` & `pdm_build_locked-0.1.2/tests/data/large/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/tests/unit/test_build_locked.py` & `pdm_build_locked-0.1.2/tests/unit/test_build_locked.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.1/PKG-INFO` & `pdm_build_locked-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-build-locked
-Version: 0.1.1
+Version: 0.1.2
 Summary: \
                 pdm-build-locked is a pdm plugin to add locked packages as additional optional dependency groups
                 to the distribution metadata
             
 Keywords: pdm plugin
 Author-Email: sigma67 <sigma67.github@gmail.com>
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

