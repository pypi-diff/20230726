# Comparing `tmp/bump_pydantic-0.6.0.tar.gz` & `tmp/bump_pydantic-0.6.1.tar.gz`

## Comparing `bump_pydantic-0.6.0.tar` & `bump_pydantic-0.6.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/__init__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/__main__.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/glob_helpers.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/py.typed
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/__init__.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/add_default_none.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/class_def_visitor.py
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/con_func.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/field.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/replace_config.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/replace_generic_model.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/replace_imports.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/root_model.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/bump_pydantic/codemods/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/case.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/file.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/folder.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/add_none.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/base_settings.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/con_func.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/config_to_model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/field.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/folder_inside_folder.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/is_base_model.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/replace_validator.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/root_model.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/integration/cases/unicode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_add_default_none.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_class_def_visitor.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_con_func.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_field.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_generic_model.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_glob_helpers.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_replace_config.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_replace_imports.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_root_model.py
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/tests/unit/test_validator.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/README.md
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 bump_pydantic-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/__init__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/__main__.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/glob_helpers.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/py.typed
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/__init__.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/add_default_none.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/class_def_visitor.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/con_func.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/field.py
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/replace_config.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/replace_generic_model.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/replace_imports.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/root_model.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/bump_pydantic/codemods/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/case.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/file.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/folder.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/add_none.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/base_settings.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/con_func.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/config_to_model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/field.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/folder_inside_folder.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/is_base_model.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/replace_validator.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/root_model.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/integration/cases/unicode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_add_default_none.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_class_def_visitor.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_con_func.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_field.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_generic_model.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_glob_helpers.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_replace_config.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_replace_imports.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_root_model.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/tests/unit/test_validator.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/README.md
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 bump_pydantic-0.6.1/PKG-INFO
```

### Comparing `bump_pydantic-0.6.0/.github/workflows/main.yml` & `bump_pydantic-0.6.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/glob_helpers.py` & `bump_pydantic-0.6.1/bump_pydantic/glob_helpers.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/main.py` & `bump_pydantic-0.6.1/bump_pydantic/main.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/.github/workflows/ci.yml` & `bump_pydantic-0.6.1/bump_pydantic/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/__init__.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     BP005 = "BP005"
     """Replace `GenericModel` with `BaseModel`."""
     BP006 = "BP006"
     """Replace `BaseModel.__root__ = T` with `RootModel[T]`."""
     BP007 = "BP007"
     """Replace `@validator` with `@field_validator`."""
     BP008 = "BP008"
-    """Replace `constr(<args>)` with `Annotated[str, StringConstraints(<args>)`."""
+    """Replace `con*` functions by `Annotated` versions."""
 
 
 def gather_codemods(disabled: List[Rule]) -> List[Type[ContextAwareTransformer]]:
     codemods: List[Type[ContextAwareTransformer]] = []
 
     if Rule.BP001 not in disabled:
         codemods.append(AddDefaultNoneCommand)
```

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/add_default_none.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/add_default_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/class_def_visitor.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/class_def_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/con_func.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/con_func.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,32 +2,26 @@
 
 import libcst as cst
 from libcst import matchers as m
 from libcst.codemod import CodemodContext, VisitorBasedCodemodCommand
 from libcst.codemod.visitors import AddImportsVisitor, RemoveImportsVisitor
 
 CONSTR_CALL = m.Call(func=m.Name("constr") | m.Attribute(value=m.Name("pydantic"), attr=m.Name("constr")))
-ANN_ASSIGN_CONSTR_CALL = m.AnnAssign(annotation=m.Annotation(annotation=CONSTR_CALL))
-
-
 CON_NUMBER_CALL = m.OneOf(
     *[
         m.Call(func=m.Name(name) | m.Attribute(value=m.Name("pydantic"), attr=m.Name(name)))
         for name in ("conint", "confloat", "condecimal", "conbytes")
     ]
 )
-ANN_ASSIGN_CON_NUMBER_CALL = m.AnnAssign(annotation=m.Annotation(annotation=CON_NUMBER_CALL))
-
 CON_COLLECTION_CALL = m.OneOf(
     *[
         m.Call(func=m.Name(name) | m.Attribute(value=m.Name("pydantic"), attr=m.Name(name)))
         for name in ("conlist", "conset", "confrozenset")
     ]
 )
-ANN_ASSIGN_COLLECTION_CALL = m.AnnAssign(annotation=m.Annotation(annotation=CON_COLLECTION_CALL))
 
 MAP_FUNC_TO_TYPE = {
     "constr": "str",
     "conint": "int",
     "confloat": "float",
     "condecimal": "Decimal",
     "conbytes": "bytes",
@@ -44,27 +38,22 @@
 COLLECTIONS = ("List", "Set", "FrozenSet")
 
 
 class ConFuncCallCommand(VisitorBasedCodemodCommand):
     def __init__(self, context: CodemodContext) -> None:
         super().__init__(context)
 
-    @m.leave(ANN_ASSIGN_CONSTR_CALL | ANN_ASSIGN_CON_NUMBER_CALL | ANN_ASSIGN_COLLECTION_CALL)
-    def leave_ann_assign_constr_call(self, original_node: cst.AnnAssign, updated_node: cst.AnnAssign) -> cst.AnnAssign:
-        annotation = cast(cst.Call, original_node.annotation.annotation)
-        if m.matches(annotation.func, m.Name()):
-            func_name = cast(str, annotation.func.value)  # type: ignore
+    @m.leave(CON_NUMBER_CALL | CON_COLLECTION_CALL | CONSTR_CALL)
+    def leave_annotation_call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Subscript:
+        if m.matches(original_node.func, m.Name()):
+            func_name = cast(str, original_node.func.value)  # type: ignore
         else:
-            func_name = cast(str, annotation.func.attr.value)  # type: ignore
+            func_name = cast(str, original_node.func.attr.value)  # type: ignore
         type_name = MAP_FUNC_TO_TYPE[func_name]
 
-        # TODO: When FastAPI supports Pydantic 2.0.4+, remove the conditional below.
-        if func_name == "constr":
-            return updated_node
-
         needed_import = MAP_TYPE_TO_NEEDED_IMPORT.get(type_name)
         if needed_import is not None:
             AddImportsVisitor.add_needed_import(context=self.context, **needed_import)  # type: ignore[arg-type]
 
         if type_name in COLLECTIONS:
             slice_value = cst.Index(
                 value=cst.Subscript(
@@ -72,31 +61,28 @@
                     slice=[cst.SubscriptElement(slice=cst.Index(value=self.inner_type))],
                 )
             )
         else:
             slice_value = cst.Index(value=cst.Name(type_name))
 
         AddImportsVisitor.add_needed_import(context=self.context, module="typing_extensions", obj="Annotated")
-        annotated = cst.Subscript(
+        return cst.Subscript(
             value=cst.Name("Annotated"),
             slice=[
                 cst.SubscriptElement(slice=slice_value),
-                cst.SubscriptElement(slice=cst.Index(value=updated_node.annotation.annotation)),
+                cst.SubscriptElement(slice=cst.Index(value=updated_node)),
             ],
         )
-        annotation = cst.Annotation(annotation=annotated)  # type: ignore[assignment]
-        return updated_node.with_changes(annotation=annotation)
 
-    # TODO: When FastAPI supports Pydantic 2.0.4+, remove the comments below.
     @m.leave(CONSTR_CALL)
     def leave_constr_call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
         self._remove_import(original_node.func)
-        # AddImportsVisitor.add_needed_import(context=self.context, module="pydantic", obj="StringConstraints")
+        AddImportsVisitor.add_needed_import(context=self.context, module="pydantic", obj="StringConstraints")
         return updated_node.with_changes(
-            # func=cst.Name("StringConstraints"),
+            func=cst.Name("StringConstraints"),
             args=[
                 arg if arg.keyword and arg.keyword.value != "regex" else arg.with_changes(keyword=cst.Name("pattern"))
                 for arg in updated_node.args
             ],
         )
 
     @m.leave(CON_NUMBER_CALL)
```

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/field.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/replace_config.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/replace_generic_model.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/replace_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/replace_imports.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/root_model.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/bump_pydantic/codemods/validator.py` & `bump_pydantic-0.6.1/bump_pydantic/codemods/validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/folder.py` & `bump_pydantic-0.6.1/tests/integration/folder.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/test_cli.py` & `bump_pydantic-0.6.1/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/__init__.py` & `bump_pydantic-0.6.1/tests/integration/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/add_none.py` & `bump_pydantic-0.6.1/tests/integration/cases/add_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/base_settings.py` & `bump_pydantic-0.6.1/tests/integration/cases/base_settings.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/con_func.py` & `bump_pydantic-0.6.1/tests/integration/cases/con_func.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,30 +14,34 @@
                 "    a: constr(regex='[a-z]+')",
                 "    b: conlist(int, min_items=1, max_items=10)",
                 "    c: conint(gt=0, lt=10)",
                 "    d: conbytes(min_length=1, max_length=10)",
                 "    e: condecimal(gt=0, lt=10)",
                 "    f: confloat(gt=0, lt=10)",
                 "    g: conset(int, min_items=1, max_items=10)",
+                "    h: Optional[conint(ge=1, le=4294967295)] = None",
+                "    i: dict[str, condecimal(max_digits=10, decimal_places=2)]",
             ],
         ),
         expected=File(
             "con_func.py",
             content=[
-                "from pydantic import Field, BaseModel, constr",
+                "from pydantic import Field, StringConstraints, BaseModel",
                 "from decimal import Decimal",
                 "from typing import List, Set",
                 "from typing_extensions import Annotated",
                 "",
                 "",
                 "class Potato(BaseModel):",
-                "    a: constr(pattern='[a-z]+')",
+                "    a: Annotated[str, StringConstraints(pattern='[a-z]+')]",
                 "    b: Annotated[List[int], Field(min_length=1, max_length=10)]",
                 "    c: Annotated[int, Field(gt=0, lt=10)]",
                 "    d: Annotated[bytes, Field(min_length=1, max_length=10)]",
                 "    e: Annotated[Decimal, Field(gt=0, lt=10)]",
                 "    f: Annotated[float, Field(gt=0, lt=10)]",
                 "    g: Annotated[Set[int], Field(min_length=1, max_length=10)]",
+                "    h: Optional[Annotated[int, Field(ge=1, le=4294967295)]] = None",
+                "    i: dict[str, Annotated[Decimal, Field(max_digits=10, decimal_places=2)]]",
             ],
         ),
     )
 ]
```

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/config_to_model.py` & `bump_pydantic-0.6.1/tests/integration/cases/config_to_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/field.py` & `bump_pydantic-0.6.1/tests/integration/cases/field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/folder_inside_folder.py` & `bump_pydantic-0.6.1/tests/integration/cases/folder_inside_folder.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/is_base_model.py` & `bump_pydantic-0.6.1/tests/integration/cases/is_base_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/replace_validator.py` & `bump_pydantic-0.6.1/tests/integration/cases/replace_validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/root_model.py` & `bump_pydantic-0.6.1/tests/integration/cases/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/integration/cases/unicode.py` & `bump_pydantic-0.6.1/tests/integration/cases/unicode.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_add_default_none.py` & `bump_pydantic-0.6.1/tests/unit/test_add_default_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_class_def_visitor.py` & `bump_pydantic-0.6.1/tests/unit/test_class_def_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_con_func.py` & `bump_pydantic-0.6.1/tests/unit/test_con_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import pytest
 from libcst.codemod import CodemodTest
 
 from bump_pydantic.codemods.con_func import ConFuncCallCommand
 
 
 class TestFieldCommand(CodemodTest):
     TRANSFORM = ConFuncCallCommand
 
     maxDiff = None
 
-    @pytest.mark.xfail(reason="Annotated is not supported yet!")
     def test_constr_to_annotated(self) -> None:
         before = """
         from pydantic import BaseModel, constr
 
         class Potato(BaseModel):
             potato: constr(min_length=1, max_length=10)
         """
@@ -22,15 +20,14 @@
         from typing_extensions import Annotated
 
         class Potato(BaseModel):
             potato: Annotated[str, StringConstraints(min_length=1, max_length=10)]
         """
         self.assertCodemod(before, after)
 
-    @pytest.mark.xfail(reason="Annotated is not supported yet!")
     def test_pydantic_constr_to_annotated(self) -> None:
         before = """
         import pydantic
         from pydantic import BaseModel
 
         class Potato(BaseModel):
             potato: pydantic.constr(min_length=1, max_length=10)
@@ -72,7 +69,25 @@
         from pydantic import Field, BaseModel
         from typing_extensions import Annotated
 
         class Potato(BaseModel):
             potato: Annotated[int, Field(ge=0, le=100)]
         """
         self.assertCodemod(before, after)
+
+    def test_conint_to_optional_annotated(self) -> None:
+        before = """
+        from typing import Optional
+        from pydantic import BaseModel, conint
+
+        class Potato(BaseModel):
+            potato: Optional[conint(ge=0, le=100)]
+        """
+        after = """
+        from typing import Optional
+        from pydantic import Field, BaseModel
+        from typing_extensions import Annotated
+
+        class Potato(BaseModel):
+            potato: Optional[Annotated[int, Field(ge=0, le=100)]]
+        """
+        self.assertCodemod(before, after)
```

### Comparing `bump_pydantic-0.6.0/tests/unit/test_field.py` & `bump_pydantic-0.6.1/tests/unit/test_field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_generic_model.py` & `bump_pydantic-0.6.1/tests/unit/test_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_glob_helpers.py` & `bump_pydantic-0.6.1/tests/unit/test_glob_helpers.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_replace_config.py` & `bump_pydantic-0.6.1/tests/unit/test_replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_replace_imports.py` & `bump_pydantic-0.6.1/tests/unit/test_replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_root_model.py` & `bump_pydantic-0.6.1/tests/unit/test_root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/tests/unit/test_validator.py` & `bump_pydantic-0.6.1/tests/unit/test_validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/.gitignore` & `bump_pydantic-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/LICENSE.txt` & `bump_pydantic-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/README.md` & `bump_pydantic-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 
 
 Bump Pydantic is a tool to help you migrate your code from Pydantic V1 to V2.
 
 
-> **Note**
+> [!NOTE]\
 > If you find bugs, please report them on the [issue tracker](https://github.com/pydantic/bump-pydantic/issues/new).
 
 ## Table of contents
 
 - [Bump Pydantic ♻️](#bump-pydantic-️)
   - [Table of contents](#table-of-contents)
   - [Installation](#installation)
@@ -182,14 +182,15 @@
     name: str
 ```
 
 Into:
 
 ```py
 from typing import Generic, TypeVar
+from pydantic import BaseModel
 
 T = TypeVar('T')
 
 class User(BaseModel, Generic[T]):
     name: str
 ```
 
@@ -213,15 +214,15 @@
 ```
 
 Into:
 
 ```py
 from typing import List
 
-from pydantic import RootModel
+from pydantic import RootModel, BaseModel
 
 class User(BaseModel):
     age: int
     name: str
 
 class Users(RootModel[List[User]]):
     pass
```

### Comparing `bump_pydantic-0.6.0/pyproject.toml` & `bump_pydantic-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.6.0/PKG-INFO` & `bump_pydantic-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-pydantic
-Version: 0.6.0
+Version: 0.6.1
 Summary: Convert Pydantic from V1 to V2 ♻
 Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
 Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
 Project-URL: Source, https://github.com/pydantic/bump-pydantic
 Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -29,15 +29,15 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 
 
 Bump Pydantic is a tool to help you migrate your code from Pydantic V1 to V2.
 
 
-> **Note**
+> [!NOTE]\
 > If you find bugs, please report them on the [issue tracker](https://github.com/pydantic/bump-pydantic/issues/new).
 
 ## Table of contents
 
 - [Bump Pydantic ♻️](#bump-pydantic-️)
   - [Table of contents](#table-of-contents)
   - [Installation](#installation)
@@ -208,14 +208,15 @@
     name: str
 ```
 
 Into:
 
 ```py
 from typing import Generic, TypeVar
+from pydantic import BaseModel
 
 T = TypeVar('T')
 
 class User(BaseModel, Generic[T]):
     name: str
 ```
 
@@ -239,15 +240,15 @@
 ```
 
 Into:
 
 ```py
 from typing import List
 
-from pydantic import RootModel
+from pydantic import RootModel, BaseModel
 
 class User(BaseModel):
     age: int
     name: str
 
 class Users(RootModel[List[User]]):
     pass
```

