# Comparing `tmp/zswag-1.5.0-py3-none-any.whl.zip` & `tmp/zswag-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 32543 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat       79 b- defN 23-Feb-09 14:20 zswag/__init__.py
--rw-rw-rw-  2.0 fat     8574 b- defN 23-Feb-09 14:20 zswag/app.py
--rw-rw-rw-  2.0 fat     4402 b- defN 23-Feb-09 14:20 zswag/doc.py
--rw-rw-rw-  2.0 fat    28993 b- defN 23-Feb-09 14:20 zswag/gen.py
--rw-rw-rw-  2.0 fat    10594 b- defN 23-Feb-09 14:20 zswag/reflect.py
--rw-rw-rw-  2.0 fat      240 b- defN 23-Feb-09 14:20 zswag/test/calc/__init__.py
--rw-rw-rw-  2.0 fat      767 b- defN 23-Feb-09 14:20 zswag/test/calc/__main__.py
--rw-rw-rw-  2.0 fat     6738 b- defN 23-Feb-09 14:20 zswag/test/calc/api.yaml
--rw-rw-rw-  2.0 fat     1139 b- defN 23-Feb-09 14:20 zswag/test/calc/calculator.zs
--rw-rw-rw-  2.0 fat     3963 b- defN 23-Feb-09 14:20 zswag/test/calc/client.py
--rw-rw-rw-  2.0 fat     1355 b- defN 23-Feb-09 14:20 zswag/test/calc/server.py
--rw-rw-rw-  2.0 fat     1557 b- defN 23-Feb-09 14:25 zswag-1.5.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    34064 b- defN 23-Feb-09 14:25 zswag-1.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-09 14:25 zswag-1.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Feb-09 14:25 zswag-1.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1227 b- defN 23-Feb-09 14:25 zswag-1.5.0.dist-info/RECORD
-16 files, 103790 bytes uncompressed, 30555 bytes compressed:  70.6%
+Zip file size: 32438 bytes, number of entries: 16
+-rw-r--r--  2.0 unx       75 b- defN 23-Jul-26 06:53 zswag/__init__.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-Jul-26 06:53 zswag/app.py
+-rw-r--r--  2.0 unx     4279 b- defN 23-Jul-26 06:53 zswag/doc.py
+-rw-r--r--  2.0 unx    28403 b- defN 23-Jul-26 06:53 zswag/gen.py
+-rw-r--r--  2.0 unx    10347 b- defN 23-Jul-26 06:53 zswag/reflect.py
+-rw-r--r--  2.0 unx      231 b- defN 23-Jul-26 06:53 zswag/test/calc/__init__.py
+-rw-r--r--  2.0 unx      743 b- defN 23-Jul-26 06:53 zswag/test/calc/__main__.py
+-rw-r--r--  2.0 unx     6462 b- defN 23-Jul-26 06:53 zswag/test/calc/api.yaml
+-rw-r--r--  2.0 unx     1036 b- defN 23-Jul-26 06:53 zswag/test/calc/calculator.zs
+-rw-r--r--  2.0 unx     3831 b- defN 23-Jul-26 06:53 zswag/test/calc/client.py
+-rw-r--r--  2.0 unx     1304 b- defN 23-Jul-26 06:53 zswag/test/calc/server.py
+-rw-r--r--  2.0 unx     1528 b- defN 23-Jul-26 07:02 zswag-1.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    32150 b- defN 23-Jul-26 07:02 zswag-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 07:02 zswag-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-26 07:02 zswag-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1227 b- defN 23-Jul-26 07:02 zswag-1.6.0.dist-info/RECORD
+16 files, 100087 bytes uncompressed, 30450 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: zswag/test/calc/client.py
 Comment: 
 
 Filename: zswag/test/calc/server.py
 Comment: 
 
-Filename: zswag-1.5.0.dist-info/LICENSE
+Filename: zswag-1.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: zswag-1.5.0.dist-info/METADATA
+Filename: zswag-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: zswag-1.5.0.dist-info/WHEEL
+Filename: zswag-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: zswag-1.5.0.dist-info/top_level.txt
+Filename: zswag-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zswag-1.5.0.dist-info/RECORD
+Filename: zswag-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zswag/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-from .app import *
-
-from pyzswagcl import OAClient, HTTPError, HTTPConfig
-
+from .app import *
+
+from pyzswagcl import OAClient, HTTPError, HTTPConfig
+
```

## zswag/app.py

 * *Ordering differences only*

```diff
@@ -1,201 +1,201 @@
-import connexion
-import os
-import inspect
-import zserio
-import sys
-import yaml
-from typing import Type
-from flask import request as flask_request
-
-from pyzswagcl import \
-    parse_openapi_config, \
-    OAMethod
-
-from .reflect import request_object_blob, service_method_request_type, to_snake
-
-# Name of variable that is added to controller
-# to hold the service instance.
-CONTROLLER_SERVICE_INSTANCE = "_service"
-
-# Name of OpenApi extension field from which connexion
-# reads the target wsgi function.
-CONTROLLER_OPENAPI_FIELD = "x-openapi-router-controller"
-
-# Utility function for slash conversion in format strings
-def to_slashes(s: str):
-    return s.replace("\\", "/")
-
-
-# Raised if the controller passed to OAServer is missing a function
-class IncompleteSchemaError(RuntimeError):
-    def __init__(self, schema_path: str, fn_name: str):
-        super(IncompleteSchemaError, self).__init__(f"Missing operation `{fn_name}` in {schema_path}!")
-        self.schema_path = schema_path
-        self.fn_name = fn_name
-
-
-class OAServer(connexion.App):
-
-    def __init__(self, *,
-                 controller_module,
-                 service_type: Type[zserio.ServiceInterface],
-                 zs_pkg_path: str = None,
-                 yaml_path: str = None):
-        """
-        Brief
-
-            Marry a user-written app controller with a zserio-generated app server class
-            (argument parser/response serialiser) and a fitting Swagger OpenApi spec.
-
-            The OpenApi spec is auto-generated if the user does not specify an existing file.
-            If the user specifies an empty YAML path, the yaml file is placed next to the
-            zserio python-service source-file.
-
-            If you have installed `pip install connexion[swagger-ui]`, you can view
-            API docs of your service under [/prefix]/ui.
-
-            Documentation for the service is automatically extracted if `zs_pkg_path` is issued.
-
-        Code example
-
-            In file my.app.__init__:
-
-                from zserio_gen.my.service import Service
-                from zswag import Server
-                import
-
-                app = Server(my.app.controller, Service)
-
-            In file my.app.controller:
-
-                # NOTE: Injected by Server, invisible to developer!
-                #  In swagger yaml, the path specs reference `my.app.controller._service.myApi`
-                _service = Service()
-                _service.myApi = lambda request: _service._myApiMethod(request)
-                _service._myApiImpl = my.app.controller.my_api
-
-                # Written by user
-                def my_api(request):
-                    return "response"
-
-        General call structure:
-
-            OpenAPI `yaml_file` "paths/service" references
-             Zserio Server instance injected method (ns.service.service(base64): blob), which calls
-             ns.service._serviceMethod(blob), which calls
-             ns.service._serviceImpl(value) which is remapped to
-             User function (ns.serviceImpl(value): value).
-
-        """
-        if not yaml_path:
-            service_module = sys.modules[service_type.__module__]
-            yaml_path = os.path.join(
-                os.path.dirname(os.path.abspath(service_module.__file__)),
-                f"{service_module.__name__.split('.')[-1]}.{service_type.__name__}.yaml")
-            print(f"Using yaml path {yaml_path}")
-        self.yaml_path = yaml_path
-        yaml_parent_path = os.path.dirname(yaml_path)
-        self.zs_pkg_path = zs_pkg_path
-
-        # Initialise zserio service
-        self.service_type = service_type
-        assert inspect.isclass(self.service_type)
-
-        # Initialise zserio service working instance
-        self.controller_path = controller_module.__name__
-        self.controller = controller_module
-        self.service_instance_path = self.controller_path+f".{CONTROLLER_SERVICE_INSTANCE}"
-        if not hasattr(self.controller, CONTROLLER_SERVICE_INSTANCE):
-            setattr(self.controller, CONTROLLER_SERVICE_INSTANCE, self.service_type())
-        self.service_instance = getattr(self.controller, CONTROLLER_SERVICE_INSTANCE)
-
-        # Verify or generate yaml file
-        if not os.path.isfile(yaml_path):
-            print("\n" + inspect.cleandoc(f"""
-                ERROR: File does not exist: {yaml_path}
-                ----------------------------{"-"*len(yaml_path)}
-                
-                You can generate the file by running ...
-                    
-                    python -m zswag.gen \\
-                        --service {self.service_instance.SERVICE_FULL_NAME} \\
-                        --input "{
-                            to_slashes(os.path.abspath(os.path.dirname(os.path.dirname(
-                                __import__(self.service_type.__module__.split('.')[0]).__file__
-                            ))))
-                        }" \\
-                        --config post,body \\
-                        --output "{to_slashes(yaml_path)}"
-                        
-                    The --config argument is a comma-separated list of tags
-                    to specify OpenAPI options. For more info, please run
-                    
-                        python -m zswag.gen --help
-            """))
-            exit(1)
-
-        self.spec = parse_openapi_config(yaml_path)
-        self.verify_openapi_schema()
-
-        # Re-route service impl methods
-        for method_name in self.service_instance.method_names:
-            method_snake_name = to_snake(method_name)
-            user_function = getattr(self.controller, method_snake_name)
-            zserio_modem_function = getattr(self.service_instance, f"_{method_snake_name}_method")
-            request_type = service_method_request_type(self.service_instance, method_name)
-            assert zserio_modem_function
-
-            if not user_function or not inspect.isfunction(user_function):
-                print(f"WARNING: The controller {self.controller_path} does not implement {method_snake_name}!")
-                continue
-
-            print(f"Found {self.controller_path}.{method_snake_name}.")
-            if len(inspect.signature(user_function).parameters) != 1:
-                print(f"ERROR: {self.controller_path}.{method_snake_name} must have single 'request' parameter!")
-                continue
-
-            method_spec: OAMethod = self.spec[method_name]
-
-            def wsgi_method(fun=zserio_modem_function, spec=method_spec, req_t=request_type, **kwargs):
-                if spec.body_request_object:
-                    request_blob = kwargs["body"]
-                else:
-                    request_blob = request_object_blob(
-                        req_t=req_t,
-                        spec=spec,
-                        headers=flask_request.headers,
-                        **kwargs)
-                return bytes(fun(request_blob, None).byte_array)
-            setattr(self.service_instance, method_name, wsgi_method)
-
-            def method_impl(request, ctx=None, fun=user_function):
-                return fun(request)
-            setattr(self.service_instance, f"_{method_snake_name}_impl", method_impl)
-
-        # Load spec and inject openapi-router-controller
-        print(f"Loading spec from {yaml_path} ...")
-        with open(yaml_path, 'r') as swagger_file:
-            openapi = yaml.load(swagger_file, Loader=yaml.FullLoader)
-        for path_name, path_spec in openapi["paths"].items():
-            for meth_name, method_spec in path_spec.items():
-                if CONTROLLER_OPENAPI_FIELD not in method_spec:
-                    method_spec[CONTROLLER_OPENAPI_FIELD] = self.service_instance_path
-                else:
-                    print(f"{meth_name} {path_name}: Using pre-set {CONTROLLER_OPENAPI_FIELD}.")
-
-        # Initialise connexion app
-        super(OAServer, self).__init__(
-            self.controller_path,
-            specification_dir=yaml_parent_path)
-
-        # Add the API according to the verified yaml spec.
-        self.add_api(
-            openapi,
-            arguments={"title": f"REST API for {service_type.__name__}"},
-            pythonic_params=False)
-
-    def verify_openapi_schema(self):
-        for method_name in self.service_instance.method_names:
-            if method_name not in self.spec:
-                raise IncompleteSchemaError(self.yaml_path, method_name)
-
+import connexion
+import os
+import inspect
+import zserio
+import sys
+import yaml
+from typing import Type
+from flask import request as flask_request
+
+from pyzswagcl import \
+    parse_openapi_config, \
+    OAMethod
+
+from .reflect import request_object_blob, service_method_request_type, to_snake
+
+# Name of variable that is added to controller
+# to hold the service instance.
+CONTROLLER_SERVICE_INSTANCE = "_service"
+
+# Name of OpenApi extension field from which connexion
+# reads the target wsgi function.
+CONTROLLER_OPENAPI_FIELD = "x-openapi-router-controller"
+
+# Utility function for slash conversion in format strings
+def to_slashes(s: str):
+    return s.replace("\\", "/")
+
+
+# Raised if the controller passed to OAServer is missing a function
+class IncompleteSchemaError(RuntimeError):
+    def __init__(self, schema_path: str, fn_name: str):
+        super(IncompleteSchemaError, self).__init__(f"Missing operation `{fn_name}` in {schema_path}!")
+        self.schema_path = schema_path
+        self.fn_name = fn_name
+
+
+class OAServer(connexion.App):
+
+    def __init__(self, *,
+                 controller_module,
+                 service_type: Type[zserio.ServiceInterface],
+                 zs_pkg_path: str = None,
+                 yaml_path: str = None):
+        """
+        Brief
+
+            Marry a user-written app controller with a zserio-generated app server class
+            (argument parser/response serialiser) and a fitting Swagger OpenApi spec.
+
+            The OpenApi spec is auto-generated if the user does not specify an existing file.
+            If the user specifies an empty YAML path, the yaml file is placed next to the
+            zserio python-service source-file.
+
+            If you have installed `pip install connexion[swagger-ui]`, you can view
+            API docs of your service under [/prefix]/ui.
+
+            Documentation for the service is automatically extracted if `zs_pkg_path` is issued.
+
+        Code example
+
+            In file my.app.__init__:
+
+                from zserio_gen.my.service import Service
+                from zswag import Server
+                import
+
+                app = Server(my.app.controller, Service)
+
+            In file my.app.controller:
+
+                # NOTE: Injected by Server, invisible to developer!
+                #  In swagger yaml, the path specs reference `my.app.controller._service.myApi`
+                _service = Service()
+                _service.myApi = lambda request: _service._myApiMethod(request)
+                _service._myApiImpl = my.app.controller.my_api
+
+                # Written by user
+                def my_api(request):
+                    return "response"
+
+        General call structure:
+
+            OpenAPI `yaml_file` "paths/service" references
+             Zserio Server instance injected method (ns.service.service(base64): blob), which calls
+             ns.service._serviceMethod(blob), which calls
+             ns.service._serviceImpl(value) which is remapped to
+             User function (ns.serviceImpl(value): value).
+
+        """
+        if not yaml_path:
+            service_module = sys.modules[service_type.__module__]
+            yaml_path = os.path.join(
+                os.path.dirname(os.path.abspath(service_module.__file__)),
+                f"{service_module.__name__.split('.')[-1]}.{service_type.__name__}.yaml")
+            print(f"Using yaml path {yaml_path}")
+        self.yaml_path = yaml_path
+        yaml_parent_path = os.path.dirname(yaml_path)
+        self.zs_pkg_path = zs_pkg_path
+
+        # Initialise zserio service
+        self.service_type = service_type
+        assert inspect.isclass(self.service_type)
+
+        # Initialise zserio service working instance
+        self.controller_path = controller_module.__name__
+        self.controller = controller_module
+        self.service_instance_path = self.controller_path+f".{CONTROLLER_SERVICE_INSTANCE}"
+        if not hasattr(self.controller, CONTROLLER_SERVICE_INSTANCE):
+            setattr(self.controller, CONTROLLER_SERVICE_INSTANCE, self.service_type())
+        self.service_instance = getattr(self.controller, CONTROLLER_SERVICE_INSTANCE)
+
+        # Verify or generate yaml file
+        if not os.path.isfile(yaml_path):
+            print("\n" + inspect.cleandoc(f"""
+                ERROR: File does not exist: {yaml_path}
+                ----------------------------{"-"*len(yaml_path)}
+                
+                You can generate the file by running ...
+                    
+                    python -m zswag.gen \\
+                        --service {self.service_instance.SERVICE_FULL_NAME} \\
+                        --input "{
+                            to_slashes(os.path.abspath(os.path.dirname(os.path.dirname(
+                                __import__(self.service_type.__module__.split('.')[0]).__file__
+                            ))))
+                        }" \\
+                        --config post,body \\
+                        --output "{to_slashes(yaml_path)}"
+                        
+                    The --config argument is a comma-separated list of tags
+                    to specify OpenAPI options. For more info, please run
+                    
+                        python -m zswag.gen --help
+            """))
+            exit(1)
+
+        self.spec = parse_openapi_config(yaml_path)
+        self.verify_openapi_schema()
+
+        # Re-route service impl methods
+        for method_name in self.service_instance.method_names:
+            method_snake_name = to_snake(method_name)
+            user_function = getattr(self.controller, method_snake_name)
+            zserio_modem_function = getattr(self.service_instance, f"_{method_snake_name}_method")
+            request_type = service_method_request_type(self.service_instance, method_name)
+            assert zserio_modem_function
+
+            if not user_function or not inspect.isfunction(user_function):
+                print(f"WARNING: The controller {self.controller_path} does not implement {method_snake_name}!")
+                continue
+
+            print(f"Found {self.controller_path}.{method_snake_name}.")
+            if len(inspect.signature(user_function).parameters) != 1:
+                print(f"ERROR: {self.controller_path}.{method_snake_name} must have single 'request' parameter!")
+                continue
+
+            method_spec: OAMethod = self.spec[method_name]
+
+            def wsgi_method(fun=zserio_modem_function, spec=method_spec, req_t=request_type, **kwargs):
+                if spec.body_request_object:
+                    request_blob = kwargs["body"]
+                else:
+                    request_blob = request_object_blob(
+                        req_t=req_t,
+                        spec=spec,
+                        headers=flask_request.headers,
+                        **kwargs)
+                return bytes(fun(request_blob, None).byte_array)
+            setattr(self.service_instance, method_name, wsgi_method)
+
+            def method_impl(request, ctx=None, fun=user_function):
+                return fun(request)
+            setattr(self.service_instance, f"_{method_snake_name}_impl", method_impl)
+
+        # Load spec and inject openapi-router-controller
+        print(f"Loading spec from {yaml_path} ...")
+        with open(yaml_path, 'r') as swagger_file:
+            openapi = yaml.load(swagger_file, Loader=yaml.FullLoader)
+        for path_name, path_spec in openapi["paths"].items():
+            for meth_name, method_spec in path_spec.items():
+                if CONTROLLER_OPENAPI_FIELD not in method_spec:
+                    method_spec[CONTROLLER_OPENAPI_FIELD] = self.service_instance_path
+                else:
+                    print(f"{meth_name} {path_name}: Using pre-set {CONTROLLER_OPENAPI_FIELD}.")
+
+        # Initialise connexion app
+        super(OAServer, self).__init__(
+            self.controller_path,
+            specification_dir=yaml_parent_path)
+
+        # Add the API according to the verified yaml spec.
+        self.add_api(
+            openapi,
+            arguments={"title": f"REST API for {service_type.__name__}"},
+            pythonic_params=False)
+
+    def verify_openapi_schema(self):
+        for method_name in self.service_instance.method_names:
+            if method_name not in self.spec:
+                raise IncompleteSchemaError(self.yaml_path, method_name)
+
```

## zswag/doc.py

 * *Ordering differences only*

```diff
@@ -1,123 +1,123 @@
-from enum import Enum
-from typing import List, Dict
-import re
-import glob
-import os
-
-RPC_DOC_PATTERN = r"""
-        service\s+{service_name}\s+\{{   # service MyService {{ (double-braces due to later .format())
-            (?:\n|.)*                    #   ...
-            /\*\*?\s*                    #   /**
-                ((?:[^*]|\*[^/])*)       #     (doc-string) -> captured
-            \*/                          #   */
-            \s*([A-Za-z0-9_]*)\s+        #   (return-type) -> captured
-            {rpc_name}                   #   method-name
-                \s*\(\s*                 #   (
-                    ([A-Za-z0-9_]*)      #     (argument-type) -> captured
-                \s*\)                    #   )
-"""
-
-STRUCT_PATTERN = r"""
-          /\*\!                          # /*!
-            ((?:[^!]|![^*]|!\*[^/])*)    #   (doc-string) -> captured
-          !\*/\s+                        # !*/
-          struct\s+{name}                # struct NAME
-"""
-
-SERVICE_PATTERN = r"""
-          /\*\!                          # /*!
-            ((?:[^!]|![^*]|!\*[^/])*)    #   (doc-string) -> captured
-          !\*/\s+                        # !*/
-          service\s+{name}               # service NAME
-"""
-
-
-class IdentType(Enum):
-    """
-    Use these enum entries with `get_doc_str()`.
-    """
-    STRUCT = 0
-    SERVICE = 1
-    RPC = 2
-
-
-"""
-Caches glob.glob() results for *.zs file searches in get_doc_str().
-The dictionary points from a package path to amalgamated zserio code
-for that package.
-"""
-zs_pkg_cache: Dict[str, str] = {}
-
-
-def get_amalgamated_zs(pkg_path):
-    global zs_pkg_cache
-    if pkg_path in zs_pkg_cache:
-        return zs_pkg_cache[pkg_path]
-    zs_files = glob.glob(os.path.join(pkg_path, "**/*.zs"), recursive="True")
-    result = ""
-    for zs_file_path in zs_files:
-        with open(zs_file_path) as zs_file:
-            result += zs_file.read() + "\n"
-    zs_pkg_cache[pkg_path] = result
-    return result
-
-
-def get_doc_str(*, ident_type: IdentType, pkg_path: str, ident: str, fallback: List[str] = None) -> List[str]:
-    f"""
-    Get a docstring for a particular zserio identifier. This method searches all .zs-files
-    under `pkg_path` for a specific pattern given by `ident_type` and `ident`
-
-    The following patterns are looked for:
-
-      With `ident_type` IdentType.STRUCT:
-        With ident as "path.to.package.NAME":
-         {STRUCT_PATTERN}
-
-      With `ident_type` IdentType.SERVICE)
-        Same as STRUCT, except looking for "service NAME".
-
-      With `ident_type` IdentType.RPC)
-        With ident as "path.to.service.SERVICE.NAME":
-         {RPC_DOC_PATTERN}
-
-    The list of all capture group values is returned.
-    """
-    if fallback is None:
-        fallback = []
-    if not pkg_path:
-        return fallback
-    zs_src = get_amalgamated_zs(pkg_path)
-    ident_parts = ident.split(".")
-    pattern_format_replacements = {}
-    if ident_type == IdentType.STRUCT:
-        if not ident_parts:
-            print("[ERROR] Need at least one identifier part to find struct docs.")
-            return fallback
-        pattern = STRUCT_PATTERN
-        pattern_format_replacements["name"] = ident_parts[-1]
-    elif ident_type == IdentType.SERVICE:
-        if not ident_parts:
-            print("[ERROR] Need at least one identifier part to find service docs.")
-            return fallback
-        pattern = SERVICE_PATTERN
-        pattern_format_replacements["name"] = ident_parts[-1]
-    elif ident_type == IdentType.RPC:
-        if not ident_parts or len(ident_parts) < 2:
-            print("[ERROR] Need at least tow identifiers (service.rpc-name) to find RPC docs.")
-            return fallback
-        pattern = RPC_DOC_PATTERN
-        pattern_format_replacements["service_name"] = ident_parts[-2]
-        pattern_format_replacements["rpc_name"] = ident_parts[-1]
-    else:
-        print("[ERROR] get_doc_str: Unsupported identifier type!")
-        return fallback
-    compiled_pattern = re.compile(pattern.format(**pattern_format_replacements), re.X)
-    match = compiled_pattern.search(zs_src)
-    if match:
-        return list(match.groups())
-    else:
-        return fallback
-
-
-def md_filter_definition(md: str) -> str:
-    return re.sub(r"\n*\*\*[Dd]efinitions?[:\s]*\*\*\n*", "", md.strip()).strip()
+from enum import Enum
+from typing import List, Dict
+import re
+import glob
+import os
+
+RPC_DOC_PATTERN = r"""
+        service\s+{service_name}\s+\{{   # service MyService {{ (double-braces due to later .format())
+            (?:\n|.)*                    #   ...
+            /\*\*?\s*                    #   /**
+                ((?:[^*]|\*[^/])*)       #     (doc-string) -> captured
+            \*/                          #   */
+            \s*([A-Za-z0-9_]*)\s+        #   (return-type) -> captured
+            {rpc_name}                   #   method-name
+                \s*\(\s*                 #   (
+                    ([A-Za-z0-9_]*)      #     (argument-type) -> captured
+                \s*\)                    #   )
+"""
+
+STRUCT_PATTERN = r"""
+          /\*\!                          # /*!
+            ((?:[^!]|![^*]|!\*[^/])*)    #   (doc-string) -> captured
+          !\*/\s+                        # !*/
+          struct\s+{name}                # struct NAME
+"""
+
+SERVICE_PATTERN = r"""
+          /\*\!                          # /*!
+            ((?:[^!]|![^*]|!\*[^/])*)    #   (doc-string) -> captured
+          !\*/\s+                        # !*/
+          service\s+{name}               # service NAME
+"""
+
+
+class IdentType(Enum):
+    """
+    Use these enum entries with `get_doc_str()`.
+    """
+    STRUCT = 0
+    SERVICE = 1
+    RPC = 2
+
+
+"""
+Caches glob.glob() results for *.zs file searches in get_doc_str().
+The dictionary points from a package path to amalgamated zserio code
+for that package.
+"""
+zs_pkg_cache: Dict[str, str] = {}
+
+
+def get_amalgamated_zs(pkg_path):
+    global zs_pkg_cache
+    if pkg_path in zs_pkg_cache:
+        return zs_pkg_cache[pkg_path]
+    zs_files = glob.glob(os.path.join(pkg_path, "**/*.zs"), recursive="True")
+    result = ""
+    for zs_file_path in zs_files:
+        with open(zs_file_path) as zs_file:
+            result += zs_file.read() + "\n"
+    zs_pkg_cache[pkg_path] = result
+    return result
+
+
+def get_doc_str(*, ident_type: IdentType, pkg_path: str, ident: str, fallback: List[str] = None) -> List[str]:
+    f"""
+    Get a docstring for a particular zserio identifier. This method searches all .zs-files
+    under `pkg_path` for a specific pattern given by `ident_type` and `ident`
+
+    The following patterns are looked for:
+
+      With `ident_type` IdentType.STRUCT:
+        With ident as "path.to.package.NAME":
+         {STRUCT_PATTERN}
+
+      With `ident_type` IdentType.SERVICE)
+        Same as STRUCT, except looking for "service NAME".
+
+      With `ident_type` IdentType.RPC)
+        With ident as "path.to.service.SERVICE.NAME":
+         {RPC_DOC_PATTERN}
+
+    The list of all capture group values is returned.
+    """
+    if fallback is None:
+        fallback = []
+    if not pkg_path:
+        return fallback
+    zs_src = get_amalgamated_zs(pkg_path)
+    ident_parts = ident.split(".")
+    pattern_format_replacements = {}
+    if ident_type == IdentType.STRUCT:
+        if not ident_parts:
+            print("[ERROR] Need at least one identifier part to find struct docs.")
+            return fallback
+        pattern = STRUCT_PATTERN
+        pattern_format_replacements["name"] = ident_parts[-1]
+    elif ident_type == IdentType.SERVICE:
+        if not ident_parts:
+            print("[ERROR] Need at least one identifier part to find service docs.")
+            return fallback
+        pattern = SERVICE_PATTERN
+        pattern_format_replacements["name"] = ident_parts[-1]
+    elif ident_type == IdentType.RPC:
+        if not ident_parts or len(ident_parts) < 2:
+            print("[ERROR] Need at least tow identifiers (service.rpc-name) to find RPC docs.")
+            return fallback
+        pattern = RPC_DOC_PATTERN
+        pattern_format_replacements["service_name"] = ident_parts[-2]
+        pattern_format_replacements["rpc_name"] = ident_parts[-1]
+    else:
+        print("[ERROR] get_doc_str: Unsupported identifier type!")
+        return fallback
+    compiled_pattern = re.compile(pattern.format(**pattern_format_replacements), re.X)
+    match = compiled_pattern.search(zs_src)
+    if match:
+        return list(match.groups())
+    else:
+        return fallback
+
+
+def md_filter_definition(md: str) -> str:
+    return re.sub(r"\n*\*\*[Dd]efinitions?[:\s]*\*\*\n*", "", md.strip()).strip()
```

## zswag/gen.py

 * *Ordering differences only*

```diff
@@ -1,590 +1,590 @@
-import copy
-import os
-import random
-
-import openapi_spec_validator.exceptions
-import yaml
-import sys
-import inspect
-import tempfile
-import importlib
-from typing import Optional, Dict, Tuple, List, IO
-from argparse import ArgumentParser, FileType, RawTextHelpFormatter
-from subprocess import CalledProcessError
-import dataclasses as dc
-from copy import deepcopy
-from enum import Enum
-from zserio.typeinfo import MemberAttribute
-from openapi_spec_validator import validate_spec
-import uuid
-import zserio
-from pyzswagcl import \
-    ZSERIO_OBJECT_CONTENT_TYPE, \
-    ZSERIO_REQUEST_PART_WHOLE, \
-    ZSERIO_REQUEST_PART, \
-    parse_openapi_config
-
-from .reflect import \
-    service_method_request_type, \
-    rgetattr, \
-    check_uninstantiable, \
-    cached_type_info, \
-    members as type_members, \
-    find_field, \
-    is_scalar
-from .doc import get_doc_str, IdentType, md_filter_definition
-
-
-class HttpParamLocation(Enum):
-    QUERY = "query"
-    BODY = "body"
-    PATH = "path"
-    HEADER = "header"
-
-
-class HttpParamFormat(Enum):
-    STRING = "string"
-    BINARY = "binary"
-    BYTE = "byte"
-    BASE64 = "base64"
-    BASE64URL = "base64url"
-    HEX = "hex"
-
-
-HTTP_METHOD_TAGS = ("get", "put", "post", "delete")
-FLATTEN_TAG = "flat"
-BLOB_TAG = "blob"
-SECURITY_ASSIGNMENT_TAG = "security="
-PATH_ASSIGNMENT_TAG = "path="
-WILDCARD_CONFIG = "*"
-
-
-def argdoc(s: str):
-    return "\n"+inspect.cleandoc(s)+"\n\n"
-
-
-def less_indent_formatter(prog):
-    return RawTextHelpFormatter(prog, max_help_position=8, width=80)
-
-
-@dc.dataclass
-class ParamSpecifier:
-    """"Can be used to annotate a method config with a desired
-    location, format and parameter name for a request-part field."""
-    request_part: str            # e.g. "request_member.subfield"
-    name: Optional[str]          # e.g. "subfieldParam"
-    location: HttpParamLocation  # e.g. QUERY
-    format: HttpParamFormat        # e.g. BASE64
-    style: Optional[str] = None
-    explode: Optional[str] = None
-
-
-@dc.dataclass
-class MethodConfig:
-    """User-specified set of parameters to control how a zserio service method
-    is converted into an OpenAPI-file entry."""
-    name: str
-    http_method: str = "post"
-    param_loc: Optional[HttpParamLocation] = None  # None -> Whole request blob in body
-    flatten: bool = False
-    param_specifiers: Optional[List[ParamSpecifier]] = dc.field(default_factory=list)
-    security: Optional[str] = None
-    path: Optional[str] = None
-    openapi_docstring: str = ""
-    openapi_return_type: str = ""
-    openapi_arg_type: str = "Unknown"
-    openapi_result_doc: str = ""
-    openapi_arg_doc: str = ""
-    openapi_parameters: dict = dc.field(default_factory=dict)
-
-
-class OpenApiGenError(RuntimeError):
-    """Raised by OpenApiSchemaGenerator when something goes wrong."""
-    def __init__(self, what: str):
-        super(OpenApiGenError, self).__init__(what)
-
-
-class OpenApiSchemaGenerator:
-
-    def __init__(self, *,
-                 service: str,
-                 path: str,
-                 package: Optional[str] = None,
-                 config: Optional[List[str]] = None,
-                 output: IO,
-                 base_config: Optional[IO],
-                 zserio_src_root: Optional[str]):
-
-        # Process service name and package path
-        self.service_name = service
-        self.zs_pkg_path = zserio_src_root
-        service_name_parts = service.split(".") + ["Service"]
-
-        if os.path.isdir(path):
-            # Generate OpenAPI from existing Python code
-            sys.path.append(path)
-            python_module = importlib.import_module(f"{service_name_parts[0]}.api")
-            self.zs_pkg_path = None
-        else:
-            if self.zs_pkg_path is None:
-                self.zs_pkg_path = os.path.abspath(os.path.dirname(path))
-                path = os.path.basename(path)
-            full_path = os.path.join(self.zs_pkg_path, path)
-            if not os.path.isfile(full_path):
-                raise OpenApiGenError(f"The path '{full_path}' is neither a zserio file nor a pythonpath.")
-            # Generate OpenAPI from zserio code. Must generate
-            # intermediate Python source to inspect service.
-            if package is None:
-                package = f"zswag_gen_{uuid.uuid1().hex}"
-            if service_name_parts[0] != package:
-                service_name_parts = [package] + service_name_parts
-            try:
-                gen_dir = tempfile.mkdtemp("zswag.gen")
-                python_module = zserio.generate(
-                    zs_dir=self.zs_pkg_path,
-                    main_zs_file=path,
-                    top_level_package=package,
-                    gen_dir=gen_dir,
-                    extra_args=["-withTypeInfoCode"])
-            except CalledProcessError as e:
-                raise OpenApiGenError(f"Failed to parse zserio sources:\n{e.stderr}")
-        if not python_module:
-            raise OpenApiGenError(f"Could not import {service_name_parts[0]}.api!")
-        self.service_type = rgetattr(python_module, ".".join(service_name_parts[1:]))
-        self.service_instance = self.service_type()
-
-        # Process method config tags ...
-        self.config: Dict[str, MethodConfig] = dict()
-        self.config[WILDCARD_CONFIG] = default_entry = MethodConfig(WILDCARD_CONFIG)
-        self.output = output
-        self.base_config = dict()
-        # ... first load base-config.
-        if base_config:
-            self.base_config = yaml.load(base_config, yaml.Loader)
-        if methods_base_config := self.base_config.get("methods", None):
-            # If there are wildcard base-config tags, process them first.
-            if default_config_tags := methods_base_config.get(WILDCARD_CONFIG, None):
-                default_entry = self.add_method_config_from_tags(WILDCARD_CONFIG, default_config_tags, default_entry)
-            # Then process tags for other methods from the base-config.
-            for method_name, tags in ((m, t) for m, t in methods_base_config.items() if m != WILDCARD_CONFIG):
-                self.add_method_config_from_tags(method_name, tags, default_entry)
-        # ... then process additional tags from the command line.
-        if config:
-            for entry in config:
-                method_name = WILDCARD_CONFIG
-                parts = entry.split(":")
-                if len(parts) > 1:
-                    method_name = parts[0]
-                tag_list = [tag.strip() for tag in parts[-1].split(",")]
-                default_entry = self.add_method_config_from_tags(method_name, tag_list, default_entry)
-
-    def add_method_config_from_tags(
-            self,
-            method_name: str,
-            tag_list: List[str],
-            default_entry: MethodConfig) -> MethodConfig:
-        new_config = deepcopy(default_entry)
-        new_config.name = method_name
-        # Make sure that HTTP method tags are always processed first!
-        tag_list.sort(key=lambda x: x in HTTP_METHOD_TAGS, reverse=True)
-        for tag in tag_list:
-            if tag in HTTP_METHOD_TAGS:
-                new_config.http_method = tag
-            elif any(tag == loc.value for loc in HttpParamLocation):
-                new_config.param_loc = HttpParamLocation(tag)
-                if new_config.param_loc == HttpParamLocation.BODY and new_config.http_method == "get":
-                    raise OpenApiGenError(f"Cannot use `body` tag with HTTP GET.")
-            elif tag == FLATTEN_TAG:
-                new_config.flatten = True
-            elif tag == BLOB_TAG:
-                new_config.flatten = False
-            elif tag.startswith(SECURITY_ASSIGNMENT_TAG):
-                new_config.security = tag[len(SECURITY_ASSIGNMENT_TAG):]
-            elif tag.startswith(PATH_ASSIGNMENT_TAG):
-                if method_name == WILDCARD_CONFIG:
-                    raise OpenApiGenError(f"Refusing to apply '{tag}' to ALL methods. Likely not on purpose.")
-                else:
-                    new_config.path = tag[len(PATH_ASSIGNMENT_TAG):]
-            elif "?" in tag:
-                try:
-                    request_part, specifiers_part = tag.split("?")
-                    spec = dict(specifier.split("=") for specifier in specifiers_part.split("&"))
-                    par_loc = HttpParamLocation(spec.get("in"))
-                    if par_loc == HttpParamLocation.BODY:
-                        if new_config.http_method == "get":
-                            raise OpenApiGenError("Cannot use `location=body` with HTTP GET.")
-                        par_format = HttpParamFormat.BINARY
-                        par_name = "body"
-                    else:
-                        par_name, par_format = spec.get("name"), HttpParamFormat(spec.get("format", "string"))
-                    if any(par.name == par_name for par in new_config.param_specifiers):
-                        raise OpenApiGenError(f"Encountered duplicate use of parameter name '{par_name}' in the same method!")
-                    new_config.param_specifiers.append(ParamSpecifier(request_part, par_name, par_loc, par_format))
-                    # Process style and explode entries
-                    if style := spec.get("style", None):
-                        new_config.param_specifiers[-1].style = style.lower()
-                    if explode := spec.get("explode", None):
-                        new_config.param_specifiers[-1].explode = explode.lower()
-                except (ValueError, IndexError) as e:
-                    raise OpenApiGenError(f"Encountered malformed parameter specifier tag '{tag}' ({e})!")
-                except KeyError as missing_key:
-                    raise OpenApiGenError(f"Parameter specifier tag {tag} has no value for '{missing_key}' key.")
-            else:
-                raise OpenApiGenError(f"Did not understand tag '{tag}'.")
-        if method_name in self.config and method_name != WILDCARD_CONFIG:
-            print(f"[WARNING] Overwriting config for method {method_name}!")
-        self.config[method_name] = new_config
-        if method_name == WILDCARD_CONFIG:
-            default_entry = new_config
-        return default_entry
-
-    def config_for_method(self, method_name: str) -> MethodConfig:
-        if method_name in self.config:
-            return self.config[method_name]
-        else:
-            result = copy.deepcopy(self.config[WILDCARD_CONFIG])
-            result.name = method_name
-            return result
-
-    def generate(self):
-        service_name_parts = self.service_instance.service_full_name.split(".")
-        schema = {
-            "openapi": "3.0.0",
-            "info": self.base_config.get("info", {
-                "title": ".".join(service_name_parts[1:]),
-                "description": md_filter_definition(get_doc_str(
-                    ident_type=IdentType.SERVICE,
-                    pkg_path=self.zs_pkg_path,
-                    ident=self.service_instance.service_full_name,
-                    fallback=[f"REST API for {'.'.join(service_name_parts[1:])} service."]
-                )[0]),
-                "contact": {
-                    "email": "TODO@TODO.TODO"
-                },
-                "license": {
-                    "name": "TODO"
-                },
-                "version": "TODO",
-            }),
-            "servers": self.base_config.get("servers", []),
-            "paths": {
-                method_info.path: {
-                    method_info.http_method: {
-                        "summary": method_info.openapi_docstring,
-                        "description": method_info.openapi_docstring,
-                        "operationId": method_info.name,
-                        **method_info.openapi_parameters,
-                        "responses": {
-                            "200": {
-                                "description": method_info.openapi_result_doc,
-                                "content": {
-                                    ZSERIO_OBJECT_CONTENT_TYPE: {
-                                        "schema": {
-                                            "type": "string",
-                                            "format": "binary"
-                                        }
-                                    }
-                                }
-                            }
-                        }
-                    },
-                } for method_info in (
-                    self.process_method_config(method_name)
-                    for method_name in self.service_instance.method_names)
-            }
-        }
-        if security_schemes := self.base_config.get("securitySchemes", None):
-            schema["components"] = {
-                "securitySchemes": security_schemes
-            }
-        if security := self.base_config.get("security", None):
-            schema["security"] = security
-        print(f"[INFO] Validating with openapi-spec-validator ... ", end="")
-        try:
-            validate_spec(schema)
-        except openapi_spec_validator.exceptions.OpenAPIValidationError as e:
-            print()
-            raise OpenApiGenError(f"Spec is invalid: {e}")
-        print("OK")
-        print(f"[INFO] Writing to '{self.output.name}' ... ", end="")
-        yaml.dump(schema, self.output, default_flow_style=False)
-        self.output.close()
-        print("OK")
-        if os.path.isfile(self.output.name):
-            print(f"[INFO] Validating with zswag parser ... ", end="")
-            try:
-                parse_openapi_config(self.output.name)
-            except RuntimeError as e:
-                print()
-                raise OpenApiGenError(f"Spec is invalid: {e}")
-            print("OK")
-        else:
-            print(f"[INFO] Skipping zswag parser validation.")
-        print(f"[INFO] Done.")
-
-    def process_method_config(self, method_name: str) -> MethodConfig:
-        result = self.config_for_method(method_name)
-        req_t = service_method_request_type(self.service_instance, result.name)
-        req_t_info = cached_type_info(req_t)
-        assert req_t_info
-        method_ident = f"{self.service_instance.service_full_name}.{method_name}"
-        if not result.path:
-            print(f"[INFO] Auto-generating path for `{method_ident}`.")
-            result.path = f"/{method_name}"
-        # Generate doc-strings
-        if self.zs_pkg_path:
-            doc_strings = get_doc_str(
-                ident_type=IdentType.RPC,
-                pkg_path=self.zs_pkg_path,
-                ident=method_ident)
-            if doc_strings:
-                result.openapi_docstring = doc_strings[0]
-                result.openapi_return_type = doc_strings[1]
-                result.openapi_arg_type = doc_strings[2]
-                result.openapi_result_doc = md_filter_definition(get_doc_str(
-                    ident_type=IdentType.STRUCT,
-                    pkg_path=self.zs_pkg_path,
-                    ident=result.openapi_return_type,
-                    fallback=[f"### struct {result.openapi_return_type}"])[0])
-                result.openapi_arg_doc = md_filter_definition(get_doc_str(
-                    ident_type=IdentType.STRUCT,
-                    pkg_path=self.zs_pkg_path,
-                    ident=result.openapi_arg_type,
-                    fallback=[f"### struct {result.openapi_arg_type}"])[0])
-        # Convert simple legacy instructions into parameter specifiers
-        if not result.param_specifiers:
-            if result.param_loc == HttpParamLocation.BODY or (not result.param_loc and not result.flatten):
-                result.param_specifiers.append(
-                    ParamSpecifier(ZSERIO_REQUEST_PART_WHOLE, "", HttpParamLocation.BODY, HttpParamFormat.BINARY))
-            elif result.flatten:
-                if not_instantiable_reason := check_uninstantiable(req_t_info):
-                    raise OpenApiGenError(str(not_instantiable_reason))
-                for field_name, member_info in type_members(req_t_info, True):
-                    if is_scalar(member_info.type_info):
-                        result.param_specifiers.append(
-                            ParamSpecifier(
-                                field_name, field_name.replace(".", "__"),
-                                result.param_loc or HttpParamLocation.QUERY,
-                                HttpParamFormat.STRING))
-            elif result.param_loc:
-                result.param_specifiers.append(
-                    ParamSpecifier(
-                        ZSERIO_REQUEST_PART_WHOLE, "requestBody", result.param_loc, HttpParamFormat.BINARY))
-        # Convert MethodConfig.param_specifiers to MethodConfig.openapi_parameters
-        self.process_method_parameters(result)
-        return result
-
-    def process_method_parameters(self, config: MethodConfig):
-        req_t = service_method_request_type(self.service_instance, config.name)
-        req_t_info = cached_type_info(req_t)
-        # Convert parameter specifiers to parameters-JSON
-        openapi_param_list = []
-        for param_specifier in config.param_specifiers:
-            # Easy - parameter only indicates binary transfer of the
-            # request object in the body
-            if param_specifier.location == HttpParamLocation.BODY:
-                config.openapi_parameters["requestBody"] = {
-                    "description": config.openapi_arg_doc,
-                    "content": {
-                        ZSERIO_OBJECT_CONTENT_TYPE: {
-                            "schema": {
-                                "type": "string"
-                            }
-                        }
-                    }
-                }
-                continue
-            # Fallthrough - the parameter has a name, a format and a request part
-            # Process type-info first and determine if the field even exists.
-            openapi_schema_info = {
-                "type": "string",
-                "format": param_specifier.format.name.lower(),
-            }
-            if param_specifier.request_part != ZSERIO_REQUEST_PART_WHOLE:
-                _, member_info = find_field(req_t_info, param_specifier.request_part)
-                if not member_info:
-                    raise OpenApiGenError(f"Could not find field '{param_specifier.request_part}' in {req_t_info.schema_name}!")
-                # If the member is an array, we must indicate this in OpenAPI
-                if MemberAttribute.ARRAY_LENGTH in member_info.attributes:
-                    openapi_schema_info.update({
-                        "type": "array",
-                        "items": {
-                            "type": "string"
-                        }
-                    })
-            # If the parameter is to be placed in the path, make sure there's a placeholder
-            if param_specifier.location == HttpParamLocation.PATH:
-                placeholder = f"{{{param_specifier.name}}}"
-                if placeholder not in config.path:
-                    print(f"[INFO] Appending /{placeholder} to path for {config.name}")
-                    config.path += f"/{placeholder}"
-            # Append the OpenAPI information for the new parameter
-            openapi_param_list.append({
-                "in": param_specifier.location.value.lower(),
-                "name": param_specifier.name,
-                "description": config.openapi_arg_doc,
-                "required": True,
-                ZSERIO_REQUEST_PART: param_specifier.request_part,
-                **({"allowEmptyValue": True} if param_specifier.location == HttpParamLocation.QUERY else {}),
-                "schema": openapi_schema_info
-            })
-            # Add style and explode hints
-            if param_specifier.style:
-                openapi_param_list[-1]["style"] = param_specifier.style
-            if param_specifier.explode:
-                openapi_param_list[-1]["explode"] = param_specifier.explode == "true"
-        # Process security scheme
-        if config.security is not None:
-            if config.security == "":
-                print(f"[WARNING] {config.name} has explicit empty security setting.")
-                config.openapi_parameters["security"] = []
-            else:
-                config.openapi_parameters["security"] = [{config.security: []}]
-        # Set the finalized parameter list
-        config.openapi_parameters["parameters"] = openapi_param_list
-
-
-if __name__ == "__main__":
-
-    parser = ArgumentParser(
-        "Zserio OpenApi YAML Generator",
-        formatter_class=less_indent_formatter)
-    parser.add_argument("-s", "--service", nargs=1, required=True,
-                        metavar="service-identifier", help=argdoc("""
-                        Fully qualified zserio service identifier.
-                        
-                        Example:
-                            -s my.package.ServiceClass
-                        """))
-    parser.add_argument("-i", "--input", nargs=1, metavar="zserio-or-python-path",
-                        required=True, help=argdoc("""
-                        Can be either ...
-                        (A) Path to a zserio .zs file. Must be either a top-
-                            level entrypoint (e.g. all.zs), or a subpackage
-                            (e.g. services/myservice.zs) in conjunction with
-                            a "--zserio-source-root|-r <dir>" argument.
-                        (B) Path to parent dir of a zserio Python package.
-                        
-                        Examples:
-                            -i path/to/schema/main.zs         (A)
-                            -i path/to/python/package/parent  (B) 
-                        """))
-    parser.add_argument("-r", "--zserio-source-root", nargs=1, metavar="zserio-src-root-dir",
-                        required=False, help=argdoc("""
-                        When -i specifies a zs file (Option A), indicate the
-                        directory for the zserio -src directory argument. If
-                        not specified, the parent directory of the zs file
-                        will be used.
-                        """))
-    parser.add_argument("-p", "--package", nargs=1, metavar="top-level-package",
-                        required=False, help=argdoc("""
-                        When -i specifies a zs file (Option A), indicate
-                        that a specific top-level zserio package name
-                        should be used.
-                        
-                        Examples:
-                            -p zserio_pkg_name
-                        """))
-    parser.add_argument("-c", "--config", nargs="+", metavar="tags",
-                        action="append", help=argdoc("""
-                        Configuration tags for a specific or all methods.
-                        The argument syntax follows this pattern:
-                            
-                           [(service-method-name):](comma-separated-tags)
-                            
-                        Note: The -c argument may be applied multiple times.
-                        The `comma-separated-tags` must be a list of tags
-                        which indicate OpenApi method generator preferences.
-                        The following tags are supported:
-                        
-                        get|put|post|delete : HTTP method tags
-                                query|path| : Parameter location tags
-                                header|body 
-                                  flat|blob : Flatten request object,
-                                              or pass it as whole blob.
-                          (param-specifier) : Specify parameter name, format
-                                              and location for a specific
-                                              request-part. See below.
-                            security=(name) : Set a particular security
-                                              scheme to be used. The scheme
-                                              details must be provided through
-                                              the --base-config-yaml.
-                         path=(method-path) : Set a particular method path.
-                                              May contain placeholders for
-                                              path params.
-                                                   
-                        A (param-specifier) tag has the following schema:
-                        
-                            (field?name=...
-                                  &in=[path|body|query|header]
-                                  &format=[binary|base64|hex]
-                                  [&style=...]
-                                  [&explode=...])
-                        
-                        Examples:
-                        
-                          Expose all methods as POST, but `getLayerByTileId`
-                          as GET with flat path-parameters:
-                          
-                            `-c post getLayerByTileId:get,flat,path`
-                            
-                          For myMethod, put the whole request blob into the a
-                          query "data" parameter as base64:
-                          
-                            `-c myMethod:*?name=data&in=query&format=base64`
-                            
-                          For myMethod, set the "AwesomeAuth" auth scheme:
-                          
-                            `-c myMethod:security=AwesomeAuth`
-                            
-                          For myMethod, provide the path and place myField
-                          explicitely in a path placeholder:
-                          
-                            `-c 'myMethod:path=/my-method/{param},...
-                                 myField?name=param&in=path&format=string'`
-                            
-                        Note:
-                            * The HTTP-method defaults to `post`.
-                            * The parameter 'in' defaults to `query` for
-                              `get`, `body` otherwise.
-                            * If a method uses a parameter specifier, the
-                              `flat`, `body`, `query`, `path`, `header` and
-                              `body`-tags are ignored.
-                            * The `flat` tag is only meaningful in conjunction
-                              with `query` or `path`.
-                            * An unspecific tag list (no service-method-name)
-                              affects the defaults only for following, not
-                              preceding specialized tag assignments.
-                        """))
-    parser.add_argument("-o", "--output", nargs=1, type=FileType("w"), default=[sys.stdout],
-                        metavar="output", help=argdoc("""
-                        Output file path. If not specified, the output will be
-                        written to stdout.
-                        """))
-    parser.add_argument("-b", "--base-config-yaml", nargs=1, type=FileType("r"), required=False, default=[None],
-                        help=argdoc("""
-                        Base configuration file. Can be used to fully or partially
-                        substitute --config arguments, and to provide additional
-                        OpenAPI information. The YAML file must look like this:
-                        
-                          method: # Optional method tags dictionary
-                            <method-name|*>: <list of config tags>
-                          securitySchemes: ... # Optional OpenAPI securitySchemes
-                          info: ...            # Optional OpenAPI info section
-                          servers: ...         # Optional OpenAPI servers section
-                          security: ...        # Optional OpenAPI global security
-                        """))
-
-    args = parser.parse_args(sys.argv[1:])
-    try:
-        OpenApiSchemaGenerator(
-            service=args.service[0],
-            path=args.input[0] if args.input else None,
-            package=args.package[0] if args.package else None,
-            config=[arg for args in args.config for arg in args] if args.config else [],
-            output=args.output[0],
-            base_config=args.base_config_yaml[0] if args.base_config_yaml else None,
-            zserio_src_root=args.zserio_source_root[0] if args.zserio_source_root else None).generate()
-    except OpenApiGenError as e:
-        print(f"[ERROR] {e}")
-        exit(1)
+import copy
+import os
+import random
+
+import openapi_spec_validator.exceptions
+import yaml
+import sys
+import inspect
+import tempfile
+import importlib
+from typing import Optional, Dict, Tuple, List, IO
+from argparse import ArgumentParser, FileType, RawTextHelpFormatter
+from subprocess import CalledProcessError
+import dataclasses as dc
+from copy import deepcopy
+from enum import Enum
+from zserio.typeinfo import MemberAttribute
+from openapi_spec_validator import validate_spec
+import uuid
+import zserio
+from pyzswagcl import \
+    ZSERIO_OBJECT_CONTENT_TYPE, \
+    ZSERIO_REQUEST_PART_WHOLE, \
+    ZSERIO_REQUEST_PART, \
+    parse_openapi_config
+
+from .reflect import \
+    service_method_request_type, \
+    rgetattr, \
+    check_uninstantiable, \
+    cached_type_info, \
+    members as type_members, \
+    find_field, \
+    is_scalar
+from .doc import get_doc_str, IdentType, md_filter_definition
+
+
+class HttpParamLocation(Enum):
+    QUERY = "query"
+    BODY = "body"
+    PATH = "path"
+    HEADER = "header"
+
+
+class HttpParamFormat(Enum):
+    STRING = "string"
+    BINARY = "binary"
+    BYTE = "byte"
+    BASE64 = "base64"
+    BASE64URL = "base64url"
+    HEX = "hex"
+
+
+HTTP_METHOD_TAGS = ("get", "put", "post", "delete")
+FLATTEN_TAG = "flat"
+BLOB_TAG = "blob"
+SECURITY_ASSIGNMENT_TAG = "security="
+PATH_ASSIGNMENT_TAG = "path="
+WILDCARD_CONFIG = "*"
+
+
+def argdoc(s: str):
+    return "\n"+inspect.cleandoc(s)+"\n\n"
+
+
+def less_indent_formatter(prog):
+    return RawTextHelpFormatter(prog, max_help_position=8, width=80)
+
+
+@dc.dataclass
+class ParamSpecifier:
+    """"Can be used to annotate a method config with a desired
+    location, format and parameter name for a request-part field."""
+    request_part: str            # e.g. "request_member.subfield"
+    name: Optional[str]          # e.g. "subfieldParam"
+    location: HttpParamLocation  # e.g. QUERY
+    format: HttpParamFormat        # e.g. BASE64
+    style: Optional[str] = None
+    explode: Optional[str] = None
+
+
+@dc.dataclass
+class MethodConfig:
+    """User-specified set of parameters to control how a zserio service method
+    is converted into an OpenAPI-file entry."""
+    name: str
+    http_method: str = "post"
+    param_loc: Optional[HttpParamLocation] = None  # None -> Whole request blob in body
+    flatten: bool = False
+    param_specifiers: Optional[List[ParamSpecifier]] = dc.field(default_factory=list)
+    security: Optional[str] = None
+    path: Optional[str] = None
+    openapi_docstring: str = ""
+    openapi_return_type: str = ""
+    openapi_arg_type: str = "Unknown"
+    openapi_result_doc: str = ""
+    openapi_arg_doc: str = ""
+    openapi_parameters: dict = dc.field(default_factory=dict)
+
+
+class OpenApiGenError(RuntimeError):
+    """Raised by OpenApiSchemaGenerator when something goes wrong."""
+    def __init__(self, what: str):
+        super(OpenApiGenError, self).__init__(what)
+
+
+class OpenApiSchemaGenerator:
+
+    def __init__(self, *,
+                 service: str,
+                 path: str,
+                 package: Optional[str] = None,
+                 config: Optional[List[str]] = None,
+                 output: IO,
+                 base_config: Optional[IO],
+                 zserio_src_root: Optional[str]):
+
+        # Process service name and package path
+        self.service_name = service
+        self.zs_pkg_path = zserio_src_root
+        service_name_parts = service.split(".") + ["Service"]
+
+        if os.path.isdir(path):
+            # Generate OpenAPI from existing Python code
+            sys.path.append(path)
+            python_module = importlib.import_module(f"{service_name_parts[0]}.api")
+            self.zs_pkg_path = None
+        else:
+            if self.zs_pkg_path is None:
+                self.zs_pkg_path = os.path.abspath(os.path.dirname(path))
+                path = os.path.basename(path)
+            full_path = os.path.join(self.zs_pkg_path, path)
+            if not os.path.isfile(full_path):
+                raise OpenApiGenError(f"The path '{full_path}' is neither a zserio file nor a pythonpath.")
+            # Generate OpenAPI from zserio code. Must generate
+            # intermediate Python source to inspect service.
+            if package is None:
+                package = f"zswag_gen_{uuid.uuid1().hex}"
+            if service_name_parts[0] != package:
+                service_name_parts = [package] + service_name_parts
+            try:
+                gen_dir = tempfile.mkdtemp("zswag.gen")
+                python_module = zserio.generate(
+                    zs_dir=self.zs_pkg_path,
+                    main_zs_file=path,
+                    top_level_package=package,
+                    gen_dir=gen_dir,
+                    extra_args=["-withTypeInfoCode"])
+            except CalledProcessError as e:
+                raise OpenApiGenError(f"Failed to parse zserio sources:\n{e.stderr}")
+        if not python_module:
+            raise OpenApiGenError(f"Could not import {service_name_parts[0]}.api!")
+        self.service_type = rgetattr(python_module, ".".join(service_name_parts[1:]))
+        self.service_instance = self.service_type()
+
+        # Process method config tags ...
+        self.config: Dict[str, MethodConfig] = dict()
+        self.config[WILDCARD_CONFIG] = default_entry = MethodConfig(WILDCARD_CONFIG)
+        self.output = output
+        self.base_config = dict()
+        # ... first load base-config.
+        if base_config:
+            self.base_config = yaml.load(base_config, yaml.Loader)
+        if methods_base_config := self.base_config.get("methods", None):
+            # If there are wildcard base-config tags, process them first.
+            if default_config_tags := methods_base_config.get(WILDCARD_CONFIG, None):
+                default_entry = self.add_method_config_from_tags(WILDCARD_CONFIG, default_config_tags, default_entry)
+            # Then process tags for other methods from the base-config.
+            for method_name, tags in ((m, t) for m, t in methods_base_config.items() if m != WILDCARD_CONFIG):
+                self.add_method_config_from_tags(method_name, tags, default_entry)
+        # ... then process additional tags from the command line.
+        if config:
+            for entry in config:
+                method_name = WILDCARD_CONFIG
+                parts = entry.split(":")
+                if len(parts) > 1:
+                    method_name = parts[0]
+                tag_list = [tag.strip() for tag in parts[-1].split(",")]
+                default_entry = self.add_method_config_from_tags(method_name, tag_list, default_entry)
+
+    def add_method_config_from_tags(
+            self,
+            method_name: str,
+            tag_list: List[str],
+            default_entry: MethodConfig) -> MethodConfig:
+        new_config = deepcopy(default_entry)
+        new_config.name = method_name
+        # Make sure that HTTP method tags are always processed first!
+        tag_list.sort(key=lambda x: x in HTTP_METHOD_TAGS, reverse=True)
+        for tag in tag_list:
+            if tag in HTTP_METHOD_TAGS:
+                new_config.http_method = tag
+            elif any(tag == loc.value for loc in HttpParamLocation):
+                new_config.param_loc = HttpParamLocation(tag)
+                if new_config.param_loc == HttpParamLocation.BODY and new_config.http_method == "get":
+                    raise OpenApiGenError(f"Cannot use `body` tag with HTTP GET.")
+            elif tag == FLATTEN_TAG:
+                new_config.flatten = True
+            elif tag == BLOB_TAG:
+                new_config.flatten = False
+            elif tag.startswith(SECURITY_ASSIGNMENT_TAG):
+                new_config.security = tag[len(SECURITY_ASSIGNMENT_TAG):]
+            elif tag.startswith(PATH_ASSIGNMENT_TAG):
+                if method_name == WILDCARD_CONFIG:
+                    raise OpenApiGenError(f"Refusing to apply '{tag}' to ALL methods. Likely not on purpose.")
+                else:
+                    new_config.path = tag[len(PATH_ASSIGNMENT_TAG):]
+            elif "?" in tag:
+                try:
+                    request_part, specifiers_part = tag.split("?")
+                    spec = dict(specifier.split("=") for specifier in specifiers_part.split("&"))
+                    par_loc = HttpParamLocation(spec.get("in"))
+                    if par_loc == HttpParamLocation.BODY:
+                        if new_config.http_method == "get":
+                            raise OpenApiGenError("Cannot use `location=body` with HTTP GET.")
+                        par_format = HttpParamFormat.BINARY
+                        par_name = "body"
+                    else:
+                        par_name, par_format = spec.get("name"), HttpParamFormat(spec.get("format", "string"))
+                    if any(par.name == par_name for par in new_config.param_specifiers):
+                        raise OpenApiGenError(f"Encountered duplicate use of parameter name '{par_name}' in the same method!")
+                    new_config.param_specifiers.append(ParamSpecifier(request_part, par_name, par_loc, par_format))
+                    # Process style and explode entries
+                    if style := spec.get("style", None):
+                        new_config.param_specifiers[-1].style = style.lower()
+                    if explode := spec.get("explode", None):
+                        new_config.param_specifiers[-1].explode = explode.lower()
+                except (ValueError, IndexError) as e:
+                    raise OpenApiGenError(f"Encountered malformed parameter specifier tag '{tag}' ({e})!")
+                except KeyError as missing_key:
+                    raise OpenApiGenError(f"Parameter specifier tag {tag} has no value for '{missing_key}' key.")
+            else:
+                raise OpenApiGenError(f"Did not understand tag '{tag}'.")
+        if method_name in self.config and method_name != WILDCARD_CONFIG:
+            print(f"[WARNING] Overwriting config for method {method_name}!")
+        self.config[method_name] = new_config
+        if method_name == WILDCARD_CONFIG:
+            default_entry = new_config
+        return default_entry
+
+    def config_for_method(self, method_name: str) -> MethodConfig:
+        if method_name in self.config:
+            return self.config[method_name]
+        else:
+            result = copy.deepcopy(self.config[WILDCARD_CONFIG])
+            result.name = method_name
+            return result
+
+    def generate(self):
+        service_name_parts = self.service_instance.service_full_name.split(".")
+        schema = {
+            "openapi": "3.0.0",
+            "info": self.base_config.get("info", {
+                "title": ".".join(service_name_parts[1:]),
+                "description": md_filter_definition(get_doc_str(
+                    ident_type=IdentType.SERVICE,
+                    pkg_path=self.zs_pkg_path,
+                    ident=self.service_instance.service_full_name,
+                    fallback=[f"REST API for {'.'.join(service_name_parts[1:])} service."]
+                )[0]),
+                "contact": {
+                    "email": "TODO@TODO.TODO"
+                },
+                "license": {
+                    "name": "TODO"
+                },
+                "version": "TODO",
+            }),
+            "servers": self.base_config.get("servers", []),
+            "paths": {
+                method_info.path: {
+                    method_info.http_method: {
+                        "summary": method_info.openapi_docstring,
+                        "description": method_info.openapi_docstring,
+                        "operationId": method_info.name,
+                        **method_info.openapi_parameters,
+                        "responses": {
+                            "200": {
+                                "description": method_info.openapi_result_doc,
+                                "content": {
+                                    ZSERIO_OBJECT_CONTENT_TYPE: {
+                                        "schema": {
+                                            "type": "string",
+                                            "format": "binary"
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    },
+                } for method_info in (
+                    self.process_method_config(method_name)
+                    for method_name in self.service_instance.method_names)
+            }
+        }
+        if security_schemes := self.base_config.get("securitySchemes", None):
+            schema["components"] = {
+                "securitySchemes": security_schemes
+            }
+        if security := self.base_config.get("security", None):
+            schema["security"] = security
+        print(f"[INFO] Validating with openapi-spec-validator ... ", end="")
+        try:
+            validate_spec(schema)
+        except openapi_spec_validator.exceptions.OpenAPIValidationError as e:
+            print()
+            raise OpenApiGenError(f"Spec is invalid: {e}")
+        print("OK")
+        print(f"[INFO] Writing to '{self.output.name}' ... ", end="")
+        yaml.dump(schema, self.output, default_flow_style=False)
+        self.output.close()
+        print("OK")
+        if os.path.isfile(self.output.name):
+            print(f"[INFO] Validating with zswag parser ... ", end="")
+            try:
+                parse_openapi_config(self.output.name)
+            except RuntimeError as e:
+                print()
+                raise OpenApiGenError(f"Spec is invalid: {e}")
+            print("OK")
+        else:
+            print(f"[INFO] Skipping zswag parser validation.")
+        print(f"[INFO] Done.")
+
+    def process_method_config(self, method_name: str) -> MethodConfig:
+        result = self.config_for_method(method_name)
+        req_t = service_method_request_type(self.service_instance, result.name)
+        req_t_info = cached_type_info(req_t)
+        assert req_t_info
+        method_ident = f"{self.service_instance.service_full_name}.{method_name}"
+        if not result.path:
+            print(f"[INFO] Auto-generating path for `{method_ident}`.")
+            result.path = f"/{method_name}"
+        # Generate doc-strings
+        if self.zs_pkg_path:
+            doc_strings = get_doc_str(
+                ident_type=IdentType.RPC,
+                pkg_path=self.zs_pkg_path,
+                ident=method_ident)
+            if doc_strings:
+                result.openapi_docstring = doc_strings[0]
+                result.openapi_return_type = doc_strings[1]
+                result.openapi_arg_type = doc_strings[2]
+                result.openapi_result_doc = md_filter_definition(get_doc_str(
+                    ident_type=IdentType.STRUCT,
+                    pkg_path=self.zs_pkg_path,
+                    ident=result.openapi_return_type,
+                    fallback=[f"### struct {result.openapi_return_type}"])[0])
+                result.openapi_arg_doc = md_filter_definition(get_doc_str(
+                    ident_type=IdentType.STRUCT,
+                    pkg_path=self.zs_pkg_path,
+                    ident=result.openapi_arg_type,
+                    fallback=[f"### struct {result.openapi_arg_type}"])[0])
+        # Convert simple legacy instructions into parameter specifiers
+        if not result.param_specifiers:
+            if result.param_loc == HttpParamLocation.BODY or (not result.param_loc and not result.flatten):
+                result.param_specifiers.append(
+                    ParamSpecifier(ZSERIO_REQUEST_PART_WHOLE, "", HttpParamLocation.BODY, HttpParamFormat.BINARY))
+            elif result.flatten:
+                if not_instantiable_reason := check_uninstantiable(req_t_info):
+                    raise OpenApiGenError(str(not_instantiable_reason))
+                for field_name, member_info in type_members(req_t_info, True):
+                    if is_scalar(member_info.type_info):
+                        result.param_specifiers.append(
+                            ParamSpecifier(
+                                field_name, field_name.replace(".", "__"),
+                                result.param_loc or HttpParamLocation.QUERY,
+                                HttpParamFormat.STRING))
+            elif result.param_loc:
+                result.param_specifiers.append(
+                    ParamSpecifier(
+                        ZSERIO_REQUEST_PART_WHOLE, "requestBody", result.param_loc, HttpParamFormat.BINARY))
+        # Convert MethodConfig.param_specifiers to MethodConfig.openapi_parameters
+        self.process_method_parameters(result)
+        return result
+
+    def process_method_parameters(self, config: MethodConfig):
+        req_t = service_method_request_type(self.service_instance, config.name)
+        req_t_info = cached_type_info(req_t)
+        # Convert parameter specifiers to parameters-JSON
+        openapi_param_list = []
+        for param_specifier in config.param_specifiers:
+            # Easy - parameter only indicates binary transfer of the
+            # request object in the body
+            if param_specifier.location == HttpParamLocation.BODY:
+                config.openapi_parameters["requestBody"] = {
+                    "description": config.openapi_arg_doc,
+                    "content": {
+                        ZSERIO_OBJECT_CONTENT_TYPE: {
+                            "schema": {
+                                "type": "string"
+                            }
+                        }
+                    }
+                }
+                continue
+            # Fallthrough - the parameter has a name, a format and a request part
+            # Process type-info first and determine if the field even exists.
+            openapi_schema_info = {
+                "type": "string",
+                "format": param_specifier.format.name.lower(),
+            }
+            if param_specifier.request_part != ZSERIO_REQUEST_PART_WHOLE:
+                _, member_info = find_field(req_t_info, param_specifier.request_part)
+                if not member_info:
+                    raise OpenApiGenError(f"Could not find field '{param_specifier.request_part}' in {req_t_info.schema_name}!")
+                # If the member is an array, we must indicate this in OpenAPI
+                if MemberAttribute.ARRAY_LENGTH in member_info.attributes:
+                    openapi_schema_info.update({
+                        "type": "array",
+                        "items": {
+                            "type": "string"
+                        }
+                    })
+            # If the parameter is to be placed in the path, make sure there's a placeholder
+            if param_specifier.location == HttpParamLocation.PATH:
+                placeholder = f"{{{param_specifier.name}}}"
+                if placeholder not in config.path:
+                    print(f"[INFO] Appending /{placeholder} to path for {config.name}")
+                    config.path += f"/{placeholder}"
+            # Append the OpenAPI information for the new parameter
+            openapi_param_list.append({
+                "in": param_specifier.location.value.lower(),
+                "name": param_specifier.name,
+                "description": config.openapi_arg_doc,
+                "required": True,
+                ZSERIO_REQUEST_PART: param_specifier.request_part,
+                **({"allowEmptyValue": True} if param_specifier.location == HttpParamLocation.QUERY else {}),
+                "schema": openapi_schema_info
+            })
+            # Add style and explode hints
+            if param_specifier.style:
+                openapi_param_list[-1]["style"] = param_specifier.style
+            if param_specifier.explode:
+                openapi_param_list[-1]["explode"] = param_specifier.explode == "true"
+        # Process security scheme
+        if config.security is not None:
+            if config.security == "":
+                print(f"[WARNING] {config.name} has explicit empty security setting.")
+                config.openapi_parameters["security"] = []
+            else:
+                config.openapi_parameters["security"] = [{config.security: []}]
+        # Set the finalized parameter list
+        config.openapi_parameters["parameters"] = openapi_param_list
+
+
+if __name__ == "__main__":
+
+    parser = ArgumentParser(
+        "Zserio OpenApi YAML Generator",
+        formatter_class=less_indent_formatter)
+    parser.add_argument("-s", "--service", nargs=1, required=True,
+                        metavar="service-identifier", help=argdoc("""
+                        Fully qualified zserio service identifier.
+                        
+                        Example:
+                            -s my.package.ServiceClass
+                        """))
+    parser.add_argument("-i", "--input", nargs=1, metavar="zserio-or-python-path",
+                        required=True, help=argdoc("""
+                        Can be either ...
+                        (A) Path to a zserio .zs file. Must be either a top-
+                            level entrypoint (e.g. all.zs), or a subpackage
+                            (e.g. services/myservice.zs) in conjunction with
+                            a "--zserio-source-root|-r <dir>" argument.
+                        (B) Path to parent dir of a zserio Python package.
+                        
+                        Examples:
+                            -i path/to/schema/main.zs         (A)
+                            -i path/to/python/package/parent  (B) 
+                        """))
+    parser.add_argument("-r", "--zserio-source-root", nargs=1, metavar="zserio-src-root-dir",
+                        required=False, help=argdoc("""
+                        When -i specifies a zs file (Option A), indicate the
+                        directory for the zserio -src directory argument. If
+                        not specified, the parent directory of the zs file
+                        will be used.
+                        """))
+    parser.add_argument("-p", "--package", nargs=1, metavar="top-level-package",
+                        required=False, help=argdoc("""
+                        When -i specifies a zs file (Option A), indicate
+                        that a specific top-level zserio package name
+                        should be used.
+                        
+                        Examples:
+                            -p zserio_pkg_name
+                        """))
+    parser.add_argument("-c", "--config", nargs="+", metavar="tags",
+                        action="append", help=argdoc("""
+                        Configuration tags for a specific or all methods.
+                        The argument syntax follows this pattern:
+                            
+                           [(service-method-name):](comma-separated-tags)
+                            
+                        Note: The -c argument may be applied multiple times.
+                        The `comma-separated-tags` must be a list of tags
+                        which indicate OpenApi method generator preferences.
+                        The following tags are supported:
+                        
+                        get|put|post|delete : HTTP method tags
+                                query|path| : Parameter location tags
+                                header|body 
+                                  flat|blob : Flatten request object,
+                                              or pass it as whole blob.
+                          (param-specifier) : Specify parameter name, format
+                                              and location for a specific
+                                              request-part. See below.
+                            security=(name) : Set a particular security
+                                              scheme to be used. The scheme
+                                              details must be provided through
+                                              the --base-config-yaml.
+                         path=(method-path) : Set a particular method path.
+                                              May contain placeholders for
+                                              path params.
+                                                   
+                        A (param-specifier) tag has the following schema:
+                        
+                            (field?name=...
+                                  &in=[path|body|query|header]
+                                  &format=[binary|base64|hex]
+                                  [&style=...]
+                                  [&explode=...])
+                        
+                        Examples:
+                        
+                          Expose all methods as POST, but `getLayerByTileId`
+                          as GET with flat path-parameters:
+                          
+                            `-c post getLayerByTileId:get,flat,path`
+                            
+                          For myMethod, put the whole request blob into the a
+                          query "data" parameter as base64:
+                          
+                            `-c myMethod:*?name=data&in=query&format=base64`
+                            
+                          For myMethod, set the "AwesomeAuth" auth scheme:
+                          
+                            `-c myMethod:security=AwesomeAuth`
+                            
+                          For myMethod, provide the path and place myField
+                          explicitely in a path placeholder:
+                          
+                            `-c 'myMethod:path=/my-method/{param},...
+                                 myField?name=param&in=path&format=string'`
+                            
+                        Note:
+                            * The HTTP-method defaults to `post`.
+                            * The parameter 'in' defaults to `query` for
+                              `get`, `body` otherwise.
+                            * If a method uses a parameter specifier, the
+                              `flat`, `body`, `query`, `path`, `header` and
+                              `body`-tags are ignored.
+                            * The `flat` tag is only meaningful in conjunction
+                              with `query` or `path`.
+                            * An unspecific tag list (no service-method-name)
+                              affects the defaults only for following, not
+                              preceding specialized tag assignments.
+                        """))
+    parser.add_argument("-o", "--output", nargs=1, type=FileType("w"), default=[sys.stdout],
+                        metavar="output", help=argdoc("""
+                        Output file path. If not specified, the output will be
+                        written to stdout.
+                        """))
+    parser.add_argument("-b", "--base-config-yaml", nargs=1, type=FileType("r"), required=False, default=[None],
+                        help=argdoc("""
+                        Base configuration file. Can be used to fully or partially
+                        substitute --config arguments, and to provide additional
+                        OpenAPI information. The YAML file must look like this:
+                        
+                          method: # Optional method tags dictionary
+                            <method-name|*>: <list of config tags>
+                          securitySchemes: ... # Optional OpenAPI securitySchemes
+                          info: ...            # Optional OpenAPI info section
+                          servers: ...         # Optional OpenAPI servers section
+                          security: ...        # Optional OpenAPI global security
+                        """))
+
+    args = parser.parse_args(sys.argv[1:])
+    try:
+        OpenApiSchemaGenerator(
+            service=args.service[0],
+            path=args.input[0] if args.input else None,
+            package=args.package[0] if args.package else None,
+            config=[arg for args in args.config for arg in args] if args.config else [],
+            output=args.output[0],
+            base_config=args.base_config_yaml[0] if args.base_config_yaml else None,
+            zserio_src_root=args.zserio_source_root[0] if args.zserio_source_root else None).generate()
+    except OpenApiGenError as e:
+        print(f"[ERROR] {e}")
+        exit(1)
```

## zswag/reflect.py

 * *Ordering differences only*

```diff
@@ -1,247 +1,247 @@
-import inspect
-import base64
-import zserio
-import struct
-import functools
-from enum import Enum
-from typing import Type, Tuple, Any, Dict, Union, Optional, List, get_type_hints, Iterator
-from pyzswagcl import OAMethod, OAParam, OAParamFormat, ZSERIO_REQUEST_PART_WHOLE
-from re import compile as re
-from zserio.typeinfo import TypeInfo, MemberInfo, TypeAttribute, MemberAttribute
-
-NONE_T = type(None)
-SCALAR_T = (bool, int, float, str)
-TYPE_INFO_CACHE = {}
-
-
-class NotInstantiableReason(RuntimeError):
-    def __init__(self, member_name: str, member_type: str, method_name: str = ""):
-        super(NotInstantiableReason, self).__init__("\n" + inspect.cleandoc(f"""
-        WARNING: Generating method `{method_name or 'unknown'}`:
-        ----------------------------{"-"*len(method_name or 'unknown')}--
-        
-            The request must be passed as a blob, since the
-            member `{member_name}` has non-flattable type
-            `{member_type}`.
-            
-            Please add the following argument to zswag.gen,
-            and remove any default parameter specifiers which
-            might affect the configuration of `method_name`:
-                
-                -c {method_name}:blob
-        """))
-        self.member_name = member_name
-        self.member_type = member_type
-
-
-# Table here: https://docs.python.org/3/library/struct.html#format-characters
-C_STRUCT_LITERAL_PER_TYPE_AND_SIZE: Dict[Tuple[Any, int], str] = {
-    (bool, 1): "!b",
-    (bool, 2): "!h",
-    (bool, 4): "!i",
-    (bool, 8): "!q",
-    (int, 1): "!b",
-    (int, 2): "!h",
-    (int, 4): "!i",
-    (int, 8): "!q",
-    (float, 4): "!f",
-    (float, 8): "!d",
-}
-
-
-# Recursive setattr function, adopted from SO:
-#  https://stackoverflow.com/questions/31174295/getattr-and-setattr-on-nested-subobjects-chained-properties
-def rsetattr(obj, attr, val):
-    pre, _, post = attr.rpartition('.')
-    return setattr(rgetattr(obj, pre) if pre else obj, post, val)
-
-
-# Recursive getattr function, adopted from SO:
-#  https://stackoverflow.com/questions/31174295/getattr-and-setattr-on-nested-subobjects-chained-properties
-def rgetattr(obj, attr):
-    def _getattr(obj, attr):
-        if not hasattr(obj, attr):
-            raise RuntimeError(
-                f"\nERROR: `{attr}` does not exist not in {obj.__name__}; choices are ..." +
-                "".join("\n  * "+choice for choice in dir(obj) if not choice.startswith("__")))
-        return getattr(obj, attr)
-    return functools.reduce(_getattr, [obj] + attr.split('.'))
-
-
-# Get the request type for a zserio service method.
-def service_method_request_type(service_instance: Any, method_name: str) -> Any:
-    zserio_impl_function = getattr(service_instance, f"_{to_snake(method_name)}_impl")
-    result = get_type_hints(zserio_impl_function)["request"]
-    assert inspect.isclass(result)
-    return result
-
-
-# Adopted from zserio PythonSymbolConverter
-def to_snake(s: str, patterns=(re("([a-z])([A-Z])"), re("([0-9A-Z])([A-Z][a-z])"))):
-    for p in patterns:
-        s = p.sub(r"\1_\2", s)
-    return s.lower()
-
-
-# Returns true if t is atomic (not a compound struct),
-# false otherwise.
-def is_scalar(t: TypeInfo):
-    return t.py_type in SCALAR_T or issubclass(t.py_type, Enum)
-
-
-# Retrieve zserio type info for a schema class -
-# result is cached for maximum performance.
-def cached_type_info(zserio_t) -> Optional[TypeInfo]:
-    if not hasattr(zserio_t, "type_info"):
-        return None
-    key = f"{zserio_t.__module__}.{zserio_t.__qualname__}"
-    if key not in TYPE_INFO_CACHE:
-        TYPE_INFO_CACHE[key] = zserio_t.type_info()
-    return TYPE_INFO_CACHE[key]
-
-
-# Recursively find a member info (e.g. "myField1.myField2") in
-# a TypeInfo. Member names may be pythonic. The input field path
-# must be with original (not necessarily pythonic) schema field
-# names. The first output tuple entry is the pythonic conversion
-# ("my_field_1.my_field_2").
-def find_field(t: TypeInfo, field: str, offset: int = 0, py_path="") -> Tuple[str, Optional[MemberInfo]]:
-    next_dot = field.find(".", offset)
-    subfield = field[offset:next_dot] if next_dot >= 0 else field[offset:]
-    for _, member_info in members(t):
-        if member_info.schema_name == subfield:
-            if offset > 0:
-                py_path += "."
-            py_path += member_info.attributes[MemberAttribute.PROPERTY_NAME]
-            if next_dot < 0:
-                return py_path, member_info
-            return find_field(member_info.type_info, field, next_dot+1, py_path)
-    return "", None
-
-
-# Simply yields all MemberInfo for a TypeInfo.
-def members(t: TypeInfo, recursive=False, field_prefix="") -> Iterator[MemberInfo]:
-    if TypeAttribute.FIELDS in t.attributes:
-        for member in t.attributes[TypeAttribute.FIELDS]:
-            field_name = field_prefix+"." if field_prefix else ""
-            field_name += member.schema_name
-            yield field_name, member
-            if recursive:
-                yield from members(member.type_info, recursive, field_name)
-
-
-# Checks whether is a type is not trivially constructable:
-# It (or a subtype) might take extra parameters, or be
-# an array of non-scalar types.
-def check_uninstantiable(t: TypeInfo, field_name="", recursive=False) -> Optional[NotInstantiableReason]:
-    if TypeAttribute.PARAMETERS in t.attributes and t.attributes[TypeAttribute.PARAMETERS]:
-        return NotInstantiableReason(field_name, t.schema_name)
-    member_info: MemberInfo
-    for _, member_info in members(t):
-        subfield_name = f"{field_name}.{member_info.schema_name}" if field_name else member_info.schema_name
-        if MemberAttribute.ARRAY_LENGTH in member_info.attributes and not is_scalar(member_info.type_info):
-            return NotInstantiableReason(subfield_name, t.schema_name+"[]")
-        if recursive:
-            if reason := check_uninstantiable(member_info.type_info, subfield_name, recursive):
-                return reason
-
-
-# Returns a fully recursively initialized class instance
-# of a zserio schema type, if possible.
-def instantiate(t: Type) -> Any:
-    result_instance = t()
-    type_info = cached_type_info(t)
-    if reason := check_uninstantiable(type_info):
-        raise reason
-    for _, member_info in members(type_info):
-        field_name: str = member_info.attributes[MemberAttribute.PROPERTY_NAME]
-        member_type_info = member_info.type_info
-        if not is_scalar(member_type_info):
-            compound_field_value = instantiate(member_type_info.py_type)
-            setattr(result_instance, f"_{field_name}_", compound_field_value)
-    return result_instance
-
-
-# Get a byte buffer from a string which is encoded in a given format
-def str_to_bytes(s: str, fmt: OAParamFormat) -> bytes:
-    if fmt == OAParamFormat.BASE64:
-        return base64.b64decode(s)
-    elif fmt == OAParamFormat.BASE64URL:
-        return base64.urlsafe_b64decode(s)
-    elif fmt == OAParamFormat.HEX:
-        return bytes.fromhex(s)
-    else:  # if fmt in (OAParamFormat.BINARY, OAParamFormat.STRING):
-        return bytes(s, encoding="raw_unicode_escape")
-
-
-# Convert a single passed parameter value to it's correct type
-def parse_param_value(param: OAParam, target_type: Type, value: str) -> Any:
-    # Check if its an enum ...
-    if issubclass(target_type, Enum):
-        return target_type(parse_param_value(param, int, value))
-    # Check if the parameter format is native string conversion
-    if param.format == OAParamFormat.STRING:
-        if target_type is bool:
-            return bool(int(value))
-        return target_type(value)
-    # Is it hex-to-int conversion?
-    if param.format == OAParamFormat.HEX and target_type is int:
-        return int(value, 16)
-    # It is some kind of blob conversion!
-    value_as_bytes = str_to_bytes(value, param.format)
-    # Is it a serialized C type (char/uchar/float/double/long...)?
-    struct_literal_key = (target_type, len(value_as_bytes))
-    if struct_literal_key in C_STRUCT_LITERAL_PER_TYPE_AND_SIZE:
-        return target_type(struct.unpack(
-            C_STRUCT_LITERAL_PER_TYPE_AND_SIZE[struct_literal_key],
-            value_as_bytes)[0])
-    # Is it a string blob?
-    if target_type is str:
-        return str(value_as_bytes, 'utf-8')
-    raise RuntimeError(f"Cannot convert {len(value_as_bytes)} to {target_type}")
-
-
-# Convert an array of passed parameter values to their correct type
-def parse_param_values(param: OAParam, target_type: Type, value: List[str]) -> List[Any]:
-    return [parse_param_value(param, target_type, item) for item in value]
-
-
-# Get a blob for a zserio request type, a set of request parameter values
-# and an OpenAPI method path spec.
-def request_object_blob(*, req_t: Type, headers: Dict[str, Any], spec: OAMethod, **kwargs) -> bytes:
-    # Lazy instantiation of request object and type info
-    req: Optional[req_t] = None
-    req_t_info = cached_type_info(req_t)
-    # Apply parameters
-    param_name: str
-    param: OAParam
-    for param_name, param in spec.parameters.items():
-        # Get raw string value
-        value: Union[str, List[str]] = param.default_value
-        param_name = param_name.replace("-", "_")
-        if param_name in kwargs:
-            value = kwargs[param_name]
-        else:
-            if param_name in headers:
-                value = headers[param_name]
-        # Convert string value to whole blob
-        if param.field == ZSERIO_REQUEST_PART_WHOLE:
-            return str_to_bytes(value, param.format)
-        # First non-whole request parameter: Synthetic request object
-        if not req:
-            req = instantiate(req_t)
-        # Convert string value to correct type
-        pythonic_field_path, target_type = find_field(req_t_info, param.field)
-        if not target_type:
-            raise RuntimeError(f"Could not find field {param.field}!")
-        if MemberAttribute.ARRAY_LENGTH in target_type.attributes:
-            converted_value = parse_param_values(param, target_type.type_info.py_type, value)
-        else:
-            converted_value = parse_param_value(param, target_type.type_info.py_type, value)
-        # Apply value to request object field
-        rsetattr(req, pythonic_field_path, converted_value)
-    # Serialise request object. Assert at least one parameter given.
-    assert req
-    serializer = zserio.BitStreamWriter()
-    req.write(serializer)
-    return serializer.byte_array
+import inspect
+import base64
+import zserio
+import struct
+import functools
+from enum import Enum
+from typing import Type, Tuple, Any, Dict, Union, Optional, List, get_type_hints, Iterator
+from pyzswagcl import OAMethod, OAParam, OAParamFormat, ZSERIO_REQUEST_PART_WHOLE
+from re import compile as re
+from zserio.typeinfo import TypeInfo, MemberInfo, TypeAttribute, MemberAttribute
+
+NONE_T = type(None)
+SCALAR_T = (bool, int, float, str)
+TYPE_INFO_CACHE = {}
+
+
+class NotInstantiableReason(RuntimeError):
+    def __init__(self, member_name: str, member_type: str, method_name: str = ""):
+        super(NotInstantiableReason, self).__init__("\n" + inspect.cleandoc(f"""
+        WARNING: Generating method `{method_name or 'unknown'}`:
+        ----------------------------{"-"*len(method_name or 'unknown')}--
+        
+            The request must be passed as a blob, since the
+            member `{member_name}` has non-flattable type
+            `{member_type}`.
+            
+            Please add the following argument to zswag.gen,
+            and remove any default parameter specifiers which
+            might affect the configuration of `method_name`:
+                
+                -c {method_name}:blob
+        """))
+        self.member_name = member_name
+        self.member_type = member_type
+
+
+# Table here: https://docs.python.org/3/library/struct.html#format-characters
+C_STRUCT_LITERAL_PER_TYPE_AND_SIZE: Dict[Tuple[Any, int], str] = {
+    (bool, 1): "!b",
+    (bool, 2): "!h",
+    (bool, 4): "!i",
+    (bool, 8): "!q",
+    (int, 1): "!b",
+    (int, 2): "!h",
+    (int, 4): "!i",
+    (int, 8): "!q",
+    (float, 4): "!f",
+    (float, 8): "!d",
+}
+
+
+# Recursive setattr function, adopted from SO:
+#  https://stackoverflow.com/questions/31174295/getattr-and-setattr-on-nested-subobjects-chained-properties
+def rsetattr(obj, attr, val):
+    pre, _, post = attr.rpartition('.')
+    return setattr(rgetattr(obj, pre) if pre else obj, post, val)
+
+
+# Recursive getattr function, adopted from SO:
+#  https://stackoverflow.com/questions/31174295/getattr-and-setattr-on-nested-subobjects-chained-properties
+def rgetattr(obj, attr):
+    def _getattr(obj, attr):
+        if not hasattr(obj, attr):
+            raise RuntimeError(
+                f"\nERROR: `{attr}` does not exist not in {obj.__name__}; choices are ..." +
+                "".join("\n  * "+choice for choice in dir(obj) if not choice.startswith("__")))
+        return getattr(obj, attr)
+    return functools.reduce(_getattr, [obj] + attr.split('.'))
+
+
+# Get the request type for a zserio service method.
+def service_method_request_type(service_instance: Any, method_name: str) -> Any:
+    zserio_impl_function = getattr(service_instance, f"_{to_snake(method_name)}_impl")
+    result = get_type_hints(zserio_impl_function)["request"]
+    assert inspect.isclass(result)
+    return result
+
+
+# Adopted from zserio PythonSymbolConverter
+def to_snake(s: str, patterns=(re("([a-z])([A-Z])"), re("([0-9A-Z])([A-Z][a-z])"))):
+    for p in patterns:
+        s = p.sub(r"\1_\2", s)
+    return s.lower()
+
+
+# Returns true if t is atomic (not a compound struct),
+# false otherwise.
+def is_scalar(t: TypeInfo):
+    return t.py_type in SCALAR_T or issubclass(t.py_type, Enum)
+
+
+# Retrieve zserio type info for a schema class -
+# result is cached for maximum performance.
+def cached_type_info(zserio_t) -> Optional[TypeInfo]:
+    if not hasattr(zserio_t, "type_info"):
+        return None
+    key = f"{zserio_t.__module__}.{zserio_t.__qualname__}"
+    if key not in TYPE_INFO_CACHE:
+        TYPE_INFO_CACHE[key] = zserio_t.type_info()
+    return TYPE_INFO_CACHE[key]
+
+
+# Recursively find a member info (e.g. "myField1.myField2") in
+# a TypeInfo. Member names may be pythonic. The input field path
+# must be with original (not necessarily pythonic) schema field
+# names. The first output tuple entry is the pythonic conversion
+# ("my_field_1.my_field_2").
+def find_field(t: TypeInfo, field: str, offset: int = 0, py_path="") -> Tuple[str, Optional[MemberInfo]]:
+    next_dot = field.find(".", offset)
+    subfield = field[offset:next_dot] if next_dot >= 0 else field[offset:]
+    for _, member_info in members(t):
+        if member_info.schema_name == subfield:
+            if offset > 0:
+                py_path += "."
+            py_path += member_info.attributes[MemberAttribute.PROPERTY_NAME]
+            if next_dot < 0:
+                return py_path, member_info
+            return find_field(member_info.type_info, field, next_dot+1, py_path)
+    return "", None
+
+
+# Simply yields all MemberInfo for a TypeInfo.
+def members(t: TypeInfo, recursive=False, field_prefix="") -> Iterator[MemberInfo]:
+    if TypeAttribute.FIELDS in t.attributes:
+        for member in t.attributes[TypeAttribute.FIELDS]:
+            field_name = field_prefix+"." if field_prefix else ""
+            field_name += member.schema_name
+            yield field_name, member
+            if recursive:
+                yield from members(member.type_info, recursive, field_name)
+
+
+# Checks whether is a type is not trivially constructable:
+# It (or a subtype) might take extra parameters, or be
+# an array of non-scalar types.
+def check_uninstantiable(t: TypeInfo, field_name="", recursive=False) -> Optional[NotInstantiableReason]:
+    if TypeAttribute.PARAMETERS in t.attributes and t.attributes[TypeAttribute.PARAMETERS]:
+        return NotInstantiableReason(field_name, t.schema_name)
+    member_info: MemberInfo
+    for _, member_info in members(t):
+        subfield_name = f"{field_name}.{member_info.schema_name}" if field_name else member_info.schema_name
+        if MemberAttribute.ARRAY_LENGTH in member_info.attributes and not is_scalar(member_info.type_info):
+            return NotInstantiableReason(subfield_name, t.schema_name+"[]")
+        if recursive:
+            if reason := check_uninstantiable(member_info.type_info, subfield_name, recursive):
+                return reason
+
+
+# Returns a fully recursively initialized class instance
+# of a zserio schema type, if possible.
+def instantiate(t: Type) -> Any:
+    result_instance = t()
+    type_info = cached_type_info(t)
+    if reason := check_uninstantiable(type_info):
+        raise reason
+    for _, member_info in members(type_info):
+        field_name: str = member_info.attributes[MemberAttribute.PROPERTY_NAME]
+        member_type_info = member_info.type_info
+        if not is_scalar(member_type_info):
+            compound_field_value = instantiate(member_type_info.py_type)
+            setattr(result_instance, f"_{field_name}_", compound_field_value)
+    return result_instance
+
+
+# Get a byte buffer from a string which is encoded in a given format
+def str_to_bytes(s: str, fmt: OAParamFormat) -> bytes:
+    if fmt == OAParamFormat.BASE64:
+        return base64.b64decode(s)
+    elif fmt == OAParamFormat.BASE64URL:
+        return base64.urlsafe_b64decode(s)
+    elif fmt == OAParamFormat.HEX:
+        return bytes.fromhex(s)
+    else:  # if fmt in (OAParamFormat.BINARY, OAParamFormat.STRING):
+        return bytes(s, encoding="raw_unicode_escape")
+
+
+# Convert a single passed parameter value to it's correct type
+def parse_param_value(param: OAParam, target_type: Type, value: str) -> Any:
+    # Check if its an enum ...
+    if issubclass(target_type, Enum):
+        return target_type(parse_param_value(param, int, value))
+    # Check if the parameter format is native string conversion
+    if param.format == OAParamFormat.STRING:
+        if target_type is bool:
+            return bool(int(value))
+        return target_type(value)
+    # Is it hex-to-int conversion?
+    if param.format == OAParamFormat.HEX and target_type is int:
+        return int(value, 16)
+    # It is some kind of blob conversion!
+    value_as_bytes = str_to_bytes(value, param.format)
+    # Is it a serialized C type (char/uchar/float/double/long...)?
+    struct_literal_key = (target_type, len(value_as_bytes))
+    if struct_literal_key in C_STRUCT_LITERAL_PER_TYPE_AND_SIZE:
+        return target_type(struct.unpack(
+            C_STRUCT_LITERAL_PER_TYPE_AND_SIZE[struct_literal_key],
+            value_as_bytes)[0])
+    # Is it a string blob?
+    if target_type is str:
+        return str(value_as_bytes, 'utf-8')
+    raise RuntimeError(f"Cannot convert {len(value_as_bytes)} to {target_type}")
+
+
+# Convert an array of passed parameter values to their correct type
+def parse_param_values(param: OAParam, target_type: Type, value: List[str]) -> List[Any]:
+    return [parse_param_value(param, target_type, item) for item in value]
+
+
+# Get a blob for a zserio request type, a set of request parameter values
+# and an OpenAPI method path spec.
+def request_object_blob(*, req_t: Type, headers: Dict[str, Any], spec: OAMethod, **kwargs) -> bytes:
+    # Lazy instantiation of request object and type info
+    req: Optional[req_t] = None
+    req_t_info = cached_type_info(req_t)
+    # Apply parameters
+    param_name: str
+    param: OAParam
+    for param_name, param in spec.parameters.items():
+        # Get raw string value
+        value: Union[str, List[str]] = param.default_value
+        param_name = param_name.replace("-", "_")
+        if param_name in kwargs:
+            value = kwargs[param_name]
+        else:
+            if param_name in headers:
+                value = headers[param_name]
+        # Convert string value to whole blob
+        if param.field == ZSERIO_REQUEST_PART_WHOLE:
+            return str_to_bytes(value, param.format)
+        # First non-whole request parameter: Synthetic request object
+        if not req:
+            req = instantiate(req_t)
+        # Convert string value to correct type
+        pythonic_field_path, target_type = find_field(req_t_info, param.field)
+        if not target_type:
+            raise RuntimeError(f"Could not find field {param.field}!")
+        if MemberAttribute.ARRAY_LENGTH in target_type.attributes:
+            converted_value = parse_param_values(param, target_type.type_info.py_type, value)
+        else:
+            converted_value = parse_param_value(param, target_type.type_info.py_type, value)
+        # Apply value to request object field
+        rsetattr(req, pythonic_field_path, converted_value)
+    # Serialise request object. Assert at least one parameter given.
+    assert req
+    serializer = zserio.BitStreamWriter()
+    req.write(serializer)
+    return serializer.byte_array
```

## zswag/test/calc/__init__.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-import zserio
-from os.path import dirname, abspath
-
-working_dir = dirname(abspath(__file__))
-zserio.generate(
-    zs_dir=working_dir,
-    main_zs_file="calculator.zs",
-    gen_dir=working_dir,
-    extra_args=["-withTypeInfoCode"])
+import zserio
+from os.path import dirname, abspath
+
+working_dir = dirname(abspath(__file__))
+zserio.generate(
+    zs_dir=working_dir,
+    main_zs_file="calculator.zs",
+    gen_dir=working_dir,
+    extra_args=["-withTypeInfoCode"])
```

## zswag/test/calc/__main__.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-import zswag
-import sys
-
-from zswag.test.calc import working_dir
-import zswag.test.calc.client as client
-import zswag.test.calc.server as server
-import calculator.api as calculator
-
-mode = sys.argv[1] if len(sys.argv) > 1 else ""
-host, port = sys.argv[2].split(':') if len(sys.argv) > 2 and ':' in sys.argv[2] else ("localhost", 5000)
-
-if mode == "client":
-    client.run(host, port)
-elif mode == "server":
-    app = zswag.OAServer(
-        controller_module=server,
-        service_type=calculator.Calculator.Service,
-        yaml_path=working_dir+"/api.yaml",
-        zs_pkg_path=working_dir)
-    app.run(host=host, port=port)
-elif mode == "path":
-    print(working_dir)
-else:
-    print("Usage: python3 -m calc {server|client} [host:port]")
+import zswag
+import sys
+
+from zswag.test.calc import working_dir
+import zswag.test.calc.client as client
+import zswag.test.calc.server as server
+import calculator.api as calculator
+
+mode = sys.argv[1] if len(sys.argv) > 1 else ""
+host, port = sys.argv[2].split(':') if len(sys.argv) > 2 and ':' in sys.argv[2] else ("localhost", 5000)
+
+if mode == "client":
+    client.run(host, port)
+elif mode == "server":
+    app = zswag.OAServer(
+        controller_module=server,
+        service_type=calculator.Calculator.Service,
+        yaml_path=working_dir+"/api.yaml",
+        zs_pkg_path=working_dir)
+    app.run(host=host, port=port)
+elif mode == "path":
+    print(working_dir)
+else:
+    print("Usage: python3 -m calc {server|client} [host:port]")
```

## zswag/test/calc/api.yaml

 * *Ordering differences only*

```diff
@@ -1,276 +1,276 @@
-components:
-  securitySchemes:
-    BasicAuth:
-      scheme: basic
-      type: http
-      x-basicInfoFunc: zswag.test.calc.server.validate_basic_auth
-    BearerAuth:
-      scheme: bearer
-      type: http
-      x-bearerInfoFunc: zswag.test.calc.server.validate_bearer
-    CookieAuth:
-      in: cookie
-      name: api-cookie
-      type: apiKey
-      x-apikeyInfoFunc: zswag.test.calc.server.validate_apikey
-    HeaderAuth:
-      in: header
-      name: X-Generic-Token
-      type: apiKey
-      x-apikeyInfoFunc: zswag.test.calc.server.validate_apikey
-    QueryAuth:
-      in: query
-      name: api-key
-      type: apiKey
-      x-apikeyInfoFunc: zswag.test.calc.server.validate_apikey
-info:
-  contact:
-    email: support@nds-association.org
-  description: REST API for calculator.Calculator
-  license:
-    name: My-Fancy-License
-  title: Calculator
-  version: 1.0.0
-openapi: 3.0.0
-paths:
-  /bmul:
-    get:
-      description: ''
-      operationId: bitMul
-      parameters:
-        - allowEmptyValue: true
-          description: ''
-          in: query
-          name: values
-          required: true
-          schema:
-            format: string
-            items:
-              type: string
-            type: array
-          x-zserio-request-part: values
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - HeaderAuth: []
-      summary: ''
-  /bsum/{values}:
-    get:
-      description: ''
-      operationId: byteSum
-      parameters:
-        - description: ''
-          in: path
-          name: values
-          required: true
-          schema:
-            format: base64url
-            items:
-              type: string
-            type: array
-          x-zserio-request-part: values
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - BasicAuth: []
-      summary: ''
-  /concat:
-    get:
-      description: ''
-      operationId: concat
-      parameters:
-        - allowEmptyValue: true
-          description: ''
-          in: query
-          name: values
-          required: true
-          schema:
-            format: base64
-            items:
-              type: string
-            type: array
-          x-zserio-request-part: values
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - BearerAuth: []
-      summary: ''
-  /fmul:
-    get:
-      description: ''
-      operationId: floatMul
-      parameters:
-        - allowEmptyValue: true
-          description: ''
-          explode: false
-          in: query
-          name: values
-          required: true
-          schema:
-            format: string
-            items:
-              type: string
-            type: array
-          x-zserio-request-part: values
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - CookieAuth: []
-      summary: ''
-  /identity:
-    post:
-      description: ''
-      operationId: identity
-      parameters: []
-      requestBody:
-        content:
-          application/x-zserio-object:
-            schema:
-              type: string
-        description: ''
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - CookieAuth: []
-      summary: ''
-  /imul/{values}:
-    get:
-      description: ''
-      operationId: intMul
-      parameters:
-        - description: ''
-          in: path
-          name: values
-          required: true
-          schema:
-            format: base64
-            items:
-              type: string
-            type: array
-          style: simple
-          x-zserio-request-part: values
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - QueryAuth: []
-      summary: ''
-  /isum:
-    get:
-      description: ''
-      operationId: intSum
-      parameters:
-        - allowEmptyValue: true
-          description: ''
-          explode: true
-          in: query
-          name: values
-          required: true
-          schema:
-            format: hex
-            items:
-              type: string
-            type: array
-          x-zserio-request-part: values
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security:
-        - BearerAuth: []
-      summary: ''
-  /name/{enum_value}:
-    get:
-      description: ''
-      operationId: name
-      parameters:
-        - description: ''
-          in: path
-          name: enum_value
-          required: true
-          schema:
-            format: string
-            type: string
-          x-zserio-request-part: value
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      summary: ''
-  /power/{base}:
-    get:
-      description: ''
-      operationId: power
-      parameters:
-        - description: ''
-          in: path
-          name: base
-          required: true
-          schema:
-            format: string
-            type: string
-          x-zserio-request-part: base.value
-        - description: ''
-          in: header
-          name: X-Ponent
-          required: true
-          schema:
-            format: string
-            type: string
-          x-zserio-request-part: exponent.value
-      responses:
-        '200':
-          content:
-            application/x-zserio-object:
-              schema:
-                format: binary
-                type: string
-          description: ''
-      security: []
-      summary: ''
-security:
-  - HeaderAuth: []
-servers: []
+components:
+  securitySchemes:
+    BasicAuth:
+      scheme: basic
+      type: http
+      x-basicInfoFunc: zswag.test.calc.server.validate_basic_auth
+    BearerAuth:
+      scheme: bearer
+      type: http
+      x-bearerInfoFunc: zswag.test.calc.server.validate_bearer
+    CookieAuth:
+      in: cookie
+      name: api-cookie
+      type: apiKey
+      x-apikeyInfoFunc: zswag.test.calc.server.validate_apikey
+    HeaderAuth:
+      in: header
+      name: X-Generic-Token
+      type: apiKey
+      x-apikeyInfoFunc: zswag.test.calc.server.validate_apikey
+    QueryAuth:
+      in: query
+      name: api-key
+      type: apiKey
+      x-apikeyInfoFunc: zswag.test.calc.server.validate_apikey
+info:
+  contact:
+    email: support@nds-association.org
+  description: REST API for calculator.Calculator
+  license:
+    name: My-Fancy-License
+  title: Calculator
+  version: 1.0.0
+openapi: 3.0.0
+paths:
+  /bmul:
+    get:
+      description: ''
+      operationId: bitMul
+      parameters:
+        - allowEmptyValue: true
+          description: ''
+          in: query
+          name: values
+          required: true
+          schema:
+            format: string
+            items:
+              type: string
+            type: array
+          x-zserio-request-part: values
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - HeaderAuth: []
+      summary: ''
+  /bsum/{values}:
+    get:
+      description: ''
+      operationId: byteSum
+      parameters:
+        - description: ''
+          in: path
+          name: values
+          required: true
+          schema:
+            format: base64url
+            items:
+              type: string
+            type: array
+          x-zserio-request-part: values
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - BasicAuth: []
+      summary: ''
+  /concat:
+    get:
+      description: ''
+      operationId: concat
+      parameters:
+        - allowEmptyValue: true
+          description: ''
+          in: query
+          name: values
+          required: true
+          schema:
+            format: base64
+            items:
+              type: string
+            type: array
+          x-zserio-request-part: values
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - BearerAuth: []
+      summary: ''
+  /fmul:
+    get:
+      description: ''
+      operationId: floatMul
+      parameters:
+        - allowEmptyValue: true
+          description: ''
+          explode: false
+          in: query
+          name: values
+          required: true
+          schema:
+            format: string
+            items:
+              type: string
+            type: array
+          x-zserio-request-part: values
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - CookieAuth: []
+      summary: ''
+  /identity:
+    post:
+      description: ''
+      operationId: identity
+      parameters: []
+      requestBody:
+        content:
+          application/x-zserio-object:
+            schema:
+              type: string
+        description: ''
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - CookieAuth: []
+      summary: ''
+  /imul/{values}:
+    get:
+      description: ''
+      operationId: intMul
+      parameters:
+        - description: ''
+          in: path
+          name: values
+          required: true
+          schema:
+            format: base64
+            items:
+              type: string
+            type: array
+          style: simple
+          x-zserio-request-part: values
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - QueryAuth: []
+      summary: ''
+  /isum:
+    get:
+      description: ''
+      operationId: intSum
+      parameters:
+        - allowEmptyValue: true
+          description: ''
+          explode: true
+          in: query
+          name: values
+          required: true
+          schema:
+            format: hex
+            items:
+              type: string
+            type: array
+          x-zserio-request-part: values
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security:
+        - BearerAuth: []
+      summary: ''
+  /name/{enum_value}:
+    get:
+      description: ''
+      operationId: name
+      parameters:
+        - description: ''
+          in: path
+          name: enum_value
+          required: true
+          schema:
+            format: string
+            type: string
+          x-zserio-request-part: value
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      summary: ''
+  /power/{base}:
+    get:
+      description: ''
+      operationId: power
+      parameters:
+        - description: ''
+          in: path
+          name: base
+          required: true
+          schema:
+            format: string
+            type: string
+          x-zserio-request-part: base.value
+        - description: ''
+          in: header
+          name: X-Ponent
+          required: true
+          schema:
+            format: string
+            type: string
+          x-zserio-request-part: exponent.value
+      responses:
+        '200':
+          content:
+            application/x-zserio-object:
+              schema:
+                format: binary
+                type: string
+          description: ''
+      security: []
+      summary: ''
+security:
+  - HeaderAuth: []
+servers: []
```

## zswag/test/calc/calculator.zs

 * *Ordering differences only*

```diff
@@ -1,103 +1,103 @@
-package calculator;
-
-/*!
-
-### This type has documentation
-
-!*/
-
-struct I32
-{
-    int32 value;
-};
-
-struct Double
-{
-    float64 value;
-};
-
-struct Bool
-{
-    bool value;
-};
-
-struct String
-{
-    string value;
-};
-
-struct BaseAndExponent
-{
-    I32 base;
-    I32 exponent;
-    int32 unused1;
-    string unused2;
-    float32 unused3;
-    bool unused5[];
-};
-
-struct Integers
-{
-    int32 values[];
-};
-
-struct Bytes
-{
-    uint8 values[];
-};
-
-struct Strings
-{
-    string values[];
-};
-
-struct Doubles
-{
-    float64 values[];
-};
-
-struct Bools
-{
-    bool values[];
-};
-
-enum int32 Enum
-{
-    TEST_ENUM_0 = 42,
-    TEST_ENUM_1 = 1,
-    TEST_ENUM_2 = 2
-};
-
-struct EnumWrapper
-{
-    Enum value;
-};
-
-/*!
-
-### Calculator Service
-
-Check out these sweet docs.
-
-!*/
-
-service Calculator
-{
-    Double power(BaseAndExponent);
-
-    Double intSum(Integers);
-
-    Double byteSum(Bytes);
-
-    Double intMul(Integers);
-
-    Double floatMul(Doubles);
-
-    Bool bitMul(Bools);
-
-    Double identity(Double);
-
-    String concat(Strings);
-
-    String name(EnumWrapper);
-};
+package calculator;
+
+/*!
+
+### This type has documentation
+
+!*/
+
+struct I32
+{
+    int32 value;
+};
+
+struct Double
+{
+    float64 value;
+};
+
+struct Bool
+{
+    bool value;
+};
+
+struct String
+{
+    string value;
+};
+
+struct BaseAndExponent
+{
+    I32 base;
+    I32 exponent;
+    int32 unused1;
+    string unused2;
+    float32 unused3;
+    bool unused5[];
+};
+
+struct Integers
+{
+    int32 values[];
+};
+
+struct Bytes
+{
+    uint8 values[];
+};
+
+struct Strings
+{
+    string values[];
+};
+
+struct Doubles
+{
+    float64 values[];
+};
+
+struct Bools
+{
+    bool values[];
+};
+
+enum int32 Enum
+{
+    TEST_ENUM_0 = 42,
+    TEST_ENUM_1 = 1,
+    TEST_ENUM_2 = 2
+};
+
+struct EnumWrapper
+{
+    Enum value;
+};
+
+/*!
+
+### Calculator Service
+
+Check out these sweet docs.
+
+!*/
+
+service Calculator
+{
+    Double power(BaseAndExponent);
+
+    Double intSum(Integers);
+
+    Double byteSum(Bytes);
+
+    Double intMul(Integers);
+
+    Double floatMul(Doubles);
+
+    Bool bitMul(Bools);
+
+    Double identity(Double);
+
+    String concat(Strings);
+
+    String name(EnumWrapper);
+};
```

## zswag/test/calc/client.py

 * *Ordering differences only*

```diff
@@ -1,132 +1,132 @@
-from enum import Enum
-import calculator.api as api
-from zswag import OAClient, HTTPConfig
-import json
-import pickle
-
-def run(host, port):
-
-    server_url = f"http://{host}:{port}/openapi.json"
-    counter = 0
-    failed = 0
-    print(f"[py-test-client] Connecting to {server_url}", flush=True)
-
-    # Make sure that HTTP Config pickling works
-    config_pickled = pickle.dumps(HTTPConfig().header("x", "42"))
-    assert pickle.loads(config_pickled)
-
-    def run_test(aspect, request, fn, expect, auth_args):
-        nonlocal counter, failed
-        counter += 1
-        try:
-            print(f"[py-test-client] Test#{counter}: {aspect}", flush=True)
-            print(f"[py-test-client]   -> Instantiating client.", flush=True)
-            oa_client = OAClient(f"http://{host}:{port}/openapi.json", **auth_args)
-            # Just make sure that OpenAPI JSON content is parsable
-            assert oa_client.config().content and json.loads(oa_client.config().content)
-            client = api.Calculator.Client(oa_client)
-            print(f"[py-test-client]   -> Running request.", flush=True)
-            resp = fn(client, request)
-            if resp.value == expect:
-                print(f"[py-test-client]   -> Success.", flush=True)
-            else:
-                raise ValueError(f"Expected {expect}, got {resp.value}!")
-        except Exception as e:
-            failed += 1
-            print(f"[py-test-client]   -> ERROR: {str(e) or type(e).__name__}", flush=True)
-
-    run_test(
-        "Pass fields in path and header",
-        api.BaseAndExponent(api.I32(2), api.I32(3)),
-        api.Calculator.Client.power,
-        8.,
-        {})
-
-    run_test(
-        "Pass hex-encoded array in query",
-        api.Integers([100, -200, 400]),
-        api.Calculator.Client.int_sum,
-        300.,
-        {
-            "config": HTTPConfig().header("Authorization", "Bearer 123")
-        })
-
-    run_test(
-        "Pass base64url-encoded byte array in path",
-        api.Bytes([8, 16, 32, 64]),
-        api.Calculator.Client.byte_sum,
-        120.,
-        {
-            "config": HTTPConfig().basic_auth("u", "pw")
-        })
-
-    run_test(
-        "Pass base64-encoded long array in path",
-        api.Integers([1, 2, 3, 4]),
-        api.Calculator.Client.int_mul,
-        24.,
-        {
-            "config": HTTPConfig().query("api-key", "42")
-        })
-
-    run_test(
-        "Pass float array in query.",
-        api.Doubles([34.5, 2.]),
-        api.Calculator.Client.float_mul,
-        69.,
-        {
-            "api_key": "42"
-        })
-
-    run_test(
-        "Pass bool array in query (expect false).",
-        api.Bools([True, False]),
-        api.Calculator.Client.bit_mul,
-        False,
-        {
-            "api_key": "42"
-        })
-
-    run_test(
-        "Pass bool array in query (expect true).",
-        api.Bools([True, True]),
-        api.Calculator.Client.bit_mul,
-        True,
-        {
-            "config": HTTPConfig().header("X-Generic-Token", "42")
-        })
-
-    run_test(
-        "Pass request as blob in body",
-        api.Double(1.),
-        api.Calculator.Client.identity,
-        1.,
-        {
-            "config": HTTPConfig().cookie("api-cookie", "42")
-        })
-
-    run_test(
-        "Pass base64-encoded strings.",
-        api.Strings(["foo", "bar"]),
-        api.Calculator.Client.concat,
-        "foobar",
-        {
-            "bearer": "123"
-        })
-
-    run_test(
-        "Pass enum.",
-        api.EnumWrapper(api.Enum.TEST_ENUM_0),
-        api.Calculator.Client.name,
-        "TEST_ENUM_0",
-        {
-            "config": HTTPConfig().api_key("42")
-        })
-
-    if failed > 0:
-        print(f"[py-test-client] Done, {failed} test(s) failed!", flush=True)
-        exit(1)
-    else:
-        print(f"[py-test-client] All tests succeeded.!", flush=True)
-        exit(0)
-
+from enum import Enum
+import calculator.api as api
+from zswag import OAClient, HTTPConfig
+import json
+import pickle
+
+def run(host, port):
+
+    server_url = f"http://{host}:{port}/openapi.json"
+    counter = 0
+    failed = 0
+    print(f"[py-test-client] Connecting to {server_url}", flush=True)
+
+    # Make sure that HTTP Config pickling works
+    config_pickled = pickle.dumps(HTTPConfig().header("x", "42"))
+    assert pickle.loads(config_pickled)
+
+    def run_test(aspect, request, fn, expect, auth_args):
+        nonlocal counter, failed
+        counter += 1
+        try:
+            print(f"[py-test-client] Test#{counter}: {aspect}", flush=True)
+            print(f"[py-test-client]   -> Instantiating client.", flush=True)
+            oa_client = OAClient(f"http://{host}:{port}/openapi.json", **auth_args)
+            # Just make sure that OpenAPI JSON content is parsable
+            assert oa_client.config().content and json.loads(oa_client.config().content)
+            client = api.Calculator.Client(oa_client)
+            print(f"[py-test-client]   -> Running request.", flush=True)
+            resp = fn(client, request)
+            if resp.value == expect:
+                print(f"[py-test-client]   -> Success.", flush=True)
+            else:
+                raise ValueError(f"Expected {expect}, got {resp.value}!")
+        except Exception as e:
+            failed += 1
+            print(f"[py-test-client]   -> ERROR: {str(e) or type(e).__name__}", flush=True)
+
+    run_test(
+        "Pass fields in path and header",
+        api.BaseAndExponent(api.I32(2), api.I32(3)),
+        api.Calculator.Client.power,
+        8.,
+        {})
+
+    run_test(
+        "Pass hex-encoded array in query",
+        api.Integers([100, -200, 400]),
+        api.Calculator.Client.int_sum,
+        300.,
+        {
+            "config": HTTPConfig().header("Authorization", "Bearer 123")
+        })
+
+    run_test(
+        "Pass base64url-encoded byte array in path",
+        api.Bytes([8, 16, 32, 64]),
+        api.Calculator.Client.byte_sum,
+        120.,
+        {
+            "config": HTTPConfig().basic_auth("u", "pw")
+        })
+
+    run_test(
+        "Pass base64-encoded long array in path",
+        api.Integers([1, 2, 3, 4]),
+        api.Calculator.Client.int_mul,
+        24.,
+        {
+            "config": HTTPConfig().query("api-key", "42")
+        })
+
+    run_test(
+        "Pass float array in query.",
+        api.Doubles([34.5, 2.]),
+        api.Calculator.Client.float_mul,
+        69.,
+        {
+            "api_key": "42"
+        })
+
+    run_test(
+        "Pass bool array in query (expect false).",
+        api.Bools([True, False]),
+        api.Calculator.Client.bit_mul,
+        False,
+        {
+            "api_key": "42"
+        })
+
+    run_test(
+        "Pass bool array in query (expect true).",
+        api.Bools([True, True]),
+        api.Calculator.Client.bit_mul,
+        True,
+        {
+            "config": HTTPConfig().header("X-Generic-Token", "42")
+        })
+
+    run_test(
+        "Pass request as blob in body",
+        api.Double(1.),
+        api.Calculator.Client.identity,
+        1.,
+        {
+            "config": HTTPConfig().cookie("api-cookie", "42")
+        })
+
+    run_test(
+        "Pass base64-encoded strings.",
+        api.Strings(["foo", "bar"]),
+        api.Calculator.Client.concat,
+        "foobar",
+        {
+            "bearer": "123"
+        })
+
+    run_test(
+        "Pass enum.",
+        api.EnumWrapper(api.Enum.TEST_ENUM_0),
+        api.Calculator.Client.name,
+        "TEST_ENUM_0",
+        {
+            "config": HTTPConfig().api_key("42")
+        })
+
+    if failed > 0:
+        print(f"[py-test-client] Done, {failed} test(s) failed!", flush=True)
+        exit(1)
+    else:
+        print(f"[py-test-client] All tests succeeded.!", flush=True)
+        exit(0)
+
```

## zswag/test/calc/server.py

 * *Ordering differences only*

```diff
@@ -1,51 +1,51 @@
-import math
-import calculator.api as api
-from functools import reduce
-from connexion.exceptions import Unauthorized
-
-# ------------ Auth validation helpers ------------
-
-def validate_basic_auth(username, password, required_scopes):
-    if username != "u" or password != "pw":
-        raise Unauthorized()
-    return dict()
-
-def validate_apikey(token, required_scopes):
-    if token != "42":
-        raise Unauthorized()
-    return dict()
-
-def validate_bearer(token):
-    if token != "123":
-        raise Unauthorized()
-    return dict()
-
-# ------------------- Endpoints -------------------
-
-def power(request: api.BaseAndExponent):
-    response = api.Double(request.base.value**request.exponent.value)
-    return response
-
-def int_sum(request: api.Integers):
-    return api.Double(sum(request.values))
-
-def byte_sum(request):
-    return api.Double(sum(request.values))
-
-def int_mul(request):
-    return api.Double(reduce(int.__mul__, request.values))
-
-def float_mul(request):
-    return api.Double(reduce(float.__mul__, request.values))
-
-def bit_mul(request):
-    return api.Bool(reduce(bool.__and__, request.values))
-
-def identity(request):
-    return request
-
-def concat(request):
-    return api.String(reduce(str.__add__, request.values))
-
-def name(request):
-    return api.String(request.value.name)
+import math
+import calculator.api as api
+from functools import reduce
+from connexion.exceptions import Unauthorized
+
+# ------------ Auth validation helpers ------------
+
+def validate_basic_auth(username, password, required_scopes):
+    if username != "u" or password != "pw":
+        raise Unauthorized()
+    return dict()
+
+def validate_apikey(token, required_scopes):
+    if token != "42":
+        raise Unauthorized()
+    return dict()
+
+def validate_bearer(token):
+    if token != "123":
+        raise Unauthorized()
+    return dict()
+
+# ------------------- Endpoints -------------------
+
+def power(request: api.BaseAndExponent):
+    response = api.Double(request.base.value**request.exponent.value)
+    return response
+
+def int_sum(request: api.Integers):
+    return api.Double(sum(request.values))
+
+def byte_sum(request):
+    return api.Double(sum(request.values))
+
+def int_mul(request):
+    return api.Double(reduce(int.__mul__, request.values))
+
+def float_mul(request):
+    return api.Double(reduce(float.__mul__, request.values))
+
+def bit_mul(request):
+    return api.Bool(reduce(bool.__and__, request.values))
+
+def identity(request):
+    return request
+
+def concat(request):
+    return api.String(reduce(str.__add__, request.values))
+
+def name(request):
+    return api.String(request.value.name)
```

## Comparing `zswag-1.5.0.dist-info/LICENSE` & `zswag-1.6.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, NDS e.V. Association
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, NDS e.V. Association
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## Comparing `zswag-1.5.0.dist-info/METADATA` & `zswag-1.6.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,1675 +1,860 @@
-Metadata-Version: 2.1
-Name: zswag
-Version: 1.5.0
-Summary: OpenAPI service transport layer for zserio.
-Home-page: https://github.com/klebert-engineering/zswag
-Author: Klebert Engineering
-Author-email: j.birkner@klebert-engineering.de
-License: BSD-3 Clause
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: connexion
-Requires-Dist: requests
-Requires-Dist: zserio (>=2.4.2)
-Requires-Dist: pyyaml
-Requires-Dist: pyzswagcl (>=1.5.0)
-Requires-Dist: openapi-spec-validator
-
-# Zswag
-
-
-
-[![CI](https://github.com/Klebert-Engineering/zswag/actions/workflows/cmake.yml/badge.svg)](https://github.com/Klebert-Engineering/zswag/actions/workflows/cmake.yml)
-
-[![Release](https://img.shields.io/github/release/Klebert-Engineering/zswag)](https://GitHub.com/Klebert-Engineering/zswag/releases/)
-
-[![License](https://img.shields.io/github/license/klebert-engineering/zswag)](https://github.com/Klebert-Engineering/zswag/blob/master/LICENSE)
-
-
-
-zswag is a set of libraries for using/hosting zserio services through OpenAPI.
-
-
-
-**Table of Contents:**
-
-
-
-  * [Components](#components)
-
-  * [Setup](#setup)
-
-    + [For Python Users](#for-python-users)
-
-    + [For C++ Users](#for-c-users)
-
-  * [OpenAPI Generator CLI](#openapi-generator-cli)
-
-    + [Generator Usage Example](#generator-usage-example)
-
-    + [Documentation extraction](#documentation-extraction)
-
-  * [Server Component (Python)](#server-component)
-
-  * [Using the Python Client](#using-the-python-client)
-
-  * [C++ Client](#c-client)
-
-  * [Client Environment Settings](#client-environment-settings)
-
-  * [HTTP Proxies and Authentication](#persistent-http-headers-proxy-cookie-and-authentication)
-
-  * [Swagger User Interface](#swagger-user-interface)
-
-  * [OpenAPI Options Interoperability](#openapi-options-interoperability)
-
-    + [HTTP method](#http-method)
-
-    + [Request Body](#request-body)
-
-    + [URL Blob Parameter](#url-blob-parameter)
-
-    + [URL Scalar Parameter](#url-scalar-parameter)
-
-    + [URL Array Parameter](#url-array-parameter)
-
-    + [URL Compound Parameter](#url-compound-parameter)
-
-    + [Server URL Base Path](#server-url-base-path)
-
-    + [Authentication Schemes](#authentication-schemes)
-
-
-
-## Components
-
-
-
-The zswag repository contains two main libraries which provide
-
-OpenAPI layers for zserio Python and C++ clients. For Python, there
-
-is even a generic zserio OpenAPI server layer.
-
-
-
-The following UML diagram provides a more in-depth overview:
-
-
-
-![Component Overview](doc/zswag-architecture.png)
-
-
-
-Here are some brief descriptions of the main components:
-
-
-
-* `zswagcl` is a C++ Library which exposes the zserio OpenAPI service client `OAClient`
-
-  as well as the more generic `OpenApiClient` and `OpenApiConfig` classes.
-
-  The latter two are reused for the Python client library.
-
-* `zswag` is a Python Library which provides both a zserio Python service client
-
-  (`OAClient`) as well as a zserio-OpenAPI server layer based on Flask/Connexion
-
-  (`OAServer`). It also contains the command-line tool `zswag.gen`, which can be
-
-  used to generate an OpenAPI specification from a zserio Python service class.
-
-* `pyzswagcl` is a binding library which exposes the C++-based OpenApi
-
-  parsing/request functionality to Python. **Please consider it "internal".**
-
-* `httpcl` is a wrapper around [cpp-httplib](https://github.com/yhirose/cpp-httplib),
-
-  HTTP request configuration and OS secret storage abilities based on
-
-  the [keychain](https://github.com/hrantzsch/keychain) library.
-
-  
-
-## Setup
-
-
-
-### For Python Users
-
-
-
-Simply run `pip install zswag`. **Note: This only works with ...**
-
-
-
-* 64-bit Python 3.8.x, `pip --version` >= 19.3
-
-* 64-bit Python 3.9.x, `pip --version` >= 19.3
-
-
-
-**Note:** On Windows, make sure that you have the *Microsoft Visual C++ Redistributable Binaries* installed. You can find the x64 installer here: https://aka.ms/vs/16/release/vc_redist.x64.exe
-
- 
-
-### For C++ Users
-
-
-
-Using CMake, you can ...
-
-
-
-* 🌟run tests.
-
-* 🌟build the zswag wheels for a custom Python version.
-
-* 🌟[integrate the C++ client into a C++ project.](#c-client)
-
-
-
-The basic setup follows the usual CMake configure/build steps:
-
-```bash
-
-mkdir build && cd build
-
-cmake ..
-
-cmake --build .
-
-```
-
-
-
-**Note:** The Python environment used for configuration will be used
-
-to build the resulting wheels. After building, you will find the Python
-
-wheels under `build/bin/wheel`.
-
-
-
-**To run tests**, just execute CTest at the top of the build directory:
-
-```bash
-
-cd build && ctest --verbose
-
-```
-
-
-
-
-
-## OpenAPI Generator CLI
-
-
-
-After installing `zswag` via pip as [described above](#for-python-users),
-
-you can run `python -m zswag.gen`, a CLI to generate OpenAPI YAML files.
-
-The CLI offers the following options
-
-
-
-```
-
-usage: Zserio OpenApi YAML Generator [-h] -s service-identifier -i
-
-                                     zserio-or-python-path
-
-                                     [-r zserio-src-root-dir]
-
-                                     [-p top-level-package] [-c tags [tags ...]]
-
-                                     [-o output] [-b BASE_CONFIG_YAML]
-
-
-
-optional arguments:
-
-  -h, --help
-
-        show this help message and exit
-
-  -s service-identifier, --service service-identifier
-
-
-
-        Fully qualified zserio service identifier.
-
-
-
-        Example:
-
-            -s my.package.ServiceClass
-
-
-
-  -i zserio-or-python-path, --input zserio-or-python-path
-
-
-
-        Can be either ...
-
-        (A) Path to a zserio .zs file. Must be either a top-
-
-            level entrypoint (e.g. all.zs), or a subpackage
-
-            (e.g. services/myservice.zs) in conjunction with
-
-            a "--zserio-source-root|-r <dir>" argument.
-
-        (B) Path to parent dir of a zserio Python package.
-
-
-
-        Examples:
-
-            -i path/to/schema/main.zs         (A)
-
-            -i path/to/python/package/parent  (B)
-
-
-
-  -r zserio-src-root-dir, --zserio-source-root zserio-src-root-dir
-
-
-
-        When -i specifies a zs file (Option A), indicate the
-
-        directory for the zserio -src directory argument. If
-
-        not specified, the parent directory of the zs file
-
-        will be used.
-
-
-
-  -p top-level-package, --package top-level-package
-
-
-
-        When -i specifies a zs file (Option A), indicate
-
-        that a specific top-level zserio package name
-
-        should be used.
-
-
-
-        Examples:
-
-            -p zserio_pkg_name
-
-
-
-  -c tags [tags ...], --config tags [tags ...]
-
-
-
-        Configuration tags for a specific or all methods.
-
-        The argument syntax follows this pattern:
-
-
-
-           [(service-method-name):](comma-separated-tags)
-
-
-
-        Note: The -c argument may be applied multiple times.
-
-        The `comma-separated-tags` must be a list of tags
-
-        which indicate OpenApi method generator preferences.
-
-        The following tags are supported:
-
-
-
-        get|put|post|delete : HTTP method tags
-
-                query|path| : Parameter location tags
-
-                header|body
-
-                  flat|blob : Flatten request object,
-
-                              or pass it as whole blob.
-
-          (param-specifier) : Specify parameter name, format
-
-                              and location for a specific
-
-                              request-part. See below.
-
-            security=(name) : Set a particular security
-
-                              scheme to be used. The scheme
-
-                              details must be provided through
-
-                              the --base-config-yaml.
-
-         path=(method-path) : Set a particular method path.
-
-                              May contain placeholders for
-
-                              path params.
-
-
-
-        A (param-specifier) tag has the following schema:
-
-
-
-            (field?name=...
-
-                  &in=[path|body|query|header]
-
-                  &format=[binary|base64|hex]
-
-                  [&style=...]
-
-                  [&explode=...])
-
-
-
-        Examples:
-
-
-
-          Expose all methods as POST, but `getLayerByTileId`
-
-          as GET with flat path-parameters:
-
-
-
-            `-c post getLayerByTileId:get,flat,path`
-
-
-
-          For myMethod, put the whole request blob into the a
-
-          query "data" parameter as base64:
-
-
-
-            `-c myMethod:*?name=data&in=query&format=base64`
-
-
-
-          For myMethod, set the "AwesomeAuth" auth scheme:
-
-
-
-            `-c myMethod:security=AwesomeAuth`
-
-
-
-          For myMethod, provide the path and place myField
-
-          explicitely in a path placeholder:
-
-
-
-            `-c 'myMethod:path=/my-method/{param},...
-
-                 myField?name=param&in=path&format=string'`
-
-
-
-        Note:
-
-            * The HTTP-method defaults to `post`.
-
-            * The parameter 'in' defaults to `query` for
-
-              `get`, `body` otherwise.
-
-            * If a method uses a parameter specifier, the
-
-              `flat`, `body`, `query`, `path`, `header` and
-
-              `body`-tags are ignored.
-
-            * The `flat` tag is only meaningful in conjunction
-
-              with `query` or `path`.
-
-            * An unspecific tag list (no service-method-name)
-
-              affects the defaults only for following, not
-
-              preceding specialized tag assignments.
-
-
-
-  -o output, --output output
-
-
-
-        Output file path. If not specified, the output will be
-
-        written to stdout.
-
-
-
-  -b BASE_CONFIG_YAML, --base-config-yaml BASE_CONFIG_YAML
-
-
-
-        Base configuration file. Can be used to fully or partially
-
-        substitute --config arguments, and to provide additional
-
-        OpenAPI information. The YAML file must look like this:
-
-
-
-          method: # Optional method tags dictionary
-
-            <method-name|*>: <list of config tags>
-
-          securitySchemes: ... # Optional OpenAPI securitySchemes
-
-          info: ...            # Optional OpenAPI info section
-
-          servers: ...         # Optional OpenAPI servers section
-
-          security: ...        # Optional OpenAPI global security
-
-```
-
-
-
-### Generator Usage example
-
-
-
-Let's consider the following zserio service saved under `myapp/services.zs`:
-
-
-
-```
-
-package services;
-
-
-
-struct Request {
-
-  int32 value;
-
-};
-
-
-
-struct Response {
-
-  int32 value;
-
-};
-
-
-
-service MyService {
-
-  Response myApi(Request);
-
-};
-
-```
-
-
-
-An OpenAPI file `api.yaml` for `MyService` can now be
-
-created with the following `zswag.gen` invocation:
-
-
-
-```bash
-
-cd myapp
-
-python -m zswag.gen -s services.MyService -i services.zs -o api.yaml
-
-```
-
-
-
-You can further customize the generation using `-c` configuration
-
-arguments. For example, `-c get,flat,path` will recursively "flatten"
-
-the zserio request object into it's compound scalar fields using
-
-[x-zserio-request-part](#url-scalar-parameter) for all methods.
-
-If you want to change OpenAPI parameters only for one particular
-
-method, you can prefix the tag config argument with the method
-
-name (`-c methodName:tags...`).
-
-
-
-### Documentation Extraction
-
-
-
-When invoking `zswag.gen` with `-i zserio-file` an attempt
-
-will be made to populate the service/method/request/response
-
-descriptions with doc-strings that are extracted from the zserio
-
-sources.
-
-
-
-For structs and services, the documentation is expected to be
-
-enclosed by `/*! .... !*/` markers preceding the declaration:
-
-
-
-```C
-
-/*!
-
-### My Markdown Struct Doc
-
-I choose to __highlight__ this word.
-
-!*/
-
-
-
-struct MyStruct {
-
-    ...
-
-};
-
-```
-
-
-
-For service methods, a single-line doc-string is parsed which
-
-immediately precedes the declaration:
-
-
-
-```C
-
-/** This method is documented. */
-
-ReturnType myMethod(ArgumentType);
-
-```
-
-
-
-## Server Component
-
-
-
-The `OAServer` component gives you the power to marry a zserio-generated app
-
-server class with a user-written app controller and a fitting OpenAPI specification.
-
-It is based on [Flask](https://flask.palletsprojects.com/en/1.1.x/) and
-
-[Connexion](https://connexion.readthedocs.io/en/latest/).
-
-
-
-### Integration Example
-
-
-
-We consider the same `myapp` directory with a `services.zs` zserio file
-
-as already used in the [OpenAPI Generator Example](#generator-usage-example).
-
-
-
-**Note:**
-
-
-
-* `myapp` must be available as a module (it must be
-
-possible to `import myapp`). 
-
-* We recommend to run the zserio Python generator invocation
-
-  inside the `myapp` module's `__init__.py`, like this:
-
-
-
-```py
-
-import zserio
-
-from os.path import dirname, abspath
-
-
-
-working_dir = dirname(abspath(__file__))
-
-zserio.generate(
-
-  zs_dir=working_dir,
-
-  main_zs_file="services.zs",
-
-  gen_dir=working_dir)
-
-```
-
-
-
-A server script like `myapp/server.py` might then look as follows:
-
-
-
-```py
-
-import zswag
-
-import myapp.controller as controller
-
-from myapp import working_dir
-
-
-
-# This import only works after zserio generation.
-
-import services.api as services
-
-
-
-app = zswag.OAServer(
-
-  controller_module=controller,
-
-  service_type=services.MyService.Service,
-
-  yaml_path=working_dir+"/api.yaml",
-
-  zs_pkg_path=working_dir)
-
-
-
-if __name__ == "__main__":
-
-    app.run()
-
-```
-
-
-
-The server script above references two important components:
-
-* An **OpenAPI file** (`myapp/api.yaml`): Upon startup, `OAServer`
-
-  will output an error message if this file does not exist. The
-
-  error message already contains the correct command to
-
-  invoke the [OpenAPI Generator CLI](#openapi-generator-cli)
-
-  to generate `myapp/api.yaml`.
-
-* A **controller module** (`myapp/controller.py`): This file provides
-
-  the actual implementations for your service endpoints.
-
-  
-
-For the current example, `controller.py` might look as follows:
-
-
-
-```py
-
-import services.api as services
-
-
-
-# Written by you
-
-def my_api(request: services.Request):
-
-    return services.Response(request.value * 42)
-
-```
-
-
-
-## Using the Python Client
-
-
-
-The generic Python client talks to any zserio service that is running
-
-via HTTP/REST, and provides an OpenAPI specification of it's interface.
-
-
-
-### Integration Example
-
-
-
-As an example, consider a Python module called `myapp` which has the
-
-same `myapp/__init__.py` and `myapp/services.zs` zserio definition as
-
-[previously mentioned](#generator-usage-example). We consider
-
-that the server is providing its OpenAPI spec under `localhost:5000/openapi.json`.
-
-
-
-In this setting, a client `myapp/client.py` might look as follows:
-
-
-
-```python
-
-from zswag import OAClient
-
-import services.api as services
-
-
-
-openapi_url = "http://localhost:5000/openapi.json"
-
-
-
-# The client reads per-method HTTP details from the OpenAPI URL.
-
-# You can also pass a local file by setting the `is_local_file` argument
-
-# of the OAClient constructor.
-
-client = services.MyService.Client(OAClient(openapi_url))
-
-
-
-# This will trigger an HTTP request under the hood.
-
-client.my_api(services.Request(1))
-
-```
-
-
-
-As you can see, an instance of `OAClient` is passed into the constructor
-
-for zserio to use as the service client's transport implementation.
-
-
-
-**Note:** While connecting, the client will also use ...
-
-1. [Persistent HTTP configuration](#persistent-http-headers-proxy-cookie-and-authentication).
-
-2. Additional HTTP query/header/cookie/proxy/basic-auth configs passed
-
-   into the `OAClient` constructor using an instance of `zswag.HTTPConfig`.
-
-   For example:
-
-   
-
-   ```python
-
-   from zswag import OAClient, HTTPConfig
-
-   import services.api as services
-
-   config = HTTPConfig() \
-
-       .header(key="X-My-Header", val="value") \  # Can be specified 
-
-       .cookie(key="MyCookie", val="value")    \  # multiple times.
-
-       .query(key="MyCookie", val="value")     \  # 
-
-       .proxy(host="localhost", port=5050, user="john", pw="doe") \
-
-       .basic_auth(user="john", pw="doe") \
-
-       .bearer("bearer-token") \
-
-       .api_key("token")
-
-   
-
-   client = services.MyService.Client(
-
-       OAClient("http://localhost:8080/openapi.", config=config))
-
-   
-
-   # Alternative when specifying api-key or bearer
-
-   client = services.MyService.Client(
-
-       OAClient("http://localhost:8080/openapi.", api_key="token", bearer="token"))
-
-   ```
-
-   
-
-   **Note:** The additional `config` will only enrich, not overwrite the
-
-   default persistent configuration. If you would like to prevent persistent
-
-   config from being considered at all, set `HTTP_SETTINGS_FILE` to empty,
-
-   e.g. via `os.environ['HTTP_SETTINGS_FILE']=''`
-
-
-
-## C++ Client
-
-
-
-The generic C++ client talks to any zserio service that is running
-
-via HTTP/REST, and provides an OpenAPI specification of its interface.
-
-When using the C++ `OAClient` with your zserio schema, make sure
-
-that the flag `-withTypeInfoCode` is passed to the zserio C++ emitter.
-
-
-
-### Integration Example
-
-
-
-As an example, we consider the `myapp` directory which contains a `services.zs`
-
-zserio definition as [previously mentioned](#generator-usage-example).
-
-
-
-We assume that zswag is added to `myapp` as a [Git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules)
-
-under `myapp/zswag`.
-
-
-
-Next to `myapp/services.zs`, we place a `myapp/CMakeLists.txt` which describes our project:
-
-
-
-```cmake
-
-project(myapp)
-
-
-
-# If you are not interested in building zswag Python
-
-# wheels, you can set the following option:
-
-# set(ZSWAG_BUILD_WHEELS OFF)
-
-
-
-# If your compilation environment does not provide
-
-# libsecret, the following switch will disable keychain integration:
-
-# set(ZSWAG_KEYCHAIN_SUPPORT OFF)
-
-
-
-# This is how C++ will know about the zswag lib
-
-# and its dependencies, such as zserio.
-
-add_subdirectory(zswag)
-
-
-
-# This command is provided by zswag to easily create
-
-# a CMake C++ reflection library from zserio code.
-
-add_zserio_library(${PROJECT_NAME}-zserio-cpp
-
-  WITH_REFLECTION
-
-  ROOT "${CMAKE_CURRENT_SOURCE_DIR}"
-
-  ENTRY services.zs
-
-  TOP_LEVEL_PKG myapp_services)
-
-
-
-# We create a myapp client executable which links to
-
-# the generated zserio C++ library and the zswag client
-
-# library.
-
-add_executable(${PROJECT_NAME} client.cpp)
-
-
-
-# Make sure to link to the `zswagcl` target
-
-target_link_libraries(${PROJECT_NAME}
-
-    ${PROJECT_NAME}-zserio-cpp zswagcl)
-
-```
-
-
-
-The `add_executable` command above references the file `myapp/client.cpp`,
-
-which contains the code to actually use the zswag C++ client.
-
-
-
-```cpp
-
-#include "zswagcl/oaclient.hpp"
-
-#include <iostream>
-
-#include "myapp_services/services/MyService.h"
-
-
-
-using namespace zswagcl;
-
-using namespace httpcl;
-
-namespace MyService = myapp_services::services::MyService;
-
-
-
-int main (int argc, char* argv[])
-
-{
-
-    // Assume that the server provides its OpenAPI definition here
-
-    auto openApiUrl = "http://localhost:5000/openapi.json";
-
-    
-
-    // Create an HTTP client to be used by our OpenAPI client
-
-    auto httpClient = std::make_unique<HttpLibHttpClient>();
-
-    
-
-    // Fetch the OpenAPI configuration using the HTTP client
-
-    auto openApiConfig = fetchOpenAPIConfig(openApiUrl, *httpClient);
-
-    
-
-    // Create a Zserio reflection-based OpenAPI client that
-
-    // uses the OpenAPI configuration we just retrieved.
-
-    auto openApiClient = OAClient(openApiConfig, std::move(httpClient));
-
-        
-
-    // Create a MyService client based on the OpenApi-Client
-
-    // implementation of the zserio::IServiceClient interface.
-
-    auto myServiceClient = MyService::Client(openApiClient);
-
-    
-
-    // Create the request object
-
-    auto request = myapp_services::services::Request(2);
-
-
-
-    // Invoke the REST endpoint. Mind that your method-
-
-    // name from the schema is appended with a "...Method" suffix.
-
-    auto response = myServiceClient.myApiMethod(request);
-
-    
-
-    // Print the response
-
-    std::cout << "Got " << response.getValue() << std::endl;
-
-}
-
-```
-
-
-
-**Note:** While connecting, `HttpLibHttpClient` will also use ...
-
-1. [Persistent HTTP configuration](#persistent-http-headers-proxy-cookie-and-authentication).
-
-2. Additional HTTP query/header/cookie/proxy/basic-auth configs passed
-
-   into the `OAClient` constructor using an instance of `httpcl::Config`.
-
-   You can include this class via `#include "httpcl/http-settings.hpp"`.
-
-   The additional `Config` will only enrich, not overwrite the
-
-   default persistent configuration. If you would like to prevent persistent
-
-   config from being considered at all, set `HTTP_SETTINGS_FILE` to empty,
-
-   e.g. via `setenv`.
-
-
-
-## Client Environment Settings
-
-
-
-Both the Python and C++ Clients can be configured using the following
-
-environment variables:
-
-
-
-| Variable Name | Details   |
-
-| ------------- | --------- |
-
-| `HTTP_SETTINGS_FILE` | Path to settings file for HTTP proxies and authentication, see [next section](#persistent-http-headers-proxy-cookie-and-authentication) |
-
-| `HTTP_LOG_LEVEL` | Verbosity level for console/log output. Set to `debug` for detailed output. |
-
-| `HTTP_LOG_FILE` | Logfile-path (including filename) to redirect console output. The log will rotate with three files (`HTTP_LOG_FILE`, `HTTP_LOG_FILE-1`, `HTTP_LOG_FILE-2`). |
-
-| `HTTP_LOG_FILE_MAXSIZE` | Maximum size of the logfile, in bytes. Defaults to 1GB. |
-
-| `HTTP_TIMEOUT` | Timeout for HTTP requests (connection+transfer) in seconds. Defaults to 60s. |
-
-| `HTTP_SSL_STRICT` | Set to any nonempty value for strict SSL certificate validation. |
-
-
-
-## Persistent HTTP Headers, Proxy, Cookie and Authentication
-
-
-
-Both the Python `OAClient` and C++ `HttpLibHttpClient` read a YAML file
-
-stored under a path which is given by the `HTTP_SETTINGS_FILE` environment
-
-variable. The YAML file contains a list of HTTP-related configs that are
-
-applied to HTTP requests based on a regular expression which is matched
-
-against the requested URL.
-
-
-
-For example, the following entry would match all requests due to the `.*`
-
-url-match-pattern:
-
-
-
-```yaml
-
-- url: .*
-
-  basic-auth:
-
-    user: johndoe
-
-    keychain: keychain-service-string
-
-  proxy:
-
-    host: localhost
-
-    port: 8888
-
-    user: test
-
-    keychain: ...
-
-  cookies:
-
-    key: value
-
-  headers:
-
-    key: value
-
-  query:
-
-    key: value
-
-  api-key: value
-
-```
-
-
-
-**Note:** For `proxy` configs, the credentials are optional.
-
-
-
-The **`api-key`** setting will be applied under the correct
-
-cookie/header/query parameter, if the service
-
-you are connecting to uses an [OpenAPI `apiKey` auth scheme](#authentication-schemes).
-
-
-
-Passwords can be stored in clear text by setting a `password` field instead
-
-of the `keychain` field. Keychain entries can be made with different tools
-
-on each platform:
-
-
-
-* [Linux `secret-tool`](https://www.marian-dan.ro/blog/storing-secrets-using-secret-tool) 
-
-* [macOS `add-generic-password`](https://www.netmeister.org/blog/keychain-passwords.html)
-
-* [Windows `cmdkey`](https://www.scriptinglibrary.com/languages/powershell/how-to-manage-secrets-and-passwords-with-credentialmanager-and-powershell/)
-
-
-
-## Swagger User Interface 
-
-
-
-If you have installed `pip install "connexion[swagger-ui]"`, you can view
-
-API docs of your service under `[/prefix]/ui`.
-
-
-
-## OpenAPI Options Interoperability
-
-
-
-The Server, Clients and Generator offer various degrees of freedom
-
-regarding the OpenAPI YAML file. The following sections detail which
-
-components support which aspects of OpenAPI. The difference in compliance
-
-is mostly due to limited development scopes. If you are missing a particular
-
-OpenAPI feature for a particular component, feel free to create an issue!
-
-
-
-**Note:** For all options that are not supported by `zswag.gen`, you
-
-will need to manually edit the OpenAPI YAML file to achieve the desired
-
-configuration. You will also need to edit the file manually to fill in
-
-meta-info (provider name, service version, etc.).
-
-
-
-### HTTP method
-
-
-
-To change the **HTTP method**, the desired method name is placed 
-
-as the key under the method path, such as in the following example:
-
-```yaml
-
-paths:
-
-  /methodName:
-
-    {get|post|put|delete}:
-
-      ...
-
-```
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `get` `post` `put` `delete` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `patch` | ❌️ | ❌️ | ❌️ | ❌️ |
-
-
-
-**Note:** Patch is unsupported, because the required semantics of
-
-a partial object update cannot be realized in the zserio transport
-
-layer interface.
-
-
-
-### Request Body
-
-
-
-A server can instruct clients to transmit their zserio request object in the
-
-request body when using HTTP `post`, `put` or `delete`.
-
-This is done by setting the OpenAPI `requestBody/content` to
-
-`application/x-zserio-object`:
-
-
-
-```yaml
-
-requestBody:
-
-  content:
-
-    application/x-zserio-object:
-
-      schema:
-
-        type: string
-
-```
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `application/x-zserio-object` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-
-
-### URL Blob Parameter
-
-
-
-Zswag tools support an additional OpenAPI method parameter
-
-field called `x-zserio-request-part`. Through this field,
-
-a service provider can express that a certain request parameter
-
-only contains a part of, or the whole zserio request object.
-
-When parameter contains the whole request object, `x-zserio-request-part`
-
-should be set to an asterisk (`*`):
-
-
-
-```yaml
-
-parameters:
-
-- description: ''
-
-  in: query|path|header
-
-  name: parameterName
-
-  required: true
-
-  x-zserio-request-part: "*"
-
-  schema:
-
-    format: string|byte|base64|base64url|hex|binary
-
-```
-
-
-
-About the `format` specifier value:
-
-* Both `string` and `binary` result in a raw URL-encoded string buffer.
-
-* Both `byte` and `base64` result in a standard Base64-encoded value.
-
-  The `base64url` option indicates URL-safe Base64 format.
-
-* The `hex` encoding produces a hexadecimal encoding of the request blob.
-
-
-
-**Note:** When a parameter is passed with `in=path`, its value
-
-**must not be empty**. This holds true for strings and bytes,
-
-but also for arrays (see below).
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `x-zserio-request-part: *` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `format: string` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `format: byte` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `format: hex` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-
-
-### URL Scalar Parameter
-
-
-
-Using `x-zserio-request-part`, it is also possible to transfer
-
-only a single scalar (nested) member of the request object:
-
-
-
-```yaml
-
-parameters:
-
-- description: ''
-
-  in: query|path|header
-
-  name: parameterName
-
-  required: true
-
-  x-zserio-request-part: "[parent.]*member"
-
-  schema:
-
-    format: string|byte|base64|base64url|hex|binary
-
-```
-
-
-
-In this case, `x-zserio-request-part` should point to a scalar type,
-
-such as `uint8`, `float32`, `string` etc.
-
-
-
-The `format` value effect remains as explained above. A small
-
-difference exists for integer types: Their hexadecimal representation
-
-will be the natural numeric one, not binary.
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `x-zserio-request-part: <[parent.]*member>` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-
-
-### URL Array Parameter
-
-
-
-The `x-zserio-request-part` may also point to an array member of
-
-the zserio request struct, like so:
-
-
-
-```yaml
-
-parameters:
-
-- description: ''
-
-  in: query|path|header
-
-  style: form|simple|label|matrix
-
-  explode: true|false
-
-  name: parameterName
-
-  required: true
-
-  x-zserio-request-part: "[parent.]*array_member"
-
-  schema:
-
-    format: string|byte|base64|base64url|hex|binary
-
-```
-
-
-
-In this case, `x-zserio-request-part` should point to an array of
-
-scalar types. The array will be encoded according
-
-to the [format, style and explode](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md#parameter-object)
-
-specifiers.
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `x-zserio-request-part: <[parent.]*array_member>`  | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `style: simple` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `style: form` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `style: label` | ✔️ | ✔️ | ❌ | ✔️ |
-
-| `style: matrix` | ✔️ | ✔️ | ❌ | ✔️ |
-
-| `explode: true` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-| `explode: false` | ✔️ | ✔️ | ✔️ | ✔️ |
-
-
-
-### URL Compound Parameter
-
-
-
-In this case, `x-zserio-request-part` points to a zserio compound struct
-
-instead of a field with a scalar value. **This is currently not supported.**
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `x-zserio-request-part: <[parent.]*compound_member>`  | ❌️ | ❌️ | ❌️ | ❌️ |
-
-
-
-### Server URL Base Path
-
-
-
-OpenAPI allows for a `servers` field in the spec that lists URL path prefixes
-
-under which the specified API may be reached. The OpenAPI clients
-
-looks into this list to determine a URL base path from
-
-the first entry in this list. A sample entry might look as follows:
-
-
-
-```
-
-servers:
-
-- http://unused-host-information/path/to/my/api
-
-``` 
-
-
-
-The OpenAPI client will then call methods with your specified host
-
-and port, but prefix the `/path/to/my/api` string. 
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `servers`  | ✔️ | ✔️ | ✔️ | ✔️ |
-
-
-
-### Authentication Schemes
-
-
-
-To facilitate the communication of authentication needs for the whole or parts
-
-of a service, OpenAPI allows for `securitySchemes` and `security` fields in the spec.
-
-Please refer to the relevant parts of the [OpenAPI 3 specification](https://swagger.io/docs/specification/authentication/) for some
-
-examples on how to integrate these fields into your spec.
-
-
-
-Zswag currently understands the following authentication schemes:
-
-
-
-* **HTTP Basic Authorization:** If a called endpoint requires HTTP basic auth,
-
-  zswag will verify that the HTTP config contains basic-auth credentials.
-
-  If there are none, zswag will throw a descriptive runtime error.
-
-* **HTTP Bearer Authorization:** If a called endpoint requires HTTP bearer auth,
-
-  zswag will verify that the HTTP config contains a header with the
-
-  key name `Authorization` and the value `Bearer <token>`, *case-sensitive*.
-
-* **API-Key Cookie:** If a called endpoint requires a Cookie API-Key,
-
-  zswag will either apply [the `api-key` setting](#persistent-http-headers-proxy-cookie-and-authentication), or verify that the
-
-  HTTP config contains a cookie with the required name, *case-sensitive*.
-
-* **API-Key Query Parameter:** If a called endpoint requires a Query API-Key,
-
-  zswag will either apply the `api-key` setting, or verify that the
-
-  HTTP config contains a query key-value pair with the required name, *case-sensitive*.
-
-* **API-Key Header:** If a called endpoint requires an API-Key Header,
-
-  zswag will either apply the `api-key` setting, or verify that the
-
-  HTTP config contains a header key-value pair with the required name, *case-sensitive*.
-
-
-
-**Note**: If you don't want to pass your Basic-Auth/Bearer/Query/Cookie/Header
-
-credential through your [persistent config](#persistent-http-headers-proxy-cookie-and-authentication),
-
-you can pass a `httpcl::Config`/[`HTTPConfig`](#using-the-python-client) object to the `OAClient`/[`OAClient`](#using-the-python-client).
-
-constructor in C++/Python with the relevant detail.
-
-
-
-#### Component Support
-
-
-
-| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
-
-| ------------------ | ---------- | ------------- | -------- | --------- |
-
-| `HTTP Basic-Auth` `HTTP Bearer-Auth` `Cookie API-Key` `Header API-Key` `Query API-Key`  | ✔️ | ✔️ | ✔️(**) | ✔️ |
-
-| `OpenID Connect` `OAuth2`  | ❌️ | ❌️ | ✔️(**) | ❌️ |
-
-
-
-**(\*\*)**: The server support for all authentication schemes depends on your
-
-configuration of the WSGI server (Apache/Nginx/...) which wraps the zswag Flask app.
-
+Metadata-Version: 2.1
+Name: zswag
+Version: 1.6.0
+Summary: OpenAPI service transport layer for zserio.
+Home-page: https://github.com/klebert-engineering/zswag
+Author: Klebert Engineering
+Author-email: j.birkner@klebert-engineering.de
+License: BSD-3 Clause
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: connexion
+Requires-Dist: requests
+Requires-Dist: zserio (>=2.4.2)
+Requires-Dist: pyyaml
+Requires-Dist: pyzswagcl (>=1.6.0)
+Requires-Dist: openapi-spec-validator
+
+# Zswag
+
+[![CI](https://github.com/Klebert-Engineering/zswag/actions/workflows/cmake.yml/badge.svg)](https://github.com/Klebert-Engineering/zswag/actions/workflows/cmake.yml)
+[![Release](https://img.shields.io/github/release/Klebert-Engineering/zswag)](https://GitHub.com/Klebert-Engineering/zswag/releases/)
+[![License](https://img.shields.io/github/license/klebert-engineering/zswag)](https://github.com/Klebert-Engineering/zswag/blob/master/LICENSE)
+
+zswag is a set of libraries for using/hosting zserio services through OpenAPI.
+
+**Table of Contents:**
+
+  * [Components](#components)
+  * [Setup](#setup)
+    + [For Python Users](#for-python-users)
+    + [For C++ Users](#for-c-users)
+  * [OpenAPI Generator CLI](#openapi-generator-cli)
+    + [Generator Usage Example](#generator-usage-example)
+    + [Documentation extraction](#documentation-extraction)
+  * [Server Component (Python)](#server-component)
+  * [Using the Python Client](#using-the-python-client)
+  * [C++ Client](#c-client)
+  * [Client Environment Settings](#client-environment-settings)
+  * [HTTP Proxies and Authentication](#persistent-http-headers-proxy-cookie-and-authentication)
+  * [Swagger User Interface](#swagger-user-interface)
+  * [OpenAPI Options Interoperability](#openapi-options-interoperability)
+    + [HTTP method](#http-method)
+    + [Request Body](#request-body)
+    + [URL Blob Parameter](#url-blob-parameter)
+    + [URL Scalar Parameter](#url-scalar-parameter)
+    + [URL Array Parameter](#url-array-parameter)
+    + [URL Compound Parameter](#url-compound-parameter)
+    + [Server URL Base Path](#server-url-base-path)
+    + [Authentication Schemes](#authentication-schemes)
+
+## Components
+
+The zswag repository contains two main libraries which provide
+OpenAPI layers for zserio Python and C++ clients. For Python, there
+is even a generic zserio OpenAPI server layer.
+
+The following UML diagram provides a more in-depth overview:
+
+![Component Overview](doc/zswag-architecture.png)
+
+Here are some brief descriptions of the main components:
+
+* `zswagcl` is a C++ Library which exposes the zserio OpenAPI service client `OAClient`
+  as well as the more generic `OpenApiClient` and `OpenApiConfig` classes.
+  The latter two are reused for the Python client library.
+* `zswag` is a Python Library which provides both a zserio Python service client
+  (`OAClient`) as well as a zserio-OpenAPI server layer based on Flask/Connexion
+  (`OAServer`). It also contains the command-line tool `zswag.gen`, which can be
+  used to generate an OpenAPI specification from a zserio Python service class.
+* `pyzswagcl` is a binding library which exposes the C++-based OpenApi
+  parsing/request functionality to Python. **Please consider it "internal".**
+* `httpcl` is a wrapper around [cpp-httplib](https://github.com/yhirose/cpp-httplib),
+  HTTP request configuration and OS secret storage abilities based on
+  the [keychain](https://github.com/hrantzsch/keychain) library.
+  
+## Setup
+
+### For Python Users
+
+Simply run `pip install zswag`. **Note: This only works with ...**
+
+* 64-bit Python 3.8.x, `pip --version` >= 19.3
+* 64-bit Python 3.9.x, `pip --version` >= 19.3
+
+**Note:** On Windows, make sure that you have the *Microsoft Visual C++ Redistributable Binaries* installed. You can find the x64 installer here: https://aka.ms/vs/16/release/vc_redist.x64.exe
+ 
+### For C++ Users
+
+Using CMake, you can ...
+
+* 🌟run tests.
+* 🌟build the zswag wheels for a custom Python version.
+* 🌟[integrate the C++ client into a C++ project.](#c-client)
+
+Dependencies are managed via CMake's `FetchContent` mechanism and Conan 2.0.
+Make sure you have a recent version of CMake (>= 3.24) and Conan (>= 2.0.5) installed.
+
+The basic setup follows the usual CMake configure/build steps:
+```bash
+mkdir build && cd build
+cmake ..
+cmake --build .
+```
+
+**Note:** The Python environment used for configuration will be used
+to build the resulting wheels. After building, you will find the Python
+wheels under `build/bin/wheel`.
+
+**To run tests**, just execute CTest at the top of the build directory:
+```bash
+cd build && ctest --verbose
+```
+
+
+## OpenAPI Generator CLI
+
+After installing `zswag` via pip as [described above](#for-python-users),
+you can run `python -m zswag.gen`, a CLI to generate OpenAPI YAML files.
+The CLI offers the following options
+
+```
+usage: Zserio OpenApi YAML Generator [-h] -s service-identifier -i
+                                     zserio-or-python-path
+                                     [-r zserio-src-root-dir]
+                                     [-p top-level-package] [-c tags [tags ...]]
+                                     [-o output] [-b BASE_CONFIG_YAML]
+
+optional arguments:
+  -h, --help
+        show this help message and exit
+  -s service-identifier, --service service-identifier
+
+        Fully qualified zserio service identifier.
+
+        Example:
+            -s my.package.ServiceClass
+
+  -i zserio-or-python-path, --input zserio-or-python-path
+
+        Can be either ...
+        (A) Path to a zserio .zs file. Must be either a top-
+            level entrypoint (e.g. all.zs), or a subpackage
+            (e.g. services/myservice.zs) in conjunction with
+            a "--zserio-source-root|-r <dir>" argument.
+        (B) Path to parent dir of a zserio Python package.
+
+        Examples:
+            -i path/to/schema/main.zs         (A)
+            -i path/to/python/package/parent  (B)
+
+  -r zserio-src-root-dir, --zserio-source-root zserio-src-root-dir
+
+        When -i specifies a zs file (Option A), indicate the
+        directory for the zserio -src directory argument. If
+        not specified, the parent directory of the zs file
+        will be used.
+
+  -p top-level-package, --package top-level-package
+
+        When -i specifies a zs file (Option A), indicate
+        that a specific top-level zserio package name
+        should be used.
+
+        Examples:
+            -p zserio_pkg_name
+
+  -c tags [tags ...], --config tags [tags ...]
+
+        Configuration tags for a specific or all methods.
+        The argument syntax follows this pattern:
+
+           [(service-method-name):](comma-separated-tags)
+
+        Note: The -c argument may be applied multiple times.
+        The `comma-separated-tags` must be a list of tags
+        which indicate OpenApi method generator preferences.
+        The following tags are supported:
+
+        get|put|post|delete : HTTP method tags
+                query|path| : Parameter location tags
+                header|body
+                  flat|blob : Flatten request object,
+                              or pass it as whole blob.
+          (param-specifier) : Specify parameter name, format
+                              and location for a specific
+                              request-part. See below.
+            security=(name) : Set a particular security
+                              scheme to be used. The scheme
+                              details must be provided through
+                              the --base-config-yaml.
+         path=(method-path) : Set a particular method path.
+                              May contain placeholders for
+                              path params.
+
+        A (param-specifier) tag has the following schema:
+
+            (field?name=...
+                  &in=[path|body|query|header]
+                  &format=[binary|base64|hex]
+                  [&style=...]
+                  [&explode=...])
+
+        Examples:
+
+          Expose all methods as POST, but `getLayerByTileId`
+          as GET with flat path-parameters:
+
+            `-c post getLayerByTileId:get,flat,path`
+
+          For myMethod, put the whole request blob into the a
+          query "data" parameter as base64:
+
+            `-c myMethod:*?name=data&in=query&format=base64`
+
+          For myMethod, set the "AwesomeAuth" auth scheme:
+
+            `-c myMethod:security=AwesomeAuth`
+
+          For myMethod, provide the path and place myField
+          explicitely in a path placeholder:
+
+            `-c 'myMethod:path=/my-method/{param},...
+                 myField?name=param&in=path&format=string'`
+
+        Note:
+            * The HTTP-method defaults to `post`.
+            * The parameter 'in' defaults to `query` for
+              `get`, `body` otherwise.
+            * If a method uses a parameter specifier, the
+              `flat`, `body`, `query`, `path`, `header` and
+              `body`-tags are ignored.
+            * The `flat` tag is only meaningful in conjunction
+              with `query` or `path`.
+            * An unspecific tag list (no service-method-name)
+              affects the defaults only for following, not
+              preceding specialized tag assignments.
+
+  -o output, --output output
+
+        Output file path. If not specified, the output will be
+        written to stdout.
+
+  -b BASE_CONFIG_YAML, --base-config-yaml BASE_CONFIG_YAML
+
+        Base configuration file. Can be used to fully or partially
+        substitute --config arguments, and to provide additional
+        OpenAPI information. The YAML file must look like this:
+
+          method: # Optional method tags dictionary
+            <method-name|*>: <list of config tags>
+          securitySchemes: ... # Optional OpenAPI securitySchemes
+          info: ...            # Optional OpenAPI info section
+          servers: ...         # Optional OpenAPI servers section
+          security: ...        # Optional OpenAPI global security
+```
+
+### Generator Usage example
+
+Let's consider the following zserio service saved under `myapp/services.zs`:
+
+```
+package services;
+
+struct Request {
+  int32 value;
+};
+
+struct Response {
+  int32 value;
+};
+
+service MyService {
+  Response myApi(Request);
+};
+```
+
+An OpenAPI file `api.yaml` for `MyService` can now be
+created with the following `zswag.gen` invocation:
+
+```bash
+cd myapp
+python -m zswag.gen -s services.MyService -i services.zs -o api.yaml
+```
+
+You can further customize the generation using `-c` configuration
+arguments. For example, `-c get,flat,path` will recursively "flatten"
+the zserio request object into it's compound scalar fields using
+[x-zserio-request-part](#url-scalar-parameter) for all methods.
+If you want to change OpenAPI parameters only for one particular
+method, you can prefix the tag config argument with the method
+name (`-c methodName:tags...`).
+
+### Documentation Extraction
+
+When invoking `zswag.gen` with `-i zserio-file` an attempt
+will be made to populate the service/method/request/response
+descriptions with doc-strings that are extracted from the zserio
+sources.
+
+For structs and services, the documentation is expected to be
+enclosed by `/*! .... !*/` markers preceding the declaration:
+
+```C
+/*!
+### My Markdown Struct Doc
+I choose to __highlight__ this word.
+!*/
+
+struct MyStruct {
+    ...
+};
+```
+
+For service methods, a single-line doc-string is parsed which
+immediately precedes the declaration:
+
+```C
+/** This method is documented. */
+ReturnType myMethod(ArgumentType);
+```
+
+## Server Component
+
+The `OAServer` component gives you the power to marry a zserio-generated app
+server class with a user-written app controller and a fitting OpenAPI specification.
+It is based on [Flask](https://flask.palletsprojects.com/en/1.1.x/) and
+[Connexion](https://connexion.readthedocs.io/en/latest/).
+
+### Integration Example
+
+We consider the same `myapp` directory with a `services.zs` zserio file
+as already used in the [OpenAPI Generator Example](#generator-usage-example).
+
+**Note:**
+
+* `myapp` must be available as a module (it must be
+possible to `import myapp`). 
+* We recommend to run the zserio Python generator invocation
+  inside the `myapp` module's `__init__.py`, like this:
+
+```py
+import zserio
+from os.path import dirname, abspath
+
+working_dir = dirname(abspath(__file__))
+zserio.generate(
+  zs_dir=working_dir,
+  main_zs_file="services.zs",
+  gen_dir=working_dir)
+```
+
+A server script like `myapp/server.py` might then look as follows:
+
+```py
+import zswag
+import myapp.controller as controller
+from myapp import working_dir
+
+# This import only works after zserio generation.
+import services.api as services
+
+app = zswag.OAServer(
+  controller_module=controller,
+  service_type=services.MyService.Service,
+  yaml_path=working_dir+"/api.yaml",
+  zs_pkg_path=working_dir)
+
+if __name__ == "__main__":
+    app.run()
+```
+
+The server script above references two important components:
+* An **OpenAPI file** (`myapp/api.yaml`): Upon startup, `OAServer`
+  will output an error message if this file does not exist. The
+  error message already contains the correct command to
+  invoke the [OpenAPI Generator CLI](#openapi-generator-cli)
+  to generate `myapp/api.yaml`.
+* A **controller module** (`myapp/controller.py`): This file provides
+  the actual implementations for your service endpoints.
+  
+For the current example, `controller.py` might look as follows:
+
+```py
+import services.api as services
+
+# Written by you
+def my_api(request: services.Request):
+    return services.Response(request.value * 42)
+```
+
+## Using the Python Client
+
+The generic Python client talks to any zserio service that is running
+via HTTP/REST, and provides an OpenAPI specification of it's interface.
+
+### Integration Example
+
+As an example, consider a Python module called `myapp` which has the
+same `myapp/__init__.py` and `myapp/services.zs` zserio definition as
+[previously mentioned](#generator-usage-example). We consider
+that the server is providing its OpenAPI spec under `localhost:5000/openapi.json`.
+
+In this setting, a client `myapp/client.py` might look as follows:
+
+```python
+from zswag import OAClient
+import services.api as services
+
+openapi_url = "http://localhost:5000/openapi.json"
+
+# The client reads per-method HTTP details from the OpenAPI URL.
+# You can also pass a local file by setting the `is_local_file` argument
+# of the OAClient constructor.
+client = services.MyService.Client(OAClient(openapi_url))
+
+# This will trigger an HTTP request under the hood.
+client.my_api(services.Request(1))
+```
+
+As you can see, an instance of `OAClient` is passed into the constructor
+for zserio to use as the service client's transport implementation.
+
+**Note:** While connecting, the client will also use ...
+1. [Persistent HTTP configuration](#persistent-http-headers-proxy-cookie-and-authentication).
+2. Additional HTTP query/header/cookie/proxy/basic-auth configs passed
+   into the `OAClient` constructor using an instance of `zswag.HTTPConfig`.
+   For example:
+   
+   ```python
+   from zswag import OAClient, HTTPConfig
+   import services.api as services
+   config = HTTPConfig() \
+       .header(key="X-My-Header", val="value") \  # Can be specified 
+       .cookie(key="MyCookie", val="value")    \  # multiple times.
+       .query(key="MyCookie", val="value")     \  # 
+       .proxy(host="localhost", port=5050, user="john", pw="doe") \
+       .basic_auth(user="john", pw="doe") \
+       .bearer("bearer-token") \
+       .api_key("token")
+   
+   client = services.MyService.Client(
+       OAClient("http://localhost:8080/openapi.", config=config))
+   
+   # Alternative when specifying api-key or bearer
+   client = services.MyService.Client(
+       OAClient("http://localhost:8080/openapi.", api_key="token", bearer="token"))
+   ```
+   
+   **Note:** The additional `config` will only enrich, not overwrite the
+   default persistent configuration. If you would like to prevent persistent
+   config from being considered at all, set `HTTP_SETTINGS_FILE` to empty,
+   e.g. via `os.environ['HTTP_SETTINGS_FILE']=''`
+
+## C++ Client
+
+The generic C++ client talks to any zserio service that is running
+via HTTP/REST, and provides an OpenAPI specification of its interface.
+When using the C++ `OAClient` with your zserio schema, make sure
+that the flags [`-withTypeInfoCode` and `-withReflectionCode`](http://zserio.org/doc/ZserioUserGuide.html#zserio-command-line-interface) are passed to the zserio C++ emitter.
+
+### Integration Example
+
+As an example, we consider the `myapp` directory which contains a `services.zs`
+zserio definition as [previously mentioned](#generator-usage-example).
+
+We assume that zswag is added to `myapp` as a [Git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules)
+under `myapp/zswag`.
+
+Next to `myapp/services.zs`, we place a `myapp/CMakeLists.txt` which describes our project:
+
+```cmake
+project(myapp)
+
+# If you are not interested in building zswag Python
+# wheels, you can set the following option:
+# set(ZSWAG_BUILD_WHEELS OFF)
+
+# If your compilation environment does not provide
+# libsecret, the following switch will disable keychain integration:
+# set(ZSWAG_KEYCHAIN_SUPPORT OFF)
+
+# This is how C++ will know about the zswag lib
+# and its dependencies, such as zserio.
+if (NOT TARGET zswag)
+        FetchContent_Declare(zswag
+                GIT_REPOSITORY "https://github.com/ndsev/zswag.git"
+                GIT_TAG        "v1.5.0"
+                GIT_SHALLOW    ON)
+        FetchContent_MakeAvailable(zswag)
+endif()
+
+find_package(OpenSSL CONFIG REQUIRED)
+target_link_libraries(httplib INTERFACE OpenSSL::SSL)
+
+# This command is provided by zswag to easily create
+# a CMake C++ reflection library from zserio code.
+add_zserio_library(${PROJECT_NAME}-zserio-cpp
+  WITH_REFLECTION
+  ROOT "${CMAKE_CURRENT_SOURCE_DIR}"
+  ENTRY services.zs
+  TOP_LEVEL_PKG myapp_services)
+
+# We create a myapp client executable which links to
+# the generated zserio C++ library and the zswag client
+# library.
+add_executable(${PROJECT_NAME} client.cpp)
+
+# Make sure to link to the `zswagcl` target
+target_link_libraries(${PROJECT_NAME}
+    ${PROJECT_NAME}-zserio-cpp zswagcl)
+```
+
+The `add_executable` command above references the file `myapp/client.cpp`,
+which contains the code to actually use the zswag C++ client.
+
+```cpp
+#include "zswagcl/oaclient.hpp"
+#include <iostream>
+#include "myapp_services/services/MyService.h"
+
+using namespace zswagcl;
+using namespace httpcl;
+namespace MyService = myapp_services::services::MyService;
+
+int main (int argc, char* argv[])
+{
+    // Assume that the server provides its OpenAPI definition here
+    auto openApiUrl = "http://localhost:5000/openapi.json";
+    
+    // Create an HTTP client to be used by our OpenAPI client
+    auto httpClient = std::make_unique<HttpLibHttpClient>();
+    
+    // Fetch the OpenAPI configuration using the HTTP client
+    auto openApiConfig = fetchOpenAPIConfig(openApiUrl, *httpClient);
+    
+    // Create a Zserio reflection-based OpenAPI client that
+    // uses the OpenAPI configuration we just retrieved.
+    auto openApiClient = OAClient(openApiConfig, std::move(httpClient));
+        
+    // Create a MyService client based on the OpenApi-Client
+    // implementation of the zserio::IServiceClient interface.
+    auto myServiceClient = MyService::Client(openApiClient);
+    
+    // Create the request object
+    auto request = myapp_services::services::Request(2);
+
+    // Invoke the REST endpoint. Mind that your method-
+    // name from the schema is appended with a "...Method" suffix.
+    auto response = myServiceClient.myApiMethod(request);
+    
+    // Print the response
+    std::cout << "Got " << response.getValue() << std::endl;
+}
+```
+
+**Note:** While connecting, `HttpLibHttpClient` will also use ...
+1. [Persistent HTTP configuration](#persistent-http-headers-proxy-cookie-and-authentication).
+2. Additional HTTP query/header/cookie/proxy/basic-auth configs passed
+   into the `OAClient` constructor using an instance of `httpcl::Config`.
+   You can include this class via `#include "httpcl/http-settings.hpp"`.
+   The additional `Config` will only enrich, not overwrite the
+   default persistent configuration. If you would like to prevent persistent
+   config from being considered at all, set `HTTP_SETTINGS_FILE` to empty,
+   e.g. via `setenv`.
+
+## Client Environment Settings
+
+Both the Python and C++ Clients can be configured using the following
+environment variables:
+
+| Variable Name | Details   |
+| ------------- | --------- |
+| `HTTP_SETTINGS_FILE` | Path to settings file for HTTP proxies and authentication, see [next section](#persistent-http-headers-proxy-cookie-and-authentication) |
+| `HTTP_LOG_LEVEL` | Verbosity level for console/log output. Set to `debug` for detailed output. |
+| `HTTP_LOG_FILE` | Logfile-path (including filename) to redirect console output. The log will rotate with three files (`HTTP_LOG_FILE`, `HTTP_LOG_FILE-1`, `HTTP_LOG_FILE-2`). |
+| `HTTP_LOG_FILE_MAXSIZE` | Maximum size of the logfile, in bytes. Defaults to 1GB. |
+| `HTTP_TIMEOUT` | Timeout for HTTP requests (connection+transfer) in seconds. Defaults to 60s. |
+| `HTTP_SSL_STRICT` | Set to any nonempty value for strict SSL certificate validation. |
+
+## Persistent HTTP Headers, Proxy, Cookie and Authentication
+
+Both the Python `OAClient` and C++ `HttpLibHttpClient` read a YAML file
+stored under a path which is given by the `HTTP_SETTINGS_FILE` environment
+variable. The YAML file contains a list of HTTP-related configs that are
+applied to HTTP requests based on a regular expression which is matched
+against the requested URL.
+
+For example, the following entry would match all requests due to the `.*`
+url-match-pattern:
+
+```yaml
+- url: .*
+  basic-auth:
+    user: johndoe
+    keychain: keychain-service-string
+  proxy:
+    host: localhost
+    port: 8888
+    user: test
+    keychain: ...
+  cookies:
+    key: value
+  headers:
+    key: value
+  query:
+    key: value
+  api-key: value
+```
+
+**Note:** For `proxy` configs, the credentials are optional.
+
+The **`api-key`** setting will be applied under the correct
+cookie/header/query parameter, if the service
+you are connecting to uses an [OpenAPI `apiKey` auth scheme](#authentication-schemes).
+
+Passwords can be stored in clear text by setting a `password` field instead
+of the `keychain` field. Keychain entries can be made with different tools
+on each platform:
+
+* [Linux `secret-tool`](https://www.marian-dan.ro/blog/storing-secrets-using-secret-tool) 
+* [macOS `add-generic-password`](https://www.netmeister.org/blog/keychain-passwords.html)
+* [Windows `cmdkey`](https://www.scriptinglibrary.com/languages/powershell/how-to-manage-secrets-and-passwords-with-credentialmanager-and-powershell/)
+
+## Swagger User Interface 
+
+If you have installed `pip install "connexion[swagger-ui]"`, you can view
+API docs of your service under `[/prefix]/ui`.
+
+## OpenAPI Options Interoperability
+
+The Server, Clients and Generator offer various degrees of freedom
+regarding the OpenAPI YAML file. The following sections detail which
+components support which aspects of OpenAPI. The difference in compliance
+is mostly due to limited development scopes. If you are missing a particular
+OpenAPI feature for a particular component, feel free to create an issue!
+
+**Note:** For all options that are not supported by `zswag.gen`, you
+will need to manually edit the OpenAPI YAML file to achieve the desired
+configuration. You will also need to edit the file manually to fill in
+meta-info (provider name, service version, etc.).
+
+### HTTP method
+
+To change the **HTTP method**, the desired method name is placed 
+as the key under the method path, such as in the following example:
+```yaml
+paths:
+  /methodName:
+    {get|post|put|delete}:
+      ...
+```
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `get` `post` `put` `delete` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `patch` | ❌️ | ❌️ | ❌️ | ❌️ |
+
+**Note:** Patch is unsupported, because the required semantics of
+a partial object update cannot be realized in the zserio transport
+layer interface.
+
+### Request Body
+
+A server can instruct clients to transmit their zserio request object in the
+request body when using HTTP `post`, `put` or `delete`.
+This is done by setting the OpenAPI `requestBody/content` to
+`application/x-zserio-object`:
+
+```yaml
+requestBody:
+  content:
+    application/x-zserio-object:
+      schema:
+        type: string
+```
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `application/x-zserio-object` | ✔️ | ✔️ | ✔️ | ✔️ |
+
+### URL Blob Parameter
+
+Zswag tools support an additional OpenAPI method parameter
+field called `x-zserio-request-part`. Through this field,
+a service provider can express that a certain request parameter
+only contains a part of, or the whole zserio request object.
+When parameter contains the whole request object, `x-zserio-request-part`
+should be set to an asterisk (`*`):
+
+```yaml
+parameters:
+- description: ''
+  in: query|path|header
+  name: parameterName
+  required: true
+  x-zserio-request-part: "*"
+  schema:
+    format: string|byte|base64|base64url|hex|binary
+```
+
+About the `format` specifier value:
+* Both `string` and `binary` result in a raw URL-encoded string buffer.
+* Both `byte` and `base64` result in a standard Base64-encoded value.
+  The `base64url` option indicates URL-safe Base64 format.
+* The `hex` encoding produces a hexadecimal encoding of the request blob.
+
+**Note:** When a parameter is passed with `in=path`, its value
+**must not be empty**. This holds true for strings and bytes,
+but also for arrays (see below).
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `x-zserio-request-part: *` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `format: string` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `format: byte` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `format: hex` | ✔️ | ✔️ | ✔️ | ✔️ |
+
+### URL Scalar Parameter
+
+Using `x-zserio-request-part`, it is also possible to transfer
+only a single scalar (nested) member of the request object:
+
+```yaml
+parameters:
+- description: ''
+  in: query|path|header
+  name: parameterName
+  required: true
+  x-zserio-request-part: "[parent.]*member"
+  schema:
+    format: string|byte|base64|base64url|hex|binary
+```
+
+In this case, `x-zserio-request-part` should point to a scalar type,
+such as `uint8`, `float32`, `string` etc.
+
+The `format` value effect remains as explained above. A small
+difference exists for integer types: Their hexadecimal representation
+will be the natural numeric one, not binary.
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `x-zserio-request-part: <[parent.]*member>` | ✔️ | ✔️ | ✔️ | ✔️ |
+
+### URL Array Parameter
+
+The `x-zserio-request-part` may also point to an array member of
+the zserio request struct, like so:
+
+```yaml
+parameters:
+- description: ''
+  in: query|path|header
+  style: form|simple|label|matrix
+  explode: true|false
+  name: parameterName
+  required: true
+  x-zserio-request-part: "[parent.]*array_member"
+  schema:
+    format: string|byte|base64|base64url|hex|binary
+```
+
+In this case, `x-zserio-request-part` should point to an array of
+scalar types. The array will be encoded according
+to the [format, style and explode](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md#parameter-object)
+specifiers.
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `x-zserio-request-part: <[parent.]*array_member>`  | ✔️ | ✔️ | ✔️ | ✔️ |
+| `style: simple` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `style: form` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `style: label` | ✔️ | ✔️ | ❌ | ✔️ |
+| `style: matrix` | ✔️ | ✔️ | ❌ | ✔️ |
+| `explode: true` | ✔️ | ✔️ | ✔️ | ✔️ |
+| `explode: false` | ✔️ | ✔️ | ✔️ | ✔️ |
+
+### URL Compound Parameter
+
+In this case, `x-zserio-request-part` points to a zserio compound struct
+instead of a field with a scalar value. **This is currently not supported.**
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `x-zserio-request-part: <[parent.]*compound_member>`  | ❌️ | ❌️ | ❌️ | ❌️ |
+
+### Server URL Base Path
+
+OpenAPI allows for a `servers` field in the spec that lists URL path prefixes
+under which the specified API may be reached. The OpenAPI clients
+looks into this list to determine a URL base path from
+the first entry in this list. A sample entry might look as follows:
+
+```
+servers:
+- http://unused-host-information/path/to/my/api
+``` 
+
+The OpenAPI client will then call methods with your specified host
+and port, but prefix the `/path/to/my/api` string. 
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `servers`  | ✔️ | ✔️ | ✔️ | ✔️ |
+
+### Authentication Schemes
+
+To facilitate the communication of authentication needs for the whole or parts
+of a service, OpenAPI allows for `securitySchemes` and `security` fields in the spec.
+Please refer to the relevant parts of the [OpenAPI 3 specification](https://swagger.io/docs/specification/authentication/) for some
+examples on how to integrate these fields into your spec.
+
+Zswag currently understands the following authentication schemes:
+
+* **HTTP Basic Authorization:** If a called endpoint requires HTTP basic auth,
+  zswag will verify that the HTTP config contains basic-auth credentials.
+  If there are none, zswag will throw a descriptive runtime error.
+* **HTTP Bearer Authorization:** If a called endpoint requires HTTP bearer auth,
+  zswag will verify that the HTTP config contains a header with the
+  key name `Authorization` and the value `Bearer <token>`, *case-sensitive*.
+* **API-Key Cookie:** If a called endpoint requires a Cookie API-Key,
+  zswag will either apply [the `api-key` setting](#persistent-http-headers-proxy-cookie-and-authentication), or verify that the
+  HTTP config contains a cookie with the required name, *case-sensitive*.
+* **API-Key Query Parameter:** If a called endpoint requires a Query API-Key,
+  zswag will either apply the `api-key` setting, or verify that the
+  HTTP config contains a query key-value pair with the required name, *case-sensitive*.
+* **API-Key Header:** If a called endpoint requires an API-Key Header,
+  zswag will either apply the `api-key` setting, or verify that the
+  HTTP config contains a header key-value pair with the required name, *case-sensitive*.
+
+**Note**: If you don't want to pass your Basic-Auth/Bearer/Query/Cookie/Header
+credential through your [persistent config](#persistent-http-headers-proxy-cookie-and-authentication),
+you can pass a `httpcl::Config`/[`HTTPConfig`](#using-the-python-client) object to the `OAClient`/[`OAClient`](#using-the-python-client).
+constructor in C++/Python with the relevant detail.
+
+#### Component Support
+
+| Feature            | C++ Client | Python Client | OAServer | zswag.gen |
+| ------------------ | ---------- | ------------- | -------- | --------- |
+| `HTTP Basic-Auth` `HTTP Bearer-Auth` `Cookie API-Key` `Header API-Key` `Query API-Key`  | ✔️ | ✔️ | ✔️(**) | ✔️ |
+| `OpenID Connect` `OAuth2`  | ❌️ | ❌️ | ✔️(**) | ❌️ |
+
+**(\*\*)**: The server support for all authentication schemes depends on your
+configuration of the WSGI server (Apache/Nginx/...) which wraps the zswag Flask app.
```

## Comparing `zswag-1.5.0.dist-info/RECORD` & `zswag-1.6.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-zswag/__init__.py,sha256=bYX0cT3vrmyIPHoJtLhuaphO49SQ-DtPghHK_iqNKrw,79
-zswag/app.py,sha256=Tq_kZV4i-A8RK1hwsZlRC9t79Zctv0DnhuxfXQYaYZE,8574
-zswag/doc.py,sha256=OSeP2LR6Nr5lNW72iWrq0IMUsgGZcJOYWSziDFW4Mzs,4402
-zswag/gen.py,sha256=qwOZtLQH0MNj1F4RqhdxgR6sis99OTLkamYNBvz2hnE,28993
-zswag/reflect.py,sha256=FJeUKeCzrFzDNktHszg77AbPMgQWLIddpH2eknmH64s,10594
-zswag/test/calc/__init__.py,sha256=pMevxf47n8C6z3kyLj9iqcMT9yADUj8pyaCK6NBxvfo,240
-zswag/test/calc/__main__.py,sha256=X9zPuhlUmZ2mAlOU9i9f-ka9yHea98KR3JCPKR9Jips,767
-zswag/test/calc/api.yaml,sha256=-Y16Z6Hw2sRAREY2sIQmj2MrBvvvJb2SFOzBVcSZn5c,6738
-zswag/test/calc/calculator.zs,sha256=oRMBMH9753ssw6MJrKlCSRi5YcyyJVMlrUS6s1AaVoM,1139
-zswag/test/calc/client.py,sha256=LlyF-yL2wGaDgqf4HpbtbK7265K7gc1TOYMYL787zXM,3963
-zswag/test/calc/server.py,sha256=dzEXZE0_wpZv55yg602Y3BxAU7QCCF_6H37cjGO__9U,1355
-zswag-1.5.0.dist-info/LICENSE,sha256=82HFE2tG6k1v7YD065fi3PSy0tCuV68AM7WXaA4Y2Mc,1557
-zswag-1.5.0.dist-info/METADATA,sha256=XX4kE2fiS1GkxVSR5dbKMlQk_bU-fb8_lKPPP4RkAeM,34064
-zswag-1.5.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-zswag-1.5.0.dist-info/top_level.txt,sha256=13gM6HyInsF9lF5Q31lOLebRu2AmFc4KbYZcuWZPY48,6
-zswag-1.5.0.dist-info/RECORD,,
+zswag/__init__.py,sha256=o_bE6m0juhfJTjGWX0PjOVh_ngRL_EiWW2uYqUqvHeo,75
+zswag/app.py,sha256=58H1R2mr36qt4VIY6DmJDTgvPdN2o4Eb2caiA0g7lvw,8373
+zswag/doc.py,sha256=iJFMGEXruFSa9_MeyYnqqsUERXJOCWdqVQPiLiwKuBM,4279
+zswag/gen.py,sha256=6Z1FBeKUrWU1UW4_nFFtPgiCARXhcvoGvWZcr8UYN-4,28403
+zswag/reflect.py,sha256=LH9avzFS7Tv_SHu3KbnnBbutm163LU2sSn-Ma7S1Dmc,10347
+zswag/test/calc/__init__.py,sha256=9mBc19ckAvk4LF6LAKRPk8jdXv7irucJ3-dBQYyvBn4,231
+zswag/test/calc/__main__.py,sha256=jH5f8FNJ2BlFLoIBIc0tAiSEv1Dn-WxgYSra1Dy7GVs,743
+zswag/test/calc/api.yaml,sha256=iPRSRyyo1bksV71mC3Yzq4LhCLJ63VWSrXDCYOX_Zr0,6462
+zswag/test/calc/calculator.zs,sha256=30bXQG9N_Lc9c01CJGJi3aChacTfE_HC_5_iTZNaTFg,1036
+zswag/test/calc/client.py,sha256=wI5j7FB17gYR6C3JoorrOpDgSzpAT9oHYZyeMKNLrao,3831
+zswag/test/calc/server.py,sha256=0L1gqO3JcdrNE4MV2xOMkvUC31sahVhuepIWDqJyPGA,1304
+zswag-1.6.0.dist-info/LICENSE,sha256=JeNdz5tf1QH7CIw_i5yqTWtlyhczLpjj3yhOyCRTEHE,1528
+zswag-1.6.0.dist-info/METADATA,sha256=gXKjNJmlfRRPZeuMQixQ5OMKG3TrYzwUH_AxWkAVBDM,32150
+zswag-1.6.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+zswag-1.6.0.dist-info/top_level.txt,sha256=13gM6HyInsF9lF5Q31lOLebRu2AmFc4KbYZcuWZPY48,6
+zswag-1.6.0.dist-info/RECORD,,
```

