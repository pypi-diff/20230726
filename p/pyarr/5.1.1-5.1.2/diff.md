# Comparing `tmp/pyarr-5.1.1.tar.gz` & `tmp/pyarr-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarr-5.1.1.tar", max compression
+gzip compressed data, was "pyarr-5.1.2.tar", max compression
```

## Comparing `pyarr-5.1.1.tar` & `pyarr-5.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1056 2023-07-23 18:56:36.025116 pyarr-5.1.1/LICENSE
--rw-r--r--   0        0        0     6525 2023-07-23 18:56:36.025116 pyarr-5.1.1/README.md
--rw-r--r--   0        0        0      249 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/__init__.py
--rw-r--r--   0        0        0    32046 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/base.py
--rw-r--r--   0        0        0      101 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/const.py
--rw-r--r--   0        0        0     1081 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/exceptions.py
--rw-r--r--   0        0        0    28051 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/lidarr.py
--rw-r--r--   0        0        0        0 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/models/__init__.py
--rw-r--r--   0        0        0     2592 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/models/common.py
--rw-r--r--   0        0        0     1059 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/models/lidarr.py
--rw-r--r--   0        0        0     1903 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/models/radarr.py
--rw-r--r--   0        0        0     1833 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/models/readarr.py
--rw-r--r--   0        0        0     2057 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/models/sonarr.py
--rw-r--r--   0        0        0        0 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/py.typed
--rw-r--r--   0        0        0    21301 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/radarr.py
--rw-r--r--   0        0        0    31608 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/readarr.py
--rw-r--r--   0        0        0     8346 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/request_handler.py
--rw-r--r--   0        0        0    26503 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/sonarr.py
--rw-r--r--   0        0        0      300 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyarr/types.py
--rw-r--r--   0        0        0     3092 2023-07-23 18:56:36.025116 pyarr-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     7629 1970-01-01 00:00:00.000000 pyarr-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-26 15:00:27.061761 pyarr-5.1.2/LICENSE
+-rw-r--r--   0        0        0     6525 2023-07-26 15:00:27.061761 pyarr-5.1.2/README.md
+-rw-r--r--   0        0        0      249 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/__init__.py
+-rw-r--r--   0        0        0    32046 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/base.py
+-rw-r--r--   0        0        0      182 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/const.py
+-rw-r--r--   0        0        0     1081 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/exceptions.py
+-rw-r--r--   0        0        0    28396 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/lidarr.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/common.py
+-rw-r--r--   0        0        0     1828 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/lidarr.py
+-rw-r--r--   0        0        0     1964 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/radarr.py
+-rw-r--r--   0        0        0     1867 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/readarr.py
+-rw-r--r--   0        0        0     2165 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/sonarr.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/py.typed
+-rw-r--r--   0        0        0    21169 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/radarr.py
+-rw-r--r--   0        0        0    31608 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/readarr.py
+-rw-r--r--   0        0        0     8346 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/request_handler.py
+-rw-r--r--   0        0        0    26239 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/sonarr.py
+-rw-r--r--   0        0        0      300 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/types.py
+-rw-r--r--   0        0        0     3092 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7629 1970-01-01 00:00:00.000000 pyarr-5.1.2/PKG-INFO
```

### Comparing `pyarr-5.1.1/LICENSE` & `pyarr-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/README.md` & `pyarr-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/pyarr/base.py` & `pyarr-5.1.2/pyarr/base.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/pyarr/exceptions.py` & `pyarr-5.1.2/pyarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/pyarr/lidarr.py` & `pyarr-5.1.2/pyarr/lidarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,24 +307,35 @@
 
         Returns:
             Response: 200 / 401
         """
         return self._delete(f"album/{id_}", self.ver_uri)
 
     # POST /command
-    def post_command(self, name: LidarrCommand) -> JsonObject:
+    def post_command(
+        self, name: LidarrCommand, **kwargs: Optional[dict[str, Union[int, list[int]]]]
+    ) -> JsonObject:
         """Send a command to Lidarr
 
         Args:
             name (LidarrCommand): Command to be run against Lidarr
+            **kwargs: Additional parameters for specific commands.
+
+        Note:
+            For available commands and required `**kwargs` see the `LidarrCommands` model
 
         Returns:
             JsonObject: dictionary of executed command information
         """
-        return self._post("command", self.ver_uri, data={"name": name})
+        data: dict[str, Any] = {
+            "name": name,
+        }
+        if kwargs:
+            data |= kwargs
+        return self._post("command", self.ver_uri, data=data)
 
     # GET /wanted
     def get_wanted(
         self,
         id_: Optional[int] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
```

### Comparing `pyarr-5.1.1/pyarr/models/common.py` & `pyarr-5.1.2/pyarr/models/common.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/pyarr/models/radarr.py` & `pyarr-5.1.2/pyarr/models/radarr.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,51 +12,56 @@
 """
 Radarr commands.
 
     Note:
         The parameters are supplied as `**kwargs` within the `post_command` method.
 
 DownloadedMoviesScan:
-    Scans for all clients for downloaded movies, or a single client by ID
+    Scans downloaded episodes for state
 
     Args:
-        clientid (int, optional): Download client ID
+        path (str): path to files
 
 MissingMoviesSearch:
     Searches for any missing movies
 
 MoviesSearch:
     Searches for the specified movie or movies
 
     Args:
         movieIds (list[int]): ID of Movie or movies
 
-RefreshMovies:
+RefreshMovie:
     Refreshes all of the movies, or specific by ID
 
     Args:
-        movieid (int, Optional): ID of Movie
+        movieId (int, Optional): ID of Movie
 
 RenameMovie:
     Rename specific movie to correct format.
 
     Args:
-        movieid (list[int]): ID of Movie or movies
+        movieId (int): ID of Movie or movies
+        movieIds (list[int]): ID of Movie or movies
 
 RescanMovie:
     Rescans specific movie
 
     Args:
-        movieid (int): ID of Movie
+        movieId (int): ID of Movie
 
 RenameFiles:
     Rename files to correct format
 
     Args:
-        movieid (int): ID of Movie
+        movieId (int): ID of Movie
+        files (int): ID of files
+
+RssSync:
+    Synchronise RSS Feeds
 
 Backup:
     Backup the server data
 """
 
 #: Radarr sort keys
 RadarrSortKey = Literal[
```

### Comparing `pyarr-5.1.1/pyarr/models/readarr.py` & `pyarr-5.1.2/pyarr/models/readarr.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,20 +52,22 @@
         authorIds (list[int], optional): IDs for Authors
 
 RenameFiles:
     Rename all files, or by specific ID
 
     Args:
         authorId (int, optional): ID for Author
+        files (str): ID of files
 
 RescanFolders:
     Rescans folders
 
 RssSync:
     Synchronise RSS Feeds
+
 Backup:
     Backup of the Database
 
 MissingBookSearch:
     Searches for any missing books
 """
```

### Comparing `pyarr-5.1.1/pyarr/models/sonarr.py` & `pyarr-5.1.2/pyarr/models/sonarr.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 Backup:
     Backup of the Database
 
 DownloadedEpisodesScan:
     Scans downloaded episodes for state
 
+    Args:
+        path (str): path to files
+
 EpisodeSearch:
     Searches for all episondes, or specific ones in supplied list
 
     Args:
         episodeIds (lsit[int], optional): One or more episodeIds in a list
 
 missingEpisodeSearch:
@@ -45,14 +48,15 @@
     Args:
         seriesIds (list[int]): List of Series IDs to rename.
 
 RenameFiles:
     Renames files to the expected naming format.
 
     Args:
+        seriesId (int, optional): ID of series files relate to
         files (list[int]): List of File IDs to rename.
 
 RescanSeries:
     Re-scan all series, if `seriesId` is provided only that series will be Re-scanned.
 
     Args:
         seriesId (int, optional): ID of series to search for.
```

### Comparing `pyarr-5.1.1/pyarr/radarr.py` & `pyarr-5.1.2/pyarr/radarr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Optional, Union
 from warnings import warn
 
 from requests import Response
 
+from pyarr.const import DEPRECATION_WARNING
 from pyarr.types import JsonArray, JsonObject
 
 from .base import BaseArrAPI
 from .exceptions import PyarrMissingArgument
 from .models.common import PyarrSortDirection
 from .models.radarr import (
     RadarrAvailabilityType,
@@ -155,15 +156,15 @@
             This method is deprecated and will be removed in a
             future release. Please use get_movie()
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_movie()",
+            f"{DEPRECATION_WARNING} Please use get_movie()",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._get(f"movie/{id_}", self.ver_uri)
 
     # DELETE /movie/{id}
     def del_movie(
@@ -222,15 +223,15 @@
         Args:
             id_ (str): TMDB ID
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. use lookup_movie(term='tmdb:123456')",
+            f"{DEPRECATION_WARNING} use lookup_movie(term='tmdb:123456')",
             DeprecationWarning,
             stacklevel=2,
         )
         params = {"term": f"tmdb:{id_}"}
         return self._get("movie/lookup", self.ver_uri, params)
 
     # GET /movie/lookup
@@ -240,15 +241,15 @@
         Args:
             id_ (str): IMDB ID
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. use lookup_movie(term='imdb:123456')",
+            f"{DEPRECATION_WARNING} use lookup_movie(term='imdb:123456')",
             DeprecationWarning,
             stacklevel=2,
         )
         params = {"term": f"imdb:{id_}"}
         return self._get("movie/lookup", self.ver_uri, params)
 
     # PUT /movie/editor
@@ -287,15 +288,15 @@
                     "addImportExclusion": true
                 }
 
         Returns:
             Response: HTTP Response
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use del_movie().",
+            f"{DEPRECATION_WARNING} Please use del_movie().",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._delete("movie/editor", self.ver_uri, data=data)
 
     # POST /movie/import
     def import_movies(self, data: JsonArray) -> JsonArray:
```

### Comparing `pyarr-5.1.1/pyarr/readarr.py` & `pyarr-5.1.2/pyarr/readarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/pyarr/request_handler.py` & `pyarr-5.1.2/pyarr/request_handler.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.1/pyarr/sonarr.py` & `pyarr-5.1.2/pyarr/sonarr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 from typing import Any, Optional, Union
 from warnings import warn
 
 from requests import Response
 
+from pyarr.const import DEPRECATION_WARNING
 from pyarr.exceptions import PyarrMissingArgument
 from pyarr.types import JsonArray, JsonObject
 
 from .base import BaseArrAPI
 from .models.common import PyarrHistorySortKey, PyarrSortDirection
 from .models.sonarr import SonarrCommands, SonarrSortKey
 
@@ -98,15 +99,15 @@
             This method is deprecated and will be removed in a
             future release. Please use get_episode()
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_episode()",
+            f"{DEPRECATION_WARNING} Please use get_episode()",
             DeprecationWarning,
             stacklevel=2,
         )
         params = {"seriesId": id_}
         return self._get("episode", self.ver_uri, params)
 
     # GET /episode/{id}
@@ -120,15 +121,15 @@
             This method is deprecated and will be removed in a
             future release. Please use get_episode()
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_episode()",
+            f"{DEPRECATION_WARNING} Please use get_episode()",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._get(f"episode/{id_}", self.ver_uri)
 
     # PUT /episode
     def upd_episode(self, id_: int, data: JsonObject) -> JsonObject:
@@ -177,15 +178,15 @@
         Args:
             id_ (int): Database id of series
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_episode_file()",
+            f"{DEPRECATION_WARNING} Please use get_episode_file()",
             DeprecationWarning,
             stacklevel=2,
         )
         params = {"seriesId": id_}
         return self._get("episodefile", self.ver_uri, params)
 
     # GET /episodefile/{id}
@@ -364,15 +365,15 @@
         Args:
             title (str): Title of series / episode
 
         Returns:
             JsonObject: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_parse_title_path()",
+            f"{DEPRECATION_WARNING} Please use get_parse_title_path()",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._get("parse", self.ver_uri, {"title": title})
 
     # GET /parse
     def get_parsed_path(self, file_path: str) -> JsonObject:
@@ -384,15 +385,15 @@
         Args:
             file_path (str): file path of series / episode
 
         Returns:
             JsonObject: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_parse_title_path()",
+            f"{DEPRECATION_WARNING} Please use get_parse_title_path()",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._get("parse", self.ver_uri, {"path": file_path})
 
     ## RELEASE
 
@@ -577,15 +578,15 @@
         Args:
             id_ (int): TVDB ID
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use lookup_series()",
+            f"{DEPRECATION_WARNING} Please use lookup_series()",
             DeprecationWarning,
             stacklevel=2,
         )
         params = {"term": f"tvdb:{id_}"}
         return self._get("series/lookup", self.ver_uri, params)
 
     # GET /history
@@ -645,15 +646,15 @@
             This method is deprecated and will be removed in a
             future release. Please use get_language()
 
         Returns:
             Union[JsonArray, dict[Any, Any]]: List of dictionaries with items
         """
         warn(
-            "This method is deprecated and will be removed in a future release. Please use get_language()",
+            f"{DEPRECATION_WARNING} Please use get_language()",
             DeprecationWarning,
             stacklevel=2,
         )
 
         path = f"languageprofile{f'/{id_}' if id_ else ''}"
         return self._get(path, self.ver_uri)
```

### Comparing `pyarr-5.1.1/pyproject.toml` & `pyarr-5.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyarr"
-version = "5.1.1"
+version = "5.1.2"
 description = "Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python"
 authors = ["Steven Marks <marksie1988@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sonarr", "radarr", "readarr", "lidarr", "api", "wrapper", "plex"]
 homepage = "https://github.com/totaldebug/pyarr"
 repository = "https://github.com/totaldebug/pyarr"
```

### Comparing `pyarr-5.1.1/PKG-INFO` & `pyarr-5.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarr
-Version: 5.1.1
+Version: 5.1.2
 Summary: Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python
 Home-page: https://github.com/totaldebug/pyarr
 License: MIT
 Keywords: sonarr,radarr,readarr,lidarr,api,wrapper,plex
 Author: Steven Marks
 Author-email: marksie1988@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyarr Version: 5.1.1 Summary: Synchronous Sonarr,
+Metadata-Version: 2.1 Name: pyarr Version: 5.1.2 Summary: Synchronous Sonarr,
 Radarr, Lidarr and Readarr API's for Python Home-page: https://github.com/
 totaldebug/pyarr License: MIT Keywords:
 sonarr,radarr,readarr,lidarr,api,wrapper,plex Author: Steven Marks Author-
 email: marksie1988@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

