# Comparing `tmp/ipyautoui-0.5.6.tar.gz` & `tmp/ipyautoui-0.5.7.tar.gz`

## Comparing `ipyautoui-0.5.6.tar` & `ipyautoui-0.5.7.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/automapschema.yaml
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/selectandclick.py
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/showopenurl.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/README.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13112 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/automapschema.yaml
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/halo_decorator.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/multi_toggle_buttons.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     9745 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/selectandclick.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.7/PKG-INFO
```

### Comparing `ipyautoui-0.5.6/src/ipyautoui/__init__.py` & `ipyautoui-0.5.7/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.7/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/_utils.py` & `ipyautoui-0.5.7/src/ipyautoui/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,22 +39,22 @@
                 subprocess.call(["explorer.exe", path])
 
 except:
 
     def make_new_path(path, *args, **kwargs):
         return path
 
-        def open_path(path):
-            import subprocess
-            import sys
-
-            if sys.platform == "linux":
-                subprocess.call(["xdg-open", path])
-            else:
-                subprocess.call(["explorer.exe", path])
+    def open_path(path):
+        import subprocess
+        import sys
+
+        if sys.platform == "linux":
+            subprocess.call(["xdg-open", path])
+        else:
+            subprocess.call(["explorer.exe", path])
 
 
 def getuser():
     try:
         return os.environ["JUPYTERHUB_USER"]
     except:
         return getpass.getuser()
```

### Comparing `ipyautoui-0.5.6/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.7/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.7/src/ipyautoui/autodisplay.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.7/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.7/src/ipyautoui/autoipywidget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.7/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/automapschema.yaml` & `ipyautoui-0.5.7/src/ipyautoui/automapschema.yaml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/autoui.py` & `ipyautoui-0.5.7/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.7/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.7/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.7/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/constants.py` & `ipyautoui-0.5.7/src/ipyautoui/constants.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo.py` & `ipyautoui-0.5.7/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/env.py` & `ipyautoui-0.5.7/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.7/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.7/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.7/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/autogrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/editgrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/selectandclick.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/selectandclick.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,40 +2,55 @@
 # ---
 # jupyter:
 #   jupytext:
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.14.7
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %load_ext lab_black
 
 # +
 import ipywidgets as w
 import traitlets as tr
-from ipyautoui.constants import DELETE_BUTTON_KWARGS, ADD_BUTTON_KWARGS
+from ipyautoui.constants import (
+    DELETE_BUTTON_KWARGS,
+    ADD_BUTTON_KWARGS,
+    LOAD_BUTTON_KWARGS,
+)
+from ipyautoui.custom.halo_decorator import halo_decorator
+from IPython.display import clear_output
 
 
 class SelectAndClick(w.Box):
+    value = tr.Unicode(allow_none=True, default_value=None)
     fn_onclick = tr.Callable(lambda v: print(f"do something: {str(v)}"))
     fn_get_options = tr.Callable(lambda: [])
+    fn_loading_msg = tr.Callable(lambda v: f"loading {v}")
+    fn_succeed_msg = tr.Callable(lambda v: f"successfully loaded {v}")
+    fn_failed_msg = tr.Callable(lambda v: f"failed to load {v}")
     options = tr.List(default_value=[])  # allow dict ?
     title = tr.Unicode(default_value="")
     message = tr.Unicode(default_value="")
     align_horizontal = tr.Bool(default_value=True)
     align_left = tr.Bool(default_value=True)
 
+    @tr.observe("value")
+    def _observe_value(self, change):
+        if change["new"] != self.select.value:
+            self.select.value = change["new"]
+
     @tr.observe("align_horizontal")
     def _observe_align_horizontal(self, change):
         self.align()
 
     @tr.observe("align_left")
     def _observe_align_left(self, change):
         self.align()
@@ -48,29 +63,38 @@
             self.layout.align_items = "stretch"
         else:
             self.layout.display = "flex"
             self.layout.flex_flow = "column"
             self.layout.align_items = "stretch"
         # left-right
         if self.align_left and self.align_horizontal:
+            self.hbx_message = w.HBox([self.html_message, self.out_message])
             self.children = [self.select, self.hbx_bbar]
-            self.hbx_text.children = [self.html_title, self.html_message]
+            self.hbx_text.children = [self.html_title, self.hbx_message]
             self.hbx_bbar.children = [self.bn, self.hbx_text]
         elif self.align_left and not self.align_horizontal:
+            self.hbx_message = w.HBox([self.html_message, self.out_message])
             self.children = [self.hbx_bbar, self.select]
-            self.hbx_text.children = [self.html_title, self.html_message]
+            self.hbx_text.children = [self.html_title, self.hbx_message]
             self.hbx_bbar.children = [self.bn, self.hbx_text]
         elif not self.align_left and not self.align_horizontal:
-            self.children = [self.hbx_bbar, self.select]
-            self.hbx_text.children = [self.html_title, self.html_message]
-            self.hbx_bbar.children = [self.bn, self.hbx_text]
-        else:
-            self.children = [self.hbx_bbar, self.select]
-            self.hbx_text.children = [self.html_message, self.html_title]
+            self.hbx_message = w.HBox([self.html_message, self.out_message])
+            self.children = [self.select, self.hbx_bbar]
+            self.hbx_text.children = [self.html_title, self.hbx_message]
             self.hbx_bbar.children = [self.hbx_text, self.bn]
+        elif not self.align_left and self.align_horizontal:
+            self.children = [
+                self.out_message,
+                self.html_message,
+                self.html_title,
+                self.select,
+                self.bn,
+            ]
+            # self.hbx_text.children = [self.hbx_message]
+            # self.hbx_bbar.children = [self.hbx_text, self.bn]
 
     @tr.observe("options")
     def _observe_options(self, change):
         self.select.options = change["new"]
 
     @tr.observe("title")
     def _observe_title(self, change):
@@ -90,58 +114,149 @@
         self._observe_align_left("")
 
     def _init_form(self):
         self.select = self.get_selector_widget()
         self.bn = w.Button()
         self.html_title = w.HTML()
         self.html_message = w.HTML()
+        self.out_message = w.Output()
+        #
         self.hbx_text = w.HBox()
         self.hbx_bbar = w.HBox()
 
     def _init_controls(self):
         self.bn.on_click(self.onclick)
         self.select.observe(self._update_message, "value")
+        self.select.observe(self._update_value, "value")
 
     def update_options(self):
         options = self.fn_get_options()
         if isinstance(options, dict):
             self.map_options = options
             self.options = list(options.keys())
         elif isinstance(options, list):
             self.map_options = None
             self.options = options
         else:
             raise ValueError("options must be a list or dict")
 
     def _update_message(self, on_change):
-        self.html_message.value = ", ".join(self.select.value)
+        self.fn_update_message()
 
-    def onclick(self, on_click):
-        if self.map_options is None:
-            self.fn_onclick(self.select.value)
+    def fn_update_message(self):
+        if isinstance(self.select.value, str):
+            self.html_message.value = self.select.value
         else:
-            self.fn_onclick(self.map_options[self.select.value])
+            self.html_message.value = ", ".join(self.select.value)
+
+    def _update_value(self, on_change):
+        self.value = self.select.value
+
+    def onclick(self, on_click):
+        @halo_decorator(
+            self.out_message,
+            loading_msg=self.fn_loading_msg(self.select.value),
+            succeed_msg=self.fn_succeed_msg(self.select.value),
+            failed_msg=self.fn_failed_msg(self.select.value),
+        )
+        def fn(*args, **kwargs):
+            if self.map_options is None:
+                self.fn_onclick(self.select.value)
+            else:
+                self.fn_onclick(self.map_options[self.select.value])
+
+        fn()
+
+        with self.out_message:
+            display("done")
+            clear_output()
+        self.onclick_extra()
+
+    def onclick_extra(self):
+        pass
 
     @tr.default("align_horizontal")
     def default_align_horizontal(self):
         return True
 
     @tr.default("align_left")
-    def default_align_leftl(self):
+    def default_align_left(self):
         return True
 
     @staticmethod
     def get_selector_widget():
         return w.Combobox(ensure_option=True)
 
 
+# +
+class Add(SelectAndClick):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        {setattr(self.bn, k, v) for k, v in ADD_BUTTON_KWARGS.items()}
+
+
+class Remove(SelectAndClick):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        {setattr(self.bn, k, v) for k, v in DELETE_BUTTON_KWARGS.items()}
+
+
+class Load(SelectAndClick):
+    loaded = tr.Unicode()
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        {setattr(self.bn, k, v) for k, v in LOAD_BUTTON_KWARGS.items()}
+        # self.fn_update_message()
+        self.bn.layout.display = "None"
+        self._init_load_controls()
+
+    def _init_load_controls(self):
+        self.select.observe(self._update_loaded, "value")
+
+    def _update_loaded(self, on_change):
+        if self.loaded == self.select.value:
+            self.bn.layout.display = "None"
+        else:
+            self.bn.layout.display = ""
+
+    def fn_update_message(self):
+        if self.loaded == self.select.value:
+            self.message = f"✔️ {self.loaded} loaded ✔️"
+        else:
+            self.message = (
+                f"⚠️ {self.loaded} loaded, click to load {self.select.value} ⚠️"
+            )
+
+    def onclick_extra(self):
+        self.loaded = self.value
+        self.fn_update_message()
+        self._update_loaded("")
+
 
 # -
 
+if __name__ == "__main__":
+    from time import sleep
+
+    LI = [str(l) for l in [3870, 4321, 6440]]
+    ui = Load(
+        loaded="3870",
+        value="3870",
+        fn_get_options=lambda: LI,
+        title="<b> | select project</b>",
+        align_left=False,
+        fn_onclick=lambda v: sleep(4),
+    )
+    display(ui)
+
+
 class SelectMultipleAndClick(SelectAndClick):
+    value = tr.List(allow_none=True)
+
     def onclick(self, on_click):
         if self.map_options is None:
             [self.fn_onclick(v) for v in self.select.value]
         else:
             [self.fn_onclick(self.map_options[v]) for v in self.select.value]
 
     @tr.default("align_horizontal")
@@ -153,47 +268,63 @@
         return True
 
     @staticmethod
     def get_selector_widget():
         return w.SelectMultiple()
 
 
-if __name__ == "__main__":
-    ui = SelectAndClick(
-        fn_get_options=lambda: ["a", "b", "c"],
-        title="asdf",
-        align_horizontal=False,
-    )
-    display(ui)
-
-
 # +
-class RemoveMultiple(SelectMultipleAndClick):
+class AddMultiple(SelectMultipleAndClick):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        {setattr(self.bn, k, v) for k, v in DELETE_BUTTON_KWARGS.items()}
+        {setattr(self.bn, k, v) for k, v in ADD_BUTTON_KWARGS.items()}
 
 
-class AddMultiple(SelectMultipleAndClick):
+class RemoveMultiple(SelectMultipleAndClick):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        {setattr(self.bn, k, v) for k, v in ADD_BUTTON_KWARGS.items()}
+        {setattr(self.bn, k, v) for k, v in DELETE_BUTTON_KWARGS.items()}
 
 
 # -
 
 if __name__ == "__main__":
+    ui = Add(
+        fn_get_options=lambda: ["a", "b", "c"],
+        fn_onclick=lambda v: print(f"loading project {v}"),
+        fn_message_onclick=lambda v: print("aasdf"),
+        title="load project:",
+        align_horizontal=False,
+    )
+    display(ui)
+
+if __name__ == "__main__":
     ui = AddMultiple(
         fn_get_options=lambda: ["a", "b", "c"],
         align_horizontal=False,
         title="<b>asdf |</b>",
     )
     display(ui)
 
 if __name__ == "__main__":
     ui.align_horizontal = True
 
 if __name__ == "__main__":
     ui.align_horizontal = False
     ui.align_left = False
 
+# # +
+# import random
+# import string
+
+
+# def get_random_string(length):
+#     # choose from all lowercase letter
+#     letters = string.ascii_lowercase
+#     return "".join(random.choice(letters) for i in range(length))
+
+
+# li = [get_random_string(8) for l in range(0, 10)]
+# w.TagsInput(allowed_tags=li)
+# # -
 
+# w.ToggleButtons(options=li)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/showopenurl.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/showopenurl.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.7/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.7/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/.gitignore` & `ipyautoui-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/LICENSE` & `ipyautoui-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/README.md` & `ipyautoui-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/pyproject.toml` & `ipyautoui-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.6/PKG-INFO` & `ipyautoui-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.6
+Version: 0.5.7
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

