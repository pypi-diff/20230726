# Comparing `tmp/sphinx_apitree-1.4.4.tar.gz` & `tmp/sphinx_apitree-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.4.4.tar` & `sphinx_apitree-1.4.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/LICENSE
--rw-r--r--   0        0        0     2858 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/README.md
--rw-r--r--   0        0        0      105 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/__init__.py
--rw-r--r--   0        0        0     6613 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/ast_utils.py
--rw-r--r--   0        0        0     5696 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/conf_util.py
--rw-r--r--   0        0        0     1058 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/context.py
--rw-r--r--   0        0        0      179 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/debug_utils.py
--rw-r--r--   0        0        0     1801 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/ext/auto_ref.py
--rw-r--r--   0        0        0      885 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/ext/docstring.py
--rw-r--r--   0        0        0     3688 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/ext/github_link.py
--rw-r--r--   0        0        0     1691 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/html_helper.py
--rw-r--r--   0        0        0     1324 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/import_utils.py
--rw-r--r--   0        0        0       30 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-26 14:32:20.480501 sphinx_apitree-1.4.4/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/structs.py
--rw-r--r--   0        0        0    11763 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/symbol_match.py
--rw-r--r--   0        0        0      212 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/templates/api.md
--rw-r--r--   0        0        0       84 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/templates/function.md
--rw-r--r--   0        0        0      183 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/templates/module.md
--rw-r--r--   0        0        0       84 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1728 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/tree_extractor.py
--rw-r--r--   0        0        0      738 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/apitree/writer.py
--rw-r--r--   0        0        0     1556 2023-07-26 14:32:20.484501 sphinx_apitree-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/LICENSE
+-rw-r--r--   0        0        0     3043 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/README.md
+-rw-r--r--   0        0        0      105 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/__init__.py
+-rw-r--r--   0        0        0     6613 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/ast_utils.py
+-rw-r--r--   0        0        0     5902 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/conf_util.py
+-rw-r--r--   0        0        0     1058 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/context.py
+-rw-r--r--   0        0        0      179 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/debug_utils.py
+-rw-r--r--   0        0        0     1801 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/ext/auto_ref.py
+-rw-r--r--   0        0        0      885 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/ext/docstring.py
+-rw-r--r--   0        0        0     3688 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/ext/github_link.py
+-rw-r--r--   0        0        0     1691 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/html_helper.py
+-rw-r--r--   0        0        0     1324 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/import_utils.py
+-rw-r--r--   0        0        0       30 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/structs.py
+-rw-r--r--   0        0        0    11763 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/symbol_match.py
+-rw-r--r--   0        0        0      212 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/templates/api.md
+-rw-r--r--   0        0        0       84 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/templates/function.md
+-rw-r--r--   0        0        0      183 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/templates/module.md
+-rw-r--r--   0        0        0       84 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1728 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      738 2023-07-26 16:54:52.999128 sphinx_apitree-1.4.5/apitree/writer.py
+-rw-r--r--   0        0        0     1556 2023-07-26 16:54:53.003128 sphinx_apitree-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.5/PKG-INFO
```

### Comparing `sphinx_apitree-1.4.4/LICENSE` & `sphinx_apitree-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/README.md` & `sphinx_apitree-1.4.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,22 @@
   :caption: API
 
   api/my_module/index
 ```
 
 ## Features
 
-* Theme
-* Auto-generate the API tree, with better features
+* All included: Single function call include the theme, the API generation,...
+* Auto-generate the API tree:
   * Do not require `__all__` (smart detect of which symbols are documented)
   * Add expandable toc tree with all symbols
+* Add links to `GitHub`.
+* Contrary to `autodoc` and `apitree`, it also document:
+  * Type annotations (`Union[]`, ...)
+  * Attributes
 * ...
 
 ## Installation in a project
 
 1.  In `pyproject.toml`
 
     ```toml
```

### Comparing `sphinx_apitree-1.4.4/apitree/ast_utils.py` & `sphinx_apitree-1.4.5/apitree/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/conf_util.py` & `sphinx_apitree-1.4.5/apitree/conf_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,25 +31,30 @@
       `my_module/submodule/README.md` to `submodule.md`). By default, only
       files inside `docs/...` can be read
     globals: The `conf.py` `globals()` dict. Will be mutated.
   """
 
   docs_dir = epath.Path(globals['__file__']).parent  # <repo>/docs/
   repo_dir = docs_dir.parent
-  # TODO(epot): Fragile if one of the module is already imported.
-  # If so, should check that imported modules are
-  # `import_utils.belong_to_project`
+
+  project_name = _get_project_name(repo_dir=repo_dir)
 
   # Clear etils before (to allow documenting `etils` itself).
   # Otherwise, `etils` imported is the one from `pip install` and
   # not the one from `git clone`.
-  _clear_etils()
-  sys.path.insert(0, os.fspath(repo_dir))
+  # This has to be done after `epath.Path()` call, which has a lazy-import
+  if project_name == 'etils':
+    _clear_etils()
 
-  project_name = _get_project_name(repo_dir=repo_dir)
+  # TODO(epot): Fragile if one of the module is already imported.
+  # If so, should check that imported modules are
+  # `import_utils.belong_to_project`
+  # Allow import without installing the project first (dependencies
+  # still have to be installed.
+  sys.path.insert(0, os.fspath(repo_dir))
 
   # API generator
   api_ext = 'sphinx.ext.autodoc'
   api_ext_config = dict(
       autodoc_typehints_format='fully-qualified',  # `x.y.MyClass`
       autodoc_default_options={
           'members': True,
@@ -74,15 +79,15 @@
       copyright=f'2023, {project_name} authors',
       author=f'{project_name} authors',
       # General configuration
       extensions=[
           api_ext,  # API Doc generator
           'myst_nb',  # Notebook support
           'sphinx.ext.napoleon',  # Numpy-style docstrings
-          # 'sphinx.ext.linkcode',  # Links to GitHub
+          'sphinx.ext.linkcode',  # Links to GitHub
           # Others:
           # 'sphinx_autodoc_typehints',
           # 'sphinx.ext.linkcode',
           # 'sphinx.ext.inheritance_diagram',
           # 'myst_parser',
           # API Tree
           'apitree.ext.docstring',  # Fix bad ```python md formatting
```

### Comparing `sphinx_apitree-1.4.4/apitree/context.py` & `sphinx_apitree-1.4.5/apitree/context.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/ext/auto_ref.py` & `sphinx_apitree-1.4.5/apitree/ext/auto_ref.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/ext/docstring.py` & `sphinx_apitree-1.4.5/apitree/ext/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/ext/github_link.py` & `sphinx_apitree-1.4.5/apitree/ext/github_link.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/html_helper.py` & `sphinx_apitree-1.4.5/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/import_utils.py` & `sphinx_apitree-1.4.5/apitree/import_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/symbol_match.py` & `sphinx_apitree-1.4.5/apitree/symbol_match.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/tree_extractor.py` & `sphinx_apitree-1.4.5/apitree/tree_extractor.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/apitree/writer.py` & `sphinx_apitree-1.4.5/apitree/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/pyproject.toml` & `sphinx_apitree-1.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.4/PKG-INFO` & `sphinx_apitree-1.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.4.4
+Version: 1.4.5
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -63,18 +63,22 @@
   :caption: API
 
   api/my_module/index
 ```
 
 ## Features
 
-* Theme
-* Auto-generate the API tree, with better features
+* All included: Single function call include the theme, the API generation,...
+* Auto-generate the API tree:
   * Do not require `__all__` (smart detect of which symbols are documented)
   * Add expandable toc tree with all symbols
+* Add links to `GitHub`.
+* Contrary to `autodoc` and `apitree`, it also document:
+  * Type annotations (`Union[]`, ...)
+  * Attributes
 * ...
 
 ## Installation in a project
 
 1.  In `pyproject.toml`
 
     ```toml
```

