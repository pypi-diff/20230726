# Comparing `tmp/sysml2py-0.4.3.tar.gz` & `tmp/sysml2py-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.4.3.tar", max compression
+gzip compressed data, was "sysml2py-0.4.4.tar", max compression
```

## Comparing `sysml2py-0.4.3.tar` & `sysml2py-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-07-25 02:52:20.556001 sysml2py-0.4.3/LICENSE
--rw-r--r--   0        0        0     3757 2023-07-25 02:52:20.556001 sysml2py-0.4.3/README.md
--rw-r--r--   0        0        0     1576 2023-07-25 02:52:21.436050 sysml2py-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3297 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/__init__.py
--rw-r--r--   0        0        0     8299 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/definition.py
--rw-r--r--   0        0        0     2297 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/formatting.py
--rw-r--r--   0        0        0    22296 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0        0        0    10762 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0        0        0    48820 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0        0        0   105339 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/classes.py
--rw-r--r--   0        0        0    28524 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/KerML.xtext
--rw-r--r--   0        0        0    14284 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/KerMLExpressions.xtext
--rw-r--r--   0        0        0    60663 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/SysML.xtext
--rw-r--r--   0        0        0     6279 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0        0        0    23886 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/usage.py
--rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-26 04:24:59.521984 sysml2py-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3757 2023-07-26 04:24:59.521984 sysml2py-0.4.4/README.md
+-rw-r--r--   0        0        0     1576 2023-07-26 04:25:00.545990 sysml2py-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3175 2023-07-26 04:24:59.521984 sysml2py-0.4.4/src/sysml2py/__init__.py
+-rw-r--r--   0        0        0     8377 2023-07-26 04:24:59.521984 sysml2py-0.4.4/src/sysml2py/definition.py
+-rw-r--r--   0        0        0     1288 2023-07-26 04:24:59.521984 sysml2py-0.4.4/src/sysml2py/formatting.py
+-rw-r--r--   0        0        0    22296 2023-07-26 04:24:59.521984 sysml2py-0.4.4/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0        0        0    10762 2023-07-26 04:24:59.521984 sysml2py-0.4.4/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0        0        0    48820 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0        0        0   105344 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/grammar/classes.py
+-rw-r--r--   0        0        0    28524 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/textx/KerML.xtext
+-rw-r--r--   0        0        0    14284 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/textx/KerMLExpressions.xtext
+-rw-r--r--   0        0        0    60663 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/textx/SysML.xtext
+-rw-r--r--   0        0        0     6279 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0        0        0    24765 2023-07-26 04:24:59.525984 sysml2py-0.4.4/src/sysml2py/usage.py
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.4/PKG-INFO
```

### Comparing `sysml2py-0.4.3/LICENSE` & `sysml2py-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/README.md` & `sysml2py-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/pyproject.toml` & `sysml2py-0.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #requires = ["setuptools>=61.0"]
 #build-backend = "setuptools.build_meta"
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "sysml2py"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -47,15 +47,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
 
 [tool.poetry]
 name = "sysml2py"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Christopher Cox <chris.cox@westfall.io>"]
 readme = "README.md"
 packages = [{ include = "sysml2py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sysml2py-0.4.3/src/sysml2py/__init__.py` & `sysml2py-0.4.4/src/sysml2py/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon May 29 23:26:16 2023
 
 @author: christophercox
 """
 
-__all__ = ["load", "loads"]
+__all__ = ["load", "loads", "load_grammar"]
 __author__ = "Christopher Cox"
 
 from sysml2py.usage import Item, Attribute, Part, Port
 from sysml2py.definition import Model, Package
 
 
-def load_grammar(fp, formatting="json"):
+def load_grammar(fp):
     """SysML load from file pointer
 
     Deserialize ``fp`` (a ``.read()``-supporting file-like object containing
     a SysML v2.0 document) or ``s`` (a ``str`` instance containing a SysML
     v2.0 document) to a Python dictionary object.
 
     Parameters
@@ -76,37 +76,29 @@
     import importlib.resources as pkg_resources
 
     from textx import metamodel_from_file, TextXSyntaxError
 
     import sysml2py
     from sysml2py.formatting import reformat
 
-    if not isinstance(s, str):
-        raise TypeError(f"the SysML object must be str, " f"not {s.__class__.__name__}")
-
-    try:
-        grammar = str((pkg_resources.files(sysml2py) / "grammar/SysML.tx"))
-    except:
-        try:
-            grammar = "./src/sysml2py/grammar/SysML.tx"
-        except:
-            grammar = "./grammar/SysML.tx"
+    # try:
+    grammar = str((pkg_resources.files(sysml2py) / "grammar/SysML.tx"))
+    # except:
+    #     try:
+    #         grammar = "./src/sysml2py/grammar/SysML.tx"
+    #     except:
+    #         grammar = "./grammar/SysML.tx"
     meta = metamodel_from_file(grammar)
     try:
         model = meta.model_from_str(s, debug=False)
     except TextXSyntaxError as e:
-        print(e)
-        import sys
+        print("TextX returned the following error: {}".format(e))
+        raise TextXSyntaxError("Invalid SysML")
 
-        sys.exit()
-
-    if formatting == "json":
-        return reformat(model)
-    else:
-        return model
+    return reformat(model)
 
 
 def load(fp):
     """SysML load from file pointer
 
     Deserialize ``fp`` (a ``.read()``-supporting file-like object containing
     a SysML v2.0 document) to a Python dictionary object.
```

### Comparing `sysml2py-0.4.3/src/sysml2py/definition.py` & `sysml2py-0.4.4/src/sysml2py/definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,31 +32,15 @@
         self.typedby = None
         self.grammar = None
 
     def load(self: type[ModelType], s: str) -> ModelType:
         from sysml2py import load_grammar
 
         # Try to load the grammar from the string
-        try:
-            definition = load_grammar(s)
-        except TextXSyntaxError:
-            import sys
-
-            print("Invalid SysML input, please correct the error.")
-            sys.exit()
-
-        # Ensure this is valid
-        if definition["name"] == "PackageBodyElement":
-            # This is a root element
-            definition = definition["ownedRelationship"]
-        else:
-            import sys
-
-            print("SysML does not match a base model.")
-            sys.exit()
+        definition = load_grammar(s)["ownedRelationship"]
 
         # Add each sub-element to children.
         member_grammar = []
         for member in definition:
             if member["ownedRelatedElement"]["name"] == "DefinitionElement":
                 de = member["ownedRelatedElement"]
                 if de["ownedRelatedElement"]["name"] == "Package":
@@ -229,14 +213,23 @@
                     == "ItemUsage"
                 ):
                     self.children.append(
                         Item().load_from_grammar(
                             child.children[0].children.children.children
                         )
                     )
+                elif (
+                    child.children[0].children.children.children.__class__.__name__
+                    == "PartUsage"
+                ):
+                    self.children.append(
+                        Part().load_from_grammar(
+                            child.children[0].children.children.children
+                        )
+                    )
                 else:
                     print(child.children[0].children[0].__class__.__name__)
                     raise NotImplementedError
             else:
                 # Not a UsageElement
                 if child.children[0].children[0].__class__.__name__ == "Package":
                     self.children.append(
@@ -250,7 +243,12 @@
                     )
                 else:
                     print(child.children[0].children[0].__class__.__name__)
                     raise NotImplementedError
 
         # self.children.append()
         return self
+
+    def _get_grammar(self):
+        # Force updates to grammar if something has changed.
+        self._ensure_body()
+        return self.grammar
```

### Comparing `sysml2py-0.4.3/src/sysml2py/formatting.py` & `sysml2py-0.4.4/src/sysml2py/formatting.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 Created on Wed May 31 13:26:53 2023
 
 @author: christophercox
 """
 
 from sysml2py.grammar.classes import RootNamespace
 
-# from sysml2py import Part
-
 
 def remove_classes(model):
     """An example docstring for a class definition."""
     if type(model) == type(dict()):
         output = {}
         for element in model:
             if not "_" in element[0] and not "parent" in element:
@@ -35,43 +33,15 @@
 
     return output
 
 
 def reformat(model):
     """An example docstring for a class definition."""
     # Convert to dictionary format
-    try:
-        model_out = {"name": model.__class__.__name__}
-        model_out.update(remove_classes(model.__dict__))
-    except Exception as e:
-        print(e)
-        print("Error in printing")
+    model_out = {"name": model.__class__.__name__}
+    model_out.update(remove_classes(model.__dict__))
 
     return model_out
 
 
 def classtree(model):
     return RootNamespace(model)
-
-
-# def collapse(model):
-#     """Take a classtree and collapse it into our special classes that
-#     package all of the sub-grammar classes."""
-#     output = []
-#     if model.__class__.__name__ == "RootNamespace":
-#         for child in model.children[0].children:
-#             if child.__class__.__name__ == "UsageElement":
-#                 ue = child.children
-#                 if ue.__class__.__name__ == "OccurrenceUsageElement":
-#                     se = ue.children
-#                     if se.children.__class__.__name__ == "PartUsage":
-#                         output.append(Part().load_from_grammar(se.children))
-#                     else:
-#                         pass
-#                 else:
-#                     # OccurrenceUsageElement
-#                     pass
-#             else:
-#                 pass
-#     else:
-#         print("no")
-#     return output
```

### Comparing `sysml2py-0.4.3/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.4.4/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.4.4/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.4.4/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/grammar/classes.py` & `sysml2py-0.4.4/src/sysml2py/grammar/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def valid_definition(definition, name):
     if isinstance(definition, dict):
         if "name" in definition:
             if definition["name"] == name:
                 return True
             else:
                 print(definition["name"])
-                raise NotImplementedError
+                raise ValueError("The name of the element did not match.")
 
         else:
             raise AttributeError("This does not seem to be valid.")
     else:
         print("\n\nDefinition: {}".format(definition))
         raise TypeError("This does not seem to be valid.")
 
@@ -43,26 +43,26 @@
 
     return "\n".join(ns)
 
 
 class RootNamespace:
     def __init__(self, definition):
         self.children = []
-        if "name" in definition:
-            if definition["name"] == "PackageBodyElement":
+        try:
+            if valid_definition(definition, "PackageBodyElement"):
                 # This is a SysML Element
                 self.load_package_body(definition["ownedRelationship"])
-            elif definition["name"] == "NamespaceBodyElement":
-                # This is a KerML Element
-                pass
-            else:
+        except ValueError:
+            try:
+                if valid_definition(definition, "NamespaceBodyElement"):
+                    # This is a KerML Element
+                    pass
+            except ValueError:
                 print(definition)
-                raise NotImplementedError("Not expecting any other root node names.")
-        else:
-            raise AttributeError("This does not seem to be valid.")
+                raise ValueError("Not expecting any other root node names.")
 
     def load_package_body(self, definition):
         for member in definition:
             if isinstance(member, dict):
                 # Options here are PackageMember, ElementFilterMember, AliasMember, Import
                 if member["name"] == "PackageMember":
                     memberclass = PackageMember(member)
```

### Comparing `sysml2py-0.4.3/src/sysml2py/textx/KerML.xtext` & `sysml2py-0.4.4/src/sysml2py/textx/KerML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/textx/KerMLExpressions.xtext` & `sysml2py-0.4.4/src/sysml2py/textx/KerMLExpressions.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/textx/SysML.xtext` & `sysml2py-0.4.4/src/sysml2py/textx/SysML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.4.4/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.3/src/sysml2py/usage.py` & `sysml2py-0.4.4/src/sysml2py/usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 "name": "DefinitionMember",
                 "prefix": None,
                 "ownedRelatedElement": [package],
             }
 
             package = {"name": "DefinitionBodyItem", "ownedRelationship": [package]}
 
-        elif child == "PackageBody":
+        elif child == "PackageBody" or child == None:
             # Add these packets to make this dump without parents
 
             package = {
                 "name": "PackageMember",
                 "ownedRelatedElement": package,
                 "prefix": None,
             }
@@ -146,16 +146,16 @@
             else:
                 package["ownedRelationship"].insert(
                     0, self.typedby._get_definition(child=child)["ownedRelationship"][0]
                 )
 
         return package
 
-    def dump(self):
-        return classtree(self._get_definition()).dump()
+    def dump(self, child=None):
+        return classtree(self._get_definition(child)).dump()
 
     def _set_name(self, name, short=False):
         if hasattr(self.grammar, "usage"):
             path = self.grammar.usage.declaration.declaration
         elif hasattr(self.grammar, "definition"):
             path = self.grammar.definition.declaration
         else:
@@ -202,15 +202,15 @@
                     return child._get_child(featurechain)
 
     def _set_typed_by(self, typed):
         # Only set if the pointed object is a definition
         if "definition" in typed.grammar.__dict__:
             self.typedby = typed
             if "definition" in self.grammar.__dict__:
-                raise NotImplementedError
+                raise ValueError("A definition element cannot be defined.")
             else:
                 if self.grammar.usage.declaration.declaration.specialization is None:
                     package = {
                         "name": "QualifiedName",
                         "name1": typed.name,
                         "names": [],
                     }
@@ -238,71 +238,77 @@
                         "specialization2": [],
                         "multiplicity2": None,
                     }
                     self.grammar.usage.declaration.declaration.specialization = (
                         FeatureSpecializationPart(package)
                     )
         else:
-            print(typed.grammar.__dict__)
-            raise NotImplementedError
+            raise ValueError("Typed by element was not a definition.")
         return self
 
+    def _get_grammar(self):
+        self._ensure_body()
+        return self.grammar
+
     def load_from_grammar(self, grammar):
         #!TODO Typed By
         self.__init__()
         self.grammar = grammar
         children = []
         if "usage" in self.grammar.__dict__:
             # This is a usage
             u_name = grammar.usage.declaration.declaration.identification.declaredName
             a_children = grammar.usage.completion.body.body.children
 
-            if len(a_children) > 0:
-                children = a_children[0].children[0].children
+            for child in a_children:
+                children.append(child.children[0].children[0])
         else:
             # This is a definition
             u_name = grammar.definition.declaration.identification.declaredName
             a_children = grammar.definition.body.children
             if len(a_children) > 0:
-                children = a_children
+                children = a_children[0]
 
         if u_name is not None:
             self.name = u_name
 
         for child in children:
-            if child.children.__class__.__name__ == "AttributeUsage":
-                self.children.append(Attribute().load_from_grammar(child.children))
-            elif child.children.__class__.__name__ == "StructureUsageElement":
-                if child.children.children.__class__.__name__ == "PartUsage":
-                    self.children.append(
-                        Part().load_from_grammar(child.children.children)
-                    )
-                elif child.children.children.__class__.__name__ == "ItemUsage":
-                    self.children.append(
-                        Item().load_from_grammar(child.children.children)
-                    )
+            sc = child.children
+            if isinstance(sc, list):
+                if len(sc) == 1:
+                    sc = sc[0]
+
+            if sc.__class__.__name__ == "AttributeUsage":
+                self.children.append(Attribute().load_from_grammar(sc))
+            elif sc.__class__.__name__ == "ItemDefinition":
+                self.children.append(Item().load_from_grammar(sc))
+            elif sc.__class__.__name__ == "StructureUsageElement":
+                if sc.children.__class__.__name__ == "PartUsage":
+                    self.children.append(Part().load_from_grammar(sc.children))
+                elif sc.children.__class__.__name__ == "ItemUsage":
+                    self.children.append(Item().load_from_grammar(sc.children))
                 else:
                     print(child.children.children.__class__.__name__)
                     raise NotImplementedError
             else:
-                print(child.children.__class__.__name__)
+                print(sc.__class__.__name__)
                 raise NotImplementedError
 
         return self
 
     def add_directed_feature(self, direction, name=str(uuidlib.uuid4())):
         self._set_child(DefaultReference()._set_name(name).set_direction(direction))
         return self
 
-    def modify_directed_feature(self, direction, name):
-        child = self._get_child(name)
-        if child is not None:
-            pass
-        else:
-            raise AttributeError("Invalid Feature Name or Chain")
+    # def modify_directed_feature(self, direction, name):
+    #     child = self._get_child(name)
+    #     if child is not None:
+    #         pass
+    #     else:
+    #         raise AttributeError("Invalid Feature Name or Chain")
 
 
 class Attribute(Usage):
     def __init__(self, definition=False, name=None):
         Usage.__init__(self)
 
         if definition:
@@ -339,157 +345,160 @@
             # Add these packets to make this dump without parents
             package = {"name": "UsageElement", "ownedRelatedElement": package}
             package = {
                 "name": "PackageMember",
                 "ownedRelatedElement": package,
                 "prefix": None,
             }
-            package = {
-                "name": "PackageBodyElement",
-                "ownedRelationship": [package],
-                "prefix": None,
-            }
         return package
 
     def set_value(self, value):
+        if not isinstance(value, u.quantity.Quantity):
+            value = value * u.one
         if isinstance(value, u.quantity.Quantity):
-            package_units = {
-                "name": "QualifiedName",
-                "name1": str(value.unit),
-                "names": [],
-            }
-            package_units = {
-                "name": "FeatureReferenceMember",
-                "memberElement": package_units,
-            }
-            package_units = {
-                "name": "FeatureReferenceExpression",
-                "ownedRelationship": [package_units],
-            }
-            package_units = {
-                "name": "BaseExpression",
-                "ownedRelationship": package_units,
-            }
-            package_units = {
-                "name": "PrimaryExpression",
-                "operand": [],
-                "base": package_units,
-                "operator": [],
-                "ownedRelationship": [],
-            }
-            package_units = {
-                "name": "ExtentExpression",
-                "operator": "",
-                "ownedRelationship": [],
-                "primary": package_units,
-            }
-            package_units = {
-                "name": "UnaryExpression",
-                "operand": [],
-                "operator": None,
-                "extent": package_units,
-            }
-            package_units = {
-                "name": "ExponentiationExpression",
-                "operand": [],
-                "operator": [],
-                "unary": package_units,
-            }
-            package_units = {
-                "name": "MultiplicativeExpression",
-                "operand": [],
-                "operator": [],
-                "exponential": package_units,
-            }
-            package_units = {
-                "name": "AdditiveExpression",
-                "operand": [],
-                "operator": [],
-                "multiplicitive": package_units,
-            }
-            package_units = {
-                "name": "RangeExpression",
-                "operand": [],
-                "operator": "",
-                "additive": package_units,
-            }
-            package_units = {
-                "name": "RelationalExpression",
-                "operand": [],
-                "operator": [],
-                "range": package_units,
-            }
-            package_units = {
-                "name": "ClassificationExpression",
-                "operand": [],
-                "operator": None,
-                "ownedRelationship": [],
-                "relational": package_units,
-            }
-            package_units = {
-                "name": "EqualityExpression",
-                "operand": [],
-                "operator": [],
-                "classification": package_units,
-            }
-            package_units = {
-                "name": "AndExpression",
-                "operand": [],
-                "operator": [],
-                "equality": package_units,
-            }
-            package_units = {
-                "name": "XorExpression",
-                "operand": [],
-                "operator": [],
-                "and": package_units,
-            }
-            package_units = {
-                "name": "OrExpression",
-                "xor": package_units,
-                "operand": [],
-                "operator": [],
-            }
-            package_units = {
-                "name": "ImpliesExpression",
-                "operand": [],
-                "operator": [],
-                "or": package_units,
-            }
-            package_units = {
-                "name": "NullCoalescingExpression",
-                "implies": package_units,
-                "operator": [],
-                "operand": [],
-            }
-            package_units = {
-                "name": "ConditionalExpression",
-                "operator": None,
-                "operand": [package_units],
-            }
-            package_units = {"name": "OwnedExpression", "expression": package_units}
-            package_units = {
-                "name": "SequenceExpression",
-                "operand": [],
-                "operator": "",
-                "ownedRelationship": package_units,
-            }
+            if str(value.unit) != "":
+                package_units = {
+                    "name": "QualifiedName",
+                    "name1": str(value.unit),
+                    "names": [],
+                }
+                package_units = {
+                    "name": "FeatureReferenceMember",
+                    "memberElement": package_units,
+                }
+                package_units = {
+                    "name": "FeatureReferenceExpression",
+                    "ownedRelationship": [package_units],
+                }
+                package_units = {
+                    "name": "BaseExpression",
+                    "ownedRelationship": package_units,
+                }
+                package_units = {
+                    "name": "PrimaryExpression",
+                    "operand": [],
+                    "base": package_units,
+                    "operator": [],
+                    "ownedRelationship": [],
+                }
+                package_units = {
+                    "name": "ExtentExpression",
+                    "operator": "",
+                    "ownedRelationship": [],
+                    "primary": package_units,
+                }
+                package_units = {
+                    "name": "UnaryExpression",
+                    "operand": [],
+                    "operator": None,
+                    "extent": package_units,
+                }
+                package_units = {
+                    "name": "ExponentiationExpression",
+                    "operand": [],
+                    "operator": [],
+                    "unary": package_units,
+                }
+                package_units = {
+                    "name": "MultiplicativeExpression",
+                    "operand": [],
+                    "operator": [],
+                    "exponential": package_units,
+                }
+                package_units = {
+                    "name": "AdditiveExpression",
+                    "operand": [],
+                    "operator": [],
+                    "multiplicitive": package_units,
+                }
+                package_units = {
+                    "name": "RangeExpression",
+                    "operand": [],
+                    "operator": "",
+                    "additive": package_units,
+                }
+                package_units = {
+                    "name": "RelationalExpression",
+                    "operand": [],
+                    "operator": [],
+                    "range": package_units,
+                }
+                package_units = {
+                    "name": "ClassificationExpression",
+                    "operand": [],
+                    "operator": None,
+                    "ownedRelationship": [],
+                    "relational": package_units,
+                }
+                package_units = {
+                    "name": "EqualityExpression",
+                    "operand": [],
+                    "operator": [],
+                    "classification": package_units,
+                }
+                package_units = {
+                    "name": "AndExpression",
+                    "operand": [],
+                    "operator": [],
+                    "equality": package_units,
+                }
+                package_units = {
+                    "name": "XorExpression",
+                    "operand": [],
+                    "operator": [],
+                    "and": package_units,
+                }
+                package_units = {
+                    "name": "OrExpression",
+                    "xor": package_units,
+                    "operand": [],
+                    "operator": [],
+                }
+                package_units = {
+                    "name": "ImpliesExpression",
+                    "operand": [],
+                    "operator": [],
+                    "or": package_units,
+                }
+                package_units = {
+                    "name": "NullCoalescingExpression",
+                    "implies": package_units,
+                    "operator": [],
+                    "operand": [],
+                }
+                package_units = {
+                    "name": "ConditionalExpression",
+                    "operator": None,
+                    "operand": [package_units],
+                }
+                package_units = {"name": "OwnedExpression", "expression": package_units}
+                package_units = {
+                    "name": "SequenceExpression",
+                    "operand": [],
+                    "operator": "",
+                    "ownedRelationship": package_units,
+                }
+                package_units = [package_units]
+                operator = ["["]
+            else:
+                package_units = []
+                operator = []
 
             package = {
                 "name": "BaseExpression",
                 "ownedRelationship": {
                     "name": "LiteralInteger",
                     "value": str(value.value),
                 },
             }
             package = {
                 "name": "PrimaryExpression",
-                "operand": [package_units],
+                "operand": package_units,
                 "base": package,
-                "operator": ["["],
+                "operator": operator,
                 "ownedRelationship": [],
             }
             package = {
                 "name": "ExtentExpression",
                 "operator": "",
                 "ownedRelationship": [],
                 "primary": package,
@@ -648,15 +657,15 @@
         if direction == "in":
             r.direction.isIn = True
         elif direction == "out":
             r.direction.isOut = True
         elif direction == "inout":
             r.direction.isInOut = True
         else:
-            raise NotImplementedError
+            raise ValueError
         self.grammar.prefix = r
         return self
 
     def usage_dump(self, child):
         # This is a usage.
 
         self._ensure_body("definition")
@@ -706,31 +715,31 @@
             else:
                 package["ownedRelationship"].insert(
                     0, self.typedby._get_definition(child=child)["ownedRelationship"][0]
                 )
 
         return package
 
-    def dump(self, child=None):
-        package = self.usage_dump(child)
+    # def dump(self, child=None):
+    #     package = self.usage_dump(child)
 
-        if child is None:
-            package = {
-                "name": "PackageBodyElement",
-                "ownedRelationship": [package],
-                "prefix": None,
-            }
-
-        # Add the typed by definition to the package output
-        if self.typedby is not None:
-            if child is None:
-                package["ownedRelationship"].insert(
-                    0, self.typedby.dump(child="PackageBody")
-                )
-            elif child == "PackageBody":
-                package = [self.typedby.dump(child="PackageBody"), package]
-            else:
-                package["ownedRelationship"].insert(
-                    0, self.typedby.dump(child=child)["ownedRelationship"][0]
-                )
+    #     if child is None:
+    #         package = {
+    #             "name": "PackageBodyElement",
+    #             "ownedRelationship": [package],
+    #             "prefix": None,
+    #         }
+
+    #     # Add the typed by definition to the package output
+    #     if self.typedby is not None:
+    #         if child is None:
+    #             package["ownedRelationship"].insert(
+    #                 0, self.typedby.dump(child="PackageBody")
+    #             )
+    #         elif child == "PackageBody":
+    #             package = [self.typedby.dump(child="PackageBody"), package]
+    #         else:
+    #             package["ownedRelationship"].insert(
+    #                 0, self.typedby.dump(child=child)["ownedRelationship"][0]
+    #             )
 
-        return package
+    #     return package
```

### Comparing `sysml2py-0.4.3/PKG-INFO` & `sysml2py-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: Christopher Cox
 Author-email: chris.cox@westfall.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

