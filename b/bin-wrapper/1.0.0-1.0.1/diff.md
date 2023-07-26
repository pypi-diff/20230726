# Comparing `tmp/bin_wrapper-1.0.0-py3-none-any.whl.zip` & `tmp/bin_wrapper-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5029 bytes, number of entries: 7
+Zip file size: 5119 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       32 b- defN 23-Jul-23 10:40 wrapper/__init__.py
--rw-r--r--  2.0 unx     5720 b- defN 23-Jul-23 10:57 wrapper/wrapper.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-25 13:35 bin_wrapper-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2959 b- defN 23-Jul-25 13:35 bin_wrapper-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 13:35 bin_wrapper-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-25 13:35 bin_wrapper-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      554 b- defN 23-Jul-25 13:35 bin_wrapper-1.0.0.dist-info/RECORD
-7 files, 10434 bytes uncompressed, 4043 bytes compressed:  61.3%
+-rw-r--r--  2.0 unx     5927 b- defN 23-Jul-26 16:03 wrapper/wrapper.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-26 16:05 bin_wrapper-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3173 b- defN 23-Jul-26 16:05 bin_wrapper-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 16:05 bin_wrapper-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-26 16:05 bin_wrapper-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      554 b- defN 23-Jul-26 16:05 bin_wrapper-1.0.1.dist-info/RECORD
+7 files, 10855 bytes uncompressed, 4133 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: wrapper/__init__.py
 Comment: 
 
 Filename: wrapper/wrapper.py
 Comment: 
 
-Filename: bin_wrapper-1.0.0.dist-info/LICENSE
+Filename: bin_wrapper-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: bin_wrapper-1.0.0.dist-info/METADATA
+Filename: bin_wrapper-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: bin_wrapper-1.0.0.dist-info/WHEEL
+Filename: bin_wrapper-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: bin_wrapper-1.0.0.dist-info/top_level.txt
+Filename: bin_wrapper-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bin_wrapper-1.0.0.dist-info/RECORD
+Filename: bin_wrapper-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wrapper/wrapper.py

```diff
@@ -37,62 +37,64 @@
     def __getattr__(self, item):
         attrs = self._parent_attrs.copy()
         attrs.append(item.replace('_', '-', -1))
 
         return ExecWrapper(self._bin, *attrs, **self._parent_kwargs)
 
     def __call__(self, *args, **kwargs) -> CompletedProcess:
-        self._pre(args, kwargs)
-
         proc_kwargs = {}
         rewrite_parent_kwargs = self._parent_kwargs.copy()
+        suppress_bool = rewrite_parent_kwargs.pop('suppress_bool', False)
+
+        self._pre(args, rewrite_parent_kwargs, kwargs)
+
         key_pfx = 'subprocess_'
         for k in list(kwargs.keys()):
             if k.startswith(key_pfx):
                 key = k[len(key_pfx):]
                 proc_kwargs[key] = kwargs.pop(k)
 
             if k in rewrite_parent_kwargs:
                 rewrite_parent_kwargs[k] = kwargs.pop(k)
 
         cmd = [str(self._bin)]
-        cmd.extend(self.args_from_dict(rewrite_parent_kwargs))
         cmd.extend(self._parent_attrs)
+        cmd.extend(self.args_from_dict(rewrite_parent_kwargs, suppress_bool))
         cmd.extend(args)
-        cmd.extend(self.args_from_dict(kwargs))
+        cmd.extend(self.args_from_dict(kwargs, suppress_bool))
 
         proc_kwargs['shell'] = True
         proc_kwargs['text'] = True
         if 'stdin' not in proc_kwargs:
             proc_kwargs['stdin'] = subprocess.PIPE
         if 'stdout' not in proc_kwargs:
             proc_kwargs['stdout'] = subprocess.PIPE
         if 'stderr' not in proc_kwargs:
             proc_kwargs['stderr'] = subprocess.PIPE
 
         return subprocess_run(*cmd, **proc_kwargs)
 
-    def _pre(self, args, kwargs):
+    def _pre(self, args, parent_kwargs, kwargs):
         pass
 
-    def args_from_dict(self, data: dict) -> list[str]:
+    def args_from_dict(self, data: dict, suppress_bool: bool) -> list[str]:
         kw_args = []
         for k, v in data.items():
-            if not k:
+            if not k or v is None:
                 continue
 
             key = k.replace('_', '-', -1)
 
             pfx, join = (self._pfx_char_short, None) if len(k) == 1 else (self._pfx_char_long, '=')
             flag = [pfx + key]
-            if v is not None:
-                val = str(v)
-                if isinstance(v, bool):
-                    val = val.lower()
-
+            val = str(v)
+            if isinstance(v, bool):
+                if v and not suppress_bool:
+                    flag.append(val.lower())
+            else:
                 flag.append(val)
 
             if not join:
                 kw_args.extend(flag)
             else:
                 kw_args.append(join.join(flag))
```

## Comparing `bin_wrapper-1.0.0.dist-info/LICENSE` & `bin_wrapper-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bin_wrapper-1.0.0.dist-info/METADATA` & `bin_wrapper-1.0.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bin-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Binary file wrapper
 Author-email: myback <54638513+myback@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 myback.space
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,12 +71,17 @@
     def __getattr__(self, item):
         h = Helm(**self._parent_kwargs)
         h._parent_attrs = self._parent_attrs.copy()
         h._parent_attrs.append(item.replace('_', '-', -1))
 
         return h
 
-    def _pre(self, args, kwargs):
-        ns = kwargs.pop('n', None)
-        if ns:
-            kwargs.setdefault('namespace', ns)
+    def _pre(self, args, parent_kwargs, kwargs):
+        ns_short = parent_kwargs.pop('n', None)
+        parent_kwargs.setdefault('namespace', ns_short)
+
+        out_short = parent_kwargs.pop('o', None)
+        out = parent_kwargs.pop('output', out_short)
+
+        out_short = kwargs.pop('o', out)
+        kwargs.setdefault('output', out_short)
 ```
```

