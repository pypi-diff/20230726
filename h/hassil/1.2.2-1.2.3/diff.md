# Comparing `tmp/hassil-1.2.2.tar.gz` & `tmp/hassil-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassil-1.2.2.tar", last modified: Tue Jul 25 16:39:14 2023, max compression
+gzip compressed data, was "hassil-1.2.3.tar", last modified: Wed Jul 26 20:44:15 2023, max compression
```

## Comparing `hassil-1.2.2.tar` & `hassil-1.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.2/HassILGrammar.g4
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.2/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.2/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-25 16:39:14.466897 hassil-1.2.2/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.2/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/hassil/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-25 14:47:00.000000 hassil-1.2.2/hassil/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.2/hassil/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.2/hassil/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.2/hassil/_resources.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/parse_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.2/hassil/py.typed
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36650 2023-07-25 16:32:53.000000 hassil-1.2.2/hassil/recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.2/hassil/sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.2/hassil/sample_template.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.2/hassil/util.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/hassil.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.2/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.2/requirements_dev.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-25 16:39:14.466897 hassil-1.2.2/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2070 2023-07-25 14:23:19.000000 hassil-1.2.2/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.2/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.2/tests/test_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.2/tests/test_intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.2/tests/test_parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23283 2023-07-25 16:32:41.000000 hassil-1.2.2/tests/test_recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.2/tests/test_sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.2/tests/test_util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.3/HassILGrammar.g4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.3/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.3/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-26 20:44:15.034646 hassil-1.2.3/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.3/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/hassil/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-26 17:40:42.000000 hassil-1.2.3/hassil/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.3/hassil/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.3/hassil/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.3/hassil/_resources.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/parse_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.3/hassil/parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.3/hassil/py.typed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38063 2023-07-26 20:39:51.000000 hassil-1.2.3/hassil/recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.3/hassil/sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.3/hassil/sample_template.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.3/hassil/util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/hassil.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-26 20:44:15.000000 hassil-1.2.3/hassil.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.3/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.3/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-26 20:44:15.034646 hassil-1.2.3/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2070 2023-07-25 14:23:19.000000 hassil-1.2.3/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-26 20:44:15.034646 hassil-1.2.3/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.3/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.3/tests/test_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.3/tests/test_intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.3/tests/test_parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    24093 2023-07-26 20:40:20.000000 hassil-1.2.3/tests/test_recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.3/tests/test_sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.3/tests/test_util.py
```

### Comparing `hassil-1.2.2/HassILGrammar.g4` & `hassil-1.2.3/HassILGrammar.g4`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/LICENSE.md` & `hassil-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/PKG-INFO` & `hassil-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.2
+Version: 1.2.3
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hassil-1.2.2/README.md` & `hassil-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/__main__.py` & `hassil-1.2.3/hassil/__main__.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/expression.py` & `hassil-1.2.3/hassil/expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/intents.py` & `hassil-1.2.3/hassil/intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/parse_expression.py` & `hassil-1.2.3/hassil/parse_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/parser.py` & `hassil-1.2.3/hassil/parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/recognize.py` & `hassil-1.2.3/hassil/recognize.py`

 * *Files 2% similar despite different names*

```diff
@@ -653,92 +653,120 @@
         # So we have to continue matching, skipping over empty or whitespace
         # chunks until the template is exhausted.
         is_context_text_empty = len(context_text.strip()) == 0
 
         if chunk.is_empty:
             # Skip empty chunk (NOT whitespace)
             yield context
-        elif context_text.startswith(chunk_text):
-            # Successful match for chunk
-            context_text = context_text[len(chunk_text) :]
-            is_chunk_word = bool(chunk_text) and (not chunk_text.isspace())
-            yield MatchContext(
-                text=context_text,
-                # must use chunk.text because it hasn't been stripped
-                is_start_of_word=chunk.text.endswith(" "),
-                # Copy over
-                entities=context.entities,
-                intent_context=context.intent_context,
-                unmatched_entities=context.unmatched_entities,
-                #
-                close_wildcards=is_chunk_word,
-                close_unmatched=is_chunk_word,
-            )
-        elif is_context_text_empty and chunk_text.isspace():
-            # No text left to match, so extra whitespace is OK to skip
-            yield context
         else:
-            # Remove punctuation and try again
-            context_text = PUNCTUATION.sub("", context.text)
-            context_starts_with = context_text.startswith(chunk_text)
-            if (not context_starts_with) and context.is_start_of_word:
-                # Try stripping whitespace
-                context_text = context_text.lstrip()
-                context_starts_with = context_text.startswith(chunk_text)
+            wildcard = context.get_open_wildcard()
+            if (wildcard is not None) and (not wildcard.text.strip()):
+                if not chunk_text.strip():
+                    yield MatchContext(
+                        text=context_text,
+                        is_start_of_word=True,
+                        # Copy over
+                        entities=context.entities,
+                        intent_context=context.intent_context,
+                        unmatched_entities=context.unmatched_entities,
+                    )
+                    return
+
+                # Wildcard cannot be empty
+                end_idx = context_text.rfind(chunk_text)
+                if end_idx < 1:
+                    # Cannot possibly match
+                    return
+
+                # Consume text until chunk is found later
+                wildcard.text += context_text[:end_idx]
+                wildcard.value = wildcard.text
+
+                # Continue matching with the wildcard started
+                context_text = context_text[end_idx:]
+                is_context_text_empty = len(context_text.strip()) == 0
 
-            if context_starts_with:
+            if context_text.startswith(chunk_text):
+                # Successful match for chunk
                 context_text = context_text[len(chunk_text) :]
+                is_chunk_word = bool(chunk_text) and (not chunk_text.isspace())
                 yield MatchContext(
                     text=context_text,
+                    # must use chunk.text because it hasn't been stripped
+                    is_start_of_word=chunk.text.endswith(" "),
                     # Copy over
                     entities=context.entities,
                     intent_context=context.intent_context,
-                    is_start_of_word=context.is_start_of_word,
                     unmatched_entities=context.unmatched_entities,
+                    #
+                    close_wildcards=is_chunk_word,
+                    close_unmatched=is_chunk_word,
                 )
-            elif wildcard := context.get_open_wildcard():
-                # Add to wildcard by skipping ahead in the text until we find
-                # the current chunk text.
-                skip_idx = context_text.find(chunk_text)
-                if skip_idx >= 0:
-                    wildcard.text += context_text[:skip_idx]
-
-                    # Wildcards cannot be empty
-                    if wildcard.text:
-                        wildcard.value = wildcard.text
-                        yield MatchContext(
-                            text=context.text[skip_idx + len(chunk_text) :],
-                            # Copy over
-                            entities=context.entities,
-                            intent_context=context.intent_context,
-                            is_start_of_word=True,
-                            unmatched_entities=context.unmatched_entities,
-                        )
-            elif settings.allow_unmatched_entities and (
-                unmatched_entity := context.get_open_entity()
-            ):
-                # Add to the most recent unmatched entity by skipping ahead in
-                # the text until we find the current chunk text.
-                skip_idx = context_text.find(chunk_text)
-                if skip_idx >= 0:
-                    unmatched_entity.text += context_text[:skip_idx]
-
-                    # Unmatched entities cannot be empty
-                    if unmatched_entity.text:
-                        yield MatchContext(
-                            text=context.text[skip_idx + len(chunk_text) :],
-                            # Copy over
-                            entities=context.entities,
-                            intent_context=context.intent_context,
-                            is_start_of_word=True,
-                            unmatched_entities=context.unmatched_entities,
-                        )
+            elif is_context_text_empty and chunk_text.isspace():
+                # No text left to match, so extra whitespace is OK to skip
+                yield context
             else:
-                # Match failed
-                pass
+                # Remove punctuation and try again
+                context_text = PUNCTUATION.sub("", context.text)
+                context_starts_with = context_text.startswith(chunk_text)
+                if (not context_starts_with) and context.is_start_of_word:
+                    # Try stripping whitespace
+                    context_text = context_text.lstrip()
+                    context_starts_with = context_text.startswith(chunk_text)
+
+                if context_starts_with:
+                    context_text = context_text[len(chunk_text) :]
+                    yield MatchContext(
+                        text=context_text,
+                        # Copy over
+                        entities=context.entities,
+                        intent_context=context.intent_context,
+                        is_start_of_word=context.is_start_of_word,
+                        unmatched_entities=context.unmatched_entities,
+                    )
+                elif wildcard is not None:
+                    # Add to wildcard by skipping ahead in the text until we find
+                    # the current chunk text.
+                    skip_idx = context_text.find(chunk_text)
+                    if skip_idx >= 0:
+                        wildcard.text += context_text[:skip_idx]
+
+                        # Wildcards cannot be empty
+                        if wildcard.text:
+                            wildcard.value = wildcard.text
+                            yield MatchContext(
+                                text=context.text[skip_idx + len(chunk_text) :],
+                                # Copy over
+                                entities=context.entities,
+                                intent_context=context.intent_context,
+                                is_start_of_word=True,
+                                unmatched_entities=context.unmatched_entities,
+                            )
+                elif settings.allow_unmatched_entities and (
+                    unmatched_entity := context.get_open_entity()
+                ):
+                    # Add to the most recent unmatched entity by skipping ahead in
+                    # the text until we find the current chunk text.
+                    skip_idx = context_text.find(chunk_text)
+                    if skip_idx >= 0:
+                        unmatched_entity.text += context_text[:skip_idx]
+
+                        # Unmatched entities cannot be empty
+                        if unmatched_entity.text:
+                            yield MatchContext(
+                                text=context.text[skip_idx + len(chunk_text) :],
+                                # Copy over
+                                entities=context.entities,
+                                intent_context=context.intent_context,
+                                is_start_of_word=True,
+                                unmatched_entities=context.unmatched_entities,
+                            )
+                else:
+                    # Match failed
+                    pass
     elif isinstance(expression, Sequence):
         seq: Sequence = expression
         if seq.type == SequenceType.ALTERNATIVE:
             # Any may match (words | in | alternative)
             # NOTE: [optional] = (optional | )
             for item in seq.items:
                 yield from match_expression(settings, context, item)
```

### Comparing `hassil-1.2.2/hassil/sample.py` & `hassil-1.2.3/hassil/sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/sample_template.py` & `hassil-1.2.3/hassil/sample_template.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil/util.py` & `hassil-1.2.3/hassil/util.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/hassil.egg-info/PKG-INFO` & `hassil-1.2.3/hassil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.2
+Version: 1.2.3
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hassil-1.2.2/hassil.egg-info/SOURCES.txt` & `hassil-1.2.3/hassil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/setup.py` & `hassil-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/tests/test_expression.py` & `hassil-1.2.3/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/tests/test_intents.py` & `hassil-1.2.3/tests/test_intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/tests/test_parser.py` & `hassil-1.2.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/tests/test_recognize.py` & `hassil-1.2.3/tests/test_recognize.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,16 +590,17 @@
     """Test that unmatched entities are not empty."""
     yaml_text = """
     language: "en"
     intents:
       Test:
         data:
           - sentences:
-              - "turn on {name}"
+              - "turn on {name}[ please]"
               - "illuminate all[ {area}] lights"
+              - "activate {name} now"
     lists:
       name:
         values:
           - light
       area:
         values:
           - bedroom
@@ -608,14 +609,19 @@
     with io.StringIO(yaml_text) as test_file:
         intents = Intents.from_yaml(test_file)
 
     sentence = "turn on "
     results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
     assert not results, f"{sentence} should not match"
 
+    # With optional word at end
+    sentence = "turn on please"
+    results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
+    assert not results, f"{sentence} should not match"
+
     sentence = "illuminate all lights"
     results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
     assert results, f"{sentence} should match"
     assert len(results) == 1, "Only 1 result expected"
     assert not results[0].unmatched_entities, "No unmatched entities expected"
 
     sentence = "illuminate all kitchen lights"
@@ -624,14 +630,19 @@
     assert len(results) == 1, "Only 1 result expected"
     result = results[0]
     assert set(result.unmatched_entities.keys()) == {"area"}
     area = result.unmatched_entities["area"]
     assert isinstance(area, UnmatchedTextEntity)
     assert area.text == "kitchen "
 
+    # With required word at end
+    sentence = "activate now"
+    results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
+    assert not results, f"{sentence} should not match"
+
 
 def test_unmatched_entity_context() -> None:
     """Test that unmatched entities work with requires/excludes context."""
     yaml_text = """
     language: "en"
     intents:
       Test:
@@ -754,14 +765,22 @@
     sentence = "start the white album by the beatles"
     result = recognize(sentence, intents)
     assert result is not None, f"{sentence} should match"
     assert set(result.entities.keys()) == {"album", "artist"}
     assert result.entities["album"].value == "the white album "
     assert result.entities["artist"].value == "the beatles"
 
+    # Test use of next word in wildcard
+    sentence = "play by by by now now now"
+    result = recognize(sentence, intents)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.entities.keys()) == {"album", "artist"}
+    assert result.entities["album"].value == "by by "
+    assert result.entities["artist"].value == "now now "
+
 
 def test_optional_wildcard() -> None:
     """Test optional wildcard slot list."""
     yaml_text = """
     language: "en"
     intents:
       Test:
```

### Comparing `hassil-1.2.2/tests/test_sample.py` & `hassil-1.2.3/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.2/tests/test_util.py` & `hassil-1.2.3/tests/test_util.py`

 * *Files identical despite different names*

