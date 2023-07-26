# Comparing `tmp/hamburg-1.0.1.tar.gz` & `tmp/hamburg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamburg-1.0.1.tar", max compression
+gzip compressed data, was "hamburg-1.1.0.tar", max compression
```

## Comparing `hamburg-1.0.1.tar` & `hamburg-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-03-29 12:27:06.839222 hamburg-1.0.1/LICENSE
--rw-r--r--   0        0        0    10506 2023-03-29 12:27:06.839222 hamburg-1.0.1/README.md
--rw-r--r--   0        0        0      380 2023-03-29 12:27:06.839222 hamburg-1.0.1/hamburg/__init__.py
--rw-r--r--   0        0        0      281 2023-03-29 12:27:06.839222 hamburg-1.0.1/hamburg/exceptions.py
--rw-r--r--   0        0        0     6255 2023-03-29 12:27:06.839222 hamburg-1.0.1/hamburg/hamburg.py
--rw-r--r--   0        0        0     5991 2023-03-29 12:27:06.839222 hamburg-1.0.1/hamburg/models.py
--rw-r--r--   0        0        0        0 2023-03-29 12:27:06.839222 hamburg-1.0.1/hamburg/py.typed
--rw-r--r--   0        0        0     3833 2023-03-29 12:27:26.395340 hamburg-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12034 1970-01-01 00:00:00.000000 hamburg-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-26 19:26:49.828276 hamburg-1.1.0/LICENSE
+-rw-r--r--   0        0        0    10830 2023-07-26 19:26:49.828276 hamburg-1.1.0/README.md
+-rw-r--r--   0        0        0     3745 2023-07-26 19:27:04.432382 hamburg-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-07-26 19:26:49.828276 hamburg-1.1.0/src/hamburg/__init__.py
+-rw-r--r--   0        0        0      281 2023-07-26 19:26:49.828276 hamburg-1.1.0/src/hamburg/exceptions.py
+-rw-r--r--   0        0        0     6031 2023-07-26 19:26:49.828276 hamburg-1.1.0/src/hamburg/hamburg.py
+-rw-r--r--   0        0        0     6089 2023-07-26 19:26:49.832276 hamburg-1.1.0/src/hamburg/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:26:49.832276 hamburg-1.1.0/src/hamburg/py.typed
+-rw-r--r--   0        0        0    12158 1970-01-01 00:00:00.000000 hamburg-1.1.0/PKG-INFO
```

### Comparing `hamburg-1.0.1/LICENSE` & `hamburg-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hamburg-1.0.1/README.md` & `hamburg-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
 [![PyPi Downloads][downloads-shield]][downloads-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
 
 [![Code Quality][code-quality-shield]][code-quality]
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
 [![Maintainability][maintainability-shield]][maintainability-url]
 [![Code Coverage][codecov-shield]][codecov-url]
@@ -142,16 +141,22 @@
 We've set up a separate document for our
 [contribution guidelines](CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up development environment
 
-This Python project is fully managed using the [Poetry][poetry] dependency
-manager.
+The simplest way to begin is by utilizing the [Dev Container][devcontainer]
+feature of Visual Studio Code or by opening a CodeSpace directly on GitHub.
+By clicking the button below you immediately start a Dev Container in Visual Studio Code.
+
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
+
+This Python project relies on [Poetry][poetry] as its dependency manager,
+providing comprehensive management and control over project dependencies.
 
 You need at least:
 
 - Python 3.9+
 - [Poetry][poetry-install]
 
 Install all packages, including all development requirements:
@@ -226,29 +231,27 @@
 [build-url]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-hamburg.svg
 [commits-url]: https://github.com/klaasnicolaas/python-hamburg/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-hamburg/branch/main/graph/badge.svg?token=4Y4YAYHR2D
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-hamburg
+[devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-hamburg
 [downloads-shield]: https://img.shields.io/pypi/dm/hamburg
 [downloads-url]: https://pypistats.org/packages/hamburg
-[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-hamburg.svg
-[issues-url]: https://github.com/klaasnicolaas/python-hamburg/issues
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-hamburg.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-hamburg.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/5041849456b7348f3bc7/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-hamburg/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/hamburg/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/hamburg
 [typing-shield]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml
 [releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-hamburg.svg
 [releases]: https://github.com/klaasnicolaas/python-hamburg/releases
-[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-hamburg.svg
-[stars-url]: https://github.com/klaasnicolaas/python-hamburg/stargazers
 
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com
```

### Comparing `hamburg-1.0.1/hamburg/hamburg.py` & `hamburg-1.1.0/src/hamburg/hamburg.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,23 +111,19 @@
             limit: Number of items to return.
             bulk: Whether to return all items or the limit.
 
         Returns:
         -------
             A list of DisabledParking objects.
         """
-        results: list[DisabledParking] = []
         locations = await self._request(
             "behindertenstellplaetze/collections/verkehr_behindertenparkpl/items",
             params={"limit": limit, "bulk": bulk},
         )
-
-        for item in locations["features"]:
-            results.append(DisabledParking.from_dict(item))
-        return results
+        return [DisabledParking.from_dict(item) for item in locations["features"]]
 
     async def park_and_rides(
         self,
         limit: int = 10,
         bulk: str = "false",
     ) -> list[ParkAndRide]:
         """Get all park and ride spaces.
@@ -137,22 +133,19 @@
             limit: Number of items to return.
             bulk: Whether to return all items or the limit.
 
         Returns:
         -------
             A list of ParkAndRide objects.
         """
-        results: list[ParkAndRide] = []
         locations = await self._request(
             "p_und_r/collections/p_und_r/items",
             params={"limit": limit, "bulk": bulk},
         )
-        for item in locations["features"]:
-            results.append(ParkAndRide.from_dict(item))
-        return results
+        return [ParkAndRide.from_dict(item) for item in locations["features"]]
 
     async def garages(
         self,
         limit: int = 10,
         bulk: str = "false",
         available: str | None = None,
     ) -> list[Garage]:
@@ -164,30 +157,30 @@
             bulk: Whether to return all items or the limit.
             available: Filter based on availability with operators.
 
         Returns:
         -------
             A list of Garage objects.
         """
-        results: list[Garage] = []
         params: dict[str, Any] = {"limit": limit, "bulk": bulk}
 
         if available is not None:
             params["frei"] = str(available)
 
         locations = await self._request(
             "parkhaeuser/collections/verkehr_parkhaeuser/items",
             params=params,
         )
 
-        for item in locations["features"]:
-            # By default filter out garages without location coordinates.
-            if item["geometry"] is not None:
-                results.append(Garage.from_dict(item))
-        return results
+        # By default filter out garages without location coordinates.
+        return [
+            Garage.from_dict(item)
+            for item in locations["features"]
+            if item["geometry"] is not None
+        ]
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> UDPHamburg:
```

### Comparing `hamburg-1.0.1/hamburg/models.py` & `hamburg-1.1.0/src/hamburg/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,24 +98,27 @@
         return cls(
             spot_id=str(data.get("id")),
             name=attr.get("name"),
             park_type=attr.get("art"),
             address=attr.get("adresse"),
             construction_year=attr.get("baujahr"),
             public_transport_line=attr.get("linie"),
-            disabled_parking_spaces=attr.get("stellplaetze_behinderte_gesamt"),
+            disabled_parking_spaces=int(attr.get("stellplaetze_behinderte_gesamt")),
             tickets={
                 "day": attr.get("ticket_1_tag"),
                 "month": attr.get("ticket_30_tage"),
                 "year": attr.get("ticket_1_jahr"),
             },
             url=attr.get("homepage"),
-            free_space=attr.get("stellplaetze_frei"),
-            capacity=attr.get("stellplaetze_gesamt"),
-            availability_pct=round(attr.get("stellpl_frei_in_prozent"), 1),
+            free_space=int(attr.get("stellplaetze_frei")),
+            capacity=int(attr.get("stellplaetze_gesamt")),
+            availability_pct=availability_calc(
+                attr.get("stellplaetze_frei"),
+                attr.get("stellplaetze_gesamt"),
+            ),
             longitude=geo[0],
             latitude=geo[1],
             updated_at=datetime.strptime(
                 attr.get("aktualitaet_belegungsdaten"),
                 "%Y-%m-%d %H:%M:%S",
             ).astimezone(pytz.timezone("Europe/Berlin")),
         )
```

### Comparing `hamburg-1.0.1/pyproject.toml` & `hamburg-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,140 +1,133 @@
 [tool.poetry]
 name = "hamburg"
-version = "1.0.1"
+version = "1.1.0"
 description = "Asynchronous Python client providing Urban Data information of Hamburg"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-hamburg"
 repository = "https://github.com/klaasnicolaas/python-hamburg"
 documentation = "https://github.com/klaasnicolaas/python-hamburg"
 keywords = ["urban", "data", "platform", "hamburg", "parking", "api", "async", "client"]
 classifiers = [
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "hamburg" }
+  { include = "hamburg", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 pytz = ">=2022.7.1,<2024.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-hamburg/issues"
 Changelog = "https://github.com/klaasnicolaas/python-hamburg/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.254,<0.0.260"
-aresponses = "^2.1.6"
-black = "^23.1"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.2"
-coverage = {version = "^7.2", extras = ["toml"]}
-mypy = "^1.1"
-pre-commit = "^3.1.1"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.16.4"
-pytest = "^7.2.2"
-pytest-asyncio = ">=0.20.3,<0.22.0"
-pytest-cov = "^4.0.0"
-yamllint = "^1.29.0"
-covdefaults = "^2.3.0"
-types-pytz = ">=2022.7.1.2,<2024.0.0.0"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["hamburg"]
+ruff = "0.0.280"
+aresponses = "2.1.6"
+black = "23.7.0"
+blacken-docs = "1.15.0"
+codespell = "2.2.5"
+coverage = {version = "7.2.7", extras = ["toml"]}
+mypy = "1.4.1"
+pre-commit = "3.3.3"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.5"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.1"
+pytest-cov = "4.1.0"
+yamllint = "1.32.0"
+covdefaults = "2.3.0"
+types-pytz = "2023.3.0.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["hamburg"]
 
+[tool.coverage.report]
+fail_under = 90
+show_missing = true
+
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.9"
 
+# flake8-mypy expects the two following for sensible formatting
+show_column_numbers = true
+
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_defs = true
 disallow_untyped_decorators = true
+disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.pylint.MASTER]
-extension-pkg-whitelist = [
-  "pydantic"
-]
-ignore= [
-  "tests"
-]
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
 ]
 
-[tool.pylint.DESIGN]
-max-attributes=15
-
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
+
+[tool.pylint.DESIGN]
+max-attributes = 15
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -154,9 +147,9 @@
 [tool.ruff.isort]
 known-first-party = ["hamburg"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `hamburg-1.0.1/PKG-INFO` & `hamburg-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamburg
-Version: 1.0.1
+Version: 1.1.0
 Summary: Asynchronous Python client providing Urban Data information of Hamburg
 Home-page: https://github.com/klaasnicolaas/python-hamburg
 License: MIT
 Keywords: urban,data,platform,hamburg,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -14,18 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: pytz (>=2022.7.1,<2024.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-hamburg/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-hamburg/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-hamburg
@@ -41,16 +37,15 @@
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
 [![PyPi Downloads][downloads-shield]][downloads-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
 
 [![Code Quality][code-quality-shield]][code-quality]
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
 [![Maintainability][maintainability-shield]][maintainability-url]
 [![Code Coverage][codecov-shield]][codecov-url]
@@ -176,16 +171,22 @@
 We've set up a separate document for our
 [contribution guidelines](CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up development environment
 
-This Python project is fully managed using the [Poetry][poetry] dependency
-manager.
+The simplest way to begin is by utilizing the [Dev Container][devcontainer]
+feature of Visual Studio Code or by opening a CodeSpace directly on GitHub.
+By clicking the button below you immediately start a Dev Container in Visual Studio Code.
+
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
+
+This Python project relies on [Poetry][poetry] as its dependency manager,
+providing comprehensive management and control over project dependencies.
 
 You need at least:
 
 - Python 3.9+
 - [Poetry][poetry-install]
 
 Install all packages, including all development requirements:
@@ -260,30 +261,28 @@
 [build-url]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-hamburg.svg
 [commits-url]: https://github.com/klaasnicolaas/python-hamburg/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-hamburg/branch/main/graph/badge.svg?token=4Y4YAYHR2D
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-hamburg
+[devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-hamburg
 [downloads-shield]: https://img.shields.io/pypi/dm/hamburg
 [downloads-url]: https://pypistats.org/packages/hamburg
-[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-hamburg.svg
-[issues-url]: https://github.com/klaasnicolaas/python-hamburg/issues
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-hamburg.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-hamburg.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/5041849456b7348f3bc7/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-hamburg/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/hamburg/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/hamburg
 [typing-shield]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml
 [releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-hamburg.svg
 [releases]: https://github.com/klaasnicolaas/python-hamburg/releases
-[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-hamburg.svg
-[stars-url]: https://github.com/klaasnicolaas/python-hamburg/stargazers
 
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com
```

