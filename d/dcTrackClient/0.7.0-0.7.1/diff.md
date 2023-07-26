# Comparing `tmp/dctrackclient-0.7.0.tar.gz` & `tmp/dctrackclient-0.7.1.tar.gz`

## Comparing `dctrackclient-0.7.0.tar` & `dctrackclient-0.7.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    17052 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/../README.md
--rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    18825 2020-02-02 00:00:00.000000 dctrackclient-0.7.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.7.1/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    22165 2020-02-02 00:00:00.000000 dctrackclient-0.7.1/../README.md
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 dctrackclient-0.7.1/PKG-INFO
```

### Comparing `dctrackclient-0.7.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.7.1/src/dcTrackClient/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -208,7 +208,31 @@
     def updateSublocation(self, subLocationId: int, payload: dict):
         """Update a sub-location. Returns a list from the Sub-Location Hash."""
         return self.__request('PUT', '/api/v2/subLocations/' + str(subLocationId) + '/?', payload)
 
     def deleteSublocation(self, subLocationId: int):
         """Deletes the given sub-location. The locationId is the ID of the location that the sub-location belongs to and the subLocationId is the ID of the location you are querying. Returns a success message upon success."""
         return self.__request('DELETE', '/api/v2/subLocations/' + str(subLocationId) + '/?')
+
+    def getLocationFavorites(self, username: str):
+        """Retrieve a List of Location Favorites for a specific User."""
+        return self.__request('GET', '/api/v2/users/' + str(username) + '/favorites/LOCATION/?')
+
+    def getLocationFavoritesAllUsers(self):
+        """Retrieve a List of Location Favorites for all Users. Returns JSON entity containing Location Favorite information for all users."""
+        return self.__request('GET', '/api/v2/users/favorites/LOCATION/?')
+
+    def updateLocationFavorites(self, username: str, payload: dict):
+        """Assign Location Favorites to a user where username is a valid dcTrack user and "favorite" is either true or false to indicate whether you are assigning or unassigning. JSON entity containing all Location Favorites for the specified user."""
+        return self.__request('PUT', '/api/v2/users/' + str(username) + '/favorites/?', payload)
+
+    def updateLocationFavoritesAllUsers(self, payload: dict):
+        """Assign Location Favorites to a user. To Assign favorites the "favorite" column should be set to true. To Unassign favorites the "favorite" column should be set to false. Returns JSON entity containing all Location Favorites for the specified users."""
+        return self.__request('PUT', '/api/v2/users/favorites/?', payload)
+
+    def searchCabinetSpace(self, payload: dict):
+        """Find Cabinets with available space based on RUs within the specified Locations."""
+        return self.__request('POST', '/api/v2/capacity/cabinets/list/search/?', payload)
+
+    def searchAvailableRUs(self, payload: dict):
+        """Find the starting RUs within a Cabinet with the specified number of contiguous RUs."""
+        return self.__request('POST', '/api/v2/items/uposition/available/?', payload)
```

### Comparing `dctrackclient-0.7.0/pyproject.toml` & `dctrackclient-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.7.0/../README.md` & `dctrackclient-0.7.1/../README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.7.0
+pip install dcTrackClient==0.7.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.7.0
+npm i dctrackclient@0.7.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -656,7 +656,60 @@
 > Deletes the given sub-location. The locationId is the ID of the location that the sub-location belongs to and the subLocationId is the ID of the location you are querying. Returns a success message upon success.
 ```
 DELETE api/v2/subLocations/{subLocationId}
 ```
 |Parameter|Type|
 |---|---|
 |subLocationId|number|
+
+## getLocationFavorites(username)
+> Retrieve a List of Location Favorites for a specific User.
+```
+GET api/v2/users/{username}/favorites/LOCATION
+```
+|Parameter|Type|
+|---|---|
+|username|string|
+
+## getLocationFavoritesAllUsers()
+> Retrieve a List of Location Favorites for all Users. Returns JSON entity containing Location Favorite information for all users.
+```
+GET api/v2/users/favorites/LOCATION
+```
+*No parameters.*
+
+## updateLocationFavorites(username, payload)
+> Assign Location Favorites to a user where username is a valid dcTrack user and "favorite" is either true or false to indicate whether you are assigning or unassigning. JSON entity containing all Location Favorites for the specified user.
+```
+PUT api/v2/users/{username}/favorites payload
+```
+|Parameter|Type|
+|---|---|
+|username|string|
+|payload|object|
+
+## updateLocationFavoritesAllUsers(payload)
+> Assign Location Favorites to a user. To Assign favorites the "favorite" column should be set to true. To Unassign favorites the "favorite" column should be set to false. Returns JSON entity containing all Location Favorites for the specified users.
+```
+PUT api/v2/users/favorites payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## searchCabinetSpace(payload)
+> Find Cabinets with available space based on RUs within the specified Locations.
+```
+POST api/v2/capacity/cabinets/list/search payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## searchAvailableRUs(payload)
+> Find the starting RUs within a Cabinet with the specified number of contiguous RUs.
+```
+POST api/v2/items/uposition/available payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
```

### Comparing `dctrackclient-0.7.0/PKG-INFO` & `dctrackclient-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.7.0
+Version: 0.7.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.7.0
+pip install dcTrackClient==0.7.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.7.0
+npm i dctrackclient@0.7.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -672,7 +672,60 @@
 > Deletes the given sub-location. The locationId is the ID of the location that the sub-location belongs to and the subLocationId is the ID of the location you are querying. Returns a success message upon success.
 ```
 DELETE api/v2/subLocations/{subLocationId}
 ```
 |Parameter|Type|
 |---|---|
 |subLocationId|number|
+
+## getLocationFavorites(username)
+> Retrieve a List of Location Favorites for a specific User.
+```
+GET api/v2/users/{username}/favorites/LOCATION
+```
+|Parameter|Type|
+|---|---|
+|username|string|
+
+## getLocationFavoritesAllUsers()
+> Retrieve a List of Location Favorites for all Users. Returns JSON entity containing Location Favorite information for all users.
+```
+GET api/v2/users/favorites/LOCATION
+```
+*No parameters.*
+
+## updateLocationFavorites(username, payload)
+> Assign Location Favorites to a user where username is a valid dcTrack user and "favorite" is either true or false to indicate whether you are assigning or unassigning. JSON entity containing all Location Favorites for the specified user.
+```
+PUT api/v2/users/{username}/favorites payload
+```
+|Parameter|Type|
+|---|---|
+|username|string|
+|payload|object|
+
+## updateLocationFavoritesAllUsers(payload)
+> Assign Location Favorites to a user. To Assign favorites the "favorite" column should be set to true. To Unassign favorites the "favorite" column should be set to false. Returns JSON entity containing all Location Favorites for the specified users.
+```
+PUT api/v2/users/favorites payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## searchCabinetSpace(payload)
+> Find Cabinets with available space based on RUs within the specified Locations.
+```
+POST api/v2/capacity/cabinets/list/search payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## searchAvailableRUs(payload)
+> Find the starting RUs within a Cabinet with the specified number of contiguous RUs.
+```
+POST api/v2/items/uposition/available payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
```

