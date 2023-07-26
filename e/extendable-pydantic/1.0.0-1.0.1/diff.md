# Comparing `tmp/extendable_pydantic-1.0.0.tar.gz` & `tmp/extendable_pydantic-1.0.1.tar.gz`

## Comparing `extendable_pydantic-1.0.0.tar` & `extendable_pydantic-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/extendable_pydantic_patcher.pth
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/_patch.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/py.typed
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/version.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/LICENSE
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/README.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/extendable_pydantic_patcher.pth
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/_patch.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/py.typed
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/version.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/PKG-INFO
```

### Comparing `extendable_pydantic-1.0.0/src/extendable_pydantic/_patch.py` & `extendable_pydantic-1.0.1/src/extendable_pydantic/_patch.py`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.0/src/extendable_pydantic/main.py` & `extendable_pydantic-1.0.1/src/extendable_pydantic/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,24 +90,14 @@
         cls, registry: Optional[ExtendableClassesRegistry] = None
     ) -> None:
         """Replace the original field type into the definition of the field by the one
         from the registry."""
         registry = registry if registry else context.extendable_registry.get()
         to_rebuild = False
         if issubclass(cls, BaseModel):
-            type_namespace = cast(BaseModel, cls).__pydantic_parent_namespace__ or {}
-            name_space = type_namespace.get("namespace", {})
-            for field_name, annoted_type in name_space.get(
-                "__annotations__", {}
-            ).items():
-                if issubclass(type(annoted_type), ExtendableModelMeta):
-                    name_space["__annotations__"][
-                        field_name
-                    ] = annoted_type._get_assembled_cls(registry)
-                    to_rebuild = True
             for field_name, field_info in cast(BaseModel, cls).model_fields.items():
                 new_type = resolve_annotation(field_info.annotation, registry)
                 if not all_identical(field_info.annotation, new_type):
                     cast(BaseModel, cls).model_fields[
                         field_name
                     ] = FieldInfo.from_annotation(new_type)
                     to_rebuild = True
```

### Comparing `extendable_pydantic-1.0.0/src/extendable_pydantic/utils.py` & `extendable_pydantic-1.0.1/src/extendable_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.0/.gitignore` & `extendable_pydantic-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.0/LICENSE` & `extendable_pydantic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.0/README.md` & `extendable_pydantic-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.0/pyproject.toml` & `extendable_pydantic-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.0/PKG-INFO` & `extendable_pydantic-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable_pydantic
-Version: 1.0.0
+Version: 1.0.1
 Project-URL: Source, https://github.com/lmignon/extendable-pydantic
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 License: MIT License
         
         Copyright (c) 2021 Laurent Mignon (ACSONE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

