# Comparing `tmp/selenium_driverless-1.2.tar.gz` & `tmp/selenium_driverless-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.2.tar", last modified: Wed Jul 26 09:26:08 2023, max compression
+gzip compressed data, was "selenium_driverless-1.2.1.tar", last modified: Wed Jul 26 11:31:02 2023, max compression
```

## Comparing `selenium_driverless-1.2.tar` & `selenium_driverless-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.150004 selenium_driverless-1.2/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3821 2023-07-26 09:26:08.150004 selenium_driverless-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2023-07-26 09:25:36.000000 selenium_driverless-1.2/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-26 09:26:08.151001 selenium_driverless-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.121741 selenium_driverless-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.130678 selenium_driverless-1.2/src/selenium_driverless/
--rw-rw-rw-   0        0        0       21 2023-07-26 09:25:45.000000 selenium_driverless-1.2/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.137841 selenium_driverless-1.2/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.141899 selenium_driverless-1.2/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    17252 2023-07-24 21:37:07.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.146005 selenium_driverless-1.2/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    15407 2023-07-26 09:11:23.000000 selenium_driverless-1.2/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.147004 selenium_driverless-1.2/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    45211 2023-07-26 09:21:31.000000 selenium_driverless-1.2/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.136843 selenium_driverless-1.2/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3821 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-07-26 09:26:08.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 09:26:07.000000 selenium_driverless-1.2/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:08.149004 selenium_driverless-1.2/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.421173 selenium_driverless-1.2.1/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.1/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3823 2023-07-26 11:31:02.422304 selenium_driverless-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-07-26 09:25:36.000000 selenium_driverless-1.2.1/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.1/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-26 11:31:02.423327 selenium_driverless-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.368348 selenium_driverless-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.383256 selenium_driverless-1.2.1/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-07-26 11:28:48.000000 selenium_driverless-1.2.1/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.396752 selenium_driverless-1.2.1/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.1/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.406099 selenium_driverless-1.2.1/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.413942 selenium_driverless-1.2.1/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.1/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.1/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.1/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.418377 selenium_driverless-1.2.1/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.1/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.1/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    45635 2023-07-26 11:23:33.000000 selenium_driverless-1.2.1/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.394708 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.420038 selenium_driverless-1.2.1/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.1/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.2/LICENSE.md` & `selenium_driverless-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/PKG-INFO` & `selenium_driverless-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.2
+Version: 1.2.1
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.2/README.md` & `selenium_driverless-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/build_upload.md` & `selenium_driverless-1.2.1/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/setup.py` & `selenium_driverless-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.2.1/src/selenium_driverless/scripts/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.2.1/src/selenium_driverless/scripts/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,14 @@
         self._extension_files = []
         self._extensions = []
         self._experimental_options = {}
         self._debugger_address = None
         self.user_data_dir = None
         self._arguments = []
         self.add_argument("--user-data-dir=" + sel_driverless_path() + "/files/tmp/" + uuid.uuid4().hex)
-        port = random_port("localhost")
-        self.add_argument(f"--remote-debugging-port={port}")
         self._ignore_local_proxy = False
 
     @property
     def capabilities(self):
         return self._caps
 
     def set_capability(self, name: str, value: dict) -> None:
```

### Comparing `selenium_driverless-1.2/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.2.1/src/selenium_driverless/scripts/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.2.1/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/src/selenium_driverless/types/by.py` & `selenium_driverless-1.2.1/src/selenium_driverless/types/by.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/src/selenium_driverless/types/webelement.py` & `selenium_driverless-1.2.1/src/selenium_driverless/types/webelement.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,20 +43,16 @@
     All method calls will do a freshness check to ensure that the element
     reference is still valid.  This essentially determines whether the
     element is still attached to the DOM.  If this test fails, then an
     ``StaleElementReferenceException`` is thrown, and all future calls to this
     instance will fail.
     """
 
-    def __init__(self, driver, js: str = None, obj_id=None, parent=None, check_existence=True) -> None:
+    def __init__(self, driver, js: str = None, obj_id=None, check_existence=True) -> None:
         self._loop = None
-        if not parent:
-            self._parent = WebElement(js="document", driver=driver, parent="undefined", check_existence=False)
-        elif parent == "undefined":
-            self._parent = None
         super().__init__(driver=driver, js=js, obj_id=obj_id, check_existence=check_existence)
 
     def __await__(self):
         return super().__await__()
 
     @property
     async def obj_id(self):
@@ -84,15 +80,15 @@
         :rtype: WebElement
         """
         elems = await self.find_elements(by=by, value=value)
         if not elems:
             raise NoSuchElementException()
         return elems[idx]
 
-    async def find_elements(self, by=By.ID, value=None, base_element=None):
+    async def find_elements(self, by=By.ID, value=None):
         """Find elements given a By strategy and locator.
 
         :Usage:
             ::
 
                 element = element.find_elements(By.CLASS_NAME, 'foo')
 
@@ -151,14 +147,19 @@
         return await self.get_property("tagName")
 
     @property
     async def text(self) -> str:
         """The text of the element."""
         return await self.get_property("textContent")
 
+    @property
+    async def value(self) -> str:
+        """The value of the element."""
+        return await self.get_property("value")
+
     async def click(self) -> None:
         """Clicks the element."""
         await self.execute_script("this.click()")
 
     async def submit(self):
         """Submits a form."""
         script = (
@@ -172,15 +173,15 @@
             "e.initEvent('submit', true, true);\n"
             "if (form.dispatchEvent(e)) { HTMLFormElement.prototype.submit.call(form) }\n"
         )
         return await self.execute_script(script)
 
     async def clear(self) -> None:
         """Clears the text if it's a text entry element."""
-        await self.execute_script("this.reset()")
+        await self.execute_script("this.value = ''")
 
     async def get_dom_attribute(self, name: str) -> str:
         """Gets the given attribute of the element. Unlike
         :func:`~selenium.webdriver.remote.BaseWebElement.get_attribute`, this
         method only returns attributes declared in the element's HTML markup.
 
         :Args:
@@ -285,78 +286,75 @@
         on the screen an element is so that we can click it. This method should
         cause the element to be scrolled into view.
 
         Returns the top lefthand corner location on the screen, or zero
         coordinates if the element is not visible.
         """
         "arguments[0].scrollIntoView(true); return arguments[0].getBoundingClientRect()"
-        self.t.exec(self.t.path("scrollIntoView", obj=self._raw), args=[True])
-        result = self.rect
+        await self.execute_script("this.scrollIntoView(true)")
+        result = await self.rect
         return {"x": round(result["x"]), "y": round(result["y"])}
 
     @property
     async def size(self) -> dict:
         """The size of the element."""
         size = await self.rect
         return {"height": size["height"], "width": size["width"]}
 
-    def value_of_css_property(self, property_name) -> str:
+    async def value_of_css_property(self, property_name) -> str:
         """The value of a CSS property."""
         raise NotImplementedError("you might use get_attribute instead")
 
     @property
-    def location(self) -> dict:
+    async def location(self) -> dict:
         """The location of the element in the renderable canvas."""
-        result = self.rect
+        result = await self.rect
         return {"x": round(result["x"]), "y": round(result["y"])}
 
     @property
     async def rect(self) -> dict:
         """A dictionary with the size and location of the element."""
-        result = await self.execute_script("this.getBoundingClientRect()", only_value=False, serialization="deep")
+        result = await self.execute_script("return this.getBoundingClientRect().toJSON()", serialization="json")
         return result
 
     @property
-    def _rect(self):
-        return self.t.exec(self.t.path("", obj=self._raw))
-
-    @property
-    def aria_role(self) -> str:
+    async def aria_role(self) -> str:
         """Returns the ARIA role of the current web element."""
-        return self.get_property("ariaRoleDescription")
+        return await self.get_property("ariaRoleDescription")
 
     @property
-    def accessible_name(self) -> str:
+    async def accessible_name(self) -> str:
         """Returns the ARIA Level of the current webelement."""
-        return self.get_property("ariaLevel")
+        return await self.get_property("ariaLevel")
 
     @property
-    def screenshot_as_base64(self) -> str:
+    async def screenshot_as_base64(self) -> str:
         """Gets the screenshot of the current element as a base64 encoded
         string.
 
         :Usage:
             ::
 
                 img_b64 = element.screenshot_as_base64
         """
         raise NotImplementedError()
 
     @property
-    def screenshot_as_png(self) -> bytes:
+    async def screenshot_as_png(self) -> bytes:
         """Gets the screenshot of the current element as a binary data.
 
         :Usage:
             ::
 
                 element_png = element.screenshot_as_png
         """
-        return b64decode(self.screenshot_as_base64.encode("ascii"))
+        res = await self.screenshot_as_base64
+        return b64decode(res.encode("ascii"))
 
-    def screenshot(self, filename) -> bool:
+    async def screenshot(self, filename) -> bool:
         """Saves a screenshot of the current element to a PNG image file.
         Returns False if there is any IOError, else returns True. Use full
         paths in your filename.
 
         :Args:
          - filename: The full path you wish to save your screenshot to. This
            should end with a `.png` extension.
@@ -367,47 +365,26 @@
                 element.screenshot('/Screenshots/foo.png')
         """
         if not filename.lower().endswith(".png"):
             warnings.warn(
                 "name used for saved screenshot does not match file " "type. It should end with a `.png` extension",
                 UserWarning,
             )
-        png = self.screenshot_as_png
+        png = await self.screenshot_as_png
         try:
             with open(filename, "wb") as f:
                 f.write(png)
         except OSError:
             return False
         finally:
             del png
         return True
 
     @property
     def parent(self):
         """Internal reference to the WebDriver instance this element was found
         from."""
-        return self._parent
+        raise NotImplementedError("can't get paren't yet")
 
     @property
     def children(self):
         return self.find_elements(By.CSS_SELECTOR, "*")
-
-    def _css_selector(self, current=False):
-        def getter():
-            from selenium_driverless.types import JSEvalException
-            script = self.t.exec(self.t.path("CSSSelector", obj=self.t.this()), args=[self._raw])
-            try:
-                return self._injector.tabs.exec(type_dict=script, tab_id=self._tab_id)["result"][0]
-            except JSEvalException as e:
-                if e.message[:25] == "Cannot read properties of":
-                    # is window.document
-                    return ""
-                else:
-                    raise e
-
-        if not self._persistent_css_selector:
-            self._persistent_css_selector = getter()
-        if current:
-            return getter()
-        return self._persistent_css_selector
-
-    # noinspection PyStatementEffect
```

### Comparing `selenium_driverless-1.2/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.2.1/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.2.1/src/selenium_driverless/webdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from base64 import urlsafe_b64encode
 from contextlib import asynccontextmanager
 from importlib import import_module
 from typing import List
 from typing import Optional
 from typing import Union
 
+from pyparsing import Char
 from selenium.common.exceptions import InvalidArgumentException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.print_page_options import PrintOptions
 from selenium.webdriver.common.virtual_authenticator import Credential
 from selenium.webdriver.common.virtual_authenticator import VirtualAuthenticatorOptions
 from selenium.webdriver.common.virtual_authenticator import (
     required_virtual_authenticator,
@@ -43,15 +44,15 @@
 from selenium.webdriver.remote.bidi_connection import BidiConnection
 from selenium.webdriver.remote.file_detector import FileDetector
 from selenium.webdriver.remote.file_detector import LocalFileDetector
 from selenium.webdriver.remote.mobile import Mobile
 from selenium.webdriver.remote.script_key import ScriptKey
 from selenium.webdriver.remote.webdriver import create_matches
 
-from selenium_driverless.scripts.options import Options
+from selenium_driverless.scripts.options import Options as ChromeOptions
 from selenium_driverless.scripts.switch_to import SwitchTo
 from selenium_driverless.sync.switch_to import SwitchTo as SyncSwitchTo
 from selenium_driverless.types.webelement import WebElement, RemoteObject
 from selenium_driverless.sync.webelement import WebElement as SyncWebElement
 
 
 def import_cdp():
@@ -67,15 +68,15 @@
 
 
 class Chrome(BaseWebDriver):
     """Allows you to drive the browser without chromedriver."""
 
     def __init__(
             self,
-            options: Options = None,
+            options: ChromeOptions = None,
     ) -> None:
         """Creates a new instance of the chrome driver. Starts the service and
         then creates new instance of chrome driver.
 
         :Args:
          - options - this takes an instance of ChromeOptions
         """
@@ -87,15 +88,15 @@
         self.session = None
         self.browser_pid = None
         if not options.binary_location:
             from selenium_driverless.utils.utils import find_chrome_executable
             options.binary_location = find_chrome_executable()
 
         try:
-            options = options or Options()
+            options = options or ChromeOptions()
             self._options = options
 
             vendor_prefix = "goog"
             self.vendor_prefix = vendor_prefix
 
             if isinstance(options, list):
                 self._capabilities = create_matches(options)
@@ -179,14 +180,19 @@
         from selenium_driverless.utils.utils import IS_POSIX, read
         from pycdp.asyncio import connect_cdp
         from pycdp import cdp
 
         if self._loop:
             self._switch_to = SyncSwitchTo(driver=self, loop=self._loop)
 
+        if not self._options.debugger_address:
+            from selenium_driverless.utils.utils import random_port
+            port = random_port("localhost")
+            self._options._debugger_address = f"localhost:{port}"
+            self._options.add_argument(f"--remote-debugging-port={port}")
         options = capabilities["goog:chromeOptions"]
 
         browser = subprocess.Popen(
             [options["binary"], *options["args"]],
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
@@ -289,15 +295,16 @@
                     elems.append(await obj.execute_script("return this[arguments[0]]", idx, serialization="deep"))
                 res["value"] = elems
             elif class_name == 'XPathResult':
                 elems = []
                 obj = await RemoteObject(driver=self, obj_id=res["objectId"], check_existence=False)
                 if await obj.execute_script("return [7].includes(this.resultType)", serialization="json"):
                     for idx in range(await obj.execute_script("return this.snapshotLength", serialization="json")):
-                        elems.append(await obj.execute_script("return this.snapshotItem(arguments[0])", idx, serialization="deep"))
+                        elems.append(await obj.execute_script("return this.snapshotItem(arguments[0])", idx,
+                                                              serialization="deep"))
                     res["value"] = elems
         return res
 
     async def execute_raw_script(self, script: str, *args, await_res: bool = False, serialization: str = None,
                                  max_depth: int = None, timeout: int = 2, obj_id=None):
         """
         example:
```

### Comparing `selenium_driverless-1.2/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.2.1/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.2
+Version: 1.2.1
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.2/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.2.1/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2/tests/test_driverless.py` & `selenium_driverless-1.2.1/tests/test_driverless.py`

 * *Files identical despite different names*

