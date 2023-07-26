# Comparing `tmp/devchat_ask-0.0.4-py3-none-any.whl.zip` & `tmp/devchat_ask-0.0.5-cp311-cp311-macosx_12_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,52 @@
-Zip file size: 50138 bytes, number of entries: 22
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/__init__.py
--rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 chat/__init__.pye
--rw-r--r--  2.0 unx      448 b- defN 80-Jan-01 00:00 chat/ask_codebase/__init__.pye
--rw-r--r--  2.0 unx      160 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/__init__.pye
--rw-r--r--  2.0 unx     2672 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/simple_qa.pye
--rw-r--r--  2.0 unx     3632 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/stuff_dc_qa.pye
--rw-r--r--  2.0 unx      160 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/__init__.pye
--rw-r--r--  2.0 unx     2784 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/embedding.pye
--rw-r--r--  2.0 unx      160 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/__init__.pye
--rw-r--r--  2.0 unx      880 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/base.pye
--rw-r--r--  2.0 unx     7072 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/file.pye
--rw-r--r--  2.0 unx     7024 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/function.pye
--rw-r--r--  2.0 unx     1040 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/util.pye
--rw-r--r--  2.0 unx      160 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/__init__.pye
--rw-r--r--  2.0 unx     2288 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/file.pye
--rw-r--r--  2.0 unx    10448 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/qdrant.pye
--rw-r--r--  2.0 unx      144 b- defN 80-Jan-01 00:00 chat/util/__init__.pye
--rw-r--r--  2.0 unx     1696 b- defN 80-Jan-01 00:00 chat/util/decorator.pye
--rw-r--r--  2.0 unx     4784 b- defN 80-Jan-01 00:00 chat/util/misc.pye
--rw-r--r--  2.0 unx      600 b- defN 80-Jan-01 00:00 devchat_ask-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 devchat_ask-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1923 b- defN 16-Jan-01 00:00 devchat_ask-0.0.4.dist-info/RECORD
-22 files, 48291 bytes uncompressed, 46972 bytes compressed:  2.7%
+Zip file size: 1097866 bytes, number of entries: 50
+-rwxr-xr-x  2.0 unx    54920 b- defN 80-Jan-01 00:00 chat/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    57464 b- defN 80-Jan-01 00:00 chat/ask_codebase/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55040 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   104184 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/simple_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   106792 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/stuff_dc_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55056 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   128296 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/embedding.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55080 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    82152 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/base.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   180920 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/file.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   167432 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/function.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   105872 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/util.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55032 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   124320 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/file.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   191200 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/qdrant.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54992 b- defN 80-Jan-01 00:00 chat/evaluation/qa/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    83864 b- defN 80-Jan-01 00:00 chat/evaluation/qa/cli.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    56104 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   129560 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/evaluate.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   102176 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/markdown.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    83656 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/resume.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    84936 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/show.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77992 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    86080 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/base.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   106064 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/prototype_bot.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   101944 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/simple_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   102272 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/stuff_dc_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    83592 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/yes_no.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   186792 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluation.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    56128 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    83200 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/base.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    84112 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/correctness.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55144 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    57296 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/conf.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    82336 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/judge_pair.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    82488 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/judge_single.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    82056 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/rate_it.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    83680 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/rating.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   102616 b- defN 80-Jan-01 00:00 chat/evaluation/qa/question_set.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   190272 b- defN 80-Jan-01 00:00 chat/evaluation/qa/report.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   104544 b- defN 80-Jan-01 00:00 chat/evaluation/qa/util.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   158976 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/load.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    60080 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/example.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   233240 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/retrieval_eval.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54952 b- defN 80-Jan-01 00:00 chat/util/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   104600 b- defN 80-Jan-01 00:00 chat/util/decorator.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   126208 b- defN 80-Jan-01 00:00 chat/util/misc.cpython-311-darwin.so
+-rw-r--r--  2.0 unx      600 b- defN 80-Jan-01 00:00 devchat_ask-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      107 b- defN 80-Jan-01 00:00 devchat_ask-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5615 b- defN 16-Jan-01 00:00 devchat_ask-0.0.5.dist-info/RECORD
+50 files, 4672034 bytes uncompressed, 1088538 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,67 +1,151 @@
-Filename: chat/__init__.py
+Filename: chat/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/__init__.pye
+Filename: chat/ask_codebase/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/__init__.pye
+Filename: chat/ask_codebase/chains/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/chains/__init__.pye
+Filename: chat/ask_codebase/chains/simple_qa.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/chains/simple_qa.pye
+Filename: chat/ask_codebase/chains/stuff_dc_qa.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/chains/stuff_dc_qa.pye
+Filename: chat/ask_codebase/indexing/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/__init__.pye
+Filename: chat/ask_codebase/indexing/embedding.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/embedding.pye
+Filename: chat/ask_codebase/indexing/loader/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/loader/__init__.pye
+Filename: chat/ask_codebase/indexing/loader/base.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/loader/base.pye
+Filename: chat/ask_codebase/indexing/loader/file.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/loader/file.pye
+Filename: chat/ask_codebase/indexing/loader/function.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/loader/function.pye
+Filename: chat/ask_codebase/indexing/util.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/indexing/util.pye
+Filename: chat/ask_codebase/store/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/store/__init__.pye
+Filename: chat/ask_codebase/store/file.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/store/file.pye
+Filename: chat/ask_codebase/store/qdrant.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/ask_codebase/store/qdrant.pye
+Filename: chat/evaluation/qa/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/util/__init__.pye
+Filename: chat/evaluation/qa/cli.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/util/decorator.pye
+Filename: chat/evaluation/qa/commands/__init__.cpython-311-darwin.so
 Comment: 
 
-Filename: chat/util/misc.pye
+Filename: chat/evaluation/qa/commands/evaluate.cpython-311-darwin.so
 Comment: 
 
-Filename: devchat_ask-0.0.4.dist-info/METADATA
+Filename: chat/evaluation/qa/commands/markdown.cpython-311-darwin.so
 Comment: 
 
-Filename: devchat_ask-0.0.4.dist-info/WHEEL
+Filename: chat/evaluation/qa/commands/resume.cpython-311-darwin.so
 Comment: 
 
-Filename: devchat_ask-0.0.4.dist-info/RECORD
+Filename: chat/evaluation/qa/commands/show.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/base.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/prototype_bot.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/simple_qa.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/stuff_dc_qa.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/yes_no.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluation.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/base.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/correctness.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/conf.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/judge_pair.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/judge_single.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/rate_it.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/rating.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/question_set.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/report.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/util.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/retrieval/data/code_search_net_eval/load.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/retrieval/example.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/retrieval/retrieval_eval.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/util/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/util/decorator.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/util/misc.cpython-311-darwin.so
+Comment: 
+
+Filename: devchat_ask-0.0.5.dist-info/METADATA
+Comment: 
+
+Filename: devchat_ask-0.0.5.dist-info/WHEEL
+Comment: 
+
+Filename: devchat_ask-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `devchat_ask-0.0.4.dist-info/METADATA` & `devchat_ask-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat-ask
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Hezheng Yin
 Author-email: hezheng@merico.dev
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: instructorembedding (>=1.0.1,<2.0.0)
```

