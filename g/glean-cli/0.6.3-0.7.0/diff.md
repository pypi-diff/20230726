# Comparing `tmp/glean-cli-0.6.3.tar.gz` & `tmp/glean-cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.6.3.tar", last modified: Mon Jul 17 14:37:33 2023, max compression
+gzip compressed data, was "glean-cli-0.7.0.tar", last modified: Wed Jul 26 17:57:21 2023, max compression
```

## Comparing `glean-cli-0.6.3.tar` & `glean-cli-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.316254 glean-cli-0.6.3/
--rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 glean-cli-0.6.3/LICENSE
--rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-17 14:37:33.316319 glean-cli-0.6.3/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      832 2023-01-19 16:41:15.000000 glean-cli-0.6.3/README.md
--rw-r--r--   0 anixon     (501) staff       (20)      103 2022-12-17 00:47:55.000000 glean-cli-0.6.3/pyproject.toml
--rw-r--r--   0 anixon     (501) staff       (20)      831 2023-07-17 14:37:33.316624 glean-cli-0.6.3/setup.cfg
--rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 glean-cli-0.6.3/setup.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.311422 glean-cli-0.6.3/src/
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.313217 glean-cli-0.6.3/src/glean/
--rw-r--r--   0 anixon     (501) staff       (20)       18 2023-07-17 14:36:59.000000 glean-cli-0.6.3/src/glean/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)    29317 2023-07-17 14:36:59.000000 glean-cli-0.6.3/src/glean/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1598 2022-12-17 00:47:55.000000 glean-cli-0.6.3/src/glean/credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3904 2023-06-20 13:04:07.000000 glean-cli-0.6.3/src/glean/filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)    11337 2023-07-17 14:36:59.000000 glean-cli-0.6.3/src/glean/glean_api.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.314408 glean-cli-0.6.3/src/glean/utils/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2022-12-17 00:47:55.000000 glean-cli-0.6.3/src/glean/utils/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)      509 2023-01-03 16:54:54.000000 glean-cli-0.6.3/src/glean/utils/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     2622 2023-06-15 18:48:08.000000 glean-cli-0.6.3/src/glean/utils/grn.py
--rw-r--r--   0 anixon     (501) staff       (20)     1356 2023-06-23 20:05:46.000000 glean-cli-0.6.3/src/glean/utils/resource.py
--rw-r--r--   0 anixon     (501) staff       (20)     1089 2023-06-15 18:48:08.000000 glean-cli-0.6.3/src/glean/utils/validate_config.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.315216 glean-cli-0.6.3/src/glean_cli.egg-info/
--rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      616 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anixon     (501) staff       (20)        1 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anixon     (501) staff       (20)       41 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 anixon     (501) staff       (20)      116 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 anixon     (501) staff       (20)        6 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.316133 glean-cli-0.6.3/tests/
--rw-r--r--   0 anixon     (501) staff       (20)      309 2022-12-17 00:47:55.000000 glean-cli-0.6.3/tests/test_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1652 2022-12-17 00:47:55.000000 glean-cli-0.6.3/tests/test_credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     4632 2023-06-23 20:05:46.000000 glean-cli-0.6.3/tests/test_filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      666 2022-12-17 00:47:55.000000 glean-cli-0.6.3/tests/test_glean_api.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.259591 glean-cli-0.7.0/
+-rw-r--r--   0 calderhoover   (501) staff       (20)    11357 2023-03-17 14:57:47.000000 glean-cli-0.7.0/LICENSE
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1209 2023-07-26 17:57:21.259642 glean-cli-0.7.0/PKG-INFO
+-rw-r--r--   0 calderhoover   (501) staff       (20)      758 2023-07-26 17:48:44.000000 glean-cli-0.7.0/README.md
+-rw-r--r--   0 calderhoover   (501) staff       (20)      103 2023-03-17 14:57:47.000000 glean-cli-0.7.0/pyproject.toml
+-rw-r--r--   0 calderhoover   (501) staff       (20)      831 2023-07-26 17:57:21.259904 glean-cli-0.7.0/setup.cfg
+-rw-r--r--   0 calderhoover   (501) staff       (20)       38 2023-03-17 14:57:47.000000 glean-cli-0.7.0/setup.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.254325 glean-cli-0.7.0/src/
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.256541 glean-cli-0.7.0/src/glean/
+-rw-r--r--   0 calderhoover   (501) staff       (20)       18 2023-07-26 17:48:47.000000 glean-cli-0.7.0/src/glean/__init__.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)    31225 2023-07-26 17:48:44.000000 glean-cli-0.7.0/src/glean/cli.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)      146 2023-07-26 17:48:44.000000 glean-cli-0.7.0/src/glean/constants.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1598 2023-03-17 14:57:47.000000 glean-cli-0.7.0/src/glean/credentials.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     3904 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/filesystem.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)    17269 2023-07-26 17:48:44.000000 glean-cli-0.7.0/src/glean/glean_api.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.257542 glean-cli-0.7.0/src/glean/utils/
+-rw-r--r--   0 calderhoover   (501) staff       (20)        0 2023-03-17 14:57:47.000000 glean-cli-0.7.0/src/glean/utils/__init__.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)      509 2023-03-17 14:57:47.000000 glean-cli-0.7.0/src/glean/utils/cli.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     2622 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/utils/grn.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1356 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/utils/resource.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1089 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/utils/validate_config.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.258437 glean-cli-0.7.0/src/glean_cli.egg-info/
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1209 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 calderhoover   (501) staff       (20)      639 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)        1 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)       41 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)      116 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)        6 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.259433 glean-cli-0.7.0/tests/
+-rw-r--r--   0 calderhoover   (501) staff       (20)      309 2023-03-17 14:57:47.000000 glean-cli-0.7.0/tests/test_cli.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1652 2023-03-17 14:57:47.000000 glean-cli-0.7.0/tests/test_credentials.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     4632 2023-07-11 21:20:42.000000 glean-cli-0.7.0/tests/test_filesystem.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)      666 2023-03-17 14:57:47.000000 glean-cli-0.7.0/tests/test_glean_api.py
```

### Comparing `glean-cli-0.6.3/LICENSE` & `glean-cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/PKG-INFO` & `glean-cli-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.3
+Version: 0.7.0
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,26 +13,24 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # glean-cli
 
 Command-line tools for interacting with Glean (https://glean.io).
 
-Glean is currently in closed beta and the CLI is under active development.
-
 ## Development
 
 During local development, you likely want to point the CLI at your local
-Glean web server. You can do so with the following enviroment variable:
+Glean web server. You can do so with the following environment variable:
 
 ```bash
 export GLEAN_CLI_BASE_URI=http://localhost:5000
 ```
 
-You should work with the Glean CLI in its own virtual enviroment. In this
+You should work with the Glean CLI in its own virtual environment. In this
 new environment, ensure you have `pip`, then do `pip install build` to get
 the correct build tool.
 
 The Glean CLI is a project built by `setuptools`. You can package it for
 publish with `python -m build`, or link it for local development by running
 `pip install --editable .` in the root folder of this repo.
```

### Comparing `glean-cli-0.6.3/setup.cfg` & `glean-cli-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/src/glean/cli.py` & `glean-cli-0.7.0/src/glean/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from typing import Optional, List
 from uuid import UUID, uuid3
 from pathlib import Path, PurePath, PurePosixPath
 
 import click
 import git
 from requests import Session
+from glean.constants import DEFAULT_CREDENTIALS_FILEPATH, GLEAN_DEBUG
 import ruamel.yaml as yaml
 
 from glean import VERSION
 
 from glean.filesystem import local_resources
 from glean.credentials import get_credentials
 from glean.glean_api import (
     build_details_uri,
     clear_model_cache,
+    create_access_key,
     create_build_from_git_revision,
     create_build_from_local_files,
     upload_files_to_glean,
     login,
     get_datasources,
     get_tables,
     pull_resource,
 )
 from glean.utils.cli import cli_error_boundary, getenv_bool
 from glean.utils.grn import GRN_TYPE_KEY_MODEL, GRNComponents, parse_grn
 from glean.utils.resource import Resource
 
 
-GLEAN_DEBUG = getenv_bool("GLEAN_DEBUG")
-
 # Turning this on will result in secrets getting logged to stdout.
 GLEAN_VERBOSE_DEBUG_UNSAFE = getenv_bool("GLEAN_VERBOSE_DEBUG_UNSAFE")
 
 
 MAX_COLUMN_REGEX_LENGTH = 30
 MAX_COLUMN_FILTER_CHARS = 1000
 
@@ -104,27 +104,60 @@
 
 
 @click.group(context_settings=dict(max_content_width=130))
 @click.version_option(version=VERSION, prog_name="Glean")
 @click.option(
     "--credentials-filepath",
     type=str,
-    default="~/.glean/glean_access_key.json",
+    default=DEFAULT_CREDENTIALS_FILEPATH,
     show_default=True,
     help="Path to your Glean access key credentials. You can also control this by setting a "
     "GLEAN_CREDENTIALS_FILEPATH environment variable.",
     envvar="GLEAN_CREDENTIALS_FILEPATH",
 )
 @click.pass_context
 def cli(ctx, credentials_filepath):
     """A command-line interface for interacting with Glean."""
     if GLEAN_DEBUG or GLEAN_VERBOSE_DEBUG_UNSAFE:
         _enable_http_logging()
     ctx.ensure_object(dict)
-    ctx.obj["credentials"] = get_credentials(os.path.expanduser(credentials_filepath))
+    ctx.obj["credentials_filepath"] = os.path.expanduser(credentials_filepath)
+
+
+@cli.command(hidden=True)
+@click.option(
+    "--project-id",
+    type=str,
+    required=False,
+    help="If specified, creates an access key for this project ID. Required if your Glean user is a member of multiple projects.",
+)
+@click.pass_context
+def start(
+    ctx: click.Context, project_id: Optional[str]
+):
+    """Log into or sign up for a Glean account and create an access key to get started.
+
+    If `--credentials-filepath` is passed, will save the access key in that location.
+
+    If an access key already exists for your project, you'll need to delete it first before
+    this command can generate a new one for you.
+    """
+    credentials_filepath = ctx.obj["credentials_filepath"]
+    if os.path.exists(credentials_filepath):
+        click.echo("If you continue, the file at the following location will be overwritten with your new access key:")
+        click.echo()
+        click.echo(credentials_filepath)
+        click.echo()
+        click.echo("💡 To save your new access key to a different file path, re-run this command with that path passed via the `--credentials-filepath` option.")
+        click.echo()
+        if not click.confirm("Continue and overwrite existing file?"):
+            raise click.Abort()
+        click.echo()
+
+    create_access_key(ctx.obj["credentials_filepath"], project_id)
 
 
 @cli.command(
     "upload",
     context_settings=dict(),
 )
 @click.argument("database")
@@ -146,33 +179,34 @@
 
 @cli.command(
     "preview",
     context_settings=dict(
         ignore_unknown_options=True,
     ),
 )
-@allow_dangerous_empty_build_option
 @git_revision_option
 @git_path_option
 @dbt_manifest_option
-@run_dbt_parse_option
 @local_path_argument
+@run_dbt_parse_option
 @dbt_parse_flags_argument
+@allow_dangerous_empty_build_option
 @click.pass_context
 def preview(
     ctx,
     git_revision,
     git_path,
     dbt_manifest_path,
     filepath,
     run_dbt_parse,
     dbt_flags,
     allow_dangerous_empty_build,
 ):
     """Validates resource configurations and generates a preview link."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
 
     click.echo("🏗️  Creating preview build...")
     build_results = _create_build_using_options(
         ctx,
         filepath,
         git_revision=git_revision,
@@ -206,14 +240,15 @@
     run_dbt_parse: bool,
     filepath: str,
     preview: bool,
     dbt_flags,
     allow_dangerous_empty_build: bool,
 ):
     """Validates and deploys resource configurations to your project."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
 
     if preview:
         click.echo("🏗️  Creating preview build...")
         build_results = _create_build_using_options(
             ctx,
             filepath,
@@ -245,26 +280,28 @@
 
 @cli.command()
 @click.pass_context
 def databases(ctx):
     """See your available database connections.
 
     A database connection can be added in the Settings tab on glean.io."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     s = Session()
     project_id = login(s, ctx.obj["credentials"])
 
     datasources = get_datasources(s, project_id)
     _echo_datasources(datasources)
 
 
 @cli.command()
 @click.argument("database")
 @click.pass_context
 def tables(ctx, database):
     """Specify a database connection and see its available tables."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     s = Session()
     project_id = login(s, ctx.obj["credentials"])
 
     datasources = get_datasources(s, project_id)
     if database not in datasources:
         _echo_datasource_not_found(database, datasources)
         exit(1)
@@ -277,22 +314,24 @@
 
 
 @cli.group()
 @click.pass_context
 def cache(ctx):
     """Glean stores the results of queries in a cache so that users don't have
     to access the database again."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     pass
 
 
 @cache.command("clear")
 @click.argument("resource_grn")
 @click.pass_context
 def cache_clear(ctx, resource_grn):
     """Clears the cache for the associated resource."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     s = Session()
     login(s, ctx.obj["credentials"])
 
     grn = parse_grn(resource_grn)
     if not grn.gluid:
         click.echo("GRN must specify an id when clearing cache.")
         exit(1)
@@ -319,14 +358,15 @@
     allow_dirty: bool = False,
 ):
     """Pull the latest DataOps resource configuration from Glean into the working directory.
 
     GRN is the Glean resource name of the target resource. If the resource has DataOps dependencies, they will also be
     retrieved. If no GRN is specified, all resources for the project are pulled.
     """
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
 
     try:
         repo = git.Repo(Path("."), search_parent_directories=True)
         if repo.is_dirty() and not allow_dirty:
             raise click.ClickException(
                 "️🚩 The working directory has uncommitted changes that might be overwritten. (Skip this check with --allow-dirty.)"
             )
```

### Comparing `glean-cli-0.6.3/src/glean/credentials.py` & `glean-cli-0.7.0/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/src/glean/filesystem.py` & `glean-cli-0.7.0/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/src/glean/utils/grn.py` & `glean-cli-0.7.0/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/src/glean/utils/resource.py` & `glean-cli-0.7.0/src/glean/utils/resource.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/src/glean/utils/validate_config.py` & `glean-cli-0.7.0/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.7.0/src/glean_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.3
+Version: 0.7.0
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,26 +13,24 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # glean-cli
 
 Command-line tools for interacting with Glean (https://glean.io).
 
-Glean is currently in closed beta and the CLI is under active development.
-
 ## Development
 
 During local development, you likely want to point the CLI at your local
-Glean web server. You can do so with the following enviroment variable:
+Glean web server. You can do so with the following environment variable:
 
 ```bash
 export GLEAN_CLI_BASE_URI=http://localhost:5000
 ```
 
-You should work with the Glean CLI in its own virtual enviroment. In this
+You should work with the Glean CLI in its own virtual environment. In this
 new environment, ensure you have `pip`, then do `pip install build` to get
 the correct build tool.
 
 The Glean CLI is a project built by `setuptools`. You can package it for
 publish with `python -m build`, or link it for local development by running
 `pip install --editable .` in the root folder of this repo.
```

### Comparing `glean-cli-0.6.3/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.7.0/src/glean_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/glean/__init__.py
 src/glean/cli.py
+src/glean/constants.py
 src/glean/credentials.py
 src/glean/filesystem.py
 src/glean/glean_api.py
 src/glean/utils/__init__.py
 src/glean/utils/cli.py
 src/glean/utils/grn.py
 src/glean/utils/resource.py
```

### Comparing `glean-cli-0.6.3/tests/test_credentials.py` & `glean-cli-0.7.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/tests/test_filesystem.py` & `glean-cli-0.7.0/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.3/tests/test_glean_api.py` & `glean-cli-0.7.0/tests/test_glean_api.py`

 * *Files identical despite different names*

