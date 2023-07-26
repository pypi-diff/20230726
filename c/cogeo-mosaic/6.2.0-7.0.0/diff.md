# Comparing `tmp/cogeo_mosaic-6.2.0.tar.gz` & `tmp/cogeo_mosaic-7.0.0.tar.gz`

## Comparing `cogeo_mosaic-6.2.0.tar` & `cogeo_mosaic-7.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/CHANGES.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/README.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/cache.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/errors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/logger.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/models.py
--rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/mosaic.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/utils.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/az.py
--rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/base.py
--rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/dynamodb.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/file.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/gs.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/memory.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/s3.py
--rw-r--r--   0        0        0    14051 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/sqlite.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/stac.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/utils.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/backends/web.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/scripts/__init__.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/cogeo_mosaic/scripts/cli.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/LICENSE
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/pyproject.toml
--rw-r--r--   0        0        0    17439 2020-02-02 00:00:00.000000 cogeo_mosaic-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/CHANGES.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/__init__.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/cache.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/errors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/logger.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/models.py
+-rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/mosaic.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/utils.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/__init__.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/az.py
+-rw-r--r--   0        0        0    13809 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/base.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/dynamodb.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/file.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/gs.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/memory.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/s3.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/sqlite.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/stac.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/utils.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/backends/web.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/scripts/__init__.py
+-rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/cogeo_mosaic/scripts/cli.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/LICENSE
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 cogeo_mosaic-7.0.0/PKG-INFO
```

### Comparing `cogeo_mosaic-6.2.0/CHANGES.md` & `cogeo_mosaic-7.0.0/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 
+## 7.0.0 (2023-07-26)
+
+* update `morecantile` requirement to `>=5.0,<6.0`
+* update `rio-tiler` requirement to `>=6.0,<7.0`
+* update `pydantic` requirement to `~=2.0`
+
 ## 6.2.0 (2023-07-11)
 
 * add `coord_crs` to `MosaicBackend.point()` method
 
 ## 6.1.0 (2023-07-11)
 
 * add `tilematrixset` in `MosaicBackend.info()` response
```

### Comparing `cogeo_mosaic-6.2.0/CONTRIBUTING.md` & `cogeo_mosaic-7.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/README.md` & `cogeo_mosaic-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/cache.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """cogeo-mosaic cache configuration"""
 
-import pydantic
+from pydantic import model_validator
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
-class CacheSettings(pydantic.BaseSettings):
+class CacheSettings(BaseSettings):
     """Application settings"""
 
     # TTL of the cache in seconds
     ttl: int = 300
 
     # Maximum size of the LRU cache in MB
     maxsize: int = 512
 
     # Whether or not caching is enabled
     disable: bool = False
 
-    class Config:
-        """model config"""
+    model_config = SettingsConfigDict(env_prefix="COGEO_MOSAIC_CACHE_")
 
-        env_prefix = "COGEO_MOSAIC_CACHE_"
-
-    @pydantic.root_validator
+    @model_validator(mode="before")
     def check_enable(cls, values):
-        """Check if cache is desabled."""
+        """Check if cache is disabled."""
         if values.get("disable"):
             values["ttl"] = 0
             values["maxsize"] = 0
+
         return values
 
 
 cache_config = CacheSettings()
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/errors.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/errors.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/mosaic.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/mosaic.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import warnings
 from contextlib import ExitStack
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple
 
 import click
 import morecantile
-from pydantic import BaseModel, Field, root_validator, validator
+from pydantic import BaseModel, Field, field_validator, model_validator
 from shapely import linearrings, polygons, total_bounds
 from shapely.strtree import STRtree
 from supermorecado import burnTiles
 
 from cogeo_mosaic.errors import MosaicError, MultipleDataTypeError
 from cogeo_mosaic.utils import _intersect_percent, get_footprints
 
@@ -53,66 +53,59 @@
 
     if maximum_items_per_tile:
         indices = indices[:maximum_items_per_tile]
 
     return [dataset[ind] for ind in indices]
 
 
-class MosaicJSON(BaseModel):
+class MosaicJSON(BaseModel, validate_assignment=True):
     """MosaicJSON model.
 
     Based on https://github.com/developmentseed/mosaicjson-spec
 
     """
 
     mosaicjson: str
-    name: Optional[str]
-    description: Optional[str]
+    name: Optional[str] = None
+    description: Optional[str] = None
     version: str = "1.0.0"
-    attribution: Optional[str]
+    attribution: Optional[str] = None
     minzoom: int = Field(0, ge=0, le=30)
     maxzoom: int = Field(30, ge=0, le=30)
-    quadkey_zoom: Optional[int]
+    quadkey_zoom: Optional[int] = None
     bounds: Tuple[float, float, float, float] = Field(default=(-180, -90, 180, 90))
-    center: Optional[Tuple[float, float, int]]
+    center: Optional[Tuple[float, float, int]] = None
     tiles: Dict[str, List[str]]
-    tilematrixset: Optional[morecantile.TileMatrixSet]
-    asset_type: Optional[str]
-    asset_prefix: Optional[str]
-    data_type: Optional[str]
-    colormap: Optional[Dict[int, Tuple[int, int, int, int]]]
-    layers: Optional[Dict]
+    tilematrixset: Optional[morecantile.TileMatrixSet] = None
+    asset_type: Optional[str] = None
+    asset_prefix: Optional[str] = None
+    data_type: Optional[str] = None
+    colormap: Optional[Dict[int, Tuple[int, int, int, int]]] = None
+    layers: Optional[Dict] = None
 
-    class Config:
-        """Validate model on update."""
-
-        validate_assignment = True
-
-    @validator("tilematrixset", pre=True, always=True)
+    @field_validator("tilematrixset")
     def parse_tms(cls, value) -> Optional[morecantile.TileMatrixSet]:
         """Parse TMS."""
-        if isinstance(value, dict):
-            value = morecantile.TileMatrixSet(**value)
-
         if value:
-            assert value._is_quadtree, f"{value.id} TMS does not support quadtree."
+            value = morecantile.TileMatrixSet.model_validate(value)
+            assert value.is_quadtree, f"{value.id} TMS does not support quadtree."
 
         return value
 
-    @root_validator
-    def compute_center(cls, values):
+    @model_validator(mode="after")
+    def compute_center(self):
         """Compute center if it does not exist."""
-        bounds = values["bounds"]
-        if not values.get("center"):
-            values["center"] = (
+        bounds = self.bounds
+        if not self.center:
+            self.center = (
                 (bounds[0] + bounds[2]) / 2,
                 (bounds[1] + bounds[3]) / 2,
-                values["minzoom"],
+                self.minzoom,
             )
-        return values
+        return self
 
     def _increase_version(self):
         """Increment mosaicjson document version."""
         version = list(map(int, self.version.split(".")))
         version[-1] += 1
         new_version = ".".join(map(str, version))
         self.version = new_version
@@ -154,15 +147,15 @@
 
         Examples:
             >>> MosaicJSON._create_mosaic([], 12, 14)
 
         """
         tms = tilematrixset or WEB_MERCATOR_TMS
 
-        assert tms._is_quadtree, f"{tms.id} TMS does not support quadtree."
+        assert tms.is_quadtree, f"{tms.id} TMS does not support quadtree."
 
         quadkey_zoom = quadkey_zoom or minzoom
 
         if not quiet:
             click.echo(f"Get quadkey list for zoom: {quadkey_zoom}", err=True)
 
         dataset_geoms = polygons(
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/utils.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/utils.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/__init__.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/az.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/az.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         super().__attrs_post_init__()
 
     def write(self, overwrite: bool = False, **kwargs: Any):
         """Write mosaicjson document to Azure Blob Storage."""
         if not overwrite and self._head_object(self.key, self.container):
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        mosaic_doc = self.mosaic_def.json(exclude_none=True)
+        mosaic_doc = self.mosaic_def.model_dump_json(exclude_none=True)
         if self.key.endswith(".gz"):
             body = _compress_gz_json(mosaic_doc)
         else:
             body = mosaic_doc.encode("utf-8")
 
         self._put_object(self.key, self.container, body, **kwargs)
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/base.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             (self.bounds[1] + self.bounds[3]) / 2,
             self.minzoom,
         )
 
     @property
     def mosaicid(self) -> str:
         """Return sha224 id of the mosaicjson document."""
-        return get_hash(**self.mosaic_def.dict(exclude_none=True))
+        return get_hash(**self.mosaic_def.model_dump(exclude_none=True))
 
     @property
     def _quadkeys(self) -> List[str]:
         """Return the list of quadkey tiles."""
         return list(self.mosaic_def.tiles)
 
     @property
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/dynamodb.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,17 @@
             self.delete()
 
         items: List[Dict[str, Any]] = []
 
         # Create Metadata item
         # Note: `parse_float=Decimal` is required because DynamoDB requires all numbers to be
         # in Decimal type (ref: https://blog.ruanbekker.com/blog/2019/02/05/convert-float-to-decimal-data-types-for-boto3-dynamodb-using-python/)
-        meta = json.loads(self.mosaic_def.json(exclude={"tiles"}), parse_float=Decimal)
+        meta = json.loads(
+            self.mosaic_def.model_dump_json(exclude={"tiles"}), parse_float=Decimal
+        )
         items.append(
             {"quadkey": self._metadata_quadkey, "mosaicId": self.mosaic_name, **meta}
         )
 
         # Create Tile items
         for quadkey, assets in self.mosaic_def.tiles.items():
             items.append(
@@ -190,15 +192,17 @@
         self.bounds = bounds
 
         items: List[Dict[str, Any]] = []
 
         # Create Metadata item
         # Note: `parse_float=Decimal` is required because DynamoDB requires all numbers to be
         # in Decimal type (ref: https://blog.ruanbekker.com/blog/2019/02/05/convert-float-to-decimal-data-types-for-boto3-dynamodb-using-python/)
-        meta = json.loads(self.mosaic_def.json(exclude={"tiles"}), parse_float=Decimal)
+        meta = json.loads(
+            self.mosaic_def.model_dump_json(exclude={"tiles"}), parse_float=Decimal
+        )
         items.append(
             {"quadkey": self._metadata_quadkey, "mosaicId": self.mosaic_name, **meta}
         )
 
         # Create Tile items
         for quadkey, new_assets in new_mosaic.tiles.items():
             mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/file.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     _backend_name = "File"
 
     def write(self, overwrite: bool = False):
         """Write mosaicjson document to a file."""
         if not overwrite and pathlib.Path(self.input).exists():
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        body = self.mosaic_def.json(exclude_none=True)
+        body = self.mosaic_def.model_dump_json(exclude_none=True)
         with open(self.input, "wb") as f:
             try:
                 if self.input.endswith(".gz"):
                     f.write(_compress_gz_json(body))
                 else:
                     f.write(body.encode("utf-8"))
             except Exception as e:
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/gs.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/gs.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         super().__attrs_post_init__()
 
     def write(self, overwrite: bool = False, **kwargs: Any):
         """Write mosaicjson document to Google Cloud Storage."""
         if not overwrite and self._head_object(self.key, self.bucket):
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        mosaic_doc = self.mosaic_def.json(exclude_none=True)
+        mosaic_doc = self.mosaic_def.model_dump_json(exclude_none=True)
         if self.key.endswith(".gz"):
             body = _compress_gz_json(mosaic_doc)
         else:
             body = mosaic_doc.encode("utf-8")
 
         self._put_object(self.key, self.bucket, body, **kwargs)
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/memory.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/memory.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/s3.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         super().__attrs_post_init__()
 
     def write(self, overwrite: bool = False, **kwargs: Any):
         """Write mosaicjson document to AWS S3."""
         if not overwrite and self._head_object(self.key, self.bucket):
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        mosaic_doc = self.mosaic_def.json(exclude_none=True)
+        mosaic_doc = self.mosaic_def.model_dump_json(exclude_none=True)
         if self.key.endswith(".gz"):
             body = _compress_gz_json(mosaic_doc)
         else:
             body = mosaic_doc.encode("utf-8")
 
         self._put_object(self.key, self.bucket, body, **kwargs)
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/sqlite.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                         :asset_type,
                         :asset_prefix,
                         :data_type,
                         :colormap,
                         :layers
                     );
                 """,
-                self.mosaic_def.dict(exclude={"tiles"}),
+                self.mosaic_def.model_dump(exclude={"tiles"}),
             )
 
             self.db.executemany(
                 f'INSERT INTO "{self.mosaic_name}" (quadkey, assets) VALUES (?, ?);',
                 self.mosaic_def.tiles.items(),
             )
 
@@ -267,15 +267,15 @@
                         asset_type = :asset_type,
                         asset_prefix = :asset_prefix,
                         data_type = :data_type,
                         colormap = :colormap,
                         layers = :layers
                     WHERE name=:name
                 """,
-                self.mosaic_def.dict(exclude={"tiles"}),
+                self.mosaic_def.model_dump(exclude={"tiles"}),
             )
 
             if add_first:
                 self.db.executemany(
                     f"""
                         UPDATE "{self.mosaic_name}"
                         SET assets = (
```

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/stac.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/stac.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/utils.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/utils.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/backends/web.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/backends/web.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/cogeo_mosaic/scripts/cli.py` & `cogeo_mosaic-7.0.0/cogeo_mosaic/scripts/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     if attribution:
         mosaicjson.attribution = attribution
 
     if output:
         with MosaicBackend(output, mosaic_def=mosaicjson) as mosaic:
             mosaic.write(overwrite=True)
     else:
-        click.echo(mosaicjson.json(exclude_none=True))
+        click.echo(mosaicjson.model_dump_json(exclude_none=True))
 
 
 @cogeo_cli.command(short_help="Upload mosaic definition to backend")
 @click.argument("file", type=click.File(mode="r"), default="-")
 @click.option(
     "--url", type=str, required=True, help="URL to which the mosaic should be uploaded."
 )
@@ -178,15 +178,15 @@
     if attribution:
         mosaicjson.attribution = attribution
 
     if output:
         with MosaicBackend(output, mosaic_def=mosaicjson) as mosaic:
             mosaic.write(overwrite=True)
     else:
-        click.echo(mosaicjson.json(exclude_none=True))
+        click.echo(mosaicjson.model_dump_json(exclude_none=True))
 
 
 @cogeo_cli.command(short_help="Update a mosaic definition from list of files")
 @click.argument("input_files", type=click.File(mode="r"), default="-")
 @click.argument("input_mosaic", type=click.Path())
 @click.option("--min-tile-cover", type=float, help="Minimum % overlap")
 @click.option(
```

### Comparing `cogeo_mosaic-6.2.0/.gitignore` & `cogeo_mosaic-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/LICENSE` & `cogeo_mosaic-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.2.0/pyproject.toml` & `cogeo_mosaic-7.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,21 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version", "readme"]
 dependencies = [
   "attrs",
-  "morecantile>=4.1,<5.0",
+  "morecantile>=5.0,<6.0",
   "shapely>=2.0,<3.0",
-  "pydantic~=1.0",
+  "pydantic~=2.0",
+  "pydantic-settings~=2.0",
   "httpx",
   "rasterio",
-  "rio-tiler>=5.0,<6.0",
+  "rio-tiler>=6.0,<7.0",
   "supermorecado",
   "cachetools",
 ]
 
 [project.optional-dependencies]
 aws = [
   "boto3",
```

### Comparing `cogeo_mosaic-6.2.0/PKG-INFO` & `cogeo_mosaic-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogeo-mosaic
-Version: 6.2.0
+Version: 7.0.0
 Summary: CLI and Backends to work with MosaicJSON.
 Project-URL: Homepage, https://github.com/developmentseed/cogeo-mosaic
 Project-URL: Documentation, https://developmentseed.org/cogeo-mosaic/
 Project-URL: Issues, https://github.com/developmentseed/cogeo-mosaic/issues
 Project-URL: Source, https://github.com/developmentseed/cogeo-mosaic
 Project-URL: Changelog, https://developmentseed.org/cogeo-mosaic/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
@@ -41,18 +41,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: cachetools
 Requires-Dist: httpx
-Requires-Dist: morecantile<5.0,>=4.1
-Requires-Dist: pydantic~=1.0
+Requires-Dist: morecantile<6.0,>=5.0
+Requires-Dist: pydantic-settings~=2.0
+Requires-Dist: pydantic~=2.0
 Requires-Dist: rasterio
-Requires-Dist: rio-tiler<6.0,>=5.0
+Requires-Dist: rio-tiler<7.0,>=6.0
 Requires-Dist: shapely<3.0,>=2.0
 Requires-Dist: supermorecado
 Provides-Extra: aws
 Requires-Dist: boto3; extra == 'aws'
 Provides-Extra: az
 Requires-Dist: azure-identity; extra == 'az'
 Requires-Dist: azure-storage-blob; extra == 'az'
@@ -142,14 +143,20 @@
 Created by [Development Seed](<http://developmentseed.org>)
 
 See [contributors](https://github.com/developmentseed/cogeo-mosaic/graphs/contributors) for a listing of individual contributors.
 
 ## Changelog
 
 
+## 7.0.0 (2023-07-26)
+
+* update `morecantile` requirement to `>=5.0,<6.0`
+* update `rio-tiler` requirement to `>=6.0,<7.0`
+* update `pydantic` requirement to `~=2.0`
+
 ## 6.2.0 (2023-07-11)
 
 * add `coord_crs` to `MosaicBackend.point()` method
 
 ## 6.1.0 (2023-07-11)
 
 * add `tilematrixset` in `MosaicBackend.info()` response
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cogeo-mosaic Version: 6.2.0 Summary: CLI and
+Metadata-Version: 2.1 Name: cogeo-mosaic Version: 7.0.0 Summary: CLI and
 Backends to work with MosaicJSON. Project-URL: Homepage, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Documentation, https://
 developmentseed.org/cogeo-mosaic/ Project-URL: Issues, https://github.com/
 developmentseed/cogeo-mosaic/issues Project-URL: Source, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Changelog, https://
 developmentseed.org/cogeo-mosaic/release-notes/ Author-email: Vincent Sarago
 developmentseed.com> License: MIT License Copyright (c) 2019 Development Seed
@@ -24,27 +24,27 @@
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS Requires-Python: >=3.8
 Requires-Dist: attrs Requires-Dist: cachetools Requires-Dist: httpx Requires-
-Dist: morecantile<5.0,>=4.1 Requires-Dist: pydantic~=1.0 Requires-Dist:
-rasterio Requires-Dist: rio-tiler<6.0,>=5.0 Requires-Dist: shapely<3.0,>=2.0
-Requires-Dist: supermorecado Provides-Extra: aws Requires-Dist: boto3; extra ==
-'aws' Provides-Extra: az Requires-Dist: azure-identity; extra == 'az' Requires-
-Dist: azure-storage-blob; extra == 'az' Provides-Extra: dev Requires-Dist: pre-
-commit; extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist:
-pytest-cov; extra == 'dev' Provides-Extra: docs Requires-Dist: mkdocs; extra ==
-'docs' Requires-Dist: mkdocs-jupyter; extra == 'docs' Requires-Dist: mkdocs-
-material; extra == 'docs' Requires-Dist: pygments; extra == 'docs' Provides-
-Extra: gcp Requires-Dist: google-cloud-storage; extra == 'gcp' Provides-Extra:
-test Requires-Dist: boto3; extra == 'test' Requires-Dist: pytest; extra ==
-'test' Requires-Dist: pytest-cov; extra == 'test' Description-Content-Type:
-text/markdown # cogeo-mosaic
+Dist: morecantile<6.0,>=5.0 Requires-Dist: pydantic-settings~=2.0 Requires-
+Dist: pydantic~=2.0 Requires-Dist: rasterio Requires-Dist: rio-tiler<7.0,>=6.0
+Requires-Dist: shapely<3.0,>=2.0 Requires-Dist: supermorecado Provides-Extra:
+aws Requires-Dist: boto3; extra == 'aws' Provides-Extra: az Requires-Dist:
+azure-identity; extra == 'az' Requires-Dist: azure-storage-blob; extra == 'az'
+Provides-Extra: dev Requires-Dist: pre-commit; extra == 'dev' Requires-Dist:
+pytest; extra == 'dev' Requires-Dist: pytest-cov; extra == 'dev' Provides-
+Extra: docs Requires-Dist: mkdocs; extra == 'docs' Requires-Dist: mkdocs-
+jupyter; extra == 'docs' Requires-Dist: mkdocs-material; extra == 'docs'
+Requires-Dist: pygments; extra == 'docs' Provides-Extra: gcp Requires-Dist:
+google-cloud-storage; extra == 'gcp' Provides-Extra: test Requires-Dist: boto3;
+extra == 'test' Requires-Dist: pytest; extra == 'test' Requires-Dist: pytest-
+cov; extra == 'test' Description-Content-Type: text/markdown # cogeo-mosaic
                                   [rio-tiler]
        Create mosaics of Cloud Optimized GeoTIFF based on the mosaicJSON
                                 specification.
           [Test] [Coverage] [Package_version] [Downloads] [Downloads]
 --- **Documentation**: https://developmentseed.org/cogeo-mosaic/ **Source
 Code**: https://github.com/developmentseed/cogeo-mosaic --- **Read the official
 announcement https://medium.com/devseed/cog-talk-part-2-mosaics-bbbf474e66df**
@@ -57,41 +57,44 @@
 developmentseed/titiler): A lightweight Cloud Optimized GeoTIFF dynamic tile
 server (COG, STAC and MosaicJSON). ## Contribution & Development See
 [CONTRIBUTING.md](https://github.com/developmentseed/cogeo-mosaic/blob/master/
 CONTRIBUTING.md) ## License See [LICENSE](https://github.com/developmentseed/
 cogeo-mosaic/blob/master/LICENSE) ## Authors Created by [Development Seed](
 developmentseed.org>) See [contributors](https://github.com/developmentseed/
 cogeo-mosaic/graphs/contributors) for a listing of individual contributors. ##
-Changelog ## 6.2.0 (2023-07-11) * add `coord_crs` to `MosaicBackend.point()`
-method ## 6.1.0 (2023-07-11) * add `tilematrixset` in `MosaicBackend.info()`
-response ## 6.0.1 (2023-07-11) * fix `HttpBackend` post_init method ## 6.0.0
-(2023-07-10) * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0`
-requirements * replace `supermercado` with [`supermorecado`](https://
-github.com/developmentseed/supermorecado) to burn geometries as tiles for
-different TMS * update MosaicJSON models to `0.0.3` specification (adds
-`tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and
-`layers` attributes) * allow Mosaic creation using other TileMatrixSet (default
-is still `WebMercatorQuad`) * add `tms` support to MosaicBackend to read tile
-in other TMS than the mosaic TileMatrixSet ```python # Before # Mosaic and
-output Tile in WebMercatorQuad with MosaicBackend("mosaic.json") as mosaic:
-img, _ = mosaic.tile(0, 0, 0) # Now # Mosaic in WebMercatorQuad (default),
-output tile in WGS84 WGS1984Quad = morecantile.tms.get("WGS1984Quad") with
-MosaicBackend("mosaic.json", tms=WGS1984Quad) as mosaic: img, _ = mosaic.tile
-(0, 0, 0) ``` ## 5.1.1 (2023-02-06) * Clip dataset bounds with of TMS bbox
-(author [@lseelenbinder](https://github.com/lseelenbinder), https://github.com/
-developmentseed/cogeo-mosaic/pull/200) ## 5.1.0 (2023-01-20) * use `az://
-` prefix for private Azure Blob Storage Backend. ## 5.0.0 (2022-11-21) * switch
-from pygeos to shapely>=2.0 ## 4.2.2 (2022-11-19) * remove useless file in
-package ## 4.2.1 (2022-11-15) * add python 3.11 support ## 4.2.0 (2022-10-24) *
-remove python 3.7 support * add python 3.10 support * switch to hatch build-
-system * update rio-tiler dependency to >=4.0.0a0 ## 4.1.1 (2022-10-21) * Add
-Azure Blob Storage backend (author [@christoe](https://github.com/christoe),
-https://github.com/developmentseed/cogeo-mosaic/pull/191) ## 4.1.0 (2022-02-22)
-* remove `mercantile` and switch to morecantile>=3.1 ## 4.0.0 (2021-11-30) * no
-change since `4.0.0a2` ## 4.0.0a2 (2021-11-22) * update rio-tiler requirement
+Changelog ## 7.0.0 (2023-07-26) * update `morecantile` requirement to
+`>=5.0,<6.0` * update `rio-tiler` requirement to `>=6.0,<7.0` * update
+`pydantic` requirement to `~=2.0` ## 6.2.0 (2023-07-11) * add `coord_crs` to
+`MosaicBackend.point()` method ## 6.1.0 (2023-07-11) * add `tilematrixset` in
+`MosaicBackend.info()` response ## 6.0.1 (2023-07-11) * fix `HttpBackend`
+post_init method ## 6.0.0 (2023-07-10) * update `morecantile>=4.1,<5.0` and
+`rio-tiler>=5.0,<6.0` requirements * replace `supermercado` with
+[`supermorecado`](https://github.com/developmentseed/supermorecado) to burn
+geometries as tiles for different TMS * update MosaicJSON models to `0.0.3`
+specification (adds `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`,
+`colormap` and `layers` attributes) * allow Mosaic creation using other
+TileMatrixSet (default is still `WebMercatorQuad`) * add `tms` support to
+MosaicBackend to read tile in other TMS than the mosaic TileMatrixSet ```python
+# Before # Mosaic and output Tile in WebMercatorQuad with MosaicBackend
+("mosaic.json") as mosaic: img, _ = mosaic.tile(0, 0, 0) # Now # Mosaic in
+WebMercatorQuad (default), output tile in WGS84 WGS1984Quad =
+morecantile.tms.get("WGS1984Quad") with MosaicBackend("mosaic.json",
+tms=WGS1984Quad) as mosaic: img, _ = mosaic.tile(0, 0, 0) ``` ## 5.1.1 (2023-
+02-06) * Clip dataset bounds with of TMS bbox (author [@lseelenbinder](https://
+github.com/lseelenbinder), https://github.com/developmentseed/cogeo-mosaic/
+pull/200) ## 5.1.0 (2023-01-20) * use `az://` prefix for private Azure Blob
+Storage Backend. ## 5.0.0 (2022-11-21) * switch from pygeos to shapely>=2.0 ##
+4.2.2 (2022-11-19) * remove useless file in package ## 4.2.1 (2022-11-15) * add
+python 3.11 support ## 4.2.0 (2022-10-24) * remove python 3.7 support * add
+python 3.10 support * switch to hatch build-system * update rio-tiler
+dependency to >=4.0.0a0 ## 4.1.1 (2022-10-21) * Add Azure Blob Storage backend
+(author [@christoe](https://github.com/christoe), https://github.com/
+developmentseed/cogeo-mosaic/pull/191) ## 4.1.0 (2022-02-22) * remove
+`mercantile` and switch to morecantile>=3.1 ## 4.0.0 (2021-11-30) * no change
+since `4.0.0a2` ## 4.0.0a2 (2021-11-22) * update rio-tiler requirement
 (`>=3.0.0a6`) and update backend reader type information ## 4.0.0a1 (2021-11-
 18) * update rio-tiler requirement (`>=3.0.0a5`) * fix `MosaicBackend` to match
 Backend input names. ## 4.0.0a0 (2021-10-20) * update morecantile requirement
 to >= 3.0 * update rio-tiler requirement to >= 3.0 and update Backend's
 properties * switch from `requests` to `httpx` * add
 `BaseBackend.assets_for_bbox()` method (https://github.com/developmentseed/
 cogeo-mosaic/pull/184) **breaking changes** * remove `BaseBackend.metadata()`
```

