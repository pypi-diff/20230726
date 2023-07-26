# Comparing `tmp/matchmock-2.1.0.tar.gz` & `tmp/matchmock-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmock-2.1.0.tar", last modified: Tue Feb 14 14:01:33 2023, max compression
+gzip compressed data, was "matchmock-2.1.1.tar", last modified: Wed Jul 26 09:27:48 2023, max compression
```

## Comparing `matchmock-2.1.0.tar` & `matchmock-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:01:33.168071 matchmock-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-14 14:01:17.000000 matchmock-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-02-14 14:01:33.168071 matchmock-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-14 14:01:17.000000 matchmock-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:01:33.168071 matchmock-2.1.0/matchmock/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-02-14 14:01:17.000000 matchmock-2.1.0/matchmock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:01:33.168071 matchmock-2.1.0/matchmock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-02-14 14:01:33.000000 matchmock-2.1.0/matchmock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-14 14:01:33.000000 matchmock-2.1.0/matchmock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 14:01:33.000000 matchmock-2.1.0/matchmock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 14:01:33.000000 matchmock-2.1.0/matchmock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-14 14:01:33.000000 matchmock-2.1.0/matchmock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-14 14:01:33.000000 matchmock-2.1.0/matchmock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-14 14:01:33.172071 matchmock-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 14:01:17.000000 matchmock-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:01:33.168071 matchmock-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-14 14:01:17.000000 matchmock-2.1.0/tests/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-02-14 14:01:17.000000 matchmock-2.1.0/tests/test_matchmock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:27:48.521448 matchmock-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-26 09:27:36.000000 matchmock-2.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-26 09:27:48.521448 matchmock-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-26 09:27:36.000000 matchmock-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:27:48.517449 matchmock-2.1.1/matchmock/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-26 09:27:36.000000 matchmock-2.1.1/matchmock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 09:27:36.000000 matchmock-2.1.1/matchmock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:27:48.521448 matchmock-2.1.1/matchmock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-26 09:27:48.000000 matchmock-2.1.1/matchmock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-26 09:27:48.000000 matchmock-2.1.1/matchmock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:27:48.000000 matchmock-2.1.1/matchmock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:27:48.000000 matchmock-2.1.1/matchmock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 09:27:48.000000 matchmock-2.1.1/matchmock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 09:27:48.000000 matchmock-2.1.1/matchmock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 09:27:48.521448 matchmock-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:27:36.000000 matchmock-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:27:48.521448 matchmock-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-26 09:27:36.000000 matchmock-2.1.1/tests/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-26 09:27:36.000000 matchmock-2.1.1/tests/test_matchmock.py
```

### Comparing `matchmock-2.1.0/LICENSE.txt` & `matchmock-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matchmock-2.1.0/PKG-INFO` & `matchmock-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmock
-Version: 2.1.0
+Version: 2.1.1
 Summary: Hamcrest matchers for mock objects.
 Home-page: https://github.com/keis/matchmock
 Author: David Keijser
 Author-email: keijser@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE.txt
```

### Comparing `matchmock-2.1.0/README.md` & `matchmock-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `matchmock-2.1.0/matchmock/__init__.py` & `matchmock-2.1.1/matchmock/__init__.py`

 * *Files identical despite different names*

### Comparing `matchmock-2.1.0/matchmock.egg-info/PKG-INFO` & `matchmock-2.1.1/matchmock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmock
-Version: 2.1.0
+Version: 2.1.1
 Summary: Hamcrest matchers for mock objects.
 Home-page: https://github.com/keis/matchmock
 Author: David Keijser
 Author-email: keijser@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE.txt
```

### Comparing `matchmock-2.1.0/setup.cfg` & `matchmock-2.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = matchmock
 author = David Keijser
 author_email = keijser@gmail.com
-version = 2.1.0
+version = 2.1.1
 description = Hamcrest matchers for mock objects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/keis/matchmock
 
 [options]
 packages = matchmock
```

### Comparing `matchmock-2.1.0/tests/test_matchmock.py` & `matchmock-2.1.1/tests/test_matchmock.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,226 +7,235 @@
 
 
 @pytest.fixture
 def desc():
     return StringDescription()
 
 
-def test_called_ok():
+def test_called_ok() -> None:
     matcher = called()
     mock = Mock()
     mock()
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_called_ok_twice():
+def test_called_member_ok() -> None:
+    matcher = called()
+    mock = Mock()
+    mock.fun()
+
+    ok = matcher.matches(mock.fun)
+    assert_that(ok, equal_to(True))
+
+
+def test_called_ok_twice() -> None:
     matcher = called()
     mock = Mock()
     mock()
     mock()
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_called_ok_explicitly_twice():
+def test_called_ok_explicitly_twice() -> None:
     matcher = called_n_times(2)
     mock = Mock()
     mock()
     mock()
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_called_ok_explicitly_twice_fail(desc):
+def test_called_ok_explicitly_twice_fail(desc) -> None:
     expected = 'was called 3 times'
     matcher = called_n_times(2)
     mock = Mock()
     mock()
     mock()
     mock()
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
     assert_that(str(desc), starts_with(expected))
 
 
-def test_called_description(desc):
+def test_called_description(desc) -> None:
     expected = 'Mock called a value greater than <0> times with ANYTHING'
     matcher = called()
     matcher.describe_to(desc)
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_fail(desc):
+def test_called_fail(desc) -> None:
     expected = 'was called 0 times'
     matcher = called()
     mock = Mock()
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_not_called_ok():
+def test_not_called_ok() -> None:
     matcher = not_called()
     mock = Mock()
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_not_called_description(desc):
+def test_not_called_description(desc) -> None:
     matcher = not_called()
     expected = 'Mock called <0> times with ANYTHING'
     matcher.describe_to(desc)
     assert_that(str(desc), equal_to(expected))
 
 
-def test_not_called_fail(desc):
+def test_not_called_fail(desc) -> None:
     matcher = not_called()
     expected = "was called 1 times with ('foo', )"
 
     mock = Mock()
     mock('foo')
 
     ok = matcher.matches(mock, desc)
 
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_once_ok():
+def test_called_once_ok() -> None:
     matcher = called_once()
     mock = Mock()
     mock('foo')
 
     ok = matcher.matches(mock)
 
     assert_that(ok, equal_to(True))
 
 
-def test_called_once_description(desc):
+def test_called_once_description(desc) -> None:
     expected = 'Mock called <1> times with ANYTHING'
     matcher = called_once()
     matcher.describe_to(desc)
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_once_fail_not_called(desc):
+def test_called_once_fail_not_called(desc) -> None:
     expected = 'was called 0 times'
     matcher = called_once()
     mock = Mock()
 
     ok = matcher.matches(mock, desc)
 
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_once_fail_called_twice(desc):
+def test_called_once_fail_called_twice(desc) -> None:
     expected = "was called 2 times with ('foo', ) and ('bar', )"
     matcher = called_once()
     mock = Mock()
     mock('foo')
     mock('bar')
 
     ok = matcher.matches(mock, desc)
 
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_with_ok():
+def test_called_with_ok() -> None:
     matcher = called_with('foo', instance_of(int))
     mock = Mock()
     mock('foo', 5)
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_called_with_ok_kwargs():
+def test_called_with_ok_kwargs() -> None:
     matcher = called_with(x='foo', y=instance_of(int))
     mock = Mock()
     mock(x='foo', y=5)
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_called_with_ok_multi():
+def test_called_with_ok_multi() -> None:
     matcher = called_with('foo', instance_of(int))
     mock = Mock()
     mock('baz')
     mock('foo', 5)
     mock('bar', 5)
 
     ok = matcher.matches(mock)
     assert_that(ok, equal_to(True))
 
 
-def test_called_with_description(desc):
+def test_called_with_description(desc) -> None:
     expected = ("Mock called a value greater than <0> times with " +
                 "('foo', an instance of int, )")
     matcher = called_with('foo', instance_of(int))
 
     matcher.describe_to(desc)
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_with_failed(desc):
+def test_called_with_failed(desc) -> None:
     expected = "argument 1: was 'bar'"
     matcher = called_with('foo', instance_of(int))
     mock = Mock()
     mock('foo', 'bar')
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_with_failed_multi(desc):
+def test_called_with_failed_multi(desc) -> None:
     expected = "in call 0: argument 1: was 'bar', in call 1: 1 extra arguments"
     matcher = called_with('foo', instance_of(int))
     mock = Mock()
     mock('foo', 'bar')
     mock('foo', 'bar', 'baz')
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_with_kwarg_failed(desc):
+def test_called_with_kwarg_failed(desc) -> None:
     expected = "value for 'foo' was 'baz'"
     matcher = called_with(foo='bar')
     mock = Mock()
     mock(foo='baz')
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_with_extra_arg(desc):
+def test_called_with_extra_arg(desc) -> None:
     expected = "1 extra arguments"
     matcher = called_with('spam')
     mock = Mock()
     mock('spam', 'bar')
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
     assert_that(str(desc), equal_to(expected))
 
 
-def test_called_with_extra_kwarg(desc):
+def test_called_with_extra_kwarg(desc) -> None:
     expected = "extra keyword argument(s) 'foo' given"
     matcher = called_with('spam')
     mock = Mock()
     mock('spam', foo='bar')
 
     ok = matcher.matches(mock, desc)
     assert_that(ok, equal_to(False))
```

