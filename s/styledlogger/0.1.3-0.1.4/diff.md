# Comparing `tmp/styledlogger-0.1.3.tar.gz` & `tmp/styledlogger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.1.3.tar", last modified: Tue Jul 11 18:56:46 2023, max compression
+gzip compressed data, was "styledlogger-0.1.4.tar", last modified: Wed Jul 26 15:55:53 2023, max compression
```

## Comparing `styledlogger-0.1.3.tar` & `styledlogger-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.451903 styledlogger-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-11 18:56:29.000000 styledlogger-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 18:56:46.451903 styledlogger-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-11 18:56:29.000000 styledlogger-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:56:46.451903 styledlogger-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 18:56:29.000000 styledlogger-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.447903 styledlogger-0.1.3/styledlogger/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.451903 styledlogger-0.1.3/styledlogger/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/callbackctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/printcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/printtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/styleconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.447903 styledlogger-0.1.3/styledlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:53.291482 styledlogger-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-26 15:55:41.000000 styledlogger-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-26 15:55:53.287482 styledlogger-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-26 15:55:41.000000 styledlogger-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:55:53.291482 styledlogger-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 15:55:41.000000 styledlogger-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:53.287482 styledlogger-0.1.4/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:53.287482 styledlogger-0.1.4/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/classes/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/classes/callbackctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-26 15:55:41.000000 styledlogger-0.1.4/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:53.287482 styledlogger-0.1.4/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-26 15:55:53.000000 styledlogger-0.1.4/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-26 15:55:53.000000 styledlogger-0.1.4/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:55:53.000000 styledlogger-0.1.4/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 15:55:53.000000 styledlogger-0.1.4/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 15:55:53.000000 styledlogger-0.1.4/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.1.3/LICENSE` & `styledlogger-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.3/README.md` & `styledlogger-0.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # StyledLogger
 
-### A simple, yet beautiful logging library for Python 🐍 > 3.7
+### A simple, yet beautiful logging library for Python 🐍 >= 3.9
+[![Tests](https://github.com/barealek/StyledLogger/actions/workflows/run-tests.yml/badge.svg)](https://github.com/barealek/StyledLogger/actions/workflows/run-tests.yml)
+[![Upload Python Package](https://github.com/barealek/StyledLogger/actions/workflows/pypi-integration.yml/badge.svg)](https://github.com/barealek/StyledLogger/actions/workflows/pypi-integration.yml)
 
 To use, simply install via `pip install styledlogger`
 
 Then you can import the `StyledLogger` class from the `styledlogger` package, and initialize it with a name.
 
 ---
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
+>>> logger = StyledLogger(name="Main")
 
->>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
+>>> logger.info("Good Morning!")
+8:57:41 :: INFO @ Main - Good Morning!
 
->>> logger.debug("This is just a test print")
-10:13:30 :: DEBU @ Main - This is just a test print
+>>> logger.warn("Python < 3.7 not supported")
+8:58:03 :: WARN @ Main - Python < 3.7 not supported
 
->>> logger.error("Could not fetch url 'https://example.com'")
-10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
+>>> logger.error("User database entries not found!")
+8:58:35 :: ERRO @ Main - User database entries not found!
 
->>> from styledlogger import StyleConfig
-
->>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
-
->>> logger.warn("CPU usage exceeding 90%")
-22/04/2023 10:01 | WARN - CPU usage exceeding 90%
+>>> logger.fatal("Lost connection to the API.")
+8:58:51 :: FATL @ Main - Lost connection to the API.
 ```
 
-There's much more you can do with this library, and I encourage you to play around. Some features include file logging, custom callbacks and more.
+There's more to this library, and I encourage to play around with it. You can check out the `examples` folder for some nice examples showing the features of the library.
+
+---
 
 Check out the GitHub: https://github.com/BareAlek/StyledLogger
-Contact me at mail: alek@imalek.me
+Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.1.3/setup.py` & `styledlogger-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.3/styledlogger/classes/callback.py` & `styledlogger-0.1.4/styledlogger/classes/callback.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 from .callbackctx import CallbackContext
 
+from typing import Union
+
+
 class Callback:
     """
-    A callback that can be added to a logger. The callback will be called with the logger name as the first argument and message as the second argument.
+    A callback that can be added to a logger. The callback will be called with
+    the logger name as the first argument and message as the second argument.
 
     :param name:
     The name of the callback. This is used to identify the callback.
 
-    :param activation_level:
-    The level at which the callback will be called. 0 = debug, 1 = info, 2 = warn, 3 = error, 4 = fatal. All prints lower than the level will be ignored.
+    :param activation_levels:
+    The levels at which the callback will be called. 0 = debug, 1 = info, 2 = warn,
+    3 = error, 4 = fatal. All prints lower than the level will be ignored.
 
     :param callback:
-    The callback function. This will be called with the logger name as the first argument, the level as the second and message as the third argument.
+    The callback function. This will be called with the logger name as the first
+    argument, the level as the second and message as the third argument.
     """
 
-    def __init__(self, name: str, activation_levels: int | tuple, callback: callable):
+    def __init__(self,
+                 name: str,
+                 activation_levels: Union[int, tuple],
+                 callback: callable
+                 ):
         self.name = name
         self.activation_levels = activation_levels
         self.callback = callback
 
     def run_callback(self, level, message):
         self.callback(CallbackContext(self.name, level, message))
 
     def __repr__(self):
-        return f"<Callback name={self.name} activation_levels={self.activation_levels} callback={self.callback}>"
+        return f"<Callback name={self.name}>"
 
     def __str__(self):
         return self.__repr__()
```

### Comparing `styledlogger-0.1.3/styledlogger/classes/printcolors.py` & `styledlogger-0.1.4/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.3/styledlogger/classes/printtypes.py` & `styledlogger-0.1.4/styledlogger/classes/printtypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 class PrintType:
-    def __init__(self):
-        self.display = None
+    display = "UNKN"
 
     def __hash__(self):
-        return hash((self.display))
+        return hash(self.display)
 
     def __eq__(self, other):
         return self.display == other.display
 
 
 class Debug(PrintType):
     display = "DEBU"
```

### Comparing `styledlogger-0.1.3/styledlogger/classes/styleconfig.py` & `styledlogger-0.1.4/styledlogger/classes/styleconfig.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 from .printcolors import Colors
 from arrow import now
 
 from .printtypes import Debug, Info, Warn, Error, Fatal, System, PrintType
 
+from typing import Type, Union
+
 
 class StyleConfig:
     """
     The style configuration for the logger.
 
-    :param time_format: The format of the time.
-    See https://arrow.readthedocs.io/en/latest/guide.html#format
+    :param text_format: The format of the log message.
+    :param time_format: The format of the time in the log message.
 
-    :param time_color: The color of the time. See https://pypi.org/project/colorama/
-    - usually just the name of the color.
+    :param time_color: The color of the time in the log message.
+    :param name_color: The color of the logger name in the log message.
+    :param text_color: The color of the log message.
+
+    :param debug_color: The color of the debug name text.
+    :param info_color: The color of the info name text.
+    :param warn_color: The color of the warn name text.
+    :param error_color: The color of the error name text.
+    :param fatal_color: The color of the fatal name text.
+    :param system_color: The color of the system name text.
 
     """
 
     def __init__(
         self,
-        text_format: str = "%time% :: %type% @ %name% - %msg%",
+        *,
+        text_format: str = "{time} :: {type} @ {name} - {text}",
         time_format: str = "h:mm:ss",
         time_color: str = "dark_gray",
         name_color: str = "reset",
-        text_color: str | None = None,
+        text_color: Union[str, None] = None,
         debug_color: str = "yellow",
         info_color: str = "green",
         warn_color: str = "brown",
         error_color: str = "red",
         fatal_color: str = "purple",
         system_color: str = "cyan",
     ) -> None:
@@ -59,53 +70,52 @@
     def return_as_dict(self) -> dict:
         """
         Return the style config as a dict.
         Useful for pickling or json dumping.
         """
         return vars(self)
 
-    def style_text(self, logger_name: str, print_type: PrintType, text: str) -> str:
+    def style_text(self,
+                   logger_name: str,
+                   print_type: Type[PrintType],
+                   text: str
+                   ) -> str:
         """
         Style the text according to the style config.
         """
 
         color_map = {
             Debug: self.debug_color,
             Info: self.info_color,
             Warn: self.warn_color,
             Error: self.error_color,
             Fatal: self.fatal_color,
             System: self.system_color,
         }
         type_color = color_map.get(print_type)
 
-        format_blueprint = self.text_format
 
         replacemap = {
-            "%name%": self.name_color + logger_name + self.reset,
-            "%time%": self.time_color + now().format(self.time_format) + self.reset,
-            "%type%": type_color + str(print_type.display) + self.reset,
-            "%msg%": self.text_color + text + self.reset,
+            "{name}": self.name_color + logger_name + self.reset,
+            "{time}": self.time_color + now().format(self.time_format) + self.reset,
+            "{type}": type_color + str(print_type.display) + self.reset,
+            "{text}": self.text_color + text + self.reset,
         }
 
-        for k, v in replacemap.items():
-            format_blueprint = format_blueprint.replace(k, v)
-        return format_blueprint
+        return ' '.join([replacemap.get(_w, _w) for _w in self.text_format.split(' ')])
+
 
     def style_text_uncolored(
-        self, logger_name: str, print_type: PrintType, text: str
+        self, logger_name: str, print_type: Type[PrintType], text: str
     ) -> str:
         """
         Style the text according to the style config.
         """
-        format_blueprint = self.text_format
 
-        replacemap = {
-            "%name%": logger_name,
-            "%time%": now().format(self.time_format),
-            "%type%": str(print_type.display),
-            "%msg%": text,
+        _map = {
+            "{name}": logger_name,
+            "{time}": now().format(self.time_format),
+            "{type}": str(print_type.display),
+            "{text}": text,
         }
 
-        for k, v in replacemap.items():
-            format_blueprint = format_blueprint.replace(k, v)
-        return format_blueprint
+        return ' '.join([_map.get(_w, _w) for _w in self.text_format.split(' ')])
```

### Comparing `styledlogger-0.1.3/styledlogger/logger.py` & `styledlogger-0.1.4/styledlogger/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,63 @@
-from colorama import (
-    just_fix_windows_console,
-)
 
 from .classes.styleconfig import StyleConfig
 from .classes.printtypes import PrintType, Debug, Info, Warn, Error, Fatal, System
 from .classes.callback import Callback as LoggerCallback
 
-just_fix_windows_console()
+from typing import Type, Union, IO
 
 
 class Logger:
     """
     The main object for logging.
 
     :param name: The name of the logger
     :param file: The path of the file which logs will be written to
     :param level: The log level
+    :param style_config: The style config
     """
 
-    def __init__(self, name: str, *, file: str = None, level: int = 1) -> None:
+    def __init__(self,
+                 name: str, *,
+                 file: Union[str, IO[str], None] = None,
+                 level: int = 1,
+                 style_config: StyleConfig = None
+                 ) -> None:
         self.name = name
         self.level = level
         self.is_muted = False
-        self.style_config = StyleConfig()
-        self.file_path = file
+        self.style_config = style_config or StyleConfig()
         self.callbacks = []
 
+        self.file = open(file, "a+", encoding="utf-8") \
+            if isinstance(file, str) else file
+
     def set_level(self, level: int):
         """
-        Set the log level. 0 = debug, 1 = info, 2 = warn, 3 = error, 4 = fatal. All prints lower than the level will be ignored.
-        """
-        self.level = level
+        Set the log level.
 
-    # Create a decorator, which takes in a name, and adds the decorated function to the logger's callbacks
-    def callback(self, name: str, levels: int | tuple[int, ...]):
+        :param level: The new level.
         """
-        Decorator to add a callback to the logger.
-
-        :param name: The name of the callback
-        :param levels: The levels which the callback will be called upon.
+        self.level = level
 
-        The decorated function will receive an instance of `styledlogger.CallbackContext`,
-        with the following attributes:
-        :param name: The name of the logger which activated the callback.
-        :param level: The log level which activated the callback.
-        :param message: The content of the log message which activated the callback.
-        """
+    # noinspection PyIncorrectDocstring
+    def callback(self, name: str, levels: Union[int, tuple[int, ...]]):
+        # noinspection PyUnresolvedReferences
+        """
+            Decorator to add a callback to the logger.
+
+            :param name: The name of the callback
+            :param levels: The levels which the callback will be called upon.
+
+            The decorated function will receive an instance of
+            `styledlogger.CallbackContext`, with the following attributes:
+            :param name: The name of the logger which activated the callback.
+            :param level: The log level which activated the callback.
+            :param message: The content of the log message which activated the callback.
+                """
 
         def decorator_function(original_func):
             self.callbacks.append(LoggerCallback(name, levels, original_func))
             return original_func
 
         return decorator_function
 
@@ -65,80 +73,80 @@
 
     def debug(self, message):
         """
         Log a debug message
         """
         self._process_callbacks(message, Debug)
         if self.level <= 0:
-            self._log(message, Debug)
+            return self._log(message, Debug)
+        return False
 
     def info(self, message):
         """
         Log an info message
         """
         self._process_callbacks(message, Info)
         if self.level <= 1:
-            self._log(message, Info)
+            return self._log(message, Info)
+        return False
 
     def warn(self, message):
         """
         Log a warning message
         """
         self._process_callbacks(message, Warn)
         if self.level <= 2:
-            self._log(message, Warn)
+            return self._log(message, Warn)
+        return False
 
     def error(self, message):
         """
         Log an error message
         """
         self._process_callbacks(message, Error)
         if self.level <= 3:
-            self._log(message, Error)
+            return self._log(message, Error)
+        return False
 
     def fatal(self, message):
         """
         Log a fatal message
         """
         self._process_callbacks(message, Fatal)
         if self.level <= 4:
-            self._log(message, Fatal)
+            return self._log(message, Fatal)
+        return False
 
     def system(self, message):
         """
         Log a system message
         """
         self._process_callbacks(message, System)
-        self._log(message, System)
+        return self._log(message, System)
 
     def _process_callbacks(self, message, print_type):
         for callback in self.callbacks:
             if isinstance(callback.activation_levels, int):
                 if print_type.level == callback.activation_levels:
                     callback.run_callback(level=print_type.level, message=message)
                     return
             if isinstance(callback.activation_levels, tuple):
                 if print_type.level in callback.activation_levels:
                     callback.run_callback(level=print_type.level, message=message)
 
-    def _log(self, message, print_type: PrintType):
+    def _log(self, message, print_type: Type[PrintType]):
 
         if self.is_muted:
-            return
+            return False
 
-        if self.file_path:
-            with open(self.file_path, "a+", encoding="utf-8") as file:
-                file.write(
-                    self.style_config.style_text_uncolored(
-                        self.name, print_type, message
-                    )
-                    + "\n"
-                )
+        if self.file:
+            self._write_to_file(message, print_type)
 
         print(self.style_config.style_text(self.name, print_type, message))
+        return True
 
     def set_style(self, style_config: StyleConfig):
         """
         Change the style config of the logger.
         """
         self.style_config = style_config
 
@@ -149,7 +157,16 @@
         self.is_muted = True
 
     def unmute(self):
         """
         Unmute the logger.
         """
         self.is_muted = False
+
+    def _write_to_file(self, message, print_type: Type[PrintType]):
+        self.file.write(
+            self.style_config.style_text_uncolored(
+                self.name, print_type, message
+            )
+            + "\n"
+        )
+        self.file.flush()
```

