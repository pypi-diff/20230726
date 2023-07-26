# Comparing `tmp/beanclerk-0.0.3.tar.gz` & `tmp/beanclerk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanclerk-0.0.3.tar", last modified: Tue Jul 18 15:21:23 2023, max compression
+gzip compressed data, was "beanclerk-0.0.4.tar", last modified: Wed Jul 26 15:20:38 2023, max compression
```

## Comparing `beanclerk-0.0.3.tar` & `beanclerk-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.964979 beanclerk-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-18 15:21:10.000000 beanclerk-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-07-18 15:21:23.964979 beanclerk-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 15:21:10.000000 beanclerk-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.960979 beanclerk-0.0.3/beanclerk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/bean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/clerk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.964979 beanclerk-0.0.3/beanclerk/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/importers/banka_creditas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/importers/fio_banka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.960979 beanclerk-0.0.3/beanclerk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-18 15:21:10.000000 beanclerk-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:21:23.964979 beanclerk-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.964979 beanclerk-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-18 15:21:10.000000 beanclerk-0.0.3/tests/test_clerk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.896668 beanclerk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-26 15:20:27.000000 beanclerk-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27147 2023-07-26 15:20:38.896668 beanclerk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-26 15:20:27.000000 beanclerk-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/beanclerk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/bean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/beanclerk/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/importers/banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/importers/fio_banka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/beanclerk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27147 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-26 15:20:27.000000 beanclerk-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:20:38.896668 beanclerk-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-26 15:20:27.000000 beanclerk-0.0.4/tests/test_clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-26 15:20:27.000000 beanclerk-0.0.4/tests/test_config.py
```

### Comparing `beanclerk-0.0.3/LICENSE` & `beanclerk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.3/PKG-INFO` & `beanclerk-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -363,17 +363,74 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: devel
 License-File: LICENSE
 
 # Beanclerk
 
+[![version on pypi](https://img.shields.io/pypi/v/beanclerk)](https://pypi.org/project/beanclerk/)
+[![license](https://img.shields.io/pypi/l/beanclerk)](https://pypi.org/project/beanclerk/)
+[![python versions](https://img.shields.io/pypi/pyversions/beanclerk)](https://pypi.org/project/beanclerk/)
+[![ci tests](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
-Additional automation for [Beancount](https://github.com/beancount/beancount)
+## Description
+
+Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
+
+1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
+2. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
+    * As the first step, Beanclerk provides a way to define rules for automated categorization.
+    * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
+
+### Existing importers
+
+Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
+
+### Notes
+
+I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. So it does not have to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or even solutions to the areas described above:
+
+* [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
+* [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
+* [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
+* [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
+* [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
+
+## Installation
+
+Beanclerk requires Beancount, that may need some additional steps for its installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
+
+```
+pip install beanclerk
+```
+
+Or, you may use [pipx](https://github.com/pypa/pipx) to install Beanclerk in an isolated environment:
+```
+pipx install beanclerk
+```
+
+Confirm successful installation by running:
+```
+bean-clerk -h
+```
+
+## Usage (work in progress)
+
+### Configuration
+
+Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory, or a path to the config file may be set by the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
+
+### Running the import
+
+Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
+
+```
+bean-clerk import --from-date 2023-01-01
+```
 
 ## Contributing
 
 Set up a development environment:
 ```bash
 ./build_venv
 source venv/bin/activate
```

### Comparing `beanclerk-0.0.3/beanclerk/cli.py` & `beanclerk-0.0.4/beanclerk/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,64 +4,77 @@
 from pathlib import Path
 
 import click
 
 from .clerk import import_transactions
 from .exceptions import BeanclerkError
 
-CONFIG_FILE: str = "beanclerk-config.yml"
+CONFIG_FILE = "beanclerk-config.yml"
 
 
 @click.group(
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=False,
 )
 @click.option(
     "-c",
     "--config-file",
     default=Path.cwd() / CONFIG_FILE,
     type=click.Path(path_type=Path),
-    help=f"Path to the config file; defaults to `{CONFIG_FILE}` in the current working directory.",  # noqa: E501
+    help=f"Path to a config file; defaults to `{CONFIG_FILE}` in the current working directory.",  # noqa: E501
 )
 @click.pass_context
 def cli(ctx: click.Context, config_file: Path) -> None:
-    """Additional automation for Beancount."""
+    """Automation for Beancount.
+
+    Import and categorize transactions via API importers and user-defined rules.
+    """
     # https://click.palletsprojects.com/en/8.1.x/commands/#nested-handling-and-contexts
     ctx.ensure_object(dict)
     ctx.obj["config_file"] = config_file
 
 
-# TODO: simplify by subclassing click.DateTime?
+_ISO_DATE_FMT: str = "YYYY-MM-DD"
+
+
 class Date(click.ParamType):
     """A convenience date type for Click.
 
-    Converts dates to a date instead of datetime.
+    Converts dates to a date (instead of datetime).
     """
 
     name = "date"
 
     def convert(self, value, param, ctx):
         if isinstance(value, date):
             return value
         try:
             return date.fromisoformat(value)
         except ValueError:
-            self.fail(f"'{value}' is not a valid date format (YYYY-MM-DD)", param, ctx)
+            self.fail(
+                f"'{value}' is not a valid date format ({_ISO_DATE_FMT})",
+                param,
+                ctx,
+            )
 
 
 @cli.command("import")
-@click.option("--from-date", type=Date(), help="The first date to import (YYYY-MM-DD).")
-@click.option("--to-date", type=Date(), help="The last date to import (YYYY-MM-DD).")
+@click.option(
+    "--from-date",
+    type=Date(),
+    help=f"The first date to import ({_ISO_DATE_FMT}).",
+)
+@click.option(
+    "--to-date",
+    type=Date(),
+    help=f"The last date to import ({_ISO_DATE_FMT}).",
+)
 @click.pass_context
-def import_(
-    ctx: click.Context,
-    from_date: click.DateTime,  # FIXME: use Date() instead
-    to_date: click.DateTime,  # FIXME: use Date() instead
-) -> None:
-    """Import transactions from configured importers."""
+def import_(ctx: click.Context, from_date: Date, to_date: Date) -> None:
+    """Import transactions and check the current balance."""
     try:
         import_transactions(
             config_file=ctx.obj["config_file"],
             from_date=from_date,
             to_date=to_date,
         )
     except BeanclerkError as exc:
```

### Comparing `beanclerk-0.0.3/beanclerk/importers/banka_creditas.py` & `beanclerk-0.0.4/beanclerk/importers/banka_creditas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Banka Creditas a.s.
 
+TODO:
+    This module is a work in progress. It needs a major rework.
+
 docs:
     https://www.creditas.cz/firma/creditas-api/
 """
 
 import base64
 from datetime import date
 from decimal import Decimal
```

### Comparing `beanclerk-0.0.3/beanclerk/importers/fio_banka.py` & `beanclerk-0.0.4/beanclerk/importers/fio_banka.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Fio banka, a.s.
+"""API importer for Fio banka, a.s.
+
+TODO:
+    * handle fio_banka exceptions
 
 docs:
     https://www.fio.cz/bank-services/internetbanking-api
 """
 
 from datetime import date
 
@@ -10,35 +13,29 @@
 from beancount.core.data import Amount, Transaction
 
 from ..bean_helpers import create_posting, create_transaction
 from . import ApiImporterProtocol, TransactionReport, prepare_meta
 
 
 class ApiImporter(ApiImporterProtocol):
-    """Importer for Fio banka, a.s. API"""
+    """API importer for Fio banka, a.s.
+
+    Args:
+        token (str): Fio banka API token
+    """
 
     def __init__(self, token: str) -> None:
         self._token = token
 
     def fetch_transactions(
         self,
         bean_account: str,
         from_date: date,
         to_date: date,
     ) -> TransactionReport:
-        """Return a tuple with the list of transactions and the current balance.
-
-        Args:
-            bean_account: Beancount account name.
-            from_date: Date from which to fetch transactions.
-            to_date: Date to which to fetch transactions.
-
-        Returns:
-            tuple: A tuple with the list of transactions and the current balance.
-        """
         client = fio_banka.Account(self._token)
         statement = client.periods(from_date, to_date, fio_banka.TransactionsFmt.JSON)
 
         txns: list[Transaction] = []
         for txn in fio_banka.get_transactions(statement):
             txns.append(
                 create_transaction(
```

### Comparing `beanclerk-0.0.3/beanclerk.egg-info/PKG-INFO` & `beanclerk-0.0.4/beanclerk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -363,17 +363,74 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: devel
 License-File: LICENSE
 
 # Beanclerk
 
+[![version on pypi](https://img.shields.io/pypi/v/beanclerk)](https://pypi.org/project/beanclerk/)
+[![license](https://img.shields.io/pypi/l/beanclerk)](https://pypi.org/project/beanclerk/)
+[![python versions](https://img.shields.io/pypi/pyversions/beanclerk)](https://pypi.org/project/beanclerk/)
+[![ci tests](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
-Additional automation for [Beancount](https://github.com/beancount/beancount)
+## Description
+
+Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
+
+1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
+2. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
+    * As the first step, Beanclerk provides a way to define rules for automated categorization.
+    * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
+
+### Existing importers
+
+Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
+
+### Notes
+
+I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. So it does not have to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or even solutions to the areas described above:
+
+* [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
+* [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
+* [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
+* [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
+* [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
+
+## Installation
+
+Beanclerk requires Beancount, that may need some additional steps for its installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
+
+```
+pip install beanclerk
+```
+
+Or, you may use [pipx](https://github.com/pypa/pipx) to install Beanclerk in an isolated environment:
+```
+pipx install beanclerk
+```
+
+Confirm successful installation by running:
+```
+bean-clerk -h
+```
+
+## Usage (work in progress)
+
+### Configuration
+
+Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory, or a path to the config file may be set by the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
+
+### Running the import
+
+Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
+
+```
+bean-clerk import --from-date 2023-01-01
+```
 
 ## Contributing
 
 Set up a development environment:
 ```bash
 ./build_venv
 source venv/bin/activate
```

### Comparing `beanclerk-0.0.3/pyproject.toml` & `beanclerk-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beanclerk"
-version = "0.0.3"
-authors = [
-  { name = "Petr Beranek", email = "petrberanek.mail@gmail.com" },
-]
-license = {file = "LICENSE"}
+version = "0.0.4"
+authors = [{ name = "Petr Beranek", email = "petrberanek.mail@gmail.com" }]
+license = { file = "LICENSE" }
 description = "Automation for Beancount"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["accounting", "finance", "beancount", "automation", "API"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
@@ -20,86 +18,83 @@
   "Intended Audience :: Information Technology",
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python :: 3.11",
   "Topic :: Office/Business :: Financial :: Accounting",
 ]
 # Always sync with additional dependencies for Mypy in pyproject.toml
-# TODO: simplify dep definitions via '~=' syntax; sort
 dependencies = [
-  "PyYAML>=6.0,<7",
-  "beancount>=2.3.5,<3",
-  "fio-banka>=1.0.3,<2",
-  "creditas==1.0.0.*",
-  "lxml>=4.9.2,<5",
-  "click>=8.1.4,<9",
-  "pydantic>=2.0.3,<3",
-  "pydantic-settings>=2.0.2,<3",
-  "rich>=13.4.2,<14",
+  "PyYAML~=6.0",
+  "beancount~=2.3",
+  "click~=8.1",
+  "creditas==1.0.0.*",      # https://github.com/peberanek/creditas/blob/main/README.md#versioning
+  "fio-banka~=1.0",
+  "lxml~=4.9",
+  "pydantic-settings~=2.0",
+  "pydantic~=2.0",
+  "rich~=13.4",
 ]
 
 [project.optional-dependencies]
-devel = [
-  "pre-commit>=3.3.3,<4",
-  "pytest>=7.4.0,<8",
-]
+devel = ["pre-commit~=3.3", "pytest~=7.4"]
 
 [project.scripts]
 bean-clerk = "beanclerk.cli:cli"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 # TODO: Use https://docs.pydantic.dev/dev-v2/integrations/mypy/
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
 select = [
-  "F",    # pyflakes
-  "E",    # pycodestyle
-  "C90",  # mccabe
-  "I",    # isort
-  "N",    # pep8-naming
-  "UP",   # pyupgrade
-  "YTT",  # flake8-2020
-  "S",    # flake8-bandit
-  "BLE",  # flake8-blind-except
-  "FBT",  # flake8-boolean-trap
-  "B",    # flake8-bugbear
-  "A",    # flake8-builtins
-  "COM",  # flake8-commas
-  "C4",   # flake8-comprehensions
-  "DTZ",  # flake8-datetimez
-  "T10",  # flake8-debugger
-  "INP",  # flake8-no-pep420
-  "PIE",  # flake8-pie
-  "T20",  # flake8-print
-  "PT",   # flake8-pytest-style
-  "Q",    # flake8-quotes
-  "RSE",  # flake8-raise
-  "RET",  # flake8-return
-  "SLF",  # flake8-self
-  "SIM",  # flake8-simplify
-  "ARG",  # flake8-unused-arguments
-  "PTH",  # flake8-use-pathlib
-  "PGH",  # pygrep-hooks
-  "PL",   # pylint
-  "TRY",  # tryceptors
-  "FLY",  # flynt
-  "RUF",  # Ruff-specific rules
+  "F",   # pyflakes
+  "E",   # pycodestyle
+  "C90", # mccabe
+  "I",   # isort
+  "N",   # pep8-naming
+  "UP",  # pyupgrade
+  "YTT", # flake8-2020
+  "S",   # flake8-bandit
+  "BLE", # flake8-blind-except
+  "FBT", # flake8-boolean-trap
+  "B",   # flake8-bugbear
+  "A",   # flake8-builtins
+  "COM", # flake8-commas
+  "C4",  # flake8-comprehensions
+  "DTZ", # flake8-datetimez
+  "T10", # flake8-debugger
+  "INP", # flake8-no-pep420
+  "PIE", # flake8-pie
+  "T20", # flake8-print
+  "PT",  # flake8-pytest-style
+  "Q",   # flake8-quotes
+  "RSE", # flake8-raise
+  "RET", # flake8-return
+  "SLF", # flake8-self
+  "SIM", # flake8-simplify
+  "ARG", # flake8-unused-arguments
+  "PTH", # flake8-use-pathlib
+  "PGH", # pygrep-hooks
+  "PL",  # pylint
+  "TRY", # tryceptors
+  "FLY", # flynt
+  "RUF", # Ruff-specific rules
 ]
 ignore = ["TRY003"]
 unfixable = [
   # These may break temporarily commented-out code
   "F401",
   "F841",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = [
   "S",
+  "ARG001", # pytest fixtures and mock functions often violate this
 ]
 
 [tool.ruff.pylint]
 max-args = 7
```

