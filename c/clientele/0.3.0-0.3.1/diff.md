# Comparing `tmp/clientele-0.3.0.tar.gz` & `tmp/clientele-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.3.0.tar", max compression
+gzip compressed data, was "clientele-0.3.1.tar", max compression
```

## Comparing `clientele-0.3.0.tar` & `clientele-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1306 2023-07-25 02:54:52.074475 clientele-0.3.0/README.md
--rw-r--r--   0        0        0      896 2023-07-25 00:37:07.430216 clientele-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.3.0/src/__init__.py
--rw-r--r--   0        0        0     1894 2023-07-24 23:26:08.953873 clientele-0.3.0/src/cli.py
--rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.3.0/src/constants_template.py
--rw-r--r--   0        0        0     2055 2023-07-24 23:26:23.378037 clientele-0.3.0/src/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.3.0/src/generators/__init__.py
--rw-r--r--   0        0        0     7656 2023-07-24 21:16:51.549353 clientele-0.3.0/src/generators/clients.py
--rw-r--r--   0        0        0     2976 2023-07-24 22:56:42.864879 clientele-0.3.0/src/generators/http.py
--rw-r--r--   0        0        0     3621 2023-07-24 04:14:37.896419 clientele-0.3.0/src/generators/schemas.py
--rw-r--r--   0        0        0      190 2023-07-24 21:03:06.895168 clientele-0.3.0/src/settings.py
--rw-r--r--   0        0        0       61 2023-07-24 20:44:55.813864 clientele-0.3.0/src/template/MANIFEST
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.3.0/src/template/__init__.py
--rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.3.0/src/template/client.py
--rw-r--r--   0        0        0      974 2023-07-24 21:23:51.037441 clientele-0.3.0/src/template/http.py
--rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.3.0/src/template/schemas.py
--rw-r--r--   0        0        0     1942 2023-07-24 04:16:31.046189 clientele-0.3.0/src/utils.py
--rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.3.0/src/writer.py
--rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 clientele-0.3.0/setup.py
--rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 clientele-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1310 2023-07-25 03:26:20.606725 clientele-0.3.1/README.md
+-rw-r--r--   0        0        0      898 2023-07-25 22:19:00.792847 clientele-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.3.1/src/__init__.py
+-rw-r--r--   0        0        0     1896 2023-07-25 03:26:44.875798 clientele-0.3.1/src/cli.py
+-rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.3.1/src/constants_template.py
+-rw-r--r--   0        0        0     2055 2023-07-24 23:26:23.378037 clientele-0.3.1/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.3.1/src/generators/__init__.py
+-rw-r--r--   0        0        0     7660 2023-07-25 22:22:46.450989 clientele-0.3.1/src/generators/clients.py
+-rw-r--r--   0        0        0     2997 2023-07-25 21:56:31.511282 clientele-0.3.1/src/generators/http.py
+-rw-r--r--   0        0        0     3577 2023-07-25 22:09:26.862604 clientele-0.3.1/src/generators/schemas.py
+-rw-r--r--   0        0        0      190 2023-07-25 22:18:53.608786 clientele-0.3.1/src/settings.py
+-rw-r--r--   0        0        0       61 2023-07-24 20:44:55.813864 clientele-0.3.1/src/template/MANIFEST
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.3.1/src/template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.3.1/src/template/client.py
+-rw-r--r--   0        0        0      974 2023-07-25 22:23:05.603189 clientele-0.3.1/src/template/http.py
+-rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.3.1/src/template/schemas.py
+-rw-r--r--   0        0        0     2107 2023-07-25 22:16:25.551674 clientele-0.3.1/src/utils.py
+-rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.3.1/src/writer.py
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 clientele-0.3.1/setup.py
+-rw-r--r--   0        0        0     2152 1970-01-01 00:00:00.000000 clientele-0.3.1/PKG-INFO
```

### Comparing `clientele-0.3.0/README.md` & `clientele-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ⚜️ Clientele
 
-# Typed API Clients from OpenAPI specs
+# Typed API Clients from OpenAPI schemas
 
 ![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)
 
-Clientele lets you generate fully-typed, functional, API Clients from OpenAPI specs.
+Clientele lets you generate fully-typed, functional, API Clients from OpenAPI schemas.
 
 It uses modern tools to be blazing fast and type safe.
 
 Plus - there is no complex boilerplate and the generated code is very small.
 
 ## Features
```

### Comparing `clientele-0.3.0/pyproject.toml` & `clientele-0.3.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "clientele"
-version = "0.3.0"
-description = "Typed API Clients from OpenAPI specs"
+version = "0.3.1"
+description = "Typed API Clients from OpenAPI schemas"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
 homepage = "https://beckett-software.github.io/clientele/"
 
 [tool.poetry.scripts]
```

### Comparing `clientele-0.3.0/src/cli.py` & `clientele-0.3.1/src/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
 
 @click.group()
 def cli_group():
     """
-    Clientele:  Typed API Clients from OpenAPI specs
+    Clientele:  Typed API Clients from OpenAPI schemas
     """
 
 
 @click.command()
 @click.option("-u", "--url", help="URL to openapi schema (json file)", required=False)
 @click.option("-f", "--file", help="Path to openapi schema (json file)", required=False)
 @click.option(
```

### Comparing `clientele-0.3.0/src/constants_template.py` & `clientele-0.3.1/src/constants_template.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.0/src/generator.py` & `clientele-0.3.1/src/generator.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.0/src/generators/clients.py` & `clientele-0.3.1/src/generators/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
     def generate_post_content(self, operation: Dict, path: str) -> None:
         response_types = self.generate_response_types(operation["responses"])
         func_name = get_func_name(operation, path)
         if not operation.get("requestBody"):
             input_class_name = "None"
         else:
-            input_class_name = self.generate_input_types(operation.get("requestBody"))
+            input_class_name = self.generate_input_types(operation.get("requestBody", {}))
         function_arguments = self.generate_function_args(
             operation.get("parameters", [])
         )
         FUNCTION_ARGS = f"""
 {function_arguments['return_string']}{function_arguments['return_string'] and ", "}data: {input_class_name}"""
         CONTENT = f"""
 {self.asyncio and "async " or ""}def {func_name}({FUNCTION_ARGS}) -> {response_types}:
```

### Comparing `clientele-0.3.0/src/generators/http.py` & `clientele-0.3.1/src/generators/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from rich.console import Console
 
 from src.writer import write_to_http
 
 console = Console()
 
 BEARER_CLIENT = """
-headers = dict(Authorization=f'Bearer {c.get_bearer_token()}')
+auth_key = c.get_bearer_token()
+headers = dict(Authorization=f'Bearer ' + auth_key)
 client = httpx.{client_type}(headers=headers)
 """
 
 BASIC_CLIENT = """
 client = httpx.{client_type}(auth=(c.get_user_key(), c.get_pass_key()))
 """
```

### Comparing `clientele-0.3.0/src/generators/schemas.py` & `clientele-0.3.1/src/generators/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,36 +49,35 @@
             content = (
                 content
                 + f"""    {clean_prop(arg)}: {is_optional and f"typing.Optional[{arg_type}]" or arg_type}\n"""
             )
         return content
 
     def generate_input_class(self, schema: Dict) -> None:
-        for _, schema_details in schema.items():
-            content = schema_details["content"]
+        if content := schema.get("content"):
             for encoding, input_schema in content.items():
                 class_name = ""
                 if ref := input_schema["schema"].get("$ref", False):
                     class_name = class_name_titled(
                         ref.replace("#/components/schemas/", "")
                     )
                 elif title := input_schema["schema"].get("title", False):
                     class_name = class_name_titled(title)
                 else:
                     # No idea, using the encoding?
                     class_name = class_name_titled(encoding)
                 properties = self.generate_class_properties(
                     input_schema["schema"].get("properties", {})
                 )
-                content = f"""
+                out_content = f"""
 class {class_name}(BaseModel):
 {properties if properties else "    pass"}
     """
             write_to_schemas(
-                content,
+                out_content,
                 output_dir=self.output_dir,
             )
 
     def generate_schema_classes(self) -> None:
         """
         Generates the Pydantic response classes.
         """
```

### Comparing `clientele-0.3.0/src/template/http.py` & `clientele-0.3.1/src/template/http.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.0/src/utils.py` & `clientele-0.3.1/src/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import Dict
 
 
 class DataType:
     INTEGER = "integer"
     NUMBER = "number"
     STRING = "string"
@@ -37,19 +38,29 @@
         input_str = input_str.replace(badstr, "_")
     reserved_words = ["from"]
     if input_str in reserved_words:
         input_str = input_str + "_"
     return input_str
 
 
+def _split_upper(s):
+    return "_".join(re.findall(".[^A-Z]*", s))
+
+
+def _snake_case(s):
+    for badchar in ["/", "-", "."]:
+        s = s.replace(badchar, "_")
+    s = _split_upper(s)
+    return s.lower()
+
+
 def get_func_name(operation: Dict, path: str) -> str:
     if operation.get("operationId"):
-        return class_name_titled(operation["operationId"].split("__")[0])
-    # Probably 3.0.1
-    return path.replace("/", "_").replace("-", "_")[1:]
+        return _snake_case(operation["operationId"].split("__")[0])
+    return _snake_case(path)
 
 
 def get_type(t):
     t_type = t.get("type")
     if t_type == DataType.STRING:
         return "str"
     if t_type in [DataType.INTEGER, DataType.NUMBER]:
```

### Comparing `clientele-0.3.0/src/writer.py` & `clientele-0.3.1/src/writer.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.0/setup.py` & `clientele-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'types-pyyaml>=6.0.12.11,<7.0.0.0']
 
 entry_points = \
 {'console_scripts': ['clientele = src.cli:cli_group']}
 
 setup_kwargs = {
     'name': 'clientele',
-    'version': '0.3.0',
-    'description': 'Typed API Clients from OpenAPI specs',
-    'long_description': "# ⚜️ Clientele\n\n# Typed API Clients from OpenAPI specs\n\n![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)\n\nClientele lets you generate fully-typed, functional, API Clients from OpenAPI specs.\n\nIt uses modern tools to be blazing fast and type safe.\n\nPlus - there is no complex boilerplate and the generated code is very small.\n\n## Features\n\n* Fully typed API Client using Pydantic.\n* Minimalist and easy to use - the generated code is designed for readability.\n* Choose either sync or async - we support both, and you can switch between them easily.\n* Supports authentication (curently only HTTP Bearer and HTTP Basic auth).\n* Written entirely in Python - no need to install other languages to use OpenAPI.\n* The client footprint is minimal - it only requires `httpx` and `pydantic`.\n* Supports your own configuration - we provide an entry point that will never be overwritten.\n\nWe're built on:\n\n* [Pydantic 2.0](https://docs.pydantic.dev/latest/)\n* [httpx](https://www.python-httpx.org/)\n* [openapi-core](https://openapi-core.readthedocs.io/en/latest/)\n\n## Install\n\n```sh\npoetry add clientele\n```\n\n## Usage\n\n```sh\nclientele generate -f path/to/file.json -o my_client/ --asyncio t\n```\n\n[Read the docs](https://beckett-software.github.io/clientele/)\n",
+    'version': '0.3.1',
+    'description': 'Typed API Clients from OpenAPI schemas',
+    'long_description': "# ⚜️ Clientele\n\n# Typed API Clients from OpenAPI schemas\n\n![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)\n\nClientele lets you generate fully-typed, functional, API Clients from OpenAPI schemas.\n\nIt uses modern tools to be blazing fast and type safe.\n\nPlus - there is no complex boilerplate and the generated code is very small.\n\n## Features\n\n* Fully typed API Client using Pydantic.\n* Minimalist and easy to use - the generated code is designed for readability.\n* Choose either sync or async - we support both, and you can switch between them easily.\n* Supports authentication (curently only HTTP Bearer and HTTP Basic auth).\n* Written entirely in Python - no need to install other languages to use OpenAPI.\n* The client footprint is minimal - it only requires `httpx` and `pydantic`.\n* Supports your own configuration - we provide an entry point that will never be overwritten.\n\nWe're built on:\n\n* [Pydantic 2.0](https://docs.pydantic.dev/latest/)\n* [httpx](https://www.python-httpx.org/)\n* [openapi-core](https://openapi-core.readthedocs.io/en/latest/)\n\n## Install\n\n```sh\npoetry add clientele\n```\n\n## Usage\n\n```sh\nclientele generate -f path/to/file.json -o my_client/ --asyncio t\n```\n\n[Read the docs](https://beckett-software.github.io/clientele/)\n",
     'author': 'Paul Hallett',
     'author_email': 'paulandrewhallett@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://beckett-software.github.io/clientele/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clientele-0.3.0/PKG-INFO` & `clientele-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clientele
-Version: 0.3.0
-Summary: Typed API Clients from OpenAPI specs
+Version: 0.3.1
+Summary: Typed API Clients from OpenAPI schemas
 Home-page: https://beckett-software.github.io/clientele/
 License: MIT
 Author: Paul Hallett
 Author-email: paulandrewhallett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,19 +19,19 @@
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.11,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 # ⚜️ Clientele
 
-# Typed API Clients from OpenAPI specs
+# Typed API Clients from OpenAPI schemas
 
 ![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)
 
-Clientele lets you generate fully-typed, functional, API Clients from OpenAPI specs.
+Clientele lets you generate fully-typed, functional, API Clients from OpenAPI schemas.
 
 It uses modern tools to be blazing fast and type safe.
 
 Plus - there is no complex boilerplate and the generated code is very small.
 
 ## Features
```

