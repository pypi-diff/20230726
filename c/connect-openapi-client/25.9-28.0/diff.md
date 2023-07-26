# Comparing `tmp/connect-openapi-client-25.9.tar.gz` & `tmp/connect_openapi_client-28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect-openapi-client-25.9.tar", max compression
+gzip compressed data, was "connect_openapi_client-28.0.tar", max compression
```

## Comparing `connect-openapi-client-25.9.tar` & `connect_openapi_client-28.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0    11357 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/LICENSE
--rw-r--r--   0        0        0     1869 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/README.md
--rw-r--r--   0        0        0      298 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/cnct/__init__.py
--rw-r--r--   0        0        0      183 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/cnct/rql.py
--rw-r--r--   0        0        0      373 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/__init__.py
--rw-r--r--   0        0        0      310 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/constants.py
--rw-r--r--   0        0        0        0 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/contrib/__init__.py
--rw-r--r--   0        0        0      242 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/contrib/locust/__init__.py
--rw-r--r--   0        0        0     1641 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/contrib/locust/user.py
--rw-r--r--   0        0        0     1100 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/exceptions.py
--rw-r--r--   0        0        0     6723 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/fluent.py
--rw-r--r--   0        0        0     6907 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/help_formatter.py
--rw-r--r--   0        0        0     1655 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/logger.py
--rw-r--r--   0        0        0     6040 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/mixins.py
--rw-r--r--   0        0        0      471 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/__init__.py
--rw-r--r--   0        0        0    12633 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/base.py
--rw-r--r--   0        0        0      191 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/exceptions.py
--rw-r--r--   0        0        0     5175 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/iterators.py
--rw-r--r--   0        0        0    13052 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/mixins.py
--rw-r--r--   0        0        0    14635 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/resourceset.py
--rw-r--r--   0        0        0     6410 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/openapi.py
--rw-r--r--   0        0        0      189 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/rql/__init__.py
--rw-r--r--   0        0        0     8124 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/rql/base.py
--rw-r--r--   0        0        0     1992 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/rql/utils.py
--rw-r--r--   0        0        0      239 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/testing/__init__.py
--rw-r--r--   0        0        0      825 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/testing/fixtures.py
--rw-r--r--   0        0        0     4043 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/testing/fluent.py
--rw-r--r--   0        0        0      268 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/__init__.py
--rw-r--r--   0        0        0     1051 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/base.py
--rw-r--r--   0        0        0     3751 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/mixins.py
--rw-r--r--   0        0        0     5084 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/resourceset.py
--rw-r--r--   0        0        0     1246 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/utils.py
--rw-r--r--   0        0        0      401 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/version.py
--rw-r--r--   0        0        0     2499 2022-09-22 13:24:58.460051 connect-openapi-client-25.9/pyproject.toml
--rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 connect-openapi-client-25.9/setup.py
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 connect-openapi-client-25.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 08:14:36.239993 connect_openapi_client-28.0/LICENSE
+-rw-r--r--   0        0        0     2143 2023-07-26 08:14:36.239993 connect_openapi_client-28.0/README.md
+-rw-r--r--   0        0        0      298 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/cnct/__init__.py
+-rw-r--r--   0        0        0      184 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/cnct/rql.py
+-rw-r--r--   0        0        0      374 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/constants.py
+-rw-r--r--   0        0        0        0 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/contrib/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/contrib/locust/__init__.py
+-rw-r--r--   0        0        0     1640 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/contrib/locust/user.py
+-rw-r--r--   0        0        0     1100 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/exceptions.py
+-rw-r--r--   0        0        0     8377 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/fluent.py
+-rw-r--r--   0        0        0     6906 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/help_formatter.py
+-rw-r--r--   0        0        0     2201 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/logger.py
+-rw-r--r--   0        0        0     7567 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/mixins.py
+-rw-r--r--   0        0        0      472 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/models/__init__.py
+-rw-r--r--   0        0        0    11842 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/models/base.py
+-rw-r--r--   0        0        0      191 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/models/exceptions.py
+-rw-r--r--   0        0        0     5173 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/models/iterators.py
+-rw-r--r--   0        0        0    26077 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/models/mixins.py
+-rw-r--r--   0        0        0    14313 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/models/resourceset.py
+-rw-r--r--   0        0        0     6560 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/openapi.py
+-rw-r--r--   0        0        0      189 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/rql/__init__.py
+-rw-r--r--   0        0        0     8425 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/rql/base.py
+-rw-r--r--   0        0        0     1992 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/rql/utils.py
+-rw-r--r--   0        0        0      299 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/__init__.py
+-rw-r--r--   0        0        0     2031 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/fixtures.py
+-rw-r--r--   0        0        0     6469 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/fluent.py
+-rw-r--r--   0        0        0      268 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/models/__init__.py
+-rw-r--r--   0        0        0     1055 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/models/base.py
+-rw-r--r--   0        0        0     4164 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/models/mixins.py
+-rw-r--r--   0        0        0     6256 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/testing/models/resourceset.py
+-rw-r--r--   0        0        0     1247 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/utils.py
+-rw-r--r--   0        0        0      401 2023-07-26 08:14:36.243993 connect_openapi_client-28.0/connect/client/version.py
+-rw-r--r--   0        0        0     3243 2023-07-26 08:16:42.637186 connect_openapi_client-28.0/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 connect_openapi_client-28.0/PKG-INFO
```

### Comparing `connect-openapi-client-25.9/LICENSE` & `connect_openapi_client-28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.9/README.md` & `connect_openapi_client-28.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -13,24 +13,30 @@
 
 Due to its REPL-friendly nature, using the CloudBlue Connect OpenAPI specifications it allows developers to learn and
 play with the CloudBlue Connect API using a python REPL like [jupyter](https://jupyter.org/) or [ipython](https://ipython.org/).
 
 
 ## Install
 
-`Connect Python OpenAPI Client` requires python 3.7 or later.
+`Connect Python OpenAPI Client` requires python 3.8 or later.
 
 
 `Connect Python OpenAPI Client` can be installed from [pypi.org](https://pypi.org/project/connect-openapi-client/) using pip:
 
 ```
 $ pip install connect-openapi-client
 ```
 
 
+## Development
+We use `isort` library to order and format our imports, and `black` - to format the code. 
+We check it using `flake8-isort` and `flake8-black` libraries (automatically on `flake8` run).  
+For convenience you may run `isort . && black .` to format the code.
+
+
 ## Documentation
 
 [`Connect Python OpenAPI Client` documentation](https://connect-openapi-client.readthedocs.io/en/latest/) is hosted on the _Read the Docs_ service.
 
 
 ## License
```

### Comparing `connect-openapi-client-25.9/connect/client/contrib/locust/user.py` & `connect_openapi_client-28.0/connect/client/contrib/locust/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import time
 
 from locust import HttpUser
-
 from requests import RequestException
 
 from connect.client import ConnectClient
 
 
 class _LocustConnectClient(ConnectClient):
     def __init__(self, base_url, request_event, user, *args, **kwargs):
```

### Comparing `connect-openapi-client-25.9/connect/client/exceptions.py` & `connect_openapi_client-28.0/connect/client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 from http import HTTPStatus
 
 
 class ClientError(Exception):
     def __init__(self, message=None, status_code=None, error_code=None, errors=None, **kwargs):
         self.message = message
```

### Comparing `connect-openapi-client-25.9/connect/client/help_formatter.py` & `connect_openapi_client-28.0/connect/client/help_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 import inflect
+from connect.utils.terminal.markdown import render
 
 from connect.client.models import (
+    NS,
     Action,
     AsyncAction,
     AsyncCollection,
     AsyncNS,
     AsyncResource,
     AsyncResourceSet,
     Collection,
-    NS,
     Resource,
     ResourceSet,
 )
-from connect.utils.terminal.markdown import render
 
 
 _COL_HTTP_METHOD_TO_METHOD = {
     'get': '.all(), .filter(), .first(), .last()',
     'post': '.create()',
 }
 
 
 class DefaultFormatter:
-
     def __init__(self, specs):
         self._specs = specs
         self._p = inflect.engine()
 
     def format_client(self):
         lines = [
             f'# Welcome to {self._specs.title} {self._specs.version}',
```

### Comparing `connect-openapi-client-25.9/connect/client/models/base.py` & `connect_openapi_client-28.0/connect/client/models/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,118 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 from connect.client.models.mixins import (
     ActionMixin,
     AsyncActionMixin,
     AsyncCollectionMixin,
     AsyncResourceMixin,
     CollectionMixin,
     ResourceMixin,
 )
 from connect.client.models.resourceset import AsyncResourceSet, ResourceSet
 from connect.client.rql import R
 
 
 class _NSBase:
-    """
-    A namespace is a group of related collections.
-    """
-
     def __init__(self, client, path):
-        """
-        Create a new NS instance.
-
-        :param client: the client instance
-        :type client: ConnectClient
-        :param path: path name of the namespace
-        :type path: str
-        """
         self._client = client
         self._path = path
 
     @property
-    def path(self):
+    def path(self) -> str:
         return self._path
 
     def __getattr__(self, name):
-        """
-        Returns a collection object by its name.
-
-        :param name: the name of the Collection object.
-        :type name: str
-        :return: The Collection named ``name``.
-        :rtype: Collection
-        """
         if '_' in name:
             name = name.replace('_', '-')
         return self.collection(name)
 
     def __iter__(self):
         raise TypeError('A Namespace object is not iterable.')
 
     def __call__(self, name):
         return self.ns(name)
 
-    def collection(self, name):
+    def collection(self, name: str):
         """
-        Returns the collection called ``name``.
+        Returns a `[Async]Collection` object nested under this namespace object
+        identified by its name.
+
+        Usage:
 
-        :param name: The name of the collection.
-        :type name: str
-        :raises TypeError: if the ``name`` is not a string.
-        :raises ValueError: if the ``name`` is blank.
-        :raises NotFoundError: if the ``name`` does not exist.
-        :return: The collection called ``name``.
-        :rtype: Collection
+        ```py3
+        devops_ns = client.ns('devops')
+        services = devops_ns.collection('products')
+        ```
+
+        Concise form:
+
+        ```py3
+        services = client('devops').services
+        ```
+
+        Args:
+            name (str): The name of the collection to access.
+
+        Returns:
+            (Union[Collection, AsyncCollection]):  Returns an object nested under this namespace
+                object identified by its name.
         """
+
         if not isinstance(name, str):
             raise TypeError('`name` must be a string.')
 
         if not name:
             raise ValueError('`name` must not be blank.')
 
         return self._get_collection_class()(
             self._client,
             f'{self._path}/{name}',
         )
 
-    def ns(self, name):
+    def ns(self, name: str):
         """
-        Returns the namespace called ``name``.
+        Returns a `[Async]Namespace` object nested under this namespace
+        identified by its name.
+
+        Usage:
+
+        ```py3
+        subscriptions_ns = client.ns('subscriptions')
+        nested_ns = subcriptions_ns.ns('nested')
+        ```
+
+        Concise form:
+
+        ```py3
+        nested_ns = client('subscriptions')('nested')
+        ```
 
-        :param name: The name of the namespace.
-        :type name: str
-        :raises TypeError: if the ``name`` is not a string.
-        :raises ValueError: if the ``name`` is blank.
-        :return: The namespace called ``name``.
-        :rtype: NS
+        Args:
+            name (str): The name of the namespace to access.
+
+        Returns:
+            (Union[NS, AsyncNS]): Returns an object nested under this namespace
+                identified by its name.
         """
         if not isinstance(name, str):
             raise TypeError('`name` must be a string.')
 
         if not name:
             raise ValueError('`name` must not be blank.')
 
         return self._get_namespace_class()(
             self._client,
             f'{self._path}/{name}',
         )
 
     def help(self):
-        """
-        Output the namespace documentation to the console.
-
-        :return: self
-        :rtype: NS
-        """
         self._client.print_help(self)
         return self
 
     def _get_collection_class(self):
         raise NotImplementedError()
 
     def _get_namespace_class(self):
@@ -130,101 +132,82 @@
         return AsyncCollection
 
     def _get_namespace_class(self):
         return AsyncNS
 
 
 class _CollectionBase:
-    """
-    A collection is a group of operations on a resource.
-    """
     def __init__(self, client, path):
-        """
-        Create a new Collection instance.
-
-        :param client: the client instance
-        :type client: ConnectClient
-        :param path: path name of the collection
-        :type path: str
-        """
         self._client = client
         self._path = path
 
     @property
     def path(self):
         return self._path
 
     def __iter__(self):
         raise TypeError('A Collection object is not iterable.')
 
     def __getitem__(self, resource_id):
-        """
-        Return a Resource object representing the resource
-        identified by ``resource_id``.
-
-        :param resource_id: The identifier of the resource
-        :type resource_id: str, int
-        :return: the Resource instance identified by ``resource_id``.
-        :rtype: Resource
-        """
         return self.resource(resource_id)
 
     def __call__(self, name):
         return self.action(name)
 
     def all(self):
         """
-        Return a ResourceSet instance.
+        Returns a `[Async]ResourceSet` object that that allow to access all the resources that
+        belong to this collection.
 
-        :return: a ResourceSet instance.
-        :rtype: ResourceSet
+        Returns:
+            (Union[ResourceSet, AsyncResourceSet]): Returns an object that that allow to access
+                all the resources that belong to this collection.
         """
         return self._get_resourceset_class()(
             self._client,
             self._path,
         )
 
     def filter(self, *args, **kwargs):
         """
-        Returns a ResourceSet object.
+        Returns a `[Async]ResourceSet` object.
         The returned ResourceSet object will be filtered based on
         the arguments and keyword arguments.
 
         Arguments can be RQL filter expressions as strings
         or R objects.
 
-        Ex.
-
-        .. code-block:: python
+        Usage:
 
-            rs = collection.filter('eq(field,value)', 'eq(another.field,value2)')
-            rs = collection.filter(R().field.eq('value'), R().another.field.eq('value2'))
+        ```py3
+        rs = collection.filter('eq(field,value)', 'eq(another.field,value2)')
+        rs = collection.filter(R().field.eq('value'), R().another.field.eq('value2'))
+        ```
 
-        All the arguments will be combined with logical ``and``.
+        All the arguments will be combined with logical **and**.
 
-        Filters can be also specified as keyword argument using the ``__`` (double underscore)
+        Filters can be also specified as keyword argument using the **__** (double underscore)
         notation.
 
-        Ex.
-
-        .. code-block:: python
-
-            rs = collection.filter(
-                field=value,
-                another__field=value,
-                field2__in=('a', 'b'),
-                field3__null=True,
-            )
+        Usage:
 
-        Also keyword arguments will be combined with logical ``and``.
+        ```py3
+        rs = collection.filter(
+            field=value,
+            another__field=value,
+            field2__in=('a', 'b'),
+            field3__null=True,
+        )
+        ```
 
+        Also keyword arguments will be combined with logical **and**.
 
-        :raises TypeError: If arguments are neither strings nor R objects.
-        :return: A ResourceSet with the filters applied.
-        :rtype: ResourceSet
+        Returns:
+            (Union[ResourceSet, AsyncResourceSet]): The returned ResourceSet object will be
+                filtered based on the arguments and keyword arguments.
         """
         query = R()
         for arg in args:
             if isinstance(arg, str):
                 query &= R(_expr=arg)
                 continue
             if isinstance(arg, R):
@@ -237,64 +220,73 @@
 
         return self._get_resourceset_class()(
             self._client,
             self._path,
             query=query,
         )
 
-    def resource(self, resource_id):
+    def resource(self, resource_id: str):
         """
-        Returns an Resource object.
+        Returns a `[Async]Resource` object that represent a resource that belong to
+        this collection identified by its unique identifier.
+
+        Usage:
+
+        ```py3
+        resource = client.collection('products').resource('PRD-000-111-222')
+        ```
+
+        Concise form:
 
-        :param resource_id: The resource identifier.
-        :type resource_id: str, int
-        :return: The Resource identified by ``resource_id``.
-        :rtype: Resource
+        ```py3
+        resource = client.products['PRD-000-111-222']
+        ```
+
+        Args:
+            resource_id (str): The unique identifier of the resource.
+
+        Returns:
+            (Union[Resource, AsyncResource]): Returns an object that represent a resource that
+                belong to this collection identified by its unique identifier.
         """
         if not isinstance(resource_id, (str, int)):
             raise TypeError('`resource_id` must be a string or int.')
 
         if not resource_id:
             raise ValueError('`resource_id` must not be blank.')
 
         return self._get_resource_class()(
             self._client,
             f'{self._path}/{resource_id}',
         )
 
-    def action(self, name):
+    def action(self, name: str):
         """
-        Returns the action called ``name``.
+        Returns an `[Async]Action` object that represent an action to perform
+        on this collection identified by its name.
+
+        Args:
+            name (str): The name of the action to perform.
 
-        :param name: The name of the action.
-        :type name: str
-        :raises TypeError: if the ``name`` is not a string.
-        :raises ValueError: if the ``name`` is blank.
-        :raises NotFoundError: if the ``name`` does not exist.
-        :return: The action called ``name``.
-        :rtype: Action
+        Returns:
+            (Union[Action, AsyncAction]): Returns an object that represent an action to perform
+                on this collection identified by its name.
         """
         if not isinstance(name, str):
             raise TypeError('`name` must be a string.')
 
         if not name:
             raise ValueError('`name` must not be blank.')
 
         return self._get_action_class()(
             self._client,
             f'{self._path}/{name}',
         )
 
     def help(self):
-        """
-        Output the collection documentation to the console.
-
-        :return: self
-        :rtype: Collection
-        """
         self._client.print_help(self)
         return self
 
     def _get_resource_class(self):
         return NotImplementedError()  # pragma: no cover
 
     def _get_resourceset_class(self):
@@ -323,102 +315,110 @@
         return AsyncResourceSet
 
     def _get_action_class(self):
         return AsyncAction
 
 
 class _ResourceBase:
-    """Represent a generic resource."""
     def __init__(self, client, path):
-        """
-        Create a new Resource instance.
-
-        :param client: the client instance
-        :type client: ConnectClient
-        :param path: path name of the resource
-        :type path: str
-        :param specs: OpenAPI specs, defaults to None
-        :type specs: ResourceInfo, optional
-        """
         self._client = client
         self._path = path
 
     @property
     def path(self):
         return self._path
 
     def __getattr__(self, name):
-        """
-        Returns a nested Collection object called ``name``.
-
-        :param name: The name of the Collection to retrieve.
-        :type name: str
-        :return: a Collection called ``name``.
-        :rtype: Collection
-        """
         if '_' in name:
             name = name.replace('_', '-')
         return self.collection(name)
 
     def __call__(self, name):
         return self.action(name)
 
-    def collection(self, name):
+    def collection(self, name: str):
         """
-        Returns the collection called ``name``.
+        Returns a `[Async]Collection` object nested under this resource object
+        identified by its name.
 
-        :param name: The name of the collection.
-        :type name: str
-        :raises TypeError: if the ``name`` is not a string.
-        :raises ValueError: if the ``name`` is blank.
-        :raises NotFoundError: if the ``name`` does not exist.
-        :return: The collection called ``name``.
-        :rtype: Collection
-        """
+        Usage:
+
+        ```py3
+        environments = (
+            client.ns("devops")
+            .collection("services")
+            .resource("SRVC-0000-1111")
+            .collection("environments")
+        )
+        ```
+
+        Concise form:
+
+        ```py3
+        services = client('devops').services['SRVC-0000-1111'].environments
+        ```
+
+        Args:
+            name (str): The name of the collection to access.
+
+        Returns:
+            (Union[Collection, AsyncCollection]): Returns an object nested under this resource
+                object identified by its name.
+        """  # noqa: E501
         if not isinstance(name, str):
             raise TypeError('`name` must be a string.')
 
         if not name:
             raise ValueError('`name` must not be blank.')
 
         return self._get_collection_class()(
             self._client,
             f'{self._path}/{name}',
         )
 
-    def action(self, name):
+    def action(self, name: str):
         """
-        Returns the action called ``name``.
+        Returns an `[Async]Action` object that can be performed on this this resource object
+        identified by its name.
+
+        Usage:
+
+        ```py3
+        approve_action = (
+            client.collection('requests')
+            .resource('PR-000-111-222')
+            .action('approve')
+        )
+        ```
 
-        :param name: The name of the action.
-        :type name: str
-        :raises TypeError: if the ``name`` is not a string.
-        :raises ValueError: if the ``name`` is blank.
-        :raises NotFoundError: if the ``name`` does not exist.
-        :return: The action called ``name``.
-        :rtype: Action
+        Concise form:
+
+        ```py3
+        approve_action = client.requests[''PR-000-111-222']('approve')
+        ```
+
+        Args:
+            name (str): The name of the action to perform.
+
+        Returns:
+            (Union[Action, AsyncAction]): Returns an object that can be performed on this this
+                resource object identified by its name.
         """
         if not isinstance(name, str):
             raise TypeError('`name` must be a string.')
 
         if not name:
             raise ValueError('`name` must not be blank.')
 
         return self._get_action_class()(
             self._client,
             f'{self._path}/{name}',
         )
 
     def help(self):
-        """
-        Output the resource documentation to the console.
-
-        :return: self
-        :rtype: Resource
-        """
         self._client.print_help(self)
         return self
 
     def _get_collection_class(self):
         raise NotImplementedError()
 
     def _get_action_class(self):
@@ -438,42 +438,23 @@
         return AsyncCollection
 
     def _get_action_class(self):
         return AsyncAction
 
 
 class _ActionBase:
-    """
-    This class represent an action that can be executed on a resource.
-    """
     def __init__(self, client, path):
-        """
-        Create a new Action instance.
-
-        :param client: the client instance
-        :type client: ConnectClient
-        :param path: path name of the action
-        :type path: str
-        :param specs: OpenAPI specs, defaults to None
-        :type specs: ActionInfo, optional
-        """
         self._client = client
         self._path = path
 
     @property
     def path(self):
         return self._path
 
     def help(self):
-        """
-        Output the action documentation to the console.
-
-        :return: self
-        :rtype: Action
-        """
         self._client.print_help(self)
         return self
 
 
 class Action(_ActionBase, ActionMixin):
     pass
```

### Comparing `connect-openapi-client-25.9/connect/client/models/iterators.py` & `connect_openapi_client-28.0/connect/client/models/iterators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 from connect.client.utils import get_values, parse_content_range
 
 
 class aiter:
     def __init__(self, values):
         self._values = iter(values)
@@ -29,15 +29,14 @@
         self._loaded = False
 
     def get_item(self, item):
         raise NotImplementedError('get_item must be implemented in subclasses.')
 
 
 class AbstractIterator(AbstractBaseIterator):
-
     def _load(self):
         if not self._loaded:
             self._rs._results, self._rs._content_range = self._execute_request()
             self._results_iterator = iter(self._rs._results)
             self._loaded = True
 
     def __next__(self):  # noqa: CCR001
@@ -80,15 +79,14 @@
         content_range = parse_content_range(
             self._client.response.headers.get('Content-Range'),
         )
         return results, content_range
 
 
 class AbstractAsyncIterator(AbstractBaseIterator):
-
     async def _load(self):
         if not self._loaded:
             self._rs._results, self._rs._content_range = await self._execute_request()
             self._results_iterator = iter(self._rs._results)
             self._loaded = True
 
     async def __anext__(self):  # noqa: CCR001
```

### Comparing `connect-openapi-client-25.9/connect/client/models/resourceset.py` & `connect_openapi_client-28.0/connect/client/models/resourceset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 import copy
 
 from connect.client.models.exceptions import NotYetEvaluatedError
 from connect.client.models.iterators import (
     AsyncResourceIterator,
     AsyncValuesListIterator,
     ResourceIterator,
     ValuesListIterator,
     aiter,
 )
-from connect.client.utils import parse_content_range, resolve_attribute
 from connect.client.rql import R
+from connect.client.utils import parse_content_range, resolve_attribute
 
 
 class _ResourceSetBase:
-    """
-    Represent a set of resources.
-    """
     def __init__(
         self,
         client,
         path,
         query=None,
     ):
-
         self._client = client
         self._path = path
         self._query = query or R()
         self._results = None
         self._limit = self._client.default_limit or 100
         self._offset = 0
         self._slice = None
@@ -52,35 +48,31 @@
 
     @property
     def content_range(self):
         return self._content_range
 
     def configure(self, **kwargs):
         """
-        Set the keyword arguments that needs to be forwarded to
-        the underlying ``requests`` call.
-
-        :return: This ResourceSet object.
-        :rtype: ResourceSet
+        Set the default keyword arguments that must be provided to the
+        underlying GET call on each page fetch.
         """
         copy = self._copy()
         copy._config = kwargs or {}
         return copy
 
-    def limit(self, limit):
+    def limit(self, limit: int):
         """
-        Set the number of results to be fetched from the remote
-        endpoint at once.
+        Set the number of results that must be fetched on each
+        HTTP call.
+
+        Args:
+            limit (int): Number of results to fetch in each HTTP call.
 
-        :param limit: maximum number of results to fetch in a batch.
-        :type limit: int
-        :raises TypeError: if `limit` is not an integer.
-        :raises ValueError: if `limit` is not positive non-zero.
-        :return: A copy of this ResourceSet class with the new limit.
-        :rtype: ResourceSet
+        Returns:
+            (ResourceSet): Returns a copy of the current ResourceSet with the limit applied.
         """
         if not isinstance(limit, int):
             raise TypeError('`limit` must be an integer.')
 
         if limit <= 0:
             raise ValueError('`limit` must be a positive, non-zero integer.')
 
@@ -88,69 +80,90 @@
         copy._limit = limit
         return copy
 
     def order_by(self, *fields):
         """
         Add fields for ordering.
 
-        :return: This ResourceSet object.
-        :rtype: ResourceSet
+        Usage:
+
+        ```py3
+        purchases = client.requests.all().order_by(
+            'asset.tiers.customer.name',
+            '-created'
+        )
+        ```
+        !!! note
+            To sort results in descending order the name of the field must
+            be prefixed with a `-` (minus) sign.
+
+        Returns:
+            (ResourceSet): Returns a copy of the current ResourceSet with the order applied.
         """
         copy = self._copy()
         copy._ordering.extend(fields)
         return copy
 
     def select(self, *fields):
         """
         Apply the RQL ``select`` operator to
         this ResourceSet object.
 
-        :return: This ResourceSet object.
-        :rtype: ResourceSet
+        Usage:
+
+        ```py3
+        purchases = client.requests.all().select(
+            '-asset.items',
+            '-asset.params',
+            'activation_key',
+        )
+        ```
+        !!! note
+            To unselect a field it must
+            be prefixed with a `-` (minus) sign.
+
+        Returns:
+            (ResourceSet): Returns a copy of the current ResourceSet with the select applied.
         """
         copy = self._copy()
         copy._select.extend(fields)
         return copy
 
     def filter(self, *args, **kwargs):
         """
         Applies filters to this ResourceSet object.
 
         Arguments can be RQL filter expressions as strings
         or R objects.
 
-        Ex.
+        Usage:
 
-        .. code-block:: python
+        ```py3
+        rs = rs.filter('eq(field,value)', 'eq(another.field,value2)')
+        rs = rs.filter(R().field.eq('value'), R().another.field.eq('value2'))
+        ```
 
-            rs = rs.filter('eq(field,value)', 'eq(another.field,value2)')
-            rs = rs.filter(R().field.eq('value'), R().another.field.eq('value2'))
+        All the arguments will be combined with logical `and`.
 
-        All the arguments will be combined with logical ``and``.
-
-        Filters can be also specified as keyword argument using the ``__`` (double underscore)
+        Filters can be also specified as keyword argument using the `__` (double underscore)
         notation.
 
-        Ex.
-
-        .. code-block:: python
-
-            rs = rs.filter(
-                field=value,
-                another__field=value,
-                field2__in=('a', 'b'),
-                field3__null=True,
-            )
-
-        Also keyword arguments will be combined with logical ``and``.
+        ```py3
+        rs = rs.filter(
+            field=value,
+            another__field=value,
+            field2__in=('a', 'b'),
+            field3__null=True,
+        )
+        ```
 
+        Also keyword arguments will be combined with logical `and`.
 
-        :raises TypeError: If arguments are neither strings nor R objects.
-        :return: This ResourceSet object.
-        :rtype: ResourceSet
+        Returns:
+            (ResourceSet): Returns a copy of the current ResourceSet with the filter applied.
         """
         copy = self._copy()
         for arg in args:
             if isinstance(arg, str):
                 copy._query &= R(_expr=arg)
                 continue
             if isinstance(arg, R):
@@ -163,65 +176,58 @@
 
         return copy
 
     def all(self):
         """
         Returns a copy of the current ResourceSet.
 
-        :return: A copy of this ResourceSet.
-        :rtype: ResourceSet
+        Returns:
+            (ResourceSet): Returns a copy of the current ResourceSet.
         """
         return self._copy()
 
-    def search(self, term):
+    def search(self, term: str):
         """
-        Create a copy of the current ResourceSet with
-        the search set to `term`.
+        Create a copy of the current ResourceSet applying the `search` RQL
+        operator equal to `term`.
 
-        :param term: The term to search for.
-        :type term: str
-        :return: A copy of the current ResourceSet.
-        :rtype: ResourceSet
+        Args:
+            term (str): The term to search for.
+
+        Returns:
+            (ResourceSet): Create a copy of the current ResourceSet applying the `search` RQL
+                operator equal to `term`.
         """
         copy = self._copy()
         copy._search = term
         return copy
 
     def values_list(self, *fields):
         """
         Returns a flat dictionary containing only the fields passed as arguments
         for each resource that belongs to this ResourceSet.
 
         Nested field can be specified using dot notation.
 
-        Ex.
-
-        .. code-block:: python
+        Usage:
 
+        ```py3
         values = rs.values_list('field', 'nested.field')
-
-        :return: A list of dictionaries containing field,value pairs.
-        :rtype: list
+        ```
         """
         if self._results:
             self._fields = fields
-            return [
-                self._get_values(item)
-                for item in self._results
-            ]
+            return [self._get_values(item) for item in self._results]
 
         copy = self._copy()
         copy._fields = fields
         return copy
 
     def _get_values(self, item):
-        return {
-            field: resolve_attribute(field, item)
-            for field in self._fields
-        }
+        return {field: resolve_attribute(field, item) for field in self._fields}
 
     def _build_qs(self):
         qs = ''
         if self._select:
             qs += f'&select({",".join(self._select)})'
         if self._query:
             qs += f'&{str(self._query)}'
@@ -237,18 +243,20 @@
 
         return url
 
     def _get_request_kwargs(self):
         config = copy.deepcopy(self._config)
         config.setdefault('params', {})
 
-        config['params'].update({
-            'limit': self._limit,
-            'offset': self._offset,
-        })
+        config['params'].update(
+            {
+                'limit': self._limit,
+                'offset': self._offset,
+            },
+        )
 
         if self._search:
             config['params']['search'] = self._search
 
         return config
 
     def _copy(self):
@@ -276,62 +284,42 @@
         ):
             raise ValueError('Negative indexing is not supported.')
 
         if isinstance(key, slice) and not (key.step is None or key.step == 0):
             raise ValueError('Indexing with step is not supported.')
 
     def help(self):
-        """
-        Output the ResourceSet documentation to the console.
-
-        :return: self
-        :rtype: ResourceSet
-        """
         self._client.print_help(self)
         return self
 
 
 class ResourceSet(_ResourceSetBase):
+    """
+    Represent a set of resources.
 
-    def __iter__(self):
-        """
-        Returns an iterator to iterate over the set of resources.
+    Usage:
 
-        :return: A resources iterator.
-        :rtype: ResourceSet
-        """
+    ```py3
+    for product in client.products.all().filter(
+        R().status.eq('published')
+    ).order_by('created'):
+        ...
+    ```
+    """
+
+    def __iter__(self):
         if self._results is None:
             return self._iterator()
         return iter(self._results)
 
     def __bool__(self):
-        """
-        Return True if the ResourceSet contains at least a resource
-        otherwise return False.
-
-        :return: True if contains a resource otherwise False.
-        :rtype: bool
-        """
         self._fetch_all()
         return bool(self._results)
 
     def __getitem__(self, key):  # noqa: CCR001
-        """
-        If called with slice and integer index, returns the item
-        at index ``key``.
-
-        If key is a slice, set the pagination limit and offset
-        accordingly.
-
-        :param key: index or slice.
-        :type key: int, slice
-        :raises TypeError: If ``key`` is neither an integer nor a slice.
-        :return: The resource at index ``key`` or self if ``key`` is a slice.
-        :rtype: dict, ResultSet
-        """
         self._validate_key(key)
 
         if self._results is not None:
             return self._results[key]
 
         if isinstance(key, int):
             copy = self._copy()
@@ -344,20 +332,26 @@
         copy._offset = key.start
         copy._slice = key
         if copy._slice.stop - copy._slice.start < copy._limit:
             copy._limit = copy._slice.stop - copy._slice.start
 
         return copy
 
-    def count(self):
+    def count(self) -> int:
         """
         Returns the total number of resources within this ResourceSet object.
 
-        :return: The total number of resources present.
-        :rtype: int
+        Usage:
+
+        ```py3
+        no_of_products = client.products.all().count()
+        ```
+
+        Returns:
+            (int): Returns the total number of resources within this ResourceSet object.
         """
         if not self._content_range:
             copy = self._copy()
             url = copy._get_request_url()
             kwargs = copy._get_request_kwargs()
             kwargs['params']['limit'] = 0
             copy._execute_request(url, kwargs)
@@ -365,16 +359,23 @@
         return self._content_range.count
 
     def first(self):
         """
         Returns the first resource that belongs to this ResourceSet object
         or None if the ResourceSet doesn't contains resources.
 
-        :return: The first resource.
-        :rtype: dict, None
+        Usage:
+
+        ```py3
+        latest_news = client.news.all().order_by('-updated').first()
+        ```
+
+        Returns:
+            (Resource): Returns the first resource that belongs to this ResourceSet object
+                or None.
         """
         copy = self._copy()
         copy._limit = 1
         copy._offset = 0
         copy._fetch_all()
         return copy._results[0] if copy._results else None
 
@@ -384,15 +385,16 @@
             self._client,
             self._path,
             self._build_qs(),
             self._get_request_kwargs(),
         )
         iterator = (
             ValuesListIterator(*args, fields=self._fields)
-            if self._fields else ResourceIterator(*args)
+            if self._fields
+            else ResourceIterator(*args)
         )
         return iterator
 
     def _execute_request(self, url, kwargs):
         results = self._client.get(url, **kwargs)
         self._content_range = parse_content_range(
             self._client.response.headers.get('Content-Range'),
@@ -404,52 +406,40 @@
             self._results = self._execute_request(
                 self._get_request_url(),
                 self._get_request_kwargs(),
             )
 
 
 class AsyncResourceSet(_ResourceSetBase):
+    """
+    Represent a set of resources.
 
-    def __aiter__(self):
-        """
-        Returns an iterator to iterate over the set of resources.
+    Usage:
 
-        :return: A resources iterator.
-        :rtype: ResourceSet
-        """
+    ```py3
+    async for product in (
+        client.products.all().filter(
+            R().status.eq('published')
+        ).order_by('created')
+    ):
+        ...
+    ```
+    """
+
+    def __aiter__(self):
         if self._results is None:
             return self._iterator()
         return aiter(self._results)
 
     def __bool__(self):
-        """
-        Return True if the ResourceSet contains at least a resource
-        otherwise return False.
-
-        :return: True if contains a resource otherwise False.
-        :rtype: bool
-        """
         if self._results is None:
             raise NotYetEvaluatedError()
         return bool(self._results)
 
     def __getitem__(self, key):  # noqa: CCR001
-        """
-        If called with slice and integer index, returns the item
-        at index ``key``.
-
-        If key is a slice, set the pagination limit and offset
-        accordingly.
-
-        :param key: index or slice.
-        :type key: int, slice
-        :raises TypeError: If ``key`` is neither an integer nor a slice.
-        :return: The resource at index ``key`` or self if ``key`` is a slice.
-        :rtype: dict, ResultSet
-        """
         self._validate_key(key)
 
         if self._results is not None:
             return self._results[key]
 
         if isinstance(key, int):
             raise NotYetEvaluatedError()
@@ -458,35 +448,48 @@
         copy._offset = key.start
         copy._slice = key
         if copy._slice.stop - copy._slice.start < copy._limit:
             copy._limit = copy._slice.stop - copy._slice.start
 
         return copy
 
-    async def count(self):
+    async def count(self) -> int:
         """
         Returns the total number of resources within this ResourceSet object.
 
-        :return: The total number of resources present.
-        :rtype: int
+        Usage:
+
+        ```py3
+        no_of_products = await client.products.all().count()
+        ```
+
+        Returns:
+            (int): Returns the total number of resources within this ResourceSet object.
         """
         if not self._content_range:
             url = self._get_request_url()
             kwargs = self._get_request_kwargs()
             kwargs['params']['limit'] = 0
             await self._execute_request(url, kwargs)
         return self._content_range.count
 
     async def first(self):
         """
         Returns the first resource that belongs to this ResourceSet object
         or None if the ResourceSet doesn't contains resources.
 
-        :return: The first resource.
-        :rtype: dict, None
+        Usage:
+
+        ```py3
+        latest_news = await client.news.all().order_by('-updated').first()
+        ```
+
+        Returns:
+            (Resource): Returns the first resource that belongs to this ResourceSet object
+                or None.
         """
         copy = self._copy()
         copy._limit = 1
         copy._offset = 0
         await copy._fetch_all()
         return copy._results[0] if copy._results else None
 
@@ -497,15 +500,16 @@
             self._path,
             self._build_qs(),
             self._get_request_kwargs(),
         )
 
         iterator = (
             AsyncValuesListIterator(*args, fields=self._fields)
-            if self._fields else AsyncResourceIterator(*args)
+            if self._fields
+            else AsyncResourceIterator(*args)
         )
         return iterator
 
     async def _execute_request(self, url, kwargs):
         results = await self._client.get(url, **kwargs)
         self._content_range = parse_content_range(
             self._client.response.headers.get('Content-Range'),
```

### Comparing `connect-openapi-client-25.9/connect/client/openapi.py` & `connect_openapi_client-28.0/connect/client/openapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,137 +1,137 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
-from io import StringIO
 from functools import partial
+from io import StringIO
+from typing import (
+    Any,
+    List,
+    MutableSet,
+    Optional,
+    Tuple,
+)
 
 import requests
-
 import yaml
 
 
 class OpenAPISpecs:
-
-    def __init__(self, location):
+    def __init__(self, location: str):
         self._location = location
         self._specs = self._load()
 
     @property
-    def title(self):
+    def title(self) -> Optional[str]:
         return self._specs['info']['title'] if self._specs else None
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         return self._specs['info']['description'] if self._specs else None
 
     @property
-    def version(self):
+    def version(self) -> Optional[str]:
         return self._specs['info']['version'] if self._specs else None
 
     @property
     def tags(self):
         return self._specs.get('tags') if self._specs else None
 
-    def exists(self, method, path):
+    def exists(self, method: str, path: str) -> bool:
         p = self._get_path(path)
         if not p:
             return False
         info = self._specs['paths'][p]
         return method.lower() in info
 
-    def get_namespaces(self):
+    def get_namespaces(self) -> List:
         def _is_namespace(path):
             comp = path[1:].split('/', 1)
             return len(comp) > 1 and not comp[1].startswith('{')
+
         return sorted(
             list(
                 {
                     p[1:].split('/', 1)[0]
                     for p in filter(_is_namespace, self._specs['paths'].keys())
                 },
             ),
         )
 
-    def get_collections(self):
+    def get_collections(self) -> MutableSet:
         namespaces = self.get_namespaces()
         cols = set()
         for p in self._specs['paths'].keys():
             name = p[1:].split('/', 1)[0]
             if name not in namespaces:
                 cols.add(name)
 
         return sorted(cols)
 
-    def get_namespaced_collections(self, path):
+    def get_namespaced_collections(self, path: str) -> MutableSet:
         nested = filter(lambda x: x[1:].startswith(path), self._specs['paths'].keys())
         collections = set()
         for p in nested:
-            splitted = p[len(path) + 1:].split('/', 2)
+            splitted = p[len(path) + 1 :].split('/', 2)
             if self._is_collection(p) and len(splitted) == 2:
                 collections.add(splitted[1])
         return list(sorted(collections))
 
-    def get_collection(self, path):
+    def get_collection(self, path: str):
         return self._get_info(path)
 
-    def get_resource(self, path):
+    def get_resource(self, path: str):
         return self._get_info(path)
 
-    def get_action(self, path):
+    def get_action(self, path: str):
         return self._get_info(path)
 
-    def get_actions(self, path):
+    def get_actions(self, path: str) -> List:
         p = self._get_path(path)
         nested = filter(
             lambda x: x.startswith(p) and x != p,
             self._specs['paths'].keys(),
         )
 
         actions = set()
         descriptions = {}
         for np in nested:
-            name = np[len(p) + 1:]
+            name = np[len(p) + 1 :]
             actions.add(name)
             info = self._specs['paths'][np]
             summary = info['summary'] if 'summary' in info else ''
             if summary:
                 descriptions[name] = summary
-        return [
-            (name, descriptions.get(name))
-            for name in sorted(actions)
-        ]
+        return [(name, descriptions.get(name)) for name in sorted(actions)]
 
-    def get_nested_namespaces(self, path):
+    def get_nested_namespaces(self, path) -> List:
         def _is_nested_namespace(base_path, path):
             if path[1:].startswith(base_path):
                 comp = path[1:].split('/')
-                return (
-                    len(comp) > 1
-                    and not comp[-1].startswith('{')
-                )
+                return len(comp) > 1 and not comp[-1].startswith('{')
             return False
 
         nested = filter(
             partial(_is_nested_namespace, path),
             self._specs['paths'].keys(),
         )
         current_level = len(path[1:].split('/'))
         nested_namespaces = []
         for ns in nested:
             name = ns[1:].split('/')[current_level]
             if not self._is_collection(f'/{path}/{name}'):
                 nested_namespaces.append(name)
         return nested_namespaces
 
-    def get_nested_collections(self, path):
+    def get_nested_collections(self, path: str) -> List[Tuple]:
         p = self._get_path(path)
         nested = filter(
-            lambda x: x.startswith(p[0:p.rindex('{')]) and x != p,
+            lambda x: x.startswith(p[0 : p.rindex('{')]) and x != p,
             self._specs['paths'].keys(),
         )
         cut_pos = p.count('/')
         collections = set()
         descriptions = {}
         for np in nested:
             splitted = np[1:].split('/')
@@ -141,35 +141,32 @@
             operation_id = method_info['operationId']
             if self._is_action(operation_id):
                 continue
             collections.add(name)
             summary = info['summary'] if 'summary' in info else ''
             if summary:
                 descriptions[name] = summary
-        return [
-            (name, descriptions.get(name))
-            for name in sorted(collections)
-        ]
+        return [(name, descriptions.get(name)) for name in sorted(collections)]
 
-    def _load(self):
+    def _load(self) -> Any:
         if self._location.startswith('http'):
             return self._load_from_url()
         return self._load_from_fs()
 
-    def _load_from_url(self):
+    def _load_from_url(self) -> Any:
         res = requests.get(self._location, stream=True)
         if res.status_code == 200:
             result = StringIO()
             for chunk in res.iter_content(chunk_size=8192):
                 result.write(str(chunk, encoding='utf-8'))
             result.seek(0)
             return yaml.safe_load(result)
         res.raise_for_status()
 
-    def _load_from_fs(self):
+    def _load_from_fs(self) -> Any:
         with open(self._location, 'r') as f:
             return yaml.safe_load(f)
 
     def _get_path(self, path):
         if '?' in path:
             path, _ = path.split('?', 1)
         components = path.split('/')
```

### Comparing `connect-openapi-client-25.9/connect/client/rql/base.py` & `connect_openapi_client-28.0/connect/client/rql/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
+from typing import List
+
 from connect.client.rql.utils import parse_kwargs, to_rql_value
 
 
 class RQLQuery:
     """
     Helper class to construct complex RQL queries.
-    """
-    AND = 'and'
-    OR = 'or'
-    EXPR = 'expr'
-
-    def __init__(self, *, _op=EXPR, _children=None, _negated=False, _expr=None, **kwargs):
-        """
-        Create a new R object.
-
-        Query filters can be expressed through keyword arguments or using methods.
-
-        Ex.
 
-        .. code-block:: python
+    Usage:
 
-            rql = R(field='value', field2__in=('v1', 'v2'), field3__empty=True)
-
-        All the lookups expressed as keyword arguments are combined together with a logical ``and``.
-
-        Using the ``n`` method:
-
-        .. code-block:: python
-
-            rql = (
-                R().n('field').eq('value')
-                & R().n('field2').in_(('v1', 'v2'))
-                & R().n('field3').empty(True)
-            )
-
-        The previous query can be expressed in a more concise form like:
+    ```py3
+        rql = R(field='value', field2__in=('v1', 'v2'), field3__empty=True)
+    ```
+    !!! note
+        All the lookups expressed as keyword arguments are combined together with a logical `and`.
+
+
+    Using the ``n`` method:
+
+    ```py3
+        rql = (
+            R().n('field').eq('value')
+            & R().n('field2').anyof(('v1', 'v2'))
+            & R().n('field3').empty(True)
+        )
+    ```
 
-        .. code-block:: python
+    The previous query can be expressed in a more concise form like:
 
-            rql = R().field.eq('value') & R().field2.in_(('v1', 'v2')) & r.field3.empty(True)
+    ```py3
+    rql = R().field.eq('value') & R().field2.anyof(('v1', 'v2')) & r.field3.empty(True)
+    ```
 
-        The R object support the bitwise operators ``&``, ``|`` and ``~``.
+    The R object support the bitwise operators `&`, `|` and `~`.
 
-        Nested fields can be expressed using dot notation:
+    Nested fields can be expressed using dot notation:
 
-        .. code-block:: python
+    ```py3
+    rql = R().n('nested.field').eq('value')
+    ```
 
-            rql = R().n('nested.field').eq('value')
+    or
 
-        or
+    ```py3
+    rql = R().nested.field.eq('value')
+    ```
+    """
 
-        .. code-block:: python
+    AND = 'and'
+    OR = 'or'
+    EXPR = 'expr'
 
-            rql = R().nested.field.eq('value')
-        """
+    def __init__(self, *, _op=EXPR, _children=None, _negated=False, _expr=None, **kwargs):
         self.op = _op
         self.children = _children or []
         self.negated = _negated
         self.expr = _expr
         self._path = []
         self._field = None
         if len(kwargs) == 1:
@@ -69,162 +68,180 @@
             self.expr = parse_kwargs(kwargs)[0]
         if len(kwargs) > 1:
             self.op = self.AND
             for token in parse_kwargs(kwargs):
                 self.children.append(RQLQuery(_expr=token))
 
     def __len__(self):
-        """
-        Returns the length of this R object.
-        It will be 1 if represent a single RQL expression
-        or the number of expressions this logical operator (and, or)
-        applies to.
-
-        :return: The length of this R object.
-        :rtype: int
-        """
         if self.op == self.EXPR:
             if self.expr:
                 return 1
             return 0
         return len(self.children)
 
     def __bool__(self):
-        """
-        Returns False if it is an empty R object otherwise True.
-
-        :return: False if it is an empty R object otherwise True.
-        :rtype: bool
-        """
         return bool(self.children) or bool(self.expr)
 
     def __eq__(self, other):
-        """
-        Returns True if self == other.
-
-        :param other: Another R object.
-        :type other: R
-        :return: True if the ``other`` object is equal to self, False otherwise.
-        :rtype: bool
-        """
         return (
             self.op == other.op
             and self.children == other.children
             and self.negated == other.negated
             and self.expr == other.expr
         )
 
     def __hash__(self):
-        """
-        Calculate a hash that identifies uniquely this R object.
-
-        :return: The hash of this object.
-        :rtype: int
-        """
         return hash(
             (self.op, self.expr, self.negated, *(hash(value) for value in self.children)),
         )
 
     def __repr__(self):
         if self.op == self.EXPR:
             return f'<R({self.op}) {self.expr}>'
         return f'<R({self.op})>'
 
     def __and__(self, other):
-        """
-        Combine this R object with ``other`` using a logical ``and``.
-
-        :param other: Another R object.
-        :type other: R
-        :return: The R object representing a logical ``and`` between this and ``other``.
-        :rtype: R
-        """
         return self._join(other, self.AND)
 
     def __or__(self, other):
-        """
-        Combine this R object with ``other`` using a logical ``or``.
-
-        :param other: Another R object.
-        :type other: R
-        :return: The R object representing a logical ``or`` between this and ``other``.
-        :rtype: R
-        """
         return self._join(other, self.OR)
 
     def __invert__(self):
-        """
-        Apply the RQL ``not`` operator to this R object.
-
-        :return: The R object representing this R object negated.
-        :rtype: R
-        """
         query = RQLQuery(_op=self.AND, _expr=self.expr, _negated=True)
         query._append(self)
         return query
 
     def __getattr__(self, name):
         return self.n(name)
 
     def __str__(self):
         return self._to_string(self)
 
     def n(self, name):
         """
-        Set the current field for this R object.
+        Set the current field for this `R` object.
 
-        :param name: name of the field
-        :type name: str
-        :raises AttributeError: if this R object has already been evaluated.
-        :return: This R object.
-        :rtype: R
+        Args:
+            name (str): Name of the field.
         """
         if self._field:
             raise AttributeError('Already evaluated')
 
         self._path.extend(name.split('.'))
         return self
 
     def ne(self, value):
+        """
+        Apply the `ne` operator to the field this `R` object refers to.
+
+        Args:
+            value (str): The value to which compare the field.
+        """
         return self._bin('ne', value)
 
     def eq(self, value):
+        """
+        Apply the `eq` operator to the field this `R` object refers to.
+
+        Args:
+            value (str): The value to which compare the field.
+        """
         return self._bin('eq', value)
 
     def lt(self, value):
+        """
+        Apply the `lt` operator to the field this `R` object refers to.
+
+        Args:
+            value (str): The value to which compare the field.
+        """
         return self._bin('lt', value)
 
     def le(self, value):
+        """
+        Apply the `le` operator to the field this `R` object refers to.
+
+        Args:
+            value (str): The value to which compare the field.
+        """
         return self._bin('le', value)
 
     def gt(self, value):
+        """
+        Apply the `gt` operator to the field this `R` object refers to.
+
+        Args:
+            value (str): The value to which compare the field.
+        """
         return self._bin('gt', value)
 
     def ge(self, value):
+        """
+        Apply the `ge` operator to the field this `R` object refers to.
+
+        Args:
+            value (str): The value to which compare the field.
+        """
         return self._bin('ge', value)
 
-    def out(self, value):
+    def out(self, value: List[str]):
+        """
+        Apply the `out` operator to the field this `R` object refers to.
+
+        Args:
+            value (list[str]): The list of values to which compare the field.
+        """
         return self._list('out', value)
 
     def in_(self, value):
         return self._list('in', value)
 
-    def oneof(self, value):
+    def oneof(self, value: List[str]):
+        """
+        Apply the `in` operator to the field this `R` object refers to.
+
+        Args:
+            value (list[str]): The list of values to which compare the field.
+        """
         return self._list('in', value)
 
-    def null(self, value):
+    def null(self, value: List[str]):
+        """
+        Apply the `null` operator to the field this `R` object refers to.
+
+        Args:
+            value (list[str]): The value to which compare the field.
+        """
         return self._bool('null', value)
 
-    def empty(self, value):
+    def empty(self, value: List[str]):
+        """
+        Apply the `empty` operator to the field this `R` object refers to.
+
+        Args:
+            value (list[str]): The value to which compare the field.
+        """
         return self._bool('empty', value)
 
-    def like(self, value):
+    def like(self, value: List[str]):
+        """
+        Apply the `like` operator to the field this `R` object refers to.
+
+        Args:
+            value (list[str]): The value to which compare the field.
+        """
         return self._bin('like', value)
 
-    def ilike(self, value):
+    def ilike(self, value: List[str]):
+        """
+        Apply the `ilike` operator to the field this `R` object refers to.
+
+        Args:
+            value (list[str]): The value to which compare the field.
+        """
         return self._bin('ilike', value)
 
     def _bin(self, op, value):
         self._field = '.'.join(self._path)
         value = to_rql_value(op, value)
         self.expr = f'{op}({self._field},{value})'
         return self
@@ -286,17 +303,16 @@
         return query
 
     def _append(self, other):
         if other in self.children:
             return other
 
         if (
-            (other.op == self.op or (len(other) == 1 and other.op != self.EXPR))
-            and not other.negated
-        ):
+            other.op == self.op or (len(other) == 1 and other.op != self.EXPR)
+        ) and not other.negated:
             self.children.extend(other.children)
             return self
 
         self.children.append(other)
         return self
```

### Comparing `connect-openapi-client-25.9/connect/client/rql/utils.py` & `connect_openapi_client-28.0/connect/client/rql/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 from datetime import date, datetime
 from decimal import Decimal
 
 
 COMP = ('eq', 'ne', 'lt', 'le', 'gt', 'ge')
 SEARCH = ('like', 'ilike')
```

### Comparing `connect-openapi-client-25.9/connect/client/testing/models/base.py` & `connect_openapi_client-28.0/connect/client/testing/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
-from connect.client.models.base import _ActionBase, _CollectionBase, _NSBase, _ResourceBase
-from connect.client.testing.models.mixins import (
-    ActionMixin,
-    CollectionMixin,
-    ResourceMixin,
+from connect.client.models.base import (
+    _ActionBase,
+    _CollectionBase,
+    _NSBase,
+    _ResourceBase,
 )
+from connect.client.testing.models.mixins import ActionMixin, CollectionMixin, ResourceMixin
 from connect.client.testing.models.resourceset import ResourceSetMock
 
 
 class NSMock(_NSBase):
     def _get_collection_class(self):
         return CollectionMock
```

### Comparing `connect-openapi-client-25.9/connect/client/testing/models/mixins.py` & `connect_openapi_client-28.0/connect/client/testing/models/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2022 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 
 
 class CollectionMixin:
     def create(
         self,
         status_code=201,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
-
         return self._client.create(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
     def bulk_create(
         self,
         status_code=201,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
-
         return self._client.create(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
     def bulk_update(
         self,
         status_code=200,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
-
         return self._client.update(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
     def bulk_delete(
         self,
         status_code=204,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
-
         return self._client.delete(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
 
 class ResourceMixin:
     def exists(self, return_value):
         self.get(status_code=200 if return_value else 404)
 
@@ -81,30 +85,30 @@
         )
 
     def update(
         self,
         status_code=200,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
-
         return self._client.update(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
     def delete(
         self,
         status_code=204,
         return_value=None,
         headers=None,
     ):
-
         return self._client.delete(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
         )
 
@@ -137,41 +141,44 @@
         )
 
     def post(
         self,
         status_code=200,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
         return self._client.create(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
     def put(
         self,
         status_code=200,
         return_value=None,
         headers=None,
+        match_body=None,
     ):
         return self._client.update(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
+            match_body=match_body,
         )
 
     def delete(
         self,
         status_code=204,
         return_value=None,
         headers=None,
     ):
-
         return self._client.delete(
             self._path,
             status_code=status_code,
             return_value=return_value,
             headers=headers,
         )
```

### Comparing `connect-openapi-client-25.9/connect/client/utils.py` & `connect_openapi_client-28.0/connect/client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
-# Copyright (c) 2021 Ingram Micro. All Rights Reserved.
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
 #
 import platform
 from collections import namedtuple
 
 from connect.client.version import get_version
 
+
 ContentRange = namedtuple('ContentRange', ('first', 'last', 'count'))
 
 
 def _get_user_agent():
     version = get_version()
     pimpl = platform.python_implementation()
     pver = platform.python_version()
```

### Comparing `connect-openapi-client-25.9/setup.py` & `connect_openapi_client-28.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,79 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: connect-openapi-client
+Version: 28.0
+Summary: Connect Python OpenAPI Client
+Home-page: https://connect.cloudblue.com
+License: Apache-2.0
+Keywords: fulfillment,api,client,openapi,utility,connect,cloudblue
+Author: CloudBlue
+Requires-Python: >=3.8,<4
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Dist: PyYAML (>=5.3.1)
+Requires-Dist: asgiref (>=3.3.4,<4.0.0)
+Requires-Dist: connect-markdown-renderer (>=3,<4)
+Requires-Dist: httpx (>=0.23)
+Requires-Dist: importlib-metadata (>=6.6,<7.0)
+Requires-Dist: inflect (>=4.1)
+Requires-Dist: pytest-httpx (>=0.20)
+Requires-Dist: requests (>=2.23)
+Requires-Dist: responses (>=0.14.0,<1)
+Requires-Dist: urllib3 (<2)
+Project-URL: Documentation, https://connect-openapi-client.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/cloudblue/connect-python-openapi-client
+Description-Content-Type: text/markdown
 
-packages = \
-['cnct',
- 'connect',
- 'connect.client',
- 'connect.client.contrib',
- 'connect.client.contrib.locust',
- 'connect.client.models',
- 'connect.client.rql',
- 'connect.client.testing',
- 'connect.client.testing.models']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=5.3.1',
- 'asgiref>=3.3.4,<4.0.0',
- 'connect-markdown-renderer>=2,<3',
- 'httpx>=0.23',
- 'inflect>=4.1',
- 'pytest-httpx>=0.20',
- 'requests>=2.23',
- 'responses>=0.12.0,<0.13.0']
-
-extras_require = \
-{':python_version >= "3.7" and python_version < "3.8"': ['importlib-metadata>=4.12.0,<5.0.0']}
-
-entry_points = \
-{'pytest11': ['pytest_connect_client = connect.client.testing.fixtures']}
-
-setup_kwargs = {
-    'name': 'connect-openapi-client',
-    'version': '25.9',
-    'description': 'Connect Python OpenAPI Client',
-    'long_description': '# Connect Python OpenAPI Client\n\n![pyversions](https://img.shields.io/pypi/pyversions/connect-openapi-client.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-openapi-client.svg)](https://pypi.org/project/connect-openapi-client/) [![Build Status](https://github.com/cloudblue/connect-python-openapi-client/workflows/Build%20Connect%20Python%20OpenAPI%20Client/badge.svg)](https://github.com/cloudblue/connect-python-openapi-client/actions) [![codecov](https://codecov.io/gh/cloudblue/connect-python-openapi-client/branch/master/graph/badge.svg)](https://codecov.io/gh/cloudblue/connect-python-openapi-client) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-open-api-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-open-api-client)\n\n\n\n\n## Introduction\n\n`Connect Python OpenAPI Client` is the simple, concise, powerful and REPL-friendly CloudBlue Connect API client.\n\nIt has been designed following the [fluent interface design pattern](https://en.wikipedia.org/wiki/Fluent_interface).\n\nDue to its REPL-friendly nature, using the CloudBlue Connect OpenAPI specifications it allows developers to learn and\nplay with the CloudBlue Connect API using a python REPL like [jupyter](https://jupyter.org/) or [ipython](https://ipython.org/).\n\n\n## Install\n\n`Connect Python OpenAPI Client` requires python 3.7 or later.\n\n\n`Connect Python OpenAPI Client` can be installed from [pypi.org](https://pypi.org/project/connect-openapi-client/) using pip:\n\n```\n$ pip install connect-openapi-client\n```\n\n\n## Documentation\n\n[`Connect Python OpenAPI Client` documentation](https://connect-openapi-client.readthedocs.io/en/latest/) is hosted on the _Read the Docs_ service.\n\n\n## License\n\n``Connect Python OpenAPI Client`` is released under the [Apache License Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).\n',
-    'author': 'CloudBlue',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://connect.cloudblue.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4',
-}
+# Connect Python OpenAPI Client
 
+![pyversions](https://img.shields.io/pypi/pyversions/connect-openapi-client.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-openapi-client.svg)](https://pypi.org/project/connect-openapi-client/) [![Build Status](https://github.com/cloudblue/connect-python-openapi-client/workflows/Build%20Connect%20Python%20OpenAPI%20Client/badge.svg)](https://github.com/cloudblue/connect-python-openapi-client/actions) [![codecov](https://codecov.io/gh/cloudblue/connect-python-openapi-client/branch/master/graph/badge.svg)](https://codecov.io/gh/cloudblue/connect-python-openapi-client) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-open-api-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-open-api-client)
+
+
+
+
+## Introduction
+
+`Connect Python OpenAPI Client` is the simple, concise, powerful and REPL-friendly CloudBlue Connect API client.
+
+It has been designed following the [fluent interface design pattern](https://en.wikipedia.org/wiki/Fluent_interface).
+
+Due to its REPL-friendly nature, using the CloudBlue Connect OpenAPI specifications it allows developers to learn and
+play with the CloudBlue Connect API using a python REPL like [jupyter](https://jupyter.org/) or [ipython](https://ipython.org/).
+
+
+## Install
+
+`Connect Python OpenAPI Client` requires python 3.8 or later.
+
+
+`Connect Python OpenAPI Client` can be installed from [pypi.org](https://pypi.org/project/connect-openapi-client/) using pip:
+
+```
+$ pip install connect-openapi-client
+```
+
+
+## Development
+We use `isort` library to order and format our imports, and `black` - to format the code. 
+We check it using `flake8-isort` and `flake8-black` libraries (automatically on `flake8` run).  
+For convenience you may run `isort . && black .` to format the code.
+
+
+## Documentation
+
+[`Connect Python OpenAPI Client` documentation](https://connect-openapi-client.readthedocs.io/en/latest/) is hosted on the _Read the Docs_ service.
+
+
+## License
+
+``Connect Python OpenAPI Client`` is released under the [Apache License Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
-setup(**setup_kwargs)
```

