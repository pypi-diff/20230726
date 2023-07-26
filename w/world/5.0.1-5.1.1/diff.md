# Comparing `tmp/world-5.0.1.tar.gz` & `tmp/world-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "world-5.0.1.tar", last modified: Wed May  4 02:28:56 2022, max compression
+gzip compressed data, was "world-5.1.1.tar", last modified: Wed Jul 26 16:43:24 2023, max compression
```

## Comparing `world-5.0.1.tar` & `world-5.1.1.tar`

### file list

```diff
@@ -1,23 +1,10 @@
--rw-rw-r--   0 barry      (501) staff       (20)      556 2022-05-04 01:46:58.107233 world-5.0.1/LICENSE
--rw-rw-r--   0 barry      (501) staff       (20)     1739 2022-05-04 02:23:07.079822 world-5.0.1/README.rst
--rw-rw-r--   0 barry      (501) staff       (20)      615 2022-05-04 01:46:58.108416 world-5.0.1/conftest.py
--rw-rw-r--   0 barry      (501) staff       (20)     1451 2022-05-04 02:23:54.362069 world-5.0.1/docs/NEWS.rst
--rw-rw-r--   0 barry      (501) staff       (20)        0 2022-05-04 01:46:58.109104 world-5.0.1/docs/__init__.py
--rw-rw-r--   0 barry      (501) staff       (20)      113 2022-05-04 01:46:58.109627 world-5.0.1/docs/apiref.rst
--rw-rw-r--   0 barry      (501) staff       (20)     8424 2022-05-04 01:46:58.110197 world-5.0.1/docs/conf.py
--rw-rw-r--   0 barry      (501) staff       (20)     3111 2022-05-04 01:46:58.110766 world-5.0.1/docs/index.rst
--rw-rw-r--   0 barry      (501) staff       (20)     2074 2022-05-04 01:46:58.111170 world-5.0.1/docs/manpage.rst
--rw-rw-r--   0 barry      (501) staff       (20)     1139 2022-05-04 01:46:58.111563 world-5.0.1/docs/using.rst
--rw-rw-r--   0 barry      (501) staff       (20)     2881 2022-05-04 02:28:19.253790 world-5.0.1/pyproject.toml
--rw-rw-r--   0 barry      (501) staff       (20)       22 2022-05-04 02:24:04.610919 world-5.0.1/src/world/__init__.py
--rw-rw-r--   0 barry      (501) staff       (20)     3072 2022-05-04 01:46:58.113884 world-5.0.1/src/world/__main__.py
--rw-rw-r--   0 barry      (501) staff       (20)        0 2022-05-04 01:46:58.114006 world-5.0.1/src/world/data/__init__.py
--rw-rw-r--   0 barry      (501) staff       (20)    12505 2022-05-04 01:46:58.114299 world-5.0.1/src/world/data/codes.pck
--rw-rw-r--   0 barry      (501) staff       (20)     5144 2022-05-04 01:46:58.114839 world-5.0.1/src/world/database.py
--rw-rw-r--   0 barry      (501) staff       (20)        0 2022-05-04 01:46:58.114938 world-5.0.1/src/world/py.typed
--rw-rw-r--   0 barry      (501) staff       (20)        0 2022-05-04 01:46:58.115050 world-5.0.1/test/__init__.py
--rw-rw-r--   0 barry      (501) staff       (20)     1144 2022-05-04 01:46:58.115488 world-5.0.1/test/test_database.py
--rw-rw-r--   0 barry      (501) staff       (20)     2737 2022-05-04 01:46:58.115867 world-5.0.1/test/test_main.py
--rwxrwxr-x   0 barry      (501) staff       (20)     2014 2022-05-04 01:46:58.116347 world-5.0.1/tools/scraper.py
--rw-rw-r--   0 barry      (501) staff       (20)      891 2022-05-04 02:02:41.094063 world-5.0.1/tox.ini
--rw-------   0 barry      (501) staff       (20)     3161 2022-05-04 02:28:56.710756 world-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      556 2022-05-05 00:04:23.483853 world-5.1.1/LICENSE
+-rw-r--r--   0        0        0     1739 2022-05-05 00:04:23.484029 world-5.1.1/README.rst
+-rw-r--r--   0        0        0     3087 2023-07-26 16:43:24.776225 world-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-26 00:21:23.791768 world-5.1.1/src/world/__init__.py
+-rw-r--r--   0        0        0     3064 2023-07-24 17:21:15.130462 world-5.1.1/src/world/__main__.py
+-rw-r--r--   0        0        0        0 2022-05-05 00:04:23.485915 world-5.1.1/src/world/data/__init__.py
+-rw-r--r--   0        0        0    12505 2022-05-05 00:04:23.486094 world-5.1.1/src/world/data/codes.pck
+-rw-r--r--   0        0        0     4741 2023-07-24 17:21:15.130863 world-5.1.1/src/world/database.py
+-rw-r--r--   0        0        0        0 2022-05-05 00:04:23.486273 world-5.1.1/src/world/py.typed
+-rw-r--r--   0        0        0     2772 1970-01-01 00:00:00.000000 world-5.1.1/PKG-INFO
```

### Comparing `world-5.0.1/LICENSE` & `world-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `world-5.0.1/README.rst` & `world-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `world-5.0.1/pyproject.toml` & `world-5.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,30 +24,28 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 dependencies = [
     "atpublic",
 ]
 dynamic = []
-version = "5.0.1"
+version = "5.1.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://world.readthedocs.io"
 Documentation = "https://world.readthedocs.io"
 Source = "https://gitlab.com/warsaw/world.git"
 "Bug Tracker" = "https://gitlab.com/warsaw/world/issues"
 
 [project.scripts]
 world = "world.__main__:main"
 
-[project.optional-dependencies]
-
 [tool.pdm]
 source-includes = [
     "docs/",
     "test/",
     "tools/",
     "tox.ini",
     "conftest.py",
@@ -57,59 +55,86 @@
     "**/*.pck",
 ]
 excludes = [
     "**/.mypy_cache/",
 ]
 
 [tool.pdm.version]
-from = "src/world/__init__.py"
+source = "file"
+path = "src/world/__init__.py"
 
 [tool.pdm.dev-dependencies]
 testing = [
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "flake8",
-    "isort",
-    "mypy",
     "blue",
+    "mypy",
+    "ruff",
 ]
 docs = [
     "sphinx",
-    "sphinx-autodoc-typehints",
     "furo",
 ]
 
 [tool.pytest.ini_options]
-addopts = "--cov=world --cov-report=term --cov-report=xml"
+addopts = "--cov=world --cov-report=term --cov-report=xml -p no:doctest"
 testpaths = "test docs"
 
 [tool.coverage.report]
 fail_under = 100
 show_missing = true
 
 [tool.coverage.run]
 branch = true
 parallel = true
 
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "world"
-length_sort_straight = true
-lines_after_imports = 2
-lines_between_types = 1
-multi_line_output = 3
-order_by_type = false
-skip = [
-    "conf.py",
-]
+[tool.ruff]
+line-length = 79
+src = [
+    "src",
+]
+select = [
+    "B",
+    "D",
+    "E",
+    "F",
+    "I",
+    "RUF100",
+    "UP",
+    "W",
+]
+ignore = [
+    "D100",
+    "D103",
+    "D104",
+]
+
+[tool.ruff.per-file-ignores]
+"src/world/database.py" = [
+    "I001",
+]
+"src/world/__main__.py" = [
+    "I001",
+]
+
+[tool.ruff.pydocstyle]
+convention = "pep257"
+
+[tool.ruff.isort]
+known-first-party = [
+    "world",
+]
+lines-after-imports = 2
+lines-between-types = 1
+order-by-type = true
 
 [tool.mypy]
 mypy_path = "src"
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = false
 disallow_untyped_defs = true
@@ -137,10 +162,10 @@
     "pytest",
     "sybil.*",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `world-5.0.1/src/world/__main__.py` & `world-5.1.1/src/world/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 @public
 def main(args: Optional[List[str]] = None) -> int:
     parser = argparse.ArgumentParser(
         prog='world', description='Top level domain name mapper.'
     )
     parser.add_argument(
-        '--version', action='version', version='world {}'.format(__version__)
+        '--version', action='version', version=f'world {__version__}'
     )
     parser.add_argument_group('Querying')
     parser.add_argument(
         '-r',
         '--reverse',
         action='store_true',
         help="""Do a reverse lookup.  In this mode, the
```

### Comparing `world-5.0.1/src/world/data/codes.pck` & `world-5.1.1/src/world/data/codes.pck`

 * *Files identical despite different names*

### Comparing `world-5.0.1/src/world/database.py` & `world-5.1.1/src/world/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 @public
 class Database:
     """Database of country codes to top-level domain names."""
 
     def __init__(self) -> None:
+        """Initialize the database."""
         with open_binary('world.data', 'codes.pck') as fp:
             raw_data = pickle.load(fp)
         # We want two lookup tables.  One maps English country names to
         # 2-digit alpha country codes.  Another maps the 2-digit codes to
         # their English names.  For now, while we capture the 3-digit alpha
         # codes in the raw data, we ignore it.
         self.ccTLDs: Dict[str, str] = {
@@ -55,16 +56,15 @@
         for key, value in self._by_code.items():
             if cre.search(value):
                 matches.append((key, value))
         return sorted(matches)
 
     def __iter__(self) -> Generator[str, None, None]:
         """Iterate over all country codes, in sorted order."""
-        for code in sorted(self._by_code):
-            yield code
+        yield from sorted(self._by_code)
 
 
 # Generic top-level domains.
 # http://en.wikipedia.org/wiki/TLD
 #
 # Of course, the internet has changed considerably in the intervening years
 # since this tool was first written, and we now have a jillion new TLDs with
@@ -73,35 +73,35 @@
 gTLDs = {
     # fmt: off
     # Intrastructure.
     'arpa': 'Arpanet',
     # Additional IANA TLDs.
     'aero': 'air-transport industry',
     'asia': 'Asia-Pacific region',
-    'biz' : 'business',                             # noqa: E203
-    'cat' : 'Catalan',                              # noqa: E203
-    'com' : 'commercial',                           # noqa: E203
+    'biz' : 'business',
+    'cat' : 'Catalan',
+    'com' : 'commercial',
     'coop': 'cooperatives',
     'info': 'information',
-    'int' : 'international organizations',          # noqa: E203
+    'int' : 'international organizations',
     'jobs': 'companies',
     'mobi': 'mobile devices',
     'museum': 'museums',
     'name': 'individuals, by name',
-    'net' : 'network',                              # noqa: E203
-    'org' : 'non-commercial',                       # noqa: E203
+    'net' : 'network',
+    'org' : 'non-commercial',
     'post': 'postal services',
-    'pro' : 'professionals',                        # noqa: E203
-    'tel' : 'Internet communications services',     # noqa: E203
+    'pro' : 'professionals',
+    'tel' : 'Internet communications services',
     'travel': 'travel and tourism industry related sites',
-    'xxx' : 'adult entertainment',                  # noqa: E203
+    'xxx' : 'adult entertainment',
     # USA TLDs.
-    'edu' : 'educational',                          # noqa: E203
-    'gov' : 'governmental',                         # noqa: E203
-    'mil' : 'US military',                          # noqa: E203
+    'edu' : 'educational',
+    'gov' : 'governmental',
+    'mil' : 'US military',
     # These additional ccTLDs are included here even though they are not part
     # of ISO 3166.  IANA has 5 reserved ccTLDs as described here:
     #
     # http://www.iso.org/iso/en/prods-services/iso3166ma/04background-on-iso-3166/iso3166-1-and-ccTLDs.html
     #
     # but I can't find an official list anywhere.
     #
```

### Comparing `world-5.0.1/PKG-INFO` & `world-5.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 Metadata-Version: 2.1
 Name: world
-Version: 5.0.1
+Version: 5.1.1
 Summary: world -- top level domain code mappings
+Keywords: domain name system DNS country codes ISO 3166
+Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
-Keywords: domain name system,DNS,country codes,ISO 3166
-Author-email: Barry Warsaw <barry@python.org>
-Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Project-URL: Bug Tracker, https://gitlab.com/warsaw/world/issues
+Project-URL: Home page, https://world.readthedocs.io
 Project-URL: Documentation, https://world.readthedocs.io
-Project-URL: Home Page, https://world.readthedocs.io
 Project-URL: Source, https://gitlab.com/warsaw/world.git
+Project-URL: Bug tracker, https://gitlab.com/warsaw/world/issues
+Requires-Python: >=3.8
+Requires-Dist: atpublic
 Description-Content-Type: text/x-rst
-Description: ===================================================================
-        world -- Print mappings between country names and DNS country codes
-        ===================================================================
-        
-        This script takes a list of Internet top-level domain names and prints out
-        where in the world those domains originate from.  For example::
-        
-            $ world tz us
-            tz originates from Tanzania, United Republic of
-            us originates from United States of America (the)
-        
-        Reverse look ups are also supported::
-        
-            $ world -r united
-            Matches for "united":
-              ae: United Arab Emirates (the)
-              gb: United Kingdom of Great Britain and Northern Ireland (the)
-              tz: Tanzania, United Republic of
-              uk: United Kingdom (common practice)
-              um: United States Minor Outlying Islands (the)
-              us: United States of America (the)
-        
-        Only two-letter country codes are supported, since these are the only ones
-        that were freely available from the ISO_ 3166_ standard.  However, as of
-        2015-01-09, even these are no longer freely available in a machine readable
-        format.
-        
-        This script also knows about non-geographic, generic, USA-centric, historical,
-        common usage, and reserved top-level domains.
-        
-        
-        Project details
-        ===============
-        
-        * Project home: https://gitlab.com/warsaw/world
-        * Report bugs at: https://gitlab.com/warsaw/world/issues
-        * Code hosting: https://gitlab.com/warsaw/world.git
-        * Documentation: http://world.readthedocs.io/en/latest/
-        
-        
-        Author
-        ======
-        
-        ``world`` is Copyright (C) 2013-2022 Barry Warsaw <barry@python.org>
-        
-        Licensed under the Apache License, Version 2.0 (the "License").  See the
-        LICENSE file for details.
-        
-        
-        .. _ISO: http://www.iso.org/iso/home.html
-        .. _3166: http://www.iso.org/iso/home/standards/country_codes/
 
+===================================================================
+world -- Print mappings between country names and DNS country codes
+===================================================================
+
+This script takes a list of Internet top-level domain names and prints out
+where in the world those domains originate from.  For example::
+
+    $ world tz us
+    tz originates from Tanzania, United Republic of
+    us originates from United States of America (the)
+
+Reverse look ups are also supported::
+
+    $ world -r united
+    Matches for "united":
+      ae: United Arab Emirates (the)
+      gb: United Kingdom of Great Britain and Northern Ireland (the)
+      tz: Tanzania, United Republic of
+      uk: United Kingdom (common practice)
+      um: United States Minor Outlying Islands (the)
+      us: United States of America (the)
+
+Only two-letter country codes are supported, since these are the only ones
+that were freely available from the ISO_ 3166_ standard.  However, as of
+2015-01-09, even these are no longer freely available in a machine readable
+format.
+
+This script also knows about non-geographic, generic, USA-centric, historical,
+common usage, and reserved top-level domains.
+
+
+Project details
+===============
+
+* Project home: https://gitlab.com/warsaw/world
+* Report bugs at: https://gitlab.com/warsaw/world/issues
+* Code hosting: https://gitlab.com/warsaw/world.git
+* Documentation: http://world.readthedocs.io/en/latest/
+
+
+Author
+======
+
+``world`` is Copyright (C) 2013-2022 Barry Warsaw <barry@python.org>
+
+Licensed under the Apache License, Version 2.0 (the "License").  See the
+LICENSE file for details.
+
+
+.. _ISO: http://www.iso.org/iso/home.html
+.. _3166: http://www.iso.org/iso/home/standards/country_codes/
```

