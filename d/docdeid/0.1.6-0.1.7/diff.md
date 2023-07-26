# Comparing `tmp/docdeid-0.1.6.tar.gz` & `tmp/docdeid-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docdeid-0.1.6.tar", max compression
+gzip compressed data, was "docdeid-0.1.7.tar", max compression
```

## Comparing `docdeid-0.1.6.tar` & `docdeid-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1033 2023-03-28 14:40:16.106491 docdeid-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     3972 2023-03-28 14:40:16.106491 docdeid-0.1.6/README.md
--rw-r--r--   0        0        0      291 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/annotation.py
--rw-r--r--   0        0        0     2289 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/deidentifier.py
--rw-r--r--   0        0        0     4677 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/document.py
--rw-r--r--   0        0        0      103 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/ds/__init__.py
--rw-r--r--   0        0        0      243 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/ds/ds.py
--rw-r--r--   0        0        0     9440 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/ds/lookup.py
--rw-r--r--   0        0        0     2028 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/pattern.py
--rw-r--r--   0        0        0      372 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/process/__init__.py
--rw-r--r--   0        0        0     7970 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/process/annotation_set.py
--rw-r--r--   0        0        0     7824 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/process/annotator.py
--rw-r--r--   0        0        0     4079 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/process/doc.py
--rw-r--r--   0        0        0     5365 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/process/redactor.py
--rw-r--r--   0        0        0        0 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/py.typed
--rw-r--r--   0        0        0      247 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/str/__init__.py
--rw-r--r--   0        0        0     3930 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/str/processor.py
--rw-r--r--   0        0        0    10273 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/tokenize.py
--rw-r--r--   0        0        0      879 2023-03-28 14:40:16.106491 docdeid-0.1.6/docdeid/utils.py
--rw-r--r--   0        0        0     1464 2023-03-28 14:40:16.110491 docdeid-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 docdeid-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1033 2023-07-26 09:11:40.718201 docdeid-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     3972 2023-07-26 09:11:40.718201 docdeid-0.1.7/README.md
+-rw-r--r--   0        0        0      291 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/__init__.py
+-rw-r--r--   0        0        0     4203 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/annotation.py
+-rw-r--r--   0        0        0     2289 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/deidentifier.py
+-rw-r--r--   0        0        0     4677 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/document.py
+-rw-r--r--   0        0        0      103 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/ds/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/ds/ds.py
+-rw-r--r--   0        0        0     9440 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/ds/lookup.py
+-rw-r--r--   0        0        0     2028 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/pattern.py
+-rw-r--r--   0        0        0      372 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/__init__.py
+-rw-r--r--   0        0        0     7970 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/annotation_set.py
+-rw-r--r--   0        0        0     7824 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/annotator.py
+-rw-r--r--   0        0        0     4079 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/doc.py
+-rw-r--r--   0        0        0     5366 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/redactor.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/py.typed
+-rw-r--r--   0        0        0      247 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/str/__init__.py
+-rw-r--r--   0        0        0     3930 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/str/processor.py
+-rw-r--r--   0        0        0    10273 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/tokenize.py
+-rw-r--r--   0        0        0      879 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/utils.py
+-rw-r--r--   0        0        0     1464 2023-07-26 09:11:40.722201 docdeid-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 docdeid-0.1.7/PKG-INFO
```

### Comparing `docdeid-0.1.6/LICENSE.md` & `docdeid-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/README.md` & `docdeid-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/annotation.py` & `docdeid-0.1.7/docdeid/annotation.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/deidentifier.py` & `docdeid-0.1.7/docdeid/deidentifier.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/document.py` & `docdeid-0.1.7/docdeid/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from docdeid.annotation import AnnotationSet
 from docdeid.tokenize import Tokenizer, TokenList
 
 
 class MetaData:
     """
-    Contains additional information on a text that is provided by the user on input. A :class:`.MetaData` object is
-    kept with the text in a :class:`.Document`, where it can be accessed by document processors. Note that a
-    :class:`.MetaData` object does not allow overwriting keys. This is done to prevent document processors
-    accidentally interfering with each other.
+    Contains additional information on a text that is provided by the user on input. A :class:`.MetaData` object is kept
+    with the text in a :class:`.Document`, where it can be accessed by document processors. Note that a
+    :class:`.MetaData` object does not allow overwriting keys. This is done to prevent document processors accidentally
+    interfering with each other.
 
     Args:
         items: A ``dict`` of items to initialize with.
     """
 
     def __init__(self, items: Optional[dict] = None) -> None:
         self._items = items or {}
```

### Comparing `docdeid-0.1.6/docdeid/ds/lookup.py` & `docdeid-0.1.7/docdeid/ds/lookup.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/pattern.py` & `docdeid-0.1.7/docdeid/pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         """
 
         return True
 
     @abstractmethod
     def match(self, token: Token, metadata: MetaData) -> Optional[tuple[Token, Token]]:
         """
-        Check if the token provided matches this pattern. Instantiations of :class:`.TokenPattern` should implement
-        the logic of the pattern in this method. For example, by checking if the text is lowercase, titlecase, longer
-        than a certain number of characters, etc. The :class:`.Token` neighbours may be accessible by
-        :meth:`.Token.previous` and :meth:`.Token.next`, if linked by the tokenizer.
+        Check if the token provided matches this pattern. Instantiations of :class:`.TokenPattern` should implement the
+        logic of the pattern in this method. For example, by checking if the text is lowercase, titlecase, longer than a
+        certain number of characters, etc. The :class:`.Token` neighbours may be accessible by :meth:`.Token.previous`
+        and :meth:`.Token.next`, if linked by the tokenizer.
 
         Args:
             token: The token.
             metadata: The metadata.
 
         Returns:
             A tuple with the start and end :class:`.Token` if matching, or ``None`` if no match is possible.
```

### Comparing `docdeid-0.1.6/docdeid/process/annotation_set.py` & `docdeid-0.1.7/docdeid/process/annotation_set.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/process/annotator.py` & `docdeid-0.1.7/docdeid/process/annotator.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/process/doc.py` & `docdeid-0.1.7/docdeid/process/doc.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/process/redactor.py` & `docdeid-0.1.7/docdeid/process/redactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     Instantiations should implement the logic in :meth:`.Redactor.redact`.
     """
 
     def process(self, doc: Document, **kwargs) -> None:
         """
         Process a document by redacting it, according to the logic in :meth:`.Redactor.redact`.
+
         Args:
             doc: The document to process.
             **kwargs: Any other arguments.
         """
         redacted_text = self.redact(doc.text, doc.annotations)
         doc.set_deidentified_text(redacted_text)
```

### Comparing `docdeid-0.1.6/docdeid/str/processor.py` & `docdeid-0.1.7/docdeid/str/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,16 @@
         return self._normalize_value(item)
 
 
 class ReplaceNonAsciiCharacters(StringModifier):
     """
     Maps non-ascii characters to ascii characters.
 
-    E.g.: Renée -> Renee. It's advised to test this before using as
-    mapping can be tricky in practice for some characters.
+    E.g.: Renée -> Renee. It's advised to test this before using as mapping can be tricky in practice for some
+    characters.
     """
 
     @staticmethod
     def _normalize_value(text: str) -> str:
         text = unicodedata.normalize("NFD", text)
         text = text.encode("ascii", "ignore").decode("utf-8")
```

### Comparing `docdeid-0.1.6/docdeid/tokenize.py` & `docdeid-0.1.7/docdeid/tokenize.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/docdeid/utils.py` & `docdeid-0.1.7/docdeid/utils.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.6/pyproject.toml` & `docdeid-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docdeid"
-version = "0.1.6"
+version = "0.1.7"
 description = "Create your own document de-identifier using docdeid, a simple framework independent of language or domain."
 license = "MIT"
 authors = [
     "Vincent Menger <vmenger@protonmail.com>"
     ]
 readme = "README.md"
 keywords = ["python", "document de-identification", "de-identification", "document de-identifier", "de-identifier"]
```

### Comparing `docdeid-0.1.6/PKG-INFO` & `docdeid-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: docdeid
-Version: 0.1.6
+Version: 0.1.7
 Summary: Create your own document de-identifier using docdeid, a simple framework independent of language or domain.
 License: MIT
 Keywords: python,document de-identification,de-identification,document de-identifier,de-identifier
 Author: Vincent Menger
 Author-email: vmenger@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Description-Content-Type: text/markdown
```

