# Comparing `tmp/weboptout-0.1.tar.gz` & `tmp/weboptout-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weboptout-0.1.tar", max compression
+gzip compressed data, was "weboptout-0.2.1.tar", max compression
```

## Comparing `weboptout-0.1.tar` & `weboptout-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-07-21 15:56:56.828920 weboptout-0.1/LICENSE
--rw-r--r--   0        0        0      750 2023-07-21 15:56:56.932928 weboptout-0.1/pyproject.toml
--rw-r--r--   0        0        0      181 2023-07-21 15:56:56.936928 weboptout-0.1/src/weboptout/__init__.py
--rw-r--r--   0        0        0      615 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/client.py
--rw-r--r--   0        0        0     1421 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/config.py
--rw-r--r--   0        0        0     3282 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/html.py
--rw-r--r--   0        0        0     5716 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/http.py
--rw-r--r--   0        0        0     1415 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/types.py
--rw-r--r--   0        0        0     1656 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/utils.py
--rw-r--r--   0        0        0      879 2023-07-21 15:56:56.828920 weboptout-0.1/src/weboptout/web.py
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 weboptout-0.1/PKG-INFO
+-rw-r--r--   0        0        0     5003 2023-07-26 20:11:12.697787 weboptout-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7628 2023-07-26 20:11:13.265795 weboptout-0.2.1/data/tos.jsonl
+-rw-r--r--   0        0        0      900 2023-07-26 20:11:13.285795 weboptout-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-26 20:11:13.285795 weboptout-0.2.1/src/weboptout/__init__.py
+-rw-r--r--   0        0        0     1228 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/client.py
+-rw-r--r--   0        0        0     1421 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/config.py
+-rw-r--r--   0        0        0     3418 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/html.py
+-rw-r--r--   0        0        0     8030 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/http.py
+-rw-r--r--   0        0        0     1537 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/types.py
+-rw-r--r--   0        0        0     6987 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/utils.py
+-rw-r--r--   0        0        0     1690 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/web.py
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 weboptout-0.2.1/PKG-INFO
```

### Comparing `weboptout-0.1/pyproject.toml` & `weboptout-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 [tool.poetry]
 name = "weboptout"
 description = "Checks the Copyright information of online works and their conditions of use."
-version = "0.1"
+version = "0.2.1"
 authors = ["Alex J. Champandard <445208+alexjc@users.noreply.github.com>"]
 repository = "https://github.com/alexjc/weboptout"
-license = "MIT"
+license = "MIT and UNLICENSED"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
 ]
 packages = [
     { include = "weboptout", from = "src" },
 ]
+include = [
+    "data/tos.jsonl",
+]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 aiohttp = ">=3.8"
 langdetect = ">=1.0.9"
 beautifulsoup4 = ">=4.12"
+selenium = { version = "0.2.1", optional = true }
+
+[tool.poetry.extras]
+webdriver = ["selenium"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
 hypothesis = ">=6.0.0"
 pytest-cov = ">=3.0.0"
 
 [build-system]
```

### Comparing `weboptout-0.1/src/weboptout/config.py` & `weboptout-0.2.1/src/weboptout/config.py`

 * *Files identical despite different names*

### Comparing `weboptout-0.1/src/weboptout/html.py` & `weboptout-0.2.1/src/weboptout/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,17 @@
     elif len(text) < 2_000:
         size = len(text)
         client.log(
             Status.FAILURE,
             f"Too little information extracted, only {size:,} bytes from "
             f"the ToS page at {url}.",
         )
-        return Status.FAILURE
+
+        # Suggest fetching page again via HTTP with Selenium.
+        return Status.RETRY
 
     else:
         legal_words = len(RE_LEGAL_WORDS.findall(text))
         if legal_words < 36:
             client.log(
                 Status.FAILURE,
                 f"The ToS page does not appear to contain a legal text at {url}.",
@@ -81,25 +83,26 @@
 def _extract_paragraphs(soup):
     """
     Iterator that returns a cleaned up list of paragraphs, lists items, from
     (ideally) the main body of HTML that are most likely to be legal text.
     """
     re_cleanup = re.compile("(\s+|\n|\t)")
 
-    for para in soup.find_all(["p", "li", "ol", "ul"]):
+    for para in soup.find_all(["p", "li", "ol", "ul", "span"]):
         if para.find_parent("a") or para.find_parent(["header", "footer"]):
             continue
+        if para.name == "span" and para.find_parent('p'):
+            continue
         if para.name in ("ol", "ul") and len(para.find_all()) > 0:
             continue
+
         children = [
-            p
-            for p in para.contents
+            p for p in para.contents
             if not isinstance(p, str) or p.strip("\t\n\r ") != ""
         ]
-
         if len(children) == 1 and children[0].name == "a":
             continue
 
         text = (
             " ".join(para.findAll(text=True, recursive=True)).replace("\n", " ").strip()
         )
         if text != "":
```

### Comparing `weboptout-0.1/src/weboptout/http.py` & `weboptout-0.2.1/src/weboptout/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 ## Copyright © 2023, Alex J. Champandard.  Licensed under MIT; see LICENSE! ⚘
 
 import asyncio
 import aiohttp
 import itertools
+from dataclasses import dataclass
 from urllib.parse import urljoin
 
 from bs4 import BeautifulSoup
 
-from .utils import cache_to_directory
 from .types import Status
 from .config import RE_HREF_TOS, RE_TEXT_TOS
+from .utils import cache_to_directory, retrieve_from_database, limit_concurrency
+from .client import instantiate_webdriver
 
 
 __all__ = ["search_tos_for_domain"]
 
 
 def _log_cache_hit(client, url, /, filename, result):
-    client.log(Status.SUCCESS, f"Loaded data for {url} from {filename}")
+    if result[-1] != "":
+        client.log(Status.SUCCESS, f"Loaded data request for {url} from {filename}")
+    else:
+        client.log(Status.FAILURE, f"Loaded failed request for {url} from {filename}")
 
 
-@cache_to_directory("./cache/www", key="url", filter=_log_cache_hit)
+@cache_to_directory("cache/www", key="url", filter=_log_cache_hit)
 async def _fetch_from_cache_or_network(client, url: str) -> tuple:
     try:
         async with client.get(url) as response:
             if response.headers.get("Content-Type", "").startswith("image/"):
                 client.log(
                     Status.FAILURE,
                     f"Response contains binary content where text/* was expected "
                     f"from {url}",
                     headers=dict(response.headers),
                 )
                 return str(response.url), dict(response.headers), ""
 
+            if "application/xml" in response.headers.get("Content-Type", ""):
+                client.log(
+                    Status.FAILURE,
+                    f"Response contains XML content where text/* was expected "
+                    f"from {url}",
+                    headers=dict(response.headers),
+                )
+                return str(response.url), dict(response.headers), ""
+
             if response.status != 200:
                 client.log(
                     Status.FAILURE,
                     f"An HTTP error code {response.status} was returned from {url}; "
                     f"trying to proceed anyway...",
                     headers=dict(response.headers),
                 )
@@ -59,37 +73,40 @@
     except aiohttp.ClientError as exc:
         client.log(
             Status.FAILURE,
             f"Problem with HTTP client while connecting to {url} server(s).",
             exception=exc,
         )
 
-    return url, {}, ""
+    return url, {}, None
 
 
+@retrieve_from_database("data/tos.jsonl", key="url")
 async def _find_tos_links_from_url(client, url: str) -> list[str]:
     url, _, html = await _fetch_from_cache_or_network(client, url)
+
+    if html is None:
+        return None, None
+
     if html == "":
-        client.log(
-            Status.FAILURE, f"Couldn't find ToS links as there's no data from {url}"
-        )
-        return url, []
+        return url, None
 
     return await _find_tos_links_from_html(client, url, html)
 
 
 async def _find_tos_links_from_html(client, url, html: str) -> list[str]:
     soup = BeautifulSoup(html, "html.parser")
 
     all_links = [
         l
         for l in soup.find_all("a")
         if l.get("href") is not None
-        and not (href := l.get("href")).startswith("#")
-        and not href.lower().startswith("javascript:")
+        and not (href := l.get("href")).lower().startswith("javascript:")
+        and not any(href.startswith(k) for k in "#?")
+        and not (l.get_text().lower in ["refresh", "reload"])
     ]
     if len(all_links) == 0 or any(
         k in html for k in ("turn on javascript", "enable-javascript.com")
     ):
         client.log(
             Status.FAILURE, f"JavaScript must be enabled to view content from {url}"
         )
@@ -134,42 +151,92 @@
         urljoin(url, l.get("href"))
         for p in itertools.zip_longest(match_links, match_texts)
         for l in p
         if l is not None
     ]
 
 
+
+def _reject_if_header_missing(url, headers, /, filename, result):
+    return "User-Agent" not in headers
+    
+
+@cache_to_directory("cache/www", key="url", filter=_reject_if_header_missing)
+@limit_concurrency(value=1)
+async def _fetch_from_browser_then_cache_result(url, headers):
+    try:
+        webdriver = instantiate_webdriver()
+        webdriver.get(url)
+    except Exception as exc: # selenium.common.exceptions.TimeoutException
+        if "Message: Navigation timed out after" not in str(exc):
+            raise
+        return url, headers, ""
+
+    def page_is_loading():            
+        x = webdriver.execute_script("return document.readyState")
+        return x == "complete"
+
+    while not page_is_loading():
+        await asyncio.sleep(0.01)
+    await asyncio.sleep(1.0)
+
+    html = webdriver.execute_script("return document.documentElement.outerHTML")
+    headers["User-Agent"] = "WebOptOut/Firefox"
+    return url, headers, html
+
+
+@dataclass
+class RequestOptions:
+    retry: bool = False
+
+
 async def search_tos_for_domain(client, domain: str) -> str:
-    assert not domain.startswith("http")
+    assert not any(domain.startswith(k) for k in ("https://", "http://"))
 
     # Step 1) find the right domain from the domain.
     while domain.count(".") > 0:
         links = []
         url, links = await _find_tos_links_from_url(client, "https://" + domain)
 
-        if len(links) == 0:
+        if url is None or len(links or []) == 0:
             domain = ".".join(domain.split(".")[1:])
             continue
         else:
             break
 
+    # No data from server, just terminate.
+    if links is None:
+        return
+
+    # Content received but no links.
     if len(links) == 0:
+        yield url, "", {}
         return
 
     # Step 2) find the right page on that domain.
     visited = set()
     while len(links) > 0:
         url = links.pop(0)
         visited.add(url)
 
-        url, _, html = await _fetch_from_cache_or_network(client, url)
+        new_url, headers, html = await _fetch_from_cache_or_network(client, url)
         if html is None:
             continue
 
         client.log(
             Status.SUCCESS,
             f"Retrieved Terms Of Service for {url} with {len(html):,} bytes of text.",
         )
-        yield url, html
+
+        options = RequestOptions()
+        yield new_url, html, options
+
+        if options.retry:
+            url, headers, html = await _fetch_from_browser_then_cache_result(url, headers)
+            client.log(
+                Status.SUCCESS,
+                f"Browsed for Terms Of Service again with Selenium and got {len(html):,} bytes of text.",
+            )
+            yield url, html, options
 
         url, further_links = await _find_tos_links_from_html(client, url, html)
         links.extend(l for l in further_links if l not in links and l not in visited)
```

### Comparing `weboptout-0.1/src/weboptout/types.py` & `weboptout-0.2.1/src/weboptout/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,44 +7,47 @@
     """
     Enumeration of status codes that can be used as return values to indicate
     the result of an operation, or as the status code of a log record.
     """
 
     SUCCESS = 1
     FAILURE = 0
-    ABORT = -1
+    RETRY = -1
+    ABORT = -2
 
 
 class Reservation:
     """
     A reservation of rights and all the information that goes with it, in
     order to provide explanations.  The reservation can apply to any concept,
     including a domain, a URL, a file.
 
     This class is intended to be used via the `rsv` namespace, along with the
     defaults YES, MAYBE, NO.  These can be cloned via the __call__ function to
     create Reservations derived from that default.
     """
 
-    def __init__(self, id: int, summary: str = None, records: list = None):
+    def __init__(self, id: int, summary: str = None, url: str = None, records: list = None):
         self._id = id
         self.summary = summary
+        self.url = url
         self.records = records or []
 
     def __eq__(self, id: int):
         return self._id == id
 
     def __repr__(self):
-        return f'<weboptout.Reservation id={self._id} summary="{self.summary}">'
+        return f'<weboptout.Reservation id={self._id} url="{self.url}" summary="{self.summary}">'
 
-    def __call__(self, /, summary: str, records: list = None):
-        return Reservation(self._id, summary, records)
+    def __call__(self, /, summary: str, url: str = None, records: list = None):
+        return Reservation(self._id, summary, url, records)
 
 
 class rsv:
     """
     Namespace with default Reservations that can be cloned and used for comparison.
     """
 
     YES = Reservation(2)
     MAYBE = Reservation(1)
     NO = Reservation(0)
+    ERROR = Reservation(-1)
```

### Comparing `weboptout-0.1/PKG-INFO` & `weboptout-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: weboptout
-Version: 0.1
+Version: 0.2.1
 Summary: Checks the Copyright information of online works and their conditions of use.
 Home-page: https://github.com/alexjc/weboptout
-License: MIT
+License: MIT and UNLICENSED
 Author: Alex J. Champandard
 Author-email: 445208+alexjc@users.noreply.github.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Provides-Extra: webdriver
 Requires-Dist: aiohttp (>=3.8)
 Requires-Dist: beautifulsoup4 (>=4.12)
 Requires-Dist: langdetect (>=1.0.9)
+Requires-Dist: selenium (==0.2.1) ; extra == "webdriver"
 Project-URL: Repository, https://github.com/alexjc/weboptout
```

