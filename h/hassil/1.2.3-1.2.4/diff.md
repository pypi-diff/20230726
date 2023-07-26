# Comparing `tmp/hassil-1.2.3.tar.gz` & `tmp/hassil-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassil-1.2.3.tar", last modified: Wed Jul 26 20:44:15 2023, max compression
+gzip compressed data, was "hassil-1.2.4.tar", last modified: Wed Jul 26 21:43:14 2023, max compression
```

## Comparing `hassil-1.2.3.tar` & `hassil-1.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.3/HassILGrammar.g4
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.3/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.3/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-26 20:44:15.034646 hassil-1.2.3/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.3/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/hassil/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-26 17:40:42.000000 hassil-1.2.3/hassil/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.3/hassil/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.3/hassil/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.3/hassil/_resources.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/parse_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.3/hassil/py.typed
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38063 2023-07-26 20:39:51.000000 hassil-1.2.3/hassil/recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.3/hassil/sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.3/hassil/sample_template.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.3/hassil/util.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/hassil.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.3/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.3/requirements_dev.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-26 20:44:15.034646 hassil-1.2.3/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2070 2023-07-25 14:23:19.000000 hassil-1.2.3/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.3/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.3/tests/test_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.3/tests/test_intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.3/tests/test_parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    24093 2023-07-26 20:40:20.000000 hassil-1.2.3/tests/test_recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.3/tests/test_sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.3/tests/test_util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 21:43:14.149237 hassil-1.2.4/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.4/HassILGrammar.g4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.4/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.4/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-26 21:43:14.149237 hassil-1.2.4/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.4/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 21:43:14.149237 hassil-1.2.4/hassil/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-26 21:36:53.000000 hassil-1.2.4/hassil/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.4/hassil/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.4/hassil/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.4/hassil/_resources.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.4/hassil/expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.4/hassil/intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.4/hassil/parse_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.4/hassil/parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.4/hassil/py.typed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38866 2023-07-26 21:33:59.000000 hassil-1.2.4/hassil/recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.4/hassil/sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.4/hassil/sample_template.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.4/hassil/util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 21:43:14.149237 hassil-1.2.4/hassil.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-26 21:43:14.000000 hassil-1.2.4/hassil.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-26 21:43:14.000000 hassil-1.2.4/hassil.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-26 21:43:14.000000 hassil-1.2.4/hassil.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-26 21:43:14.000000 hassil-1.2.4/hassil.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-26 21:43:14.000000 hassil-1.2.4/hassil.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-26 21:43:14.000000 hassil-1.2.4/hassil.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.4/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.4/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-26 21:43:14.149237 hassil-1.2.4/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2070 2023-07-25 14:23:19.000000 hassil-1.2.4/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 21:43:14.149237 hassil-1.2.4/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.4/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.4/tests/test_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.4/tests/test_intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.4/tests/test_parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    24752 2023-07-26 21:40:01.000000 hassil-1.2.4/tests/test_recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.4/tests/test_sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.4/tests/test_util.py
```

### Comparing `hassil-1.2.3/HassILGrammar.g4` & `hassil-1.2.4/HassILGrammar.g4`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/LICENSE.md` & `hassil-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/PKG-INFO` & `hassil-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.3
+Version: 1.2.4
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hassil-1.2.3/README.md` & `hassil-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/__main__.py` & `hassil-1.2.4/hassil/__main__.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/expression.py` & `hassil-1.2.4/hassil/expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/intents.py` & `hassil-1.2.4/hassil/intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/parse_expression.py` & `hassil-1.2.4/hassil/parse_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/parser.py` & `hassil-1.2.4/hassil/parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/recognize.py` & `hassil-1.2.4/hassil/recognize.py`

 * *Files 2% similar despite different names*

```diff
@@ -657,37 +657,56 @@
         if chunk.is_empty:
             # Skip empty chunk (NOT whitespace)
             yield context
         else:
             wildcard = context.get_open_wildcard()
             if (wildcard is not None) and (not wildcard.text.strip()):
                 if not chunk_text.strip():
+                    # Skip space
                     yield MatchContext(
                         text=context_text,
                         is_start_of_word=True,
                         # Copy over
                         entities=context.entities,
                         intent_context=context.intent_context,
                         unmatched_entities=context.unmatched_entities,
                     )
                     return
 
                 # Wildcard cannot be empty
-                end_idx = context_text.rfind(chunk_text)
-                if end_idx < 1:
+                start_idx = context_text.find(chunk_text)
+                if start_idx <= 0:
                     # Cannot possibly match
                     return
 
-                # Consume text until chunk is found later
-                wildcard.text += context_text[:end_idx]
-                wildcard.value = wildcard.text
+                while start_idx > 0:
+                    wildcard_text = context_text[:start_idx]
+                    yield from match_expression(
+                        settings,
+                        MatchContext(
+                            text=context_text[start_idx:],
+                            is_start_of_word=True,
+                            entities=context.entities[:-1]
+                            + [
+                                MatchEntity(
+                                    name=wildcard.name,
+                                    text=wildcard_text,
+                                    value=wildcard_text,
+                                )
+                            ],
+                            # Copy over
+                            intent_context=context.intent_context,
+                            unmatched_entities=context.unmatched_entities,
+                        ),
+                        expression,
+                    )
+                    start_idx = context_text.find(chunk_text, start_idx + 1)
 
-                # Continue matching with the wildcard started
-                context_text = context_text[end_idx:]
-                is_context_text_empty = len(context_text.strip()) == 0
+                # Do not continue with matching
+                return
 
             if context_text.startswith(chunk_text):
                 # Successful match for chunk
                 context_text = context_text[len(chunk_text) :]
                 is_chunk_word = bool(chunk_text) and (not chunk_text.isspace())
                 yield MatchContext(
                     text=context_text,
```

### Comparing `hassil-1.2.3/hassil/sample.py` & `hassil-1.2.4/hassil/sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/sample_template.py` & `hassil-1.2.4/hassil/sample_template.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil/util.py` & `hassil-1.2.4/hassil/util.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/hassil.egg-info/PKG-INFO` & `hassil-1.2.4/hassil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.3
+Version: 1.2.4
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hassil-1.2.3/hassil.egg-info/SOURCES.txt` & `hassil-1.2.4/hassil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/setup.py` & `hassil-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/tests/test_expression.py` & `hassil-1.2.4/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/tests/test_intents.py` & `hassil-1.2.4/tests/test_intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/tests/test_parser.py` & `hassil-1.2.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/tests/test_recognize.py` & `hassil-1.2.4/tests/test_recognize.py`

 * *Files 4% similar despite different names*

```diff
@@ -733,16 +733,17 @@
     """Test wildcard slot lists/entities."""
     yaml_text = """
     language: "en"
     intents:
       Test:
         data:
           - sentences:
-              - "play {album} by {artist} [please] now"
+              - "play {album} by {artist}[ please] now"
               - "start {album} by {artist}"
+              - "begin {album} by artist {artist}"
     lists:
       album:
         wildcard: true
       artist:
         wildcard: true
     """
 
@@ -766,20 +767,37 @@
     result = recognize(sentence, intents)
     assert result is not None, f"{sentence} should match"
     assert set(result.entities.keys()) == {"album", "artist"}
     assert result.entities["album"].value == "the white album "
     assert result.entities["artist"].value == "the beatles"
 
     # Test use of next word in wildcard
-    sentence = "play by by by now now now"
+    sentence = "play day by day by taken by trees now"
+    results = list(recognize_all(sentence, intents))
+    assert results, f"{sentence} should match"
+    assert len(results) == 3  # 3 "by" words
+
+    # Verify each combination of album/artist is present
+    album_artist = {
+        (result.entities["album"].value, result.entities["artist"].value)
+        for result in results
+    }
+    assert album_artist == {
+        ("day ", "day by taken by trees "),
+        ("day by day ", "taken by trees "),
+        ("day by day by taken ", "trees "),
+    }
+
+    # Add "artist" word
+    sentence = "begin day by day by artist taken by trees"
     result = recognize(sentence, intents)
     assert result is not None, f"{sentence} should match"
     assert set(result.entities.keys()) == {"album", "artist"}
-    assert result.entities["album"].value == "by by "
-    assert result.entities["artist"].value == "now now "
+    assert result.entities["album"].value == "day by day "
+    assert result.entities["artist"].value == "taken by trees"
 
 
 def test_optional_wildcard() -> None:
     """Test optional wildcard slot list."""
     yaml_text = """
     language: "en"
     intents:
```

### Comparing `hassil-1.2.3/tests/test_sample.py` & `hassil-1.2.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.3/tests/test_util.py` & `hassil-1.2.4/tests/test_util.py`

 * *Files identical despite different names*

