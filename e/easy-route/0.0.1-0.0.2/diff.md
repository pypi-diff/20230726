# Comparing `tmp/easy_route-0.0.1.tar.gz` & `tmp/easy_route-0.0.2.tar.gz`

## Comparing `easy_route-0.0.1.tar` & `easy_route-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 easy_route-0.0.1/requirements.txt
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 easy_route-0.0.1/sonar-project.properties
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 easy_route-0.0.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 easy_route-0.0.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 easy_route-0.0.1/.github/workflows/publish-to-testpypi.yaml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/controllers/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/controllers/abstract_controller.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/middlewares/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/middlewares/abstract_middleware.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/middlewares/data_validator_middleware.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/routes/__init__.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 easy_route-0.0.1/src/easy_route/routes/route.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/tests/controller/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 easy_route-0.0.1/tests/middleware/test_data_validator_middleware.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.1/tests/route/__init__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 easy_route-0.0.1/tests/route/test_route.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 easy_route-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 easy_route-0.0.1/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 easy_route-0.0.1/README.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 easy_route-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 easy_route-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 easy_route-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 easy_route-0.0.2/sonar-project.properties
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 easy_route-0.0.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 easy_route-0.0.2/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 easy_route-0.0.2/.github/workflows/publish-to-testpypi.yaml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/controllers/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/controllers/abstract_controller.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/middlewares/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/middlewares/abstract_middleware.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/middlewares/data_validator_middleware.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/routes/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 easy_route-0.0.2/src/easy_route/routes/route.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/tests/controller/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 easy_route-0.0.2/tests/middleware/test_data_validator_middleware.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easy_route-0.0.2/tests/route/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 easy_route-0.0.2/tests/route/test_route.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 easy_route-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 easy_route-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 easy_route-0.0.2/README.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 easy_route-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 easy_route-0.0.2/PKG-INFO
```

### Comparing `easy_route-0.0.1/.github/workflows/build.yaml` & `easy_route-0.0.2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `easy_route-0.0.1/.github/workflows/publish-to-pypi.yaml` & `easy_route-0.0.2/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `easy_route-0.0.1/.github/workflows/publish-to-testpypi.yaml` & `easy_route-0.0.2/.github/workflows/publish-to-testpypi.yaml`

 * *Files identical despite different names*

### Comparing `easy_route-0.0.1/src/easy_route/middlewares/abstract_middleware.py` & `easy_route-0.0.2/src/easy_route/middlewares/abstract_middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from typing import Optional
 
 from flask import Request, Response
 
 
 class AbstractMiddleware(ABC):
     """An abstract class representing a Middleware."""
-    def __init__(self):
-        pass
-
     @abstractmethod
     def dispatch(self, request: Request) -> Optional[Response]:
         """Executes the middleware.
         It returns a Response object if the middleware failed (i.e. 401, 400, ...) or None
         if the request has been validated and the stack can proceed.
         In case a Response is returned, the route flow will block and the response is returned
         to the client.
```

### Comparing `easy_route-0.0.1/src/easy_route/routes/route.py` & `easy_route-0.0.2/src/easy_route/routes/route.py`

 * *Files identical despite different names*

### Comparing `easy_route-0.0.1/tests/middleware/test_data_validator_middleware.py` & `easy_route-0.0.2/tests/middleware/test_data_validator_middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,88 +7,89 @@
 
 from easy_route.middlewares.data_validator_middleware import DataValidatorMiddleware
 
 
 class TestDataValidatorMiddleware(unittest.TestCase):
     def setUp(self) -> None:
         self.request = MagicMock()
+        self.data_provider = MagicMock()
         self.validator = MagicMock()
 
     def tearDown(self) -> None:
         self.request = None
+        self.data_provider = None
         self.validator = None
 
     def testDispatch_return400_whenDataIsEmpty(self):
         # Arrange
         rules = {}
-        middleware = DataValidatorMiddleware(rules)
-
-        self.request.get_json.return_value = None
+        middleware = DataValidatorMiddleware(rules, self.data_provider)
+        self.data_provider.get_data.return_value = None
 
         # Act
         result = middleware.dispatch(self.request)
 
         # Assert
-        self.request.get_json.assert_called_once()
+        self.data_provider.get_data.assert_called_once()
         self.assertEqual(400, result.status_code)
         self.assertFalse(result.data)
 
     def testDispatch_return400_whenInvalidParameter(self):
         # Arrange
         rules = {
             'uuid': self.validator.is_uuid
         }
-        middleware = DataValidatorMiddleware(rules)
+        middleware = DataValidatorMiddleware(rules, self.data_provider)
 
         self.validator.is_uuid.return_value = False
-        self.request.get_json.return_value = {
+        self.data_provider.get_data.return_value = {
             'uuid': 'invalid uuid'
         }
 
         # Act
         result = middleware.dispatch(self.request)
 
         # Assert
-        self.request.get_json.assert_called_once()
+        self.data_provider.get_data.assert_called_once()
         self.assertEqual(400, result.status_code)
         self.assertFalse(result.data)
 
     def testDispatch_return400_whenParameterIsNotSet(self):
         # Arrange
         rules = {
             'uuid': self.validator.is_uuid
         }
-        middleware = DataValidatorMiddleware(rules)
+        middleware = DataValidatorMiddleware(rules, self.data_provider)
 
         self.validator.is_uuid.return_value = False
-        self.request.get_json.return_value = {}
+        self.data_provider.get_data.return_value = {}
 
         # Act
         result = middleware.dispatch(self.request)
 
         # Assert
-        self.request.get_json.assert_called_once()
+        self.data_provider.get_data.assert_called_once()
         self.validator.is_uuid.assert_not_called()
         self.assertEqual(400, result.status_code)
         self.assertFalse(result.data)
 
     def testDispatch_returnNone_whenValidParameters(self):
         # Arrange
         rules = {
             'uuid': self.validator.is_uuid,
             'name': lambda name: self.validator.is_string(name) and name,
         }
-        middleware = DataValidatorMiddleware(rules)
+        middleware = DataValidatorMiddleware(rules, self.data_provider)
 
         self.validator.is_uuid.return_value = True
         self.validator.is_string.return_value = True
-        self.request.get_json.return_value = {
+        self.data_provider.get_data.return_value = {
             'uuid': str(uuid.uuid4()),
             'name': 'name'
         }
 
         # Act
         result = middleware.dispatch(self.request)
 
         # Assert
-        self.request.get_json.assert_called_once()
+        self.data_provider.get_data.assert_called_once()
         self.assertIsNone(result)
```

### Comparing `easy_route-0.0.1/tests/route/test_route.py` & `easy_route-0.0.2/tests/route/test_route.py`

 * *Files identical despite different names*

### Comparing `easy_route-0.0.1/.gitignore` & `easy_route-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `easy_route-0.0.1/LICENSE` & `easy_route-0.0.2/LICENSE`

 * *Files identical despite different names*

