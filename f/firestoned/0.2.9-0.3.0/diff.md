# Comparing `tmp/firestoned-0.2.9.tar.gz` & `tmp/firestoned-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestoned-0.2.9.tar", max compression
+gzip compressed data, was "firestoned-0.3.0.tar", max compression
```

## Comparing `firestoned-0.2.9.tar` & `firestoned-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-07-25 03:33:21.966015 firestoned-0.2.9/LICENSE
--rw-r--r--   0        0        0     9347 2023-07-25 03:33:21.966015 firestoned-0.2.9/README.md
--rw-r--r--   0        0        0        0 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/__init__.py
--rw-r--r--   0        0        0     5080 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/__main__.py
--rw-r--r--   0        0        0     2045 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/resource.py
--rw-r--r--   0        0        0        0 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/__init__.py
--rw-r--r--   0        0        0      322 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/asyncapi.jinja2
--rw-r--r--   0        0        0     7446 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/main.py.jinja2
--rw-r--r--   0        0        0      437 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/openapi.jinja2
--rw-r--r--   0        0        0     2263 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/resource.yaml
--rw-r--r--   0        0        0      175 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/__init__.py
--rw-r--r--   0        0        0      866 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/_base.py
--rw-r--r--   0        0        0    13390 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/asyncapi.py
--rw-r--r--   0        0        0     9184 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/cli.py
--rw-r--r--   0        0        0    18840 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/openapi.py
--rw-r--r--   0        0        0     1664 2023-07-25 03:33:21.974015 firestoned-0.2.9/pyproject.toml
--rw-r--r--   0        0        0    10556 1970-01-01 00:00:00.000000 firestoned-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 00:45:08.031932 firestoned-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9347 2023-07-26 00:45:08.031932 firestoned-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/__init__.py
+-rw-r--r--   0        0        0     5080 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/__main__.py
+-rw-r--r--   0        0        0     2045 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/resource.py
+-rw-r--r--   0        0        0        0 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/schema/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/schema/asyncapi.jinja2
+-rw-r--r--   0        0        0     7766 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/schema/main.py.jinja2
+-rw-r--r--   0        0        0      437 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/schema/openapi.jinja2
+-rw-r--r--   0        0        0     2263 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/schema/resource.yaml
+-rw-r--r--   0        0        0      175 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/spec/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/spec/_base.py
+-rw-r--r--   0        0        0    13390 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/spec/asyncapi.py
+-rw-r--r--   0        0        0     9820 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/spec/cli.py
+-rw-r--r--   0        0        0    19241 2023-07-26 00:45:08.039933 firestoned-0.3.0/firestone/spec/openapi.py
+-rw-r--r--   0        0        0     1695 2023-07-26 00:45:08.039933 firestoned-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10611 1970-01-01 00:00:00.000000 firestoned-0.3.0/PKG-INFO
```

### Comparing `firestoned-0.2.9/LICENSE` & `firestoned-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/README.md` & `firestoned-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/firestone/__main__.py` & `firestoned-0.3.0/firestone/__main__.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/firestone/resource.py` & `firestoned-0.3.0/firestone/resource.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/firestone/schema/main.py.jinja2` & `firestoned-0.3.0/firestone/schema/main.py.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     {{ description }}
     """
     if not trust_proxy:
         # Convert to loop
         if "http_proxy" in os.environ:
             del os.environ["http_proxy"]
         if "https_proxy" in os.environ:
-            del os.environ["all_https_proxy"]
+            del os.environ["https_proxy"]
         if "all_http_proxy" in os.environ:
             del os.environ["all_http_proxy"]
         if "all_https_proxy" in os.environ:
             del os.environ["https_proxy"]
         if "HTTP_PROXY" in os.environ:
             del os.environ["HTTP_PROXY"]
         if "HTTPS_PROXY" in os.environ:
@@ -150,17 +150,14 @@
         "{{ attr["name"] }}":  {{ attr["name"].replace("-", "_") }},
         {% endfor -%}
     }
     {% set comp_name = rsrc["name"] if not rsrc["name"].endswith("s") else rsrc["name"][:-1] %}
     {% if op["name"] == "create" %}
     req_body = create_{{ comp_name }}_model.Create{{ comp_name.capitalize() }}(**params)
     resp = await api_obj.{{ op["id"] }}(req_body)
-    {% elif op["name"] == "update" %}
-    req_body = update_{{ comp_name }}_model.Update{{ comp_name.capitalize() }}(**params)
-    resp = await api_obj.{{ op["id"] }}(req_body)
     {% else %}
     resp = await api_obj.{{ op["id"] }}(**params)
     {% endif -%}
     _LOGGER.debug(f"resp: {resp}")
 
     if isinstance(resp, list):
         click.echo(json.dumps([obj.to_dict() for obj in resp]))
@@ -174,32 +171,41 @@
 {# high-level resource instance operations -#}
 {% for op in rsrc["operations"]["instance"]|sort(attribute='name') -%}
 @{{ rsrc["name"] }}.command("{{ op["name"] }}")
 {% for attr in op["attrs"]|sort(attribute='name') -%}
 {% if attr.get("argument") -%}
 @click.argument("{{ attr["name"] }}", type={{ attr["type"] }})
 {% else -%}
-@click.option("--{{ attr["name"] }}", help="{{ attr["description"] }}", type={{ attr["type"] }}, required={{ attr["required"] }})
+@click.option("--{{ attr["name"].replace("_", "-") }}", help="{{ attr["description"] }}", type={{ attr["type"] }}, required={{ attr["required"] }})
 {% endif -%}
 {% endfor -%}
 @click.pass_obj
 @firestone_utils.click_coro
 @api_exc
 async def {{ op["id"] }}(ctx_obj{% for attr in op["attrs"]|sort(attribute='name') -%}{{ ", " + attr["name"].replace("-", "_") }}{% endfor -%}):
     """{{ op["description"] }}"""
     api_obj = ctx_obj["api_obj"]
     params = {
         {% for attr in op["attrs"]|sort(attribute='name') -%}
+        {% if not attr.get("argument") -%}
         "{{ attr["name"] }}":  {{ attr["name"].replace("-", "_") }},
+        {% endif -%}
         {% endfor -%}
     }
+    {% set comp_name = rsrc["name"] if not rsrc["name"].endswith("s") else rsrc["name"][:-1] %}
     {% if op["name"] == "create" %}
-    req_body = {{ rsrc["name"] }}_model.{{ rsrc["name"].capitalize() }}()
-    req_body.from_dict(params)
+    req_body = create_{{ comp_name }}_model.{{ comp_name.capitalize(**params) }}()
     resp = await api_obj.{{ op["id"] }}(req_body)
+    {% elif op["name"] == "update" %}
+    req_body = update_{{ comp_name }}_model.Update{{ comp_name.capitalize() }}(**params)
+    resp = await api_obj.{{ op["id"] }}(
+        {% for attr in op["attrs"]|sort(attribute='name') -%}
+            {% if attr.get("argument") -%}{{ attr["name"] }}, {% endif -%}
+        {% endfor -%}
+        req_body)
     {% else %}
     resp = await api_obj.{{ op["id"] }}(**params)
     {% endif -%}
     _LOGGER.debug(f"resp: {resp}")
 
     if isinstance(resp, list):
         print(json.dumps([obj.to_dict() for obj in resp]))
```

### Comparing `firestoned-0.2.9/firestone/schema/resource.yaml` & `firestoned-0.3.0/firestone/schema/resource.yaml`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/firestone/spec/_base.py` & `firestoned-0.3.0/firestone/spec/_base.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/firestone/spec/asyncapi.py` & `firestoned-0.3.0/firestone/spec/asyncapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.9/firestone/spec/openapi.py` & `firestoned-0.3.0/firestone/spec/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,26 @@
 RSRC_ATTR_HTTP_METHODS = ["delete", "get", "head", "put"]
 
 _LOGGER = logging.getLogger(__name__)
 
 # TODO add support for JSON Patch: https://www.jvt.me/posts/2022/05/29/openapi-json-patch/
 
 
+def _dedup_params(params: list):
+    seen = set()
+    new_list = []
+    for param in params:
+        name = param["name"]
+        if name not in seen:
+            seen.add(name)
+            new_list.append(param)
+
+    return new_list
+
+
 def get_responses(
     method: str,
     schema: dict,
     content_type: str,
     comp_name: str = None,
     attr_name: bool = None,
     is_list: bool = None,
@@ -104,14 +116,15 @@
         "operationId": spec_base.get_opid(path, method),
     }
 
     # Now set the schema for responses
     _LOGGER.debug(f"method: {method}")
     _LOGGER.debug(f"schema: {schema}")
     _LOGGER.debug(f"comp_name: {comp_name}")
+    _LOGGER.debug(f"attr_name: {attr_name}")
     _LOGGER.debug(f"is_list: {is_list}")
     opr["responses"] = get_responses(
         method,
         schema,
         content_type,
         comp_name=comp_name,
         attr_name=attr_name,
@@ -129,15 +142,16 @@
         ):
             request_schema = opr["responses"][http.client.CREATED]["content"][content_type][
                 "schema"
             ]
     elif method == "put":
         _LOGGER.debug(f"Getting {method} operation")
         request_schema = copy.deepcopy(schema)
-        if comp_name:
+        _LOGGER.debug(f"request_schema: {request_schema}")
+        if comp_name and not attr_name:
             request_schema = {"$ref": f"#/components/schemas/{comp_name}"}
     _LOGGER.debug(f"request_schema: {request_schema}")
 
     if request_schema:
         if "descriptions" in request_schema:
             del request_schema["descriptions"]
         if "key" in request_schema:
@@ -256,14 +270,15 @@
         )
         paths[baseurl][method]["tags"] = [orig_rsrc_name or rsrc_name]
 
         # Add parameters
         params = get_params(baseurl, method, schema, keys=keys)
         if default_query_params:
             params.extend(default_query_params)
+            params = _dedup_params(params)
         _LOGGER.debug(f"params: {params}")
         paths[baseurl][method]["parameters"] = params
 
     return paths
 
 
 def add_instance_methods(
```

### Comparing `firestoned-0.2.9/pyproject.toml` & `firestoned-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestoned"
-version = "0.2.9"
+version = "0.3.0"
 description = "Build OpenAPI and AsyncAPI specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/firestoned/firestone"
 packages = [
     { include = "firestone" }
@@ -19,14 +19,15 @@
 jsonschema = "^4.16.0"
 pyyaml = "^6.0"
 jsonref = "^1.0.0.post1"
 firestone-lib = "^0.1.0"
 pydantic = "^1.10.5"
 python-dateutil = "^2.8.2"
 aiohttp = "^3.8.4"
+diff-match-patch = "^20230430"
 
 [tool.poetry.group.asyncapi.dependencies]
 asyncapi = {extras = ["http"], version = "^0.14.1"}
 requests = "^2.28.1"
 websockets = "^10.4"
 typer = "^0.7.0"
 uvicorn = "^0.19.0"
```

### Comparing `firestoned-0.2.9/PKG-INFO` & `firestoned-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestoned
-Version: 0.2.9
+Version: 0.3.0
 Summary: Build OpenAPI and AsyncAPI specs based off one or more resource json schema files
 Home-page: https://github.com/firestoned/firestone
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: caching
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: diff-match-patch (>=20230430,<20230431)
 Requires-Dist: firestone-lib (>=0.1.0,<0.2.0)
 Requires-Dist: jsonref (>=1.0.0.post1,<2.0.0)
 Requires-Dist: jsonschema (>=4.16.0,<5.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching"
```

#### html2text {}

```diff
@@ -1,129 +1,130 @@
-Metadata-Version: 2.1 Name: firestoned Version: 0.2.9 Summary: Build OpenAPI
+Metadata-Version: 2.1 Name: firestoned Version: 0.3.0 Summary: Build OpenAPI
 and AsyncAPI specs based off one or more resource json schema files Home-page:
 https://github.com/firestoned/firestone License: Apache 2.0 Author: Erick
 Bourgeois Author-email: erick@jeb.ca Requires-Python: >=3.8,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: caching
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: firestone-lib
-(>=0.1.0,<0.2.0) Requires-Dist: jsonref (>=1.0.0.post1,<2.0.0) Requires-Dist:
-jsonschema (>=4.16.0,<5.0.0) Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: pyyaml
-(>=6.0,<7.0) Requires-Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching"
-Requires-Dist: setuptools (>=65.5.0,<66.0.0) Project-URL: Repository, https://
-github.com/firestoned/firestone Description-Content-Type: text/markdown [![Last
-PR Build ð](https://github.com/firestoned/firestone/actions/workflows/
-pr.yml/badge.svg)](https://github.com/firestoned/firestone/actions/workflows/
-pr.yml)  [Coverage]  # Firestone Resource-Based Approach to Building APIs
-``firestone`` allows you to build OpenAPI, AsyncAPI and gRPC specs based off
-one or more resource json schema files. This allows you to focus on what really
-matters, the resource you are developing! Once you have generated the
-appropriate specification file for your project, you can then use the myriad of
-libraries and frameworks to generate stub code for you. **The primary premise
-of this project is not to introduce any new "language" to describe your
-resources(s), use JSON Schema!** THis makes it easy to come up to speed and
-little to no prior knowledge to get going. Having said that, the schema for a
-resource provides additional helpful functionality, see [schema](#schema)
-section. ## Quick Start You can use pip or poetry to install and run
-``firestone``. We suggest using pip if you wish to install `firestone``
-machine-wide, else, for local use, use poetry. ### pip It's a simple as running
-the following ``pip`` command: ``` sudo pip install firestoned ``` NOTE: yes,
-`firestone**d**`, not `firestone`! This is because there already is a, albeit
-emtpy, repo on pypi.org with the same name... ### poetry [Poetry](https://
-python-poetry.org/) is a great build tool for python that allows you to build
-and run all locally in a virtual environment. This is great for checking out
-the tool and playing around with `firestone` itself. ``` brew install poetry
-poetry install poetry build ``` ## Running Now that you have a copy of
-``firestone``, let's try running it with the example resource provided, an
-addressbook! Note: if running within poetry build, simply prepend commands with
-``poetry run`` For the remainder of this documentation, we will assume you have
-installed firestone. ### Generate an OpenAPI Spec ``` firestone \ generate \ --
-title 'Addressbook resource' \ --description 'A simple addressBook example' \ -
--resources examples/addressBook/resource.yaml \ openapi --security '{"name":
-"bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}' \
+Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: diff-match-patch
+(>=20230430,<20230431) Requires-Dist: firestone-lib (>=0.1.0,<0.2.0) Requires-
+Dist: jsonref (>=1.0.0.post1,<2.0.0) Requires-Dist: jsonschema
+(>=4.16.0,<5.0.0) Requires-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist:
+python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-
+Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching" Requires-Dist: setuptools
+(>=65.5.0,<66.0.0) Project-URL: Repository, https://github.com/firestoned/
+firestone Description-Content-Type: text/markdown [![Last PR Build ð](https:
+//github.com/firestoned/firestone/actions/workflows/pr.yml/badge.svg)](https://
+github.com/firestoned/firestone/actions/workflows/pr.yml)  [Coverage]  #
+Firestone Resource-Based Approach to Building APIs ``firestone`` allows you to
+build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json
+schema files. This allows you to focus on what really matters, the resource you
+are developing! Once you have generated the appropriate specification file for
+your project, you can then use the myriad of libraries and frameworks to
+generate stub code for you. **The primary premise of this project is not to
+introduce any new "language" to describe your resources(s), use JSON Schema!**
+THis makes it easy to come up to speed and little to no prior knowledge to get
+going. Having said that, the schema for a resource provides additional helpful
+functionality, see [schema](#schema) section. ## Quick Start You can use pip or
+poetry to install and run ``firestone``. We suggest using pip if you wish to
+install `firestone`` machine-wide, else, for local use, use poetry. ### pip
+It's a simple as running the following ``pip`` command: ``` sudo pip install
+firestoned ``` NOTE: yes, `firestone**d**`, not `firestone`! This is because
+there already is a, albeit emtpy, repo on pypi.org with the same name... ###
+poetry [Poetry](https://python-poetry.org/) is a great build tool for python
+that allows you to build and run all locally in a virtual environment. This is
+great for checking out the tool and playing around with `firestone` itself. ```
+brew install poetry poetry install poetry build ``` ## Running Now that you
+have a copy of ``firestone``, let's try running it with the example resource
+provided, an addressbook! Note: if running within poetry build, simply prepend
+commands with ``poetry run`` For the remainder of this documentation, we will
+assume you have installed firestone. ### Generate an OpenAPI Spec ``` firestone
+\ generate \ --title 'Addressbook resource' \ --description 'A simple
+addressBook example' \ --resources examples/addressBook/resource.yaml \ openapi
+--security '{"name": "bearer_auth", "scheme": "bearer", "type": "http",
+"bearerFormat": "JWT"}' \ ``` Let's quickly dissect this command: - we are
+telling firestone to generate an `openapi` spec, given the ``title``,
+``description`` and the two given resource files. - By default, this will
+output the specification file to stdout, alternatively you can provide the `-O`
+option to output to a specific file. You can also, add the command line `--ui-
+server` tot he end, which will launch a small webserver and run the Swagger UI
+to view this specification file. ``` firestone --debug generate --title
+'Example person and addressBook API' \ --description 'An example API with more
+than one resource' \ --resources examples/addressBook.yaml,examples/person.yaml
+\ openapi \ --security '{"name": "bearer_auth", "scheme": "bearer", "type":
+"http", "bearerFormat": "JWT"}' \ --ui-server # ... * Serving Quart app
+'firestone.__main__' * Environment: production * Please use an ASGI server
+(e.g. Hypercorn) directly in production * Debug mode: False * Running on http:/
+/127.0.0.1:5000 (CTRL + C to quit) [2022-10-31 02:47:17 -0500] [87590] [INFO]
+Running on http://127.0.0.1:5000 (CTRL + C to quit) # 2022-10-31 02:47:17,120 -
+[MainThread] hypercorn.error:102 INFO - Running on http://127.0.0.1:5000 (CTRL
++ C to quit) ``` Now you can use your browser to navigate to `http://127.0.0.1:
+5000/apidocs` ## Schema It all begins with your resource definition! This is
+done using JSON schema and we have provided an example in our `examples`
+directory, called addressBook. We will use this to describe how the schema is
+setup and how you can adapt to your own. Here is the full file: ```yaml name:
+addressBook description: An example of an addressBook resource version: 1.0
+version_in_path: false default_query_params: - name: limit description: Limit
+the number of responses back in: params schema: type: integer - name: offset
+description: The offset to start returning resources in: params schema: type:
+integer descriptions: resource: get: List all addresses in this addressbook.
+head: Determine the existence and size of addresses in this addressbook. patch:
+Patch one or more addresses in this addressbook. post: Create a new address in
+this addressbook, a new address key will be created. delete: Delete all
+addresses from this addressbook. instance: get: Get a specific address from
+this addressbook. head: Determine the existence and size of this address.
+patch: Patch this address in the addressbook. put: Put a new address in this
+addressbook, with the given address key. delete: Delete an address from this
+addressbook. schema: type: array key: name: address_key schema: description: A
+unique identifier for an addressbook entry. type: string #responseCodes: # -
+200 # - 201 query_params: - name: city description: Filter by city name schema:
+type: string methods: - get items: type: object properties: addrtype:
+description: The address type, e.g. work or home type: string enum: - work -
+home street: description: The street and civic number of this address type:
+string city: description: The city of this address type: string state:
+description: The state of this address type: string country: description: The
+country of this address type: string ``` ### Metadata There is a certain amount
+of metadata that all of these specifications use/require, and this is done at
+the top of the resource,yaml; for posterity, they are: ```yaml name:
+addressBook description: An example of an addressBook resource version: 1.0 ```
+#### `name` The name is used in various places, including as the root to API
+URLs, for example in OpenAPI, `/addressBook` #### `description` This is self
+evident, I hope, the description of this resource and is used nt he generated
+specification files. #### `descriptions` This is a map/dict of either
+`resource` and/or `instance`, which itself is a map or methods to descriptions,
+e.g.: ```yaml descriptions: resource: get: List all addresses in this
+addressbook. head: Determine the existence and size of addresses in this
+addressbook. patch: Patch one or more addresses in this addressbook. post:
+Create a new address in this addressbook, a new address key will be created.
+delete: Delete all addresses from this addressbook. ``` #### `methods` This is
+a map/dict of `resource`, and/or `instance`, and/or `instance_attrs` (the
+instance attributes to expose), and a list of methods to explicitly expose,
+e.g.: ```yaml methods: resource: - get - post - put ``` #### `version` The
+version of this resource definition, this cna alternatively be used in the URL
+as well, see below `version_in_path` #### `version_in_path` This attribute
+defines whether to prepend the version defined above in the URL paths, e.g.,
+for the above, you would get: `/v1.0/addressBook`. #### `default_query_params`
+You can provide a list of default query parameters that will be added to all
+HTTP methods, or optionally you can provide a list of the HTTP methods, for
+which `firestone` will add. ### Generate OpenAPI Client Now, to generate your
+OpenAPI client, you will need the `openapi-generator` command, and this can be
+used to generate client code in many languages. For more details on this
+project, see [here](https://openapi-generator.tech/). This client code can then
+be used as an SDK or used by our CLI generation, see below. ``` openapi-
+generator generate \ -i examples/addressbook/openapi.yaml \ -g python-nextgen \
+-o /tmp/addressbook-client \ --skip-validate-spec \ -c examples/addressbook/
+openapi-gen-config.json ``` ### Generate Python CRUD CLI Now that you have
+generated the client code, you can also generate a CRUD, Python Click-based CLI
+around your code. This generator creates a standalone script or as a module to
+be used in your console scripts, as part of your project build. Here is an
+example command we use to generate the example Addressbook. ``` firestone
+generate \ --title 'Addressbook CLI' \ --description 'This is the CLI for the
+example Addressbook' \ --resources examples/addressbook/
+addressbook.yaml,examples/addressbook/person.yaml \ --version 1.0 \ cli \ --pkg
+addressbook \ --client-pkg addressbook.client > examples/addressbook/main.py
 ``` Let's quickly dissect this command: - we are telling firestone to generate
 an `openapi` spec, given the ``title``, ``description`` and the two given
 resource files. - By default, this will output the specification file to
 stdout, alternatively you can provide the `-O` option to output to a specific
-file. You can also, add the command line `--ui-server` tot he end, which will
-launch a small webserver and run the Swagger UI to view this specification
-file. ``` firestone --debug generate --title 'Example person and addressBook
-API' \ --description 'An example API with more than one resource' \ --resources
-examples/addressBook.yaml,examples/person.yaml \ openapi \ --security '{"name":
-"bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}' \ --
-ui-server # ... * Serving Quart app 'firestone.__main__' * Environment:
-production * Please use an ASGI server (e.g. Hypercorn) directly in production
-* Debug mode: False * Running on http://127.0.0.1:5000 (CTRL + C to quit)
-[2022-10-31 02:47:17 -0500] [87590] [INFO] Running on http://127.0.0.1:5000
-(CTRL + C to quit) # 2022-10-31 02:47:17,120 - [MainThread] hypercorn.error:102
-INFO - Running on http://127.0.0.1:5000 (CTRL + C to quit) ``` Now you can use
-your browser to navigate to `http://127.0.0.1:5000/apidocs` ## Schema It all
-begins with your resource definition! This is done using JSON schema and we
-have provided an example in our `examples` directory, called addressBook. We
-will use this to describe how the schema is setup and how you can adapt to your
-own. Here is the full file: ```yaml name: addressBook description: An example
-of an addressBook resource version: 1.0 version_in_path: false
-default_query_params: - name: limit description: Limit the number of responses
-back in: params schema: type: integer - name: offset description: The offset to
-start returning resources in: params schema: type: integer descriptions:
-resource: get: List all addresses in this addressbook. head: Determine the
-existence and size of addresses in this addressbook. patch: Patch one or more
-addresses in this addressbook. post: Create a new address in this addressbook,
-a new address key will be created. delete: Delete all addresses from this
-addressbook. instance: get: Get a specific address from this addressbook. head:
-Determine the existence and size of this address. patch: Patch this address in
-the addressbook. put: Put a new address in this addressbook, with the given
-address key. delete: Delete an address from this addressbook. schema: type:
-array key: name: address_key schema: description: A unique identifier for an
-addressbook entry. type: string #responseCodes: # - 200 # - 201 query_params: -
-name: city description: Filter by city name schema: type: string methods: - get
-items: type: object properties: addrtype: description: The address type, e.g.
-work or home type: string enum: - work - home street: description: The street
-and civic number of this address type: string city: description: The city of
-this address type: string state: description: The state of this address type:
-string country: description: The country of this address type: string ``` ###
-Metadata There is a certain amount of metadata that all of these specifications
-use/require, and this is done at the top of the resource,yaml; for posterity,
-they are: ```yaml name: addressBook description: An example of an addressBook
-resource version: 1.0 ``` #### `name` The name is used in various places,
-including as the root to API URLs, for example in OpenAPI, `/addressBook` ####
-`description` This is self evident, I hope, the description of this resource
-and is used nt he generated specification files. #### `descriptions` This is a
-map/dict of either `resource` and/or `instance`, which itself is a map or
-methods to descriptions, e.g.: ```yaml descriptions: resource: get: List all
-addresses in this addressbook. head: Determine the existence and size of
-addresses in this addressbook. patch: Patch one or more addresses in this
-addressbook. post: Create a new address in this addressbook, a new address key
-will be created. delete: Delete all addresses from this addressbook. ``` ####
-`methods` This is a map/dict of `resource`, and/or `instance`, and/or
-`instance_attrs` (the instance attributes to expose), and a list of methods to
-explicitly expose, e.g.: ```yaml methods: resource: - get - post - put ``` ####
-`version` The version of this resource definition, this cna alternatively be
-used in the URL as well, see below `version_in_path` #### `version_in_path`
-This attribute defines whether to prepend the version defined above in the URL
-paths, e.g., for the above, you would get: `/v1.0/addressBook`. ####
-`default_query_params` You can provide a list of default query parameters that
-will be added to all HTTP methods, or optionally you can provide a list of the
-HTTP methods, for which `firestone` will add. ### Generate OpenAPI Client Now,
-to generate your OpenAPI client, you will need the `openapi-generator` command,
-and this can be used to generate client code in many languages. For more
-details on this project, see [here](https://openapi-generator.tech/). This
-client code can then be used as an SDK or used by our CLI generation, see
-below. ``` openapi-generator generate \ -i examples/addressbook/openapi.yaml \
--g python-nextgen \ -o /tmp/addressbook-client \ --skip-validate-spec \ -
-c examples/addressbook/openapi-gen-config.json ``` ### Generate Python CRUD CLI
-Now that you have generated the client code, you can also generate a CRUD,
-Python Click-based CLI around your code. This generator creates a standalone
-script or as a module to be used in your console scripts, as part of your
-project build. Here is an example command we use to generate the example
-Addressbook. ``` firestone generate \ --title 'Addressbook CLI' \ --description
-'This is the CLI for the example Addressbook' \ --resources examples/
-addressbook/addressbook.yaml,examples/addressbook/person.yaml \ --version 1.0 \
-cli \ --pkg addressbook \ --client-pkg addressbook.client > examples/
-addressbook/main.py ``` Let's quickly dissect this command: - we are telling
-firestone to generate an `openapi` spec, given the ``title``, ``description``
-and the two given resource files. - By default, this will output the
-specification file to stdout, alternatively you can provide the `-O` option to
-output to a specific file. ## Contributing
+file. ## Contributing
```

