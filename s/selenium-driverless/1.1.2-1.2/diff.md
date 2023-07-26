# Comparing `tmp/selenium_driverless-1.1.2.tar.gz` & `tmp/selenium_driverless-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.1.2.tar", last modified: Mon Jul 24 20:26:45 2023, max compression
+gzip compressed data, was "selenium_driverless-1.2.tar", last modified: Wed Jul 26 09:26:08 2023, max compression
```

## Comparing `selenium_driverless-1.1.2.tar` & `selenium_driverless-1.2.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.731538 selenium_driverless-1.1.2/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.1.2/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3757 2023-07-24 20:26:45.731538 selenium_driverless-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2441 2023-07-24 18:55:54.000000 selenium_driverless-1.1.2/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.1.2/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-24 20:26:45.733540 selenium_driverless-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.710384 selenium_driverless-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.718449 selenium_driverless-1.1.2/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-24 20:26:26.000000 selenium_driverless-1.1.2/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.724491 selenium_driverless-1.1.2/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.1.2/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.727491 selenium_driverless-1.1.2/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2868 2023-07-24 19:21:37.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    16797 2023-07-23 12:34:39.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5596 2023-07-24 19:39:32.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.729491 selenium_driverless-1.1.2/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.1.2/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.1.2/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    44016 2023-07-24 20:22:53.000000 selenium_driverless-1.1.2/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.723491 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3757 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.730491 selenium_driverless-1.1.2/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.1.2/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.150004 selenium_driverless-1.2/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3821 2023-07-26 09:26:08.150004 selenium_driverless-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-07-26 09:25:36.000000 selenium_driverless-1.2/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-26 09:26:08.151001 selenium_driverless-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.121741 selenium_driverless-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.130678 selenium_driverless-1.2/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       21 2023-07-26 09:25:45.000000 selenium_driverless-1.2/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.137841 selenium_driverless-1.2/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.141899 selenium_driverless-1.2/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    17252 2023-07-24 21:37:07.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.146005 selenium_driverless-1.2/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    15407 2023-07-26 09:11:23.000000 selenium_driverless-1.2/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.147004 selenium_driverless-1.2/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    45211 2023-07-26 09:21:31.000000 selenium_driverless-1.2/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.136843 selenium_driverless-1.2/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3821 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-07-26 09:26:08.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.149004 selenium_driverless-1.2/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.1.2/LICENSE.md` & `selenium_driverless-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.2/PKG-INFO` & `selenium_driverless-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.1.2
+Version: 1.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -89,17 +89,18 @@
 ```
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
-
-- [ ] page-interactions
-  - [ ] find element
+- protocoll
+  - [ ] add cdp event handler
+- [x] sync
+  - [ ] move sync to threaded for allowing event_handlers
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.1.2/README.md` & `selenium_driverless-1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -59,17 +59,18 @@
 ```
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
-
-- [ ] page-interactions
-  - [ ] find element
+- protocoll
+  - [ ] add cdp event handler
+- [x] sync
+  - [ ] move sync to threaded for allowing event_handlers
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.1.2/build_upload.md` & `selenium_driverless-1.2/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.2/setup.py` & `selenium_driverless-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.2/src/selenium_driverless/scripts/alert.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Inputting a value into an alert prompt::
 
         name_prompt = Alert(driver)
         name_prompt.send_keys("Willian Shakesphere")
         name_prompt.accept()
 
 
-    Reading a the text of a prompt for verification::
+    Reading the text of a prompt for verification::
 
         alert_text = Alert(driver).text
         self.assertEqual("Do you wish to quit?", alert_text)
     """
 
     def __init__(self, driver) -> None:
         """Creates a new Alert.
@@ -57,30 +57,27 @@
     @property
     async def text(self) -> str:
         """Gets the text of the Alert."""
         return await self.driver.execute(Command.W3C_GET_ALERT_TEXT)["value"]
 
     async def dismiss(self) -> None:
         """Dismisses the alert available."""
-        from pycdp import cdp
-        await self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=False))
+        await self.driver.execute_cdp_cmd("Page.handleJavaScriptDialog", {"accept": False})
 
     async def accept(self) -> None:
         """Accepts the alert available.
 
         :Usage:
             ::
 
                 Alert(driver).accept() # Confirm a alert dialog.
         """
-        from pycdp import cdp
-        await self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=True))
+        await self.driver.execute_cdp_cmd("Page.handleJavaScriptDialog", {"accept": True})
 
     # noinspection PyPep8Naming
     async def send_keys(self, keysToSend: str) -> None:
         """Send Keys to the Alert.
 
         :Args:
          - keysToSend: The text to be sent to Alert.
         """
-        from pycdp import cdp
-        await self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=True, prompt_text=keysToSend))
+        await self.driver.execute_cdp_cmd("Page.handleJavaScriptDialog", {"accept": False, "promptText": keysToSend})
```

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.2/src/selenium_driverless/scripts/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,29 @@
         self.add_argument(f"--remote-debugging-port={port}")
         self._ignore_local_proxy = False
 
     @property
     def capabilities(self):
         return self._caps
 
-    def set_capability(self, name, value) -> None:
+    def set_capability(self, name: str, value: dict) -> None:
         """Sets a capability."""
-        raise NotImplementedError()
+        if name == "proxy":
+            proxy = None
+            proxy_keys = ['ftpProxy', 'httpProxy', 'sslProxy']
+            warnings.warn("not started with chromedriver, only aplying single proxy")
+            for key, value in value.items():
+                if key in proxy_keys:
+                    self.add_argument(f'--proxy-server={value}')
+                    if not proxy:
+                        proxy = value
+                    value[key] = proxy
+            self._proxy = Proxy(value)
+        else:
+            raise NotImplementedError()
         self._caps[name] = value
 
     @property
     def browser_version(self) -> str:
         """
         :returns: the version of the browser if set, otherwise None.
         """
@@ -224,43 +236,41 @@
         self._caps["strictFileInteractability"] = value
 
     @property
     def set_window_rect(self) -> bool:
         """
         :returns: whether the remote end supports setting window size and position
         """
-        raise NotImplementedError()
-        return self._caps.get("setWindowRect", False)
+        return True
 
     @set_window_rect.setter
     def set_window_rect(self, value: bool) -> None:
         """Whether the remote end supports all of the resizing and positioning
         commands. The default is false. https://w3c.github.io/webdriver/#dfn-
         strict-file-interactability.
 
         :param value: whether remote end must support setting window resizing and repositioning
         """
-        raise NotImplementedError()
-        self._caps["setWindowRect"] = value
+        pass
 
     @property
     def proxy(self) -> Proxy:
         """
         :Returns: Proxy if set, otherwise None.
         """
-        raise NotImplementedError()
-        return self._proxy
+        proxy = Proxy(self._proxy)
+        return proxy
 
     @proxy.setter
     def proxy(self, value: Proxy) -> None:
         raise NotImplementedError()
         if not isinstance(value, Proxy):
             raise InvalidArgumentException("Only Proxy objects can be passed in.")
-        self._proxy = value
-        self._caps["proxy"] = value.to_capabilities()
+        warnings.warn("not started with chromedriver, only aplying single proxy")
+        self.set_capability("proxy", value=value.to_dict())
 
     #
     # Options(BaseOptions) from here on
     #
 
     @property
     def arguments(self):
```

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.2/src/selenium_driverless/scripts/switch_to.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,19 +98,21 @@
                     frame_reference = await self._driver.find_element(By.NAME, frame_reference)
                 except NoSuchElementException:
                     raise NoSuchFrameException(frame_reference)
 
         raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
 
     async def target(self, target_id):
-        from pycdp import cdp
+        from selenium_driverless.types import RemoteObject
         self._driver.session.close()
         # noinspection PyProtectedMember
         self._driver.session = await self._driver._conn.connect_session(target_id)
-        await self._driver.execute(cmd=cdp.target.activate_target(await self._driver.current_window_handle))
+        self._driver._global_this = await RemoteObject(driver=self, js="globalThis", check_existence=False)
+        await self._driver.execute_cdp_cmd("Target.activateTarget",
+                                           {"targetId": await self._driver.current_window_handle})
         return self._driver.session
 
     async def new_window(self, type_hint: Optional[str] = "tab", url="") -> None:
         """Switches to a new top-level browsing context.
 
         The type hint can be one of "tab" or "window". If not specified the
         browser will automatically select it.
@@ -122,17 +124,16 @@
         """
         new_window = False
         new_tab = False
         if type_hint == "window":
             new_window = True
         if type_hint == "tab":
             new_window = True
-        from pycdp import cdp
-        cmd = cdp.target.create_target(url=url, new_window=new_window, for_tab=new_tab)
-        target_id = await self._driver.execute(cmd=cmd)
+        args = {"url": url, "newWindow": new_tab, "forTab": new_tab}
+        target_id = await self._driver.execute_cdp_cmd("Target.createTarget", args)
         await self.target(target_id)
         return target_id
 
     async def parent_frame(self) -> None:
         """Switches focus to the parent context. If the current context is the
         top level browsing context, the context remains unchanged.
```

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.2/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.2/src/selenium_driverless/webdriver.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,38 +28,34 @@
 from base64 import urlsafe_b64encode
 from contextlib import asynccontextmanager
 from importlib import import_module
 from typing import List
 from typing import Optional
 from typing import Union
 
-import pycdp.cdp.target
 from selenium.common.exceptions import InvalidArgumentException
-from selenium.common.exceptions import JavascriptException
-from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import WebDriverException
-from selenium.webdriver.common.by import By
 from selenium.webdriver.common.print_page_options import PrintOptions
 from selenium.webdriver.common.virtual_authenticator import Credential
 from selenium.webdriver.common.virtual_authenticator import VirtualAuthenticatorOptions
 from selenium.webdriver.common.virtual_authenticator import (
     required_virtual_authenticator,
 )
 from selenium.webdriver.remote.bidi_connection import BidiConnection
 from selenium.webdriver.remote.file_detector import FileDetector
 from selenium.webdriver.remote.file_detector import LocalFileDetector
+from selenium.webdriver.remote.mobile import Mobile
 from selenium.webdriver.remote.script_key import ScriptKey
 from selenium.webdriver.remote.webdriver import create_matches
-from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.support.relative_locator import RelativeBy
-from selenium.webdriver.remote.mobile import Mobile
 
 from selenium_driverless.scripts.options import Options
 from selenium_driverless.scripts.switch_to import SwitchTo
 from selenium_driverless.sync.switch_to import SwitchTo as SyncSwitchTo
+from selenium_driverless.types.webelement import WebElement, RemoteObject
+from selenium_driverless.sync.webelement import WebElement as SyncWebElement
 
 
 def import_cdp():
     return import_module("selenium.webdriver.common.bidi.cdp")
 
 
 class BaseWebDriver(metaclass=ABCMeta):
@@ -79,48 +75,51 @@
     ) -> None:
         """Creates a new instance of the chrome driver. Starts the service and
         then creates new instance of chrome driver.
 
         :Args:
          - options - this takes an instance of ChromeOptions
         """
+        self._global_this = None
         self._loop = None
         self._page_load_timeout = 300
         self._script_timeout = 30
         self._conn = None
         self.session = None
         self.browser_pid = None
+        if not options.binary_location:
+            from selenium_driverless.utils.utils import find_chrome_executable
+            options.binary_location = find_chrome_executable()
 
         try:
             options = options or Options()
             self._options = options
 
             vendor_prefix = "goog"
             self.vendor_prefix = vendor_prefix
 
             if isinstance(options, list):
                 self._capabilities = create_matches(options)
             else:
                 self._capabilities = options.to_capabilities()
             self._is_remote = True
-            self.target_id = None
             self.caps = {}
             self.pinned_scripts = {}
             self._switch_to = SwitchTo(self)
             self._mobile = Mobile(self)
             self.file_detector = LocalFileDetector()
             self._authenticator_id = None
 
         except Exception:
             self.quit()
             raise
         self._is_remote = False
 
     def __repr__(self):
-        return f'<{type(self).__module__}.{type(self).__name__} (session="{self.target_id}")>'
+        return f'<{type(self).__module__}.{type(self).__name__} (session="{self.current_window_handle}")>'
 
     async def __aenter__(self):
         await self.start_session()
         return self
 
     def __enter__(self):
         return self
@@ -200,17 +199,19 @@
                 await self.implicitly_wait(0.1)
             self._options.debugger_address = "localhost:" + read(path, sel_root=False).split("\n")[0]
         self._conn = await connect_cdp(f'http://{self._options.debugger_address}')
         self.browser_pid = browser.pid
         targets = await self._conn.execute(cdp.target.get_targets())
         for target in targets:
             if target.type_ == "page":
-                self.target_id = target.target_id
+                target_id = target.target_id
                 break
-        self.session = await self._conn.connect_session(self.target_id)
+        # noinspection PyUnboundLocalVariable
+        self.session = await self._conn.connect_session(target_id)
+        self._global_this = await RemoteObject(driver=self, js="globalThis", check_existence=False)
         self.caps = capabilities
 
     async def create_web_element(self, element_id: str) -> WebElement:
         """Creates a web element with the specified `element_id`."""
         raise NotImplementedError()
 
     async def execute(self, driver_command: str = None, params: dict = None, cmd=None):
@@ -218,22 +219,25 @@
         executes on current pycdp.cdp cmd on current session
         driver_command and params aren't used
         """
         if driver_command or params:
             raise NotImplementedError("chrome not started with chromedriver")
         return await self.session.execute(cmd=cmd)
 
-    async def get(self, url: str) -> None:
+    async def get(self, url: str, referrer: str = None) -> None:
         """Loads a web page in the current browser session."""
         from pycdp import cdp
-        await self.execute(cmd=cdp.page.enable())
+        await self.execute_cdp_cmd("Page.enable")
+        args = {"url": url}
+        if referrer:
+            args["referrer"] = referrer
 
         async def get(_url: str):
             with self.session.safe_wait_for(cdp.page.DomContentEventFired) as navigation:
-                await self.session.execute(cmd=cdp.page.navigate(_url))
+                await self.execute_cdp_cmd("Page.navigate", args)
                 await navigation
 
         try:
             await asyncio.wait_for(get(url), self._page_load_timeout)
         except asyncio.exceptions.TimeoutError:
             raise TimeoutError(f"page didn't load within timeout of {self._page_load_timeout}")
 
@@ -243,15 +247,15 @@
 
         :Usage:
             ::
 
                 title = driver.title
         """
         target = await self.current_target
-        return target.title
+        return target["title"]
 
     def pin_script(self, script: str, script_key=None) -> ScriptKey:
         """Store common javascript scripts to be executed later by a unique
         hashable ID."""
         script_key_instance = ScriptKey(script_key)
         self.pinned_scripts[script_key_instance.id] = script
         return script_key_instance
@@ -262,89 +266,120 @@
             self.pinned_scripts.pop(script_key.id)
         except KeyError:
             raise KeyError(f"No script with key: {script_key} existed in {self.pinned_scripts}") from None
 
     def get_pinned_scripts(self) -> List[str]:
         return list(self.pinned_scripts)
 
-    async def execute_script(self, script, *args):
-        """Synchronously Executes JavaScript in the current window/frame.
-
-        :Args:
-         - script: The JavaScript to execute.
-         - \\*args: Any applicable arguments for your JavaScript.
-
-        :Usage:
-            ::
-
-                driver.execute_script('return document.title;')
-        """
-        import json
-        from pycdp import cdp
-        if isinstance(script, ScriptKey):
-            try:
-                script = self.pinned_scripts[script.id]
-            except KeyError:
-                raise JavascriptException("Pinned script could not be found")
-
-        script = f"(function(...arguments){{{script}}})(...{json.dumps(args)})"
-
-        script = cdp.runtime.evaluate(expression=script, include_command_line_api=True,
-                                      user_gesture=True, await_promise=False,
-                                      allow_unsafe_eval_blocked_by_csp=True, return_by_value=True)
-        result = await asyncio.wait_for(self.execute(cmd=script), self._script_timeout)
-        if result[1]:
-            class JSEvalException(result[1], Exception):
-                pass
-
-            raise JSEvalException(result[1].description)
-        return result[0].value
-
-    async def execute_async_script(self, script: str, *args):
-        """Asynchronously Executes JavaScript in the current window/frame.
-
-        :Args:
-         - script: The JavaScript to execute.
-         - \\*args: Any applicable arguments for your JavaScript.
+    async def _parse_res(self, res):
+        if "subtype" in res.keys():
+            if res["subtype"] == 'node':
+                if self._loop:
+                    res["value"] = await SyncWebElement(driver=self, loop=self._loop,
+                                                        obj_id=res["objectId"],
+                                                        check_existence=False)
+                else:
+                    res["value"] = await WebElement(driver=self, obj_id=res["objectId"],
+                                                    check_existence=False)
+        if 'className' in res.keys():
+            class_name = res['className']
+            if class_name in ['NodeList', 'HTMLCollection']:
+                elems = []
+                obj = await RemoteObject(driver=self, obj_id=res["objectId"], check_existence=False)
+                for idx in range(int(res['description'][-2])):
+                    elems.append(await obj.execute_script("return this[arguments[0]]", idx, serialization="deep"))
+                res["value"] = elems
+            elif class_name == 'XPathResult':
+                elems = []
+                obj = await RemoteObject(driver=self, obj_id=res["objectId"], check_existence=False)
+                if await obj.execute_script("return [7].includes(this.resultType)", serialization="json"):
+                    for idx in range(await obj.execute_script("return this.snapshotLength", serialization="json")):
+                        elems.append(await obj.execute_script("return this.snapshotItem(arguments[0])", idx, serialization="deep"))
+                    res["value"] = elems
+        return res
+
+    async def execute_raw_script(self, script: str, *args, await_res: bool = False, serialization: str = None,
+                                 max_depth: int = None, timeout: int = 2, obj_id=None):
+        """
+        example:
+        script= "function(...arguments){this.click()}"
+        "this" will be the element object
+        """
+        from selenium_driverless.types import RemoteObject, JSEvalException
+        if not obj_id:
+            if not self._global_this:
+                self._global_this = await RemoteObject(driver=self, js="globalThis", check_existence=False)
+            obj_id = await self._global_this.obj_id
+        if not timeout:
+            timeout = self._script_timeout
+        if not args:
+            args = []
+        if not serialization:
+            serialization = "deep"
+        _args = []
+        for arg in args:
+            if isinstance(arg, RemoteObject):
+                _args.append({"objectId": await arg.obj_id})
+            else:
+                _args.append({"value": arg})
 
-        :Usage:
-            ::
+        ser_opts = {"serialization": serialization, "maxDepth": max_depth,
+                    "additionalParameters": {"includeShadowTree": "all", "maxNodeDepth": max_depth}}
+        args = {"functionDeclaration": script, "objectId": obj_id,
+                "arguments": _args, "userGesture": True, "awaitPromise": await_res, "serializationOptions": ser_opts}
+        res = await asyncio.wait_for(self.execute_cdp_cmd("Runtime.callFunctionOn", args), timeout=timeout)
+        if "exceptionDetails" in res.keys():
+            raise JSEvalException(res["exceptionDetails"])
+        res = res["result"]
+        res = await self._parse_res(res)
+        return res
+
+    async def execute_script(self, script: str, *args, max_depth: int = 2, serialization: str = None,
+                             timeout: int = None,
+                             only_value=True, obj_id=None):
+        """
+        exaple: script = "return elem.click()"
+        """
+        script = f"(function(...arguments){{{script}}})"
+        res = await self.execute_raw_script(script, *args, max_depth=max_depth,
+                                            serialization=serialization, timeout=timeout,
+                                            await_res=False, obj_id=obj_id)
+        if only_value:
+            if "value" in res.keys():
+                return res["value"]
+        else:
+            return res
 
-                script = "var callback = arguments[arguments.length - 1]; " \\
-                         "window.setTimeout(function(){ callback('timeout') }, 3000);"
-                driver.execute_async_script(script)
-        """
-        from pycdp import cdp
-        import json
-        script = """
-        (function(...arguments){
-            const promise = new Promise((resolve, reject) => {
-                arguments.push(resolve)
-            });""" + script + ";return promise})(..." + json.dumps(args) + ")"
-        timeout = cdp.runtime.TimeDelta
-        timeout = timeout.from_json(self._script_timeout)
-        script = cdp.runtime.evaluate(expression=script, include_command_line_api=True,
-                                      user_gesture=True, await_promise=True,
-                                      allow_unsafe_eval_blocked_by_csp=True, timeout=timeout)
-        result = await asyncio.wait_for(self.execute(cmd=script), timeout=self._script_timeout)
-        if result[1]:
-            raise Exception(result[1].description)
-        return result[0].value
+    async def execute_async_script(self, script: str, *args, max_depth: int = 2,
+                                   serialization: str = None, timeout: int = 2,
+                                   only_value=True, obj_id=None):
+        script = """(function(...arguments){
+                       const promise = new Promise((resolve, reject) => {
+                              arguments.push(resolve)
+                        });""" + script + ";return promise})"
+        res = await self.execute_raw_script(script, *args, max_depth=max_depth,
+                                            serialization=serialization, timeout=timeout,
+                                            await_res=True, obj_id=obj_id)
+        if only_value:
+            if "value" in res.keys():
+                return res["value"]
+        else:
+            return res
 
     @property
     async def current_url(self) -> str:
         """Gets the URL of the current page.
 
         :Usage:
             ::
 
                 driver.current_url
         """
         target = await self.current_target
-        return target.url
+        return target["url"]
 
     @property
     async def page_source(self) -> str:
         """Gets the source of the current page.
 
         :Usage:
             ::
@@ -357,17 +392,16 @@
         """Closes the current window.
 
         :Usage:
             ::
 
                 driver.close()
         """
-        from pycdp import cdp
         window_handles = await self.window_handles
-        await self.execute(cmd=cdp.page.close())
+        await self.execute_cdp_cmd("Page.close")
         await self.switch_to.window(window_handles[0])
 
     async def quit(self) -> None:
         """Quits the driver and closes every associated window.
 
         :Usage:
             ::
@@ -395,42 +429,39 @@
         except Exception as e:
             # We don't care about the message because something probably has gone wrong
             pass
         finally:
             pass  # self.service.stop()
 
     @property
-    async def targets(self):
-        from pycdp import cdp
-        return await self.execute(cmd=cdp.target.get_targets())
+    async def targets(self) -> dict:
+        res = await self.execute_cdp_cmd("Target.getTargets")
+        return res["targetInfos"]
 
     @property
     async def current_target(self):
-        from pycdp import cdp
-        return await self.execute(cmd=cdp.target.get_target_info(await self.current_window_handle))
+        res = await self.execute_cdp_cmd("Target.getTargetInfo", {"targetId": self.current_window_handle})
+        return res["targetInfo"]
 
     @property
-    async def current_window_handle(self) -> pycdp.cdp.target.TargetID:
+    def current_window_handle(self) -> str:
         """Returns the handle of the current window.
 
         :Usage:
             ::
 
                 driver.current_window_handle
         """
         # noinspection PyProtectedMember
-        return self.session._target_id
+        return str(self.session._target_id)
 
     @property
     async def current_window_id(self):
-        from pycdp import cdp
-        target_id = await self.current_window_handle
-        script = cdp.browser.get_window_for_target(target_id)
-        result = await self.execute(cmd=script)
-        return result[0]
+        result = await self.execute_cdp_cmd("Browser.getWindowForTarget", {"targetId": self.current_window_handle})
+        return result["windowId"]
 
     @property
     async def window_handles(self) -> List[str]:
         """Returns the handles of all windows within the current session.
 
         :Usage:
             ::
@@ -472,22 +503,21 @@
     # noinspection PyUnusedLocal
     async def print_page(self, print_options: Optional[PrintOptions] = None) -> str:
         """Takes PDF of the current page.
 
         The driver makes the best effort to return a PDF based on the
         provided parameters.
         """
-        from pycdp import cdp
         options = {}
         if print_options:
             options = print_options.to_dict()
             raise NotImplementedError()
 
-        page = await self.execute(cmd=cdp.page.print_to_pdf())
-        return page[0]
+        page = await self.execute_cdp_cmd("Page.printToPDF")
+        return page["data"]
 
     @property
     def switch_to(self) -> SwitchTo:
         """
         :Returns:
             - SwitchTo: an object containing all options to switch focus into
 
@@ -535,16 +565,15 @@
         """Refreshes the current page.
 
         :Usage:
             ::
 
                 driver.refresh()
         """
-        from pycdp import cdp
-        await self.execute(cmd=cdp.page.reload())
+        await self.execute_cdp_cmd("Page.reload")
 
     # Options
     async def get_cookies(self) -> List[dict]:
         """Returns a set of dictionaries, corresponding to cookies visible in
         the current session.
 
         :Usage:
@@ -674,75 +703,23 @@
 
     @timeouts.setter
     def timeouts(self, timeouts):
         self._page_load_timeout = timeouts["page_load"]
         self._script_timeout = timeouts["script"]
 
     # noinspection PyUnusedLocal
-    async def find_element(self, by=By.ID, value: Optional[str] = None) -> WebElement:
-        """Find an element given a By strategy and locator.
-
-        :Usage:
-            ::
-
-                element = driver.find_element(By.ID, 'foo')
-
-        :rtype: WebElement
-        """
-        # by = RelativeBy({by: value})
-        if isinstance(by, RelativeBy):
-            elements = await self.find_elements(by=by, value=value)
-            if not elements:
-                raise NoSuchElementException(f"Cannot locate relative element with: {by.root}")
-            return elements[0]
-
-        if by == By.ID:
-            by = By.CSS_SELECTOR
-            value = f'[id="{value}"]'
-        elif by == By.CLASS_NAME:
-            by = By.CSS_SELECTOR
-            value = f".{value}"
-        elif by == By.NAME:
-            by = By.CSS_SELECTOR
-            value = f'[name="{value}"]'
-
-        raise NotImplementedError("not started with chromedriver")
-
-    # noinspection PyUnusedLocal
-    async def find_elements(self, by=By.ID, value: Optional[str] = None) -> List[WebElement]:
-        """Find elements given a By strategy and locator.
-
-        :Usage:
-            ::
-
-                elements = driver.find_elements(By.CLASS_NAME, 'foo')
-
-        :rtype: list of WebElement
-        """
-        from selenium_driverless.utils.utils import sel_path, read
-        # by = RelativeBy({by: value})
-        if isinstance(by, RelativeBy):
-            _pkg = ".".join(__name__.split(".")[:-1])
-            raw_function = read(sel_path() + "webdriver/remote/findElements.js", sel_root=False)
-            find_element_js = f"/* findElements */return ({raw_function}).apply(null, arguments);"
-            return await self.execute_script(find_element_js, by.to_dict())
-
-        if by == By.ID:
-            by = By.CSS_SELECTOR
-            value = f'[id="{value}"]'
-        elif by == By.CLASS_NAME:
-            by = By.CSS_SELECTOR
-            value = f".{value}"
-        elif by == By.NAME:
-            by = By.CSS_SELECTOR
-            value = f'[name="{value}"]'
-
-        # Return empty list if driver returns null
-        # See https://github.com/SeleniumHQ/selenium/issues/4555
-        raise NotImplementedError("not started with chromedriver")
+    async def find_element(self, by: str, value: str, parent=None):
+        if not parent:
+            parent = await WebElement(driver=self, js="document", check_existence=False)
+        return await parent.find_element(by=by, value=value)
+
+    async def find_elements(self, by: str, value: str, parent=None):
+        if not parent:
+            parent = await WebElement(driver=self, js="document", check_existence=False)
+        return await parent.find_elements(by=by, value=value)
 
     @property
     def capabilities(self) -> dict:
         """returns the drivers current capabilities being used."""
         return self.caps
 
     async def get_screenshot_as_file(self, filename) -> bool:
@@ -808,16 +785,16 @@
         which is useful in embedded images in HTML.
 
         :Usage:
             ::
 
                 driver.get_screenshot_as_base64()
         """
-        from pycdp import cdp
-        return await self.execute(cmd=cdp.page.capture_screenshot(format_="png"))
+        res = await self.execute_cdp_cmd("Page.captureScreenshot", {"format": "png"})
+        return res["data"]
 
     # noinspection PyPep8Naming
     async def set_window_size(self, width, height, windowHandle: str = "current") -> None:
         """Sets the width and height of the current window. (window.resizeTo)
 
         :Args:
          - width: the width in pixels to set the window to
@@ -889,18 +866,16 @@
         of the current window.
 
         :Usage:
             ::
 
                 driver.get_window_rect()
         """
-        from pycdp import cdp
-        script = cdp.browser.get_window_bounds(await self.current_window_id)
-        bounds = await self.execute(cmd=script)
-        json = bounds.to_json()
+        json = await self.execute_cdp_cmd("Browser.getWindowBounds", {"windowId": await self.current_window_id})
+        json = json["bounds"]
         json["x"] = json["left"]
         del json["left"]
         json["y"] = json["top"]
         del json["top"]
         return json
 
     async def set_window_rect(self, x=None, y=None, width=None, height=None) -> dict:
@@ -912,31 +887,27 @@
         :Usage:
             ::
 
                 driver.set_window_rect(x=10, y=10)
                 driver.set_window_rect(width=100, height=200)
                 driver.set_window_rect(x=10, y=10, width=100, height=200)
         """
-        from pycdp import cdp
 
         if (x is None and y is None) and (not height and not width):
             raise InvalidArgumentException("x and y or height and width need values")
 
-        json = {"left": x, "top": y, "width": width, 'height': height}
-        bounds = cdp.browser.Bounds()
-        bounds = bounds.from_json(json=json)
+        bounds = {"left": x, "top": y, "width": width, 'height': height}
+        await self.execute_cdp_cmd("Browser.setWindowBounds",
+                                   {"windowId": await self.current_window_id, "bounds": bounds})
+        bounds["x"] = bounds["left"]
+        del bounds["left"]
+        bounds["y"] = bounds["top"]
+        del bounds["top"]
 
-        script = cdp.browser.set_window_bounds(await self.current_window_id, bounds)
-        await self.execute(cmd=script)
-        json["x"] = json["left"]
-        del json["left"]
-        json["y"] = json["top"]
-        del json["top"]
-
-        return json
+        return bounds
 
     @property
     def file_detector(self) -> FileDetector:
         return self._file_detector
 
     @file_detector.setter
     def file_detector(self, detector) -> None:
@@ -1124,33 +1095,45 @@
         :Returns:
             A dict. For example:
             {'latency': 4, 'download_throughput': 2, 'upload_throughput': 2,
             'offline': False}
         """
         raise NotImplementedError("not started with chromedriver")
 
-    async def set_network_conditions(self, **network_conditions) -> None:
+    async def set_network_conditions(self, offline: bool, latency: int, download_throughput: int,
+                                     upload_throughput: int, connection_type: None) -> None:
         """Sets Chromium network emulation settings.
 
         :Args:
          - network_conditions: A dict with conditions specification.
 
         :Usage:
             ::
 
                 driver.set_network_conditions(
                     offline=False,
                     latency=5,  # additional latency (ms)
                     download_throughput=500 * 1024,  # maximal throughput
-                    upload_throughput=500 * 1024)  # maximal throughput
+                    upload_throughput=500 * 1024,  # maximal throughput
+                    connection_type="wifi")
 
             Note: 'throughput' can be used to set both (for download and upload).
         """
-        from pycdp import cdp
-        await self.execute(cmd=cdp.network.emulate_network_conditions(**network_conditions))
+        args = {"offline": offline, "latency": latency,
+                "downloadThroughput": download_throughput,
+                "uploadThroughput": upload_throughput}
+
+        conn_types = ["none", "cellular2g", "cellular3g", "cellular4g", "bluetooth", "ethernet", "wifi", "wimax",
+                      "other"]
+        if connection_type:
+            if connection_type not in conn_types:
+                raise ValueError(f"expected {conn_types} for connection_type,  but got {connection_type}")
+            args["connectionType"] = connection_type
+
+        await self.execute_cdp_cmd("Network.emulateNetworkConditions", args)
 
     def delete_network_conditions(self) -> None:
         """Resets Chromium network emulation settings."""
         raise NotImplementedError("not started with chromedriver")
 
     async def set_permissions(self, name: str, value: str, origin: str = None) -> None:
         """Sets Applicable Permission.
@@ -1168,15 +1151,15 @@
         if value not in settings:
             raise ValueError(f"value needs to be within {settings}, but got {value}")
         args = {"permission": {"name": name}, "setting": value}
         if origin:
             args["origin"] = origin
         await self.execute_cdp_cmd("Browser.setPermission", args)
 
-    async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None):
+    async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None) -> dict:
         """Execute Chrome Devtools Protocol command and get returned result The
         command and command args should follow chrome devtools protocol
         domains/commands, refer to link
         https://chromedevtools.github.io/devtools-protocol/
 
         :Args:
          - cmd: A str, command name
@@ -1195,15 +1178,15 @@
 
         def execute_cdp_cmd(_cmd_dict):
             json = yield _cmd_dict
             return json
 
         cmd_dict = dict(method=cmd, params=cmd_args)
         request = execute_cdp_cmd(cmd_dict)
-        return await self.execute(cmd=request)
+        return await self.session.execute(request)
 
     # noinspection PyTypeChecker
     async def get_sinks(self) -> list:
         """
         :Returns: A list of sinks available for Cast.
         """
         await self.execute_cdp_cmd("Cast.enable")
```

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.2/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.1.2
+Version: 1.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -89,17 +89,18 @@
 ```
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
-
-- [ ] page-interactions
-  - [ ] find element
+- protocoll
+  - [ ] add cdp event handler
+- [x] sync
+  - [ ] move sync to threaded for allowing event_handlers
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.1.2/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.2/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -13,10 +13,13 @@
 src/selenium_driverless.egg-info/requires.txt
 src/selenium_driverless.egg-info/top_level.txt
 src/selenium_driverless/files/__init__.py
 src/selenium_driverless/scripts/__init__.py
 src/selenium_driverless/scripts/alert.py
 src/selenium_driverless/scripts/options.py
 src/selenium_driverless/scripts/switch_to.py
+src/selenium_driverless/types/__init__.py
+src/selenium_driverless/types/by.py
+src/selenium_driverless/types/webelement.py
 src/selenium_driverless/utils/__init__.py
 src/selenium_driverless/utils/utils.py
 tests/test_driverless.py
```

### Comparing `selenium_driverless-1.1.2/tests/test_driverless.py` & `selenium_driverless-1.2/tests/test_driverless.py`

 * *Files identical despite different names*

