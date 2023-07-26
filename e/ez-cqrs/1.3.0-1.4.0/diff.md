# Comparing `tmp/ez_cqrs-1.3.0.tar.gz` & `tmp/ez_cqrs-1.4.0.tar.gz`

## Comparing `ez_cqrs-1.3.0.tar` & `ez_cqrs-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/README.md
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-1.4.0/PKG-INFO
```

### Comparing `ez_cqrs-1.3.0/.github/workflows/release.yml` & `ez_cqrs-1.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/.github/workflows/test.yml` & `ez_cqrs-1.4.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     runs-on: ${{ matrix.os }}
     permissions:
       contents: write
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest] # [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ steps.versions.outputs.python }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `ez_cqrs-1.3.0/.vscode/settings.json` & `ez_cqrs-1.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/ez_cqrs/acid_exec.py` & `ez_cqrs-1.4.0/ez_cqrs/acid_exec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 """ACID execution goodies."""
 from __future__ import annotations
 
 import abc
-import sys
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
-
-if sys.version_info >= (3, 8):
-    from typing import final
-else:
-    from typing_extensions import final
+from typing import TYPE_CHECKING, Any, Generic, TypeVar, final
 
 if TYPE_CHECKING:
     from result import Result
 
     from ez_cqrs.error import DatabaseError
```

### Comparing `ez_cqrs-1.3.0/ez_cqrs/components.py` & `ez_cqrs-1.4.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/ez_cqrs/error.py` & `ez_cqrs-1.4.0/ez_cqrs/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Error base class."""
 from __future__ import annotations
 
 import abc
-import sys
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, final
 
-if sys.version_info >= (3, 8):
-    from typing import final
-else:
-    from typing_extensions import final
 if TYPE_CHECKING:
+    import sys
+
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
         from typing_extensions import TypeAlias
 
 
 class DomainError(abc.ABC, Exception):
```

### Comparing `ez_cqrs-1.3.0/ez_cqrs/handler.py` & `ez_cqrs-1.4.0/ez_cqrs/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
         event_registry: list[E],
-    ) -> Result[tuple[Any, list[E]], ExecutionError]:
+    ) -> Result[Any, ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
 
         _All business logic belongs in this method_.
```

### Comparing `ez_cqrs-1.3.0/ez_cqrs/testing.py` & `ez_cqrs-1.4.0/ez_cqrs/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """Testing framework."""
 from __future__ import annotations
 
 import asyncio
-import sys
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Generic
+from typing import TYPE_CHECKING, Any, Generic, final
 
 from result import Ok, Result
 
-if sys.version_info >= (3, 8):
-    from typing import final
-else:
-    from typing_extensions import final
-
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import C, E
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from ez_cqrs.error import ExecutionError
```

### Comparing `ez_cqrs-1.3.0/ez_cqrs/utilities/cli.py` & `ez_cqrs-1.4.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/requirements/dev.txt` & `ez_cqrs-1.4.0/requirements/dev.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,98 +1,93 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --extra=dev --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=dev --output-file=requirements/dev.txt pyproject.toml
 #
---trusted-host pypi.python.org
---trusted-host pypi.org
---trusted-host files.pythonhosted.org
-
-black==23.3.0
+annotated-types==0.5.0
+    # via pydantic
+black==23.7.0
     # via pyrgo
 build==0.10.0
     # via
     #   pip-tools
     #   pyrgo
-cachecontrol[filecache]==0.13.0
+cachecontrol[filecache]==0.13.1
     # via pip-audit
 certifi==2023.5.7
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   black
     #   mkdocs
     #   pip-tools
     #   pyrgo
 colorama==0.4.6
     # via mkdocs-material
 coverage[toml]==7.2.7
     # via pytest-cov
-cyclonedx-python-lib==2.7.1
+cyclonedx-python-lib==4.0.1
     # via pip-audit
-exceptiongroup==1.1.1
+defusedxml==0.7.1
+    # via py-serializable
+exceptiongroup==1.1.2
     # via pytest
-filelock==3.12.0
+filelock==3.12.2
     # via cachecontrol
 ghp-import==2.1.0
     # via mkdocs
 html5lib==1.1
     # via pip-audit
 idna==3.4
     # via requests
-importlib-metadata==6.6.0
+importlib-metadata==6.8.0
     # via
-    #   build
-    #   click
-    #   cyclonedx-python-lib
     #   markdown
     #   mkdocs
-    #   pluggy
-    #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
 loguru==0.7.0
     # via pyrgo
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
-mashumaro[orjson]==3.7
+mashumaro[orjson]==3.8.1
     # via ez_cqrs (pyproject.toml)
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.3
     # via mkdocs-material
-mkdocs-material==9.1.15
+mkdocs-material==9.1.19
     # via pyrgo
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 msgpack==1.0.5
     # via cachecontrol
-mypy==1.3.0
+mypy==1.4.1
     # via pyrgo
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-orjson==3.9.0
+orjson==3.9.2
     # via mashumaro
 packageurl-python==0.11.1
     # via cyclonedx-python-lib
 packaging==23.1
     # via
     #   black
     #   build
@@ -100,115 +95,109 @@
     #   pip-audit
     #   pip-requirements-parser
     #   pytest
 pathspec==0.11.1
     # via black
 pip-api==0.0.30
     # via pip-audit
-pip-audit==2.5.6
+pip-audit==2.6.0
     # via pyrgo
 pip-requirements-parser==32.0.1
     # via pip-audit
-pip-tools==6.13.0
+pip-tools==7.1.0
     # via pyrgo
-platformdirs==3.5.1
+platformdirs==3.9.1
     # via black
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-pydantic==1.10.8
+py-serializable==0.11.1
+    # via cyclonedx-python-lib
+pydantic==2.0.3
     # via ez_cqrs (pyproject.toml)
+pydantic-core==2.3.0
+    # via pydantic
 pygments==2.15.1
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==10.0.1
+pymdown-extensions==10.1
     # via mkdocs-material
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
-pyrgo==0.3.0
+pyrgo==0.4.1
     # via ez_cqrs (pyproject.toml)
-pytest==7.3.1
+pytest==7.4.0
     # via
     #   pyrgo
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.21.0
+pytest-asyncio==0.21.1
     # via ez_cqrs (pyproject.toml)
 pytest-cov==4.1.0
     # via ez_cqrs (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.5.5
+regex==2023.6.3
     # via mkdocs-material
 requests==2.31.0
     # via
     #   cachecontrol
     #   mkdocs-material
     #   pip-audit
 result==0.10.0
     # via
     #   ez_cqrs (pyproject.toml)
     #   pyrgo
-rich==13.4.1
+rich==13.4.2
     # via pip-audit
-ruff==0.0.270
+ruff==0.0.278
     # via pyrgo
 six==1.16.0
     # via
     #   html5lib
     #   python-dateutil
 sortedcontainers==2.4.0
     # via cyclonedx-python-lib
 toml==0.10.2
-    # via
-    #   cyclonedx-python-lib
-    #   pip-audit
+    # via pip-audit
 tomli==2.0.1
     # via
     #   black
     #   build
     #   coverage
     #   mypy
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
-typed-ast==1.5.4
+typing-extensions==4.7.1
     # via
+    #   annotated-types
     #   black
-    #   mypy
-typing-extensions==4.6.2
-    # via
-    #   black
-    #   importlib-metadata
-    #   markdown-it-py
     #   mashumaro
-    #   mkdocs
     #   mypy
-    #   platformdirs
     #   pydantic
-    #   pytest-asyncio
+    #   pydantic-core
     #   result
     #   rich
-urllib3==1.26.16
-    # via
-    #   pip-audit
-    #   requests
+urllib3==2.0.4
+    # via requests
 watchdog==3.0.0
     # via mkdocs
 webencodings==0.5.1
     # via html5lib
 wheel==0.40.0
     # via pip-tools
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `ez_cqrs-1.3.0/scripts/new_release.py` & `ez_cqrs-1.4.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/tests/integration/conftest.py` & `ez_cqrs-1.4.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/tests/integration/test_execution.py` & `ez_cqrs-1.4.0/tests/integration/test_execution.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/tests/unit/test_acid_exec.py` & `ez_cqrs-1.4.0/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/.gitignore` & `ez_cqrs-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/LICENSE` & `ez_cqrs-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.3.0/pyproject.toml` & `ez_cqrs-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.3.0"
+version = "1.4.0"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
     { name = "Tomas Perez Alvarez", email = "tomasperezalvarez@gmail.com"}
 ]
@@ -21,14 +21,15 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "pyrgo>=0.3.0",
     "pytest-cov",
     "pytest-asyncio",
+    "tomli"
 ]
 
 [project.urls]
 Documentation = "https://github.com/Tomperez98/ez-cqrs#readme"
 Issues = "https://github.com/Tomperez98/ez-cqrs/issues"
 Source = "https://github.com/Tomperez98/ez-cqrs"
```

### Comparing `ez_cqrs-1.3.0/PKG-INFO` & `ez_cqrs-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.3.0
+Version: 1.4.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: mashumaro[orjson]
 Requires-Dist: pydantic
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: pyrgo>=0.3.0; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: tomli; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ez-cqrs
 
 A lightweight, opinionated framework to write software in a procedural way.
```

