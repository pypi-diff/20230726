# Comparing `tmp/mo_logs-8.417.23168-py2.py3-none-any.whl.zip` & `tmp/mo_logs-8.425.23207-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 43103 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat    15892 b- defN 23-Jun-14 22:50 mo_logs/__init__.py
+Zip file size: 43119 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat    15856 b- defN 23-Jul-26 01:48 mo_logs/__init__.py
 -rw-rw-rw-  2.0 fat     2329 b- defN 23-Apr-30 18:00 mo_logs/constants.py
 -rw-rw-rw-  2.0 fat     2407 b- defN 23-May-30 00:22 mo_logs/convert.py
--rw-rw-rw-  2.0 fat     8762 b- defN 23-Jun-14 02:49 mo_logs/exceptions.py
+-rw-rw-rw-  2.0 fat     8768 b- defN 23-Jul-26 01:48 mo_logs/exceptions.py
 -rw-rw-rw-  2.0 fat     3524 b- defN 23-Apr-30 18:00 mo_logs/log_usingEmail.py
 -rw-rw-rw-  2.0 fat     1099 b- defN 23-Apr-30 18:00 mo_logs/log_usingFile.py
 -rw-rw-rw-  2.0 fat     3301 b- defN 23-May-09 22:44 mo_logs/log_usingHandler.py
 -rw-rw-rw-  2.0 fat     2013 b- defN 23-Apr-30 18:00 mo_logs/log_usingLogger.py
 -rw-rw-rw-  2.0 fat     2589 b- defN 23-Apr-30 18:00 mo_logs/log_usingMozLog.py
 -rw-rw-rw-  2.0 fat     1454 b- defN 23-Apr-30 18:00 mo_logs/log_usingMulti.py
 -rw-rw-rw-  2.0 fat      450 b- defN 23-Apr-30 18:00 mo_logs/log_usingNothing.py
 -rw-rw-rw-  2.0 fat     4069 b- defN 23-Apr-30 18:00 mo_logs/log_usingSES.py
 -rw-rw-rw-  2.0 fat     1525 b- defN 23-May-30 00:22 mo_logs/log_usingStream.py
 -rw-rw-rw-  2.0 fat     2325 b- defN 23-Apr-30 18:00 mo_logs/log_usingThread.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-May-30 00:22 mo_logs/startup.py
 -rw-rw-rw-  2.0 fat    25364 b- defN 23-Jun-14 02:49 mo_logs/strings.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/RECORD
-21 files, 119604 bytes uncompressed, 40369 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jul-26 01:48 mo_logs-8.425.23207.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17648 b- defN 23-Jul-26 01:48 mo_logs-8.425.23207.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-26 01:48 mo_logs-8.425.23207.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-26 01:48 mo_logs-8.425.23207.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1700 b- defN 23-Jul-26 01:48 mo_logs-8.425.23207.dist-info/RECORD
+21 files, 119574 bytes uncompressed, 40385 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: mo_logs/startup.py
 Comment: 
 
 Filename: mo_logs/strings.py
 Comment: 
 
-Filename: mo_logs-8.417.23168.dist-info/LICENSE
+Filename: mo_logs-8.425.23207.dist-info/LICENSE
 Comment: 
 
-Filename: mo_logs-8.417.23168.dist-info/METADATA
+Filename: mo_logs-8.425.23207.dist-info/METADATA
 Comment: 
 
-Filename: mo_logs-8.417.23168.dist-info/WHEEL
+Filename: mo_logs-8.425.23207.dist-info/WHEEL
 Comment: 
 
-Filename: mo_logs-8.417.23168.dist-info/top_level.txt
+Filename: mo_logs-8.425.23207.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_logs-8.417.23168.dist-info/RECORD
+Filename: mo_logs-8.425.23207.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_logs/__init__.py

```diff
@@ -163,15 +163,15 @@
             LogItem(
                 severity=exceptions.NOTE,
                 template=template,
                 params=dict(default_params, **more_params),
                 timestamp=timestamp,
             ),
             stack_depth + 1,
-            static_template=static_template
+            static_template
         )
 
     info = note
 
     @classmethod
     def alarm(cls, template, default_params={}, *, stack_depth=0, static_template=True, **more_params):
         """
@@ -187,15 +187,15 @@
             LogItem(
                 severity=exceptions.ALARM,
                 template=template,
                 params=dict(default_params, **more_params),
                 timestamp=timestamp,
             ),
             stack_depth + 1,
-            static_template=static_template
+            static_template
         )
 
     alert = alarm
 
     @classmethod
     def warning(
         cls,
@@ -222,15 +222,15 @@
             default_params = {}
 
         params = to_data(dict(default_params, **more_params))
         cause = unwraplist([Except.wrap(c, stack_depth=2) for c in listwrap(cause or exc_info)])
         trace = exceptions.get_stacktrace(stack_depth + 1)
 
         e = Except(severity=log_severity, template=template, params=params, cause=cause, trace=trace,)
-        Log._annotate(e, stack_depth + 1, static_template=static_template)
+        Log._annotate(e, stack_depth + 1, static_template)
 
     warn = warning
 
     @classmethod
     def error(
         cls,
         template,  # human readable template
@@ -268,23 +268,23 @@
         cause = unwraplist([Except.wrap(c, stack_depth=2) for c in listwrap(cause or exc_info)])
         trace = exceptions.get_stacktrace(stack_depth + 1)
 
         e = Except(severity=exceptions.ERROR, template=template, params=params, cause=cause, trace=trace,)
         raise_from_none(e)
 
     @classmethod
-    def _annotate(cls, item, stack_depth, static_template=False):
+    def _annotate(cls, item, stack_depth, static_template):
         """
         :param item:  A LogItem THE TYPE OF MESSAGE
         :param stack_depth: FOR TRACKING WHAT LINE THIS CAME FROM
         :return:
         """
         given_template = item.template
         given_template = strings.limit(given_template, 10000)
-        param_template = "".join(f"{text}{{params.{code}}}" for text, code in strings.parse_template(given_template))
+        param_template = "".join(f"{text}{{params.{code}}}" if code else text for text, code in strings.parse_template(given_template))
 
         if isinstance(item, Except):
             param_template = "{severity}: " + param_template + STACKTRACE
             temp = item.__data__()
             temp.trace_text = item.trace_text
             temp.cause_text = item.cause_text
             item = temp
```

## mo_logs/exceptions.py

```diff
@@ -139,15 +139,15 @@
         for c in listwrap(self.cause):
             try:
                 if isinstance(c, Except):
                     cause_strings.append(c._desc_text(depth+1))
                 else:
                     cause_strings.append(str(c))
             except Exception as cause:
-                sys.stderr(f"Problem serializing cause {cause}")
+                sys.stderr.write(f"Problem serializing cause {cause}")
 
         return "caused by\n\t" + "and caused by\n\t".join(cause_strings)
 
     def __data__(self):
         output = to_data({k: getattr(self, k) for k in vars(self)})
         output.cause = unwraplist([c.__data__() for c in listwrap(output.cause)])
         return output
```

## Comparing `mo_logs-8.417.23168.dist-info/LICENSE` & `mo_logs-8.425.23207.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_logs-8.417.23168.dist-info/METADATA` & `mo_logs-8.425.23207.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-logs
-Version: 8.417.23168
+Version: 8.425.23207
 Summary: More Logs! Structured Logging and Exception Handling
 Home-page: https://github.com/klahnakoski/mo-logs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

