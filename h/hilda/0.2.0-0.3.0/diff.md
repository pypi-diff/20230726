# Comparing `tmp/hilda-0.2.0.tar.gz` & `tmp/hilda-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-0.2.0.tar", last modified: Sun Jul 16 15:28:25 2023, max compression
+gzip compressed data, was "hilda-0.3.0.tar", last modified: Wed Jul 26 14:52:45 2023, max compression
```

## Comparing `hilda-0.2.0.tar` & `hilda-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-16 15:28:08.000000 hilda-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-16 15:28:25.774668 hilda-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-16 15:28:08.000000 hilda-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.770668 hilda-0.2.0/hilda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/lldb_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/lsof.m
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/boringssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/remotepairingd.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/to_ns_from_json.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.770668 hilda-0.2.0/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-16 15:28:08.000000 hilda-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 15:28:08.000000 hilda-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:28:25.774668 hilda-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 14:52:25.000000 hilda-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-26 14:52:45.284183 hilda-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-07-26 14:52:25.000000 hilda-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.280183 hilda-0.3.0/hilda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42180 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/lldb_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/boringssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/to_ns_from_json.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/ui/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/ui/ui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-26 14:52:25.000000 hilda-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 14:52:25.000000 hilda-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:52:45.284183 hilda-0.3.0/setup.cfg
```

### Comparing `hilda-0.2.0/LICENSE` & `hilda-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/PKG-INFO` & `hilda-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLDB wrapped and empowered by iPython's features
-Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
+Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
@@ -298,14 +298,73 @@
 capabilities:
 
 ```python
 # execute the following to print the command's documentation
 stop?
 ```
 
+## UI Configuration
+
+Hilda contains minimal UI for examining the target state.
+The UI is divided into views:
+
+- Registers
+- Disassembly
+- Stack
+- Backtrace
+
+![img.png](gifs/ui.png)
+
+This UI can be displayed at any time be executing:
+
+```python
+ui.show()
+```
+
+By default `step_into` and `step_over` will show this UI automatically.
+You may disable this behaviour by executing:
+
+```python
+ui.active = False
+```
+
+Attentively, if you want to display UI after hitting a breakpoint, you can register `ui.show` as callback:
+
+```python
+symbol(0x7ff7b97c21b0).bp(ui.show)
+```
+
+Try playing with the UI settings by yourself:
+
+```python
+# Disable stack view
+ui.views.stack.active = False
+
+# View words from the stack
+ui.views.stack.depth = 10
+
+# View last 10 frames
+ui.views.backtrace.depth = 10
+
+# Disassemble 5 instructions
+ui.views.disassembly.instruction_count = 5
+
+# Change disassembly syntax to AT&T
+ui.views.disassembly.flavor = 'att'
+
+# View floating point registers
+ui.views.registers.rtype = 'float'
+
+# Change addresses print color
+ui.colors.address = 'red'
+
+# Change titles color
+ui.color.title = 'green'
+```
+
 ## Symbol objects
 
 In Hilda, almost everything is wrapped using the `Symbol` Object. Symbol is just a nicer way for referring to addresses
 encapsulated with an object allowing to deref the memory inside, or use these addresses as functions.
 
 In order to create a symbol from a given address, please use:
```

### Comparing `hilda-0.2.0/README.md` & `hilda-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -256,14 +256,73 @@
 capabilities:
 
 ```python
 # execute the following to print the command's documentation
 stop?
 ```
 
+## UI Configuration
+
+Hilda contains minimal UI for examining the target state.
+The UI is divided into views:
+
+- Registers
+- Disassembly
+- Stack
+- Backtrace
+
+![img.png](gifs/ui.png)
+
+This UI can be displayed at any time be executing:
+
+```python
+ui.show()
+```
+
+By default `step_into` and `step_over` will show this UI automatically.
+You may disable this behaviour by executing:
+
+```python
+ui.active = False
+```
+
+Attentively, if you want to display UI after hitting a breakpoint, you can register `ui.show` as callback:
+
+```python
+symbol(0x7ff7b97c21b0).bp(ui.show)
+```
+
+Try playing with the UI settings by yourself:
+
+```python
+# Disable stack view
+ui.views.stack.active = False
+
+# View words from the stack
+ui.views.stack.depth = 10
+
+# View last 10 frames
+ui.views.backtrace.depth = 10
+
+# Disassemble 5 instructions
+ui.views.disassembly.instruction_count = 5
+
+# Change disassembly syntax to AT&T
+ui.views.disassembly.flavor = 'att'
+
+# View floating point registers
+ui.views.registers.rtype = 'float'
+
+# Change addresses print color
+ui.colors.address = 'red'
+
+# Change titles color
+ui.color.title = 'green'
+```
+
 ## Symbol objects
 
 In Hilda, almost everything is wrapped using the `Symbol` Object. Symbol is just a nicer way for referring to addresses
 encapsulated with an object allowing to deref the memory inside, or use these addresses as functions.
 
 In order to create a symbol from a given address, please use:
```

### Comparing `hilda-0.2.0/hilda/command.py` & `hilda-0.3.0/hilda/command.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/exceptions.py` & `hilda-0.3.0/hilda/exceptions.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/from_ns_to_json.m` & `hilda-0.3.0/hilda/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/get_objectivec_class_description.m` & `hilda-0.3.0/hilda/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/get_objectivec_symbol_data.m` & `hilda-0.3.0/hilda/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/hilda_ascii_art.html` & `hilda-0.3.0/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/hilda_client.py` & `hilda-0.3.0/hilda/hilda_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import importlib.util
 import json
 import logging
 import os
 import pickle
 import textwrap
 import time
+import typing
 from collections import namedtuple
 from contextlib import contextmanager, suppress
 from datetime import datetime, timezone
 from functools import cached_property, partial
 from pathlib import Path
-from typing import Union
+from typing import List, Optional, Union
 
 import docstring_parser
 import hexdump
 import IPython
 import lldb
 from humanfriendly import prompts
 from humanfriendly.terminal.html import html_to_ansi
@@ -36,14 +37,15 @@
     DisableJetsamMemoryChecksError, EvaluatingExpressionError, HildaException, SymbolAbsentError
 from hilda.launch_lldb import disable_logs  # noqa: F401
 from hilda.objective_c_symbol import ObjectiveCSymbol
 from hilda.registers import Registers
 from hilda.snippets.mach import CFRunLoopServiceMachPort_hooks
 from hilda.symbol import Symbol
 from hilda.symbols_jar import SymbolsJar
+from hilda.ui.ui_manager import UiManager
 
 IsaMagic = namedtuple('IsaMagic', 'mask value')
 ISA_MAGICS = [
     # ARM64
     IsaMagic(mask=0x000003f000000001, value=0x000001a000000001),
     # X86_64
     IsaMagic(mask=0x001f800000000001, value=0x001d800000000001),
@@ -77,14 +79,15 @@
         self.target = debugger.GetSelectedTarget()
         self.process = self.target.GetProcess()
         self.symbols = SymbolsJar.create(self)
         self.breakpoints = {}
         self.captured_objects = {}
         self.registers = Registers(self)
         self.arch = self.target.GetTriple().split('-')[0]
+        self.ui_manager = UiManager(self)
         # should unwind the stack on errors. change this to False in order to debug self-made calls
         # within hilda
         self._evaluation_unwind_on_error = True
 
         # should ignore breakpoints while evaluation
         self._evaluation_ignore_breakpoints = True
 
@@ -116,24 +119,30 @@
         """
         with open(os.path.join(Path(__file__).resolve().parent, 'lsof.m'), 'r') as f:
             result = json.loads(self.po(f.read()))
         # convert FDs into int
         return {int(k): v for k, v in result.items()}
 
     @command()
-    def bt(self):
+    def bt(self, should_print=True, depth: Optional[int] = None) -> List:
         """ Print an improved backtrace. """
+        backtrace = []
         for i, frame in enumerate(self.thread.frames):
+            if i == depth:
+                break
             row = ''
             row += html_to_ansi(f'<span style="color: cyan">0x{frame.addr.GetFileAddress():x}</span> ')
             row += str(frame)
             if i == 0:
                 # first line
                 row += ' 👈'
-            print(row)
+            backtrace.append([f'0x{frame.addr.file_addr:016x}', frame])
+            if should_print:
+                print(row)
+        return backtrace
 
     @command()
     def disable_jetsam_memory_checks(self):
         """
         Disable jetsam memory checks, prevent raising:
         `error: Execution was interrupted, reason: EXC_RESOURCE RESOURCE_TYPE_MEMORY (limit=15 MB, unused=0x0).`
         when evaluating expression.
@@ -510,20 +519,24 @@
             self._bp_frame = None
 
     @command()
     def step_into(self):
         """ Step into current instruction. """
         with self.sync_mode():
             self.thread.StepInto()
+        if self.ui_manager.active:
+            self.ui_manager.show()
 
     @command()
     def step_over(self):
         """ Step over current instruction. """
         with self.sync_mode():
             self.thread.StepOver()
+        if self.ui_manager.active:
+            self.ui_manager.show()
 
     @command()
     def remove_all_hilda_breakpoints(self, remove_forced=False):
         """
         Remove all breakpoints created by Hilda
         :param remove_forced: include removed of "forced" breakpoints
         """
@@ -1004,15 +1017,15 @@
 
         # add it into symbols global
         self.symbols[name] = value
         self.symbols[f'{name}{{{value.filename}}}'] = value
 
         return value
 
-    def interactive(self):
+    def interactive(self, additional_namespace: typing.Mapping = None):
         """ Start an interactive Hilda shell """
         if not self._dynamic_env_loaded:
             self.init_dynamic_environment()
         self._globalize_commands()
         print('\n')
         self.log_info(html_to_ansi(GREETING))
 
@@ -1020,14 +1033,16 @@
         c.IPCompleter.use_jedi = False
         c.InteractiveShellApp.exec_lines = [
             '''disable_logs()''',
             '''IPython.get_ipython().events.register('pre_run_cell', self._ipython_run_cell_hook)'''
         ]
         namespace = globals()
         namespace.update(locals())
+        if additional_namespace is not None:
+            namespace.update(additional_namespace)
 
         IPython.start_ipython(config=c, user_ns=namespace)
 
     @staticmethod
     def is_objc_type(symbol: Symbol) -> bool:
         """
         Test if a given symbol represents an objc object
```

### Comparing `hilda-0.2.0/hilda/launch_lldb.py` & `hilda-0.3.0/hilda/launch_lldb.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/lldb_entrypoint.py` & `hilda-0.3.0/hilda/lldb_entrypoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 lldb.hilda_client = None
 
 
 def hilda(debugger, command, result, internal_dict):
     if lldb.hilda_client is None:
         lldb.hilda_client = HildaClient(debugger)
-    lldb.hilda_client.interactive()
+
+    additional_namespace = {'ui': lldb.hilda_client.ui_manager}
+    lldb.hilda_client.interactive(additional_namespace=additional_namespace)
 
 
 def __lldb_init_module(debugger, internal_dict):
     debugger.SetAsync(True)
     debugger.HandleCommand('command script add -f lldb_entrypoint.hilda hilda')
     print('''
     👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇👇
```

### Comparing `hilda-0.2.0/hilda/lsof.m` & `hilda-0.3.0/hilda/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/objective_c_class.py` & `hilda-0.3.0/hilda/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/objective_c_symbol.py` & `hilda-0.3.0/hilda/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/registers.py` & `hilda-0.3.0/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/boringssl.py` & `hilda-0.3.0/hilda/snippets/boringssl.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/dyld.py` & `hilda-0.3.0/hilda/snippets/dyld.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py` & `hilda-0.3.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/macho/all_image_infos.py` & `hilda-0.3.0/hilda/snippets/macho/all_image_infos.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/macho/image_info.py` & `hilda-0.3.0/hilda/snippets/macho/image_info.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/macho/macho.py` & `hilda-0.3.0/hilda/snippets/macho/macho.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/macho/macho_load_commands.py` & `hilda-0.3.0/hilda/snippets/macho/macho_load_commands.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/remotepairingd.py` & `hilda-0.3.0/hilda/snippets/remotepairingd.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/snippets/xpc.py` & `hilda-0.3.0/hilda/snippets/xpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,23 @@
     """
     Convert XPC object to python object.
     :param address: Address of XPC object.
     """
     return lldb.hilda_client.from_ns(f'_CFXPCCreateCFObjectFromXPCObject({address})')
 
 
+def disable_transaction_exit():
+    """
+    xpc_transaction_exit_clean will kill the process when transaction is done.
+    By patching this function the process will stay alive.
+    """
+    hilda = lldb.hilda_client
+    hilda.symbols.xpc_transaction_exit_clean.poke_text('ret')
+
+
 def to_xpc_object(obj: object):
     """
     Convert python object to XPC object.
     :param obj: Native python object
     """
     hilda = lldb.hilda_client
     return hilda.symbols._CFXPCCreateXPCObjectFromCFObject(hilda.ns(obj))
```

### Comparing `hilda-0.2.0/hilda/symbol.py` & `hilda-0.3.0/hilda/symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/symbols_jar.py` & `hilda-0.3.0/hilda/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda/to_ns_from_json.m` & `hilda-0.3.0/hilda/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.2.0/hilda.egg-info/PKG-INFO` & `hilda-0.3.0/hilda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLDB wrapped and empowered by iPython's features
-Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
+Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
@@ -298,14 +298,73 @@
 capabilities:
 
 ```python
 # execute the following to print the command's documentation
 stop?
 ```
 
+## UI Configuration
+
+Hilda contains minimal UI for examining the target state.
+The UI is divided into views:
+
+- Registers
+- Disassembly
+- Stack
+- Backtrace
+
+![img.png](gifs/ui.png)
+
+This UI can be displayed at any time be executing:
+
+```python
+ui.show()
+```
+
+By default `step_into` and `step_over` will show this UI automatically.
+You may disable this behaviour by executing:
+
+```python
+ui.active = False
+```
+
+Attentively, if you want to display UI after hitting a breakpoint, you can register `ui.show` as callback:
+
+```python
+symbol(0x7ff7b97c21b0).bp(ui.show)
+```
+
+Try playing with the UI settings by yourself:
+
+```python
+# Disable stack view
+ui.views.stack.active = False
+
+# View words from the stack
+ui.views.stack.depth = 10
+
+# View last 10 frames
+ui.views.backtrace.depth = 10
+
+# Disassemble 5 instructions
+ui.views.disassembly.instruction_count = 5
+
+# Change disassembly syntax to AT&T
+ui.views.disassembly.flavor = 'att'
+
+# View floating point registers
+ui.views.registers.rtype = 'float'
+
+# Change addresses print color
+ui.colors.address = 'red'
+
+# Change titles color
+ui.color.title = 'green'
+```
+
 ## Symbol objects
 
 In Hilda, almost everything is wrapped using the `Symbol` Object. Symbol is just a nicer way for referring to addresses
 encapsulated with an object allowing to deref the memory inside, or use these addresses as functions.
 
 In order to create a symbol from a given address, please use:
```

### Comparing `hilda-0.2.0/hilda.egg-info/SOURCES.txt` & `hilda-0.3.0/hilda.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -38,8 +38,11 @@
 hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
 hilda/snippets/mach/__init__.py
 hilda/snippets/macho/__init__.py
 hilda/snippets/macho/all_image_infos.py
 hilda/snippets/macho/apple_version.py
 hilda/snippets/macho/image_info.py
 hilda/snippets/macho/macho.py
-hilda/snippets/macho/macho_load_commands.py
+hilda/snippets/macho/macho_load_commands.py
+hilda/ui/colors.json
+hilda/ui/ui_manager.py
+hilda/ui/views.py
```

### Comparing `hilda-0.2.0/pyproject.toml` & `hilda-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "hilda"
-version = "0.2.0"
+version = "0.3.0"
 description = "LLDB wrapped and empowered by iPython's features"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["python", "debugger", "lldb", "ipython", "ios", "debug"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
-    { name = "matan", email = "matan1008@gmail.com" }
+    { name = "matan", email = "matan1008@gmail.com" },
+    { name = "netanel", email = "matan1008@gmail.com" }
 ]
 maintainers = [
     { name = "doronz88", email = "doron88@gmail.com" },
     { name = "matan", email = "matan1008@gmail.com" }
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -33,15 +34,15 @@
 "Homepage" = "https://github.com/doronz88/hilda"
 "Bug Reports" = "https://github.com/doronz88/hilda/issues"
 
 [project.scripts]
 hilda = "hilda.__main__:main"
 
 [tool.setuptools]
-package-data = { "hilda" = ["*.html", "*.m"] }
+package-data = { "hilda" = ["*.html", "*.m", "ui/*.json"] }
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
```

