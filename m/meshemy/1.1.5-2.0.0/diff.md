# Comparing `tmp/meshemy-1.1.5.tar.gz` & `tmp/meshemy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshemy-1.1.5.tar", max compression
+gzip compressed data, was "meshemy-2.0.0.tar", max compression
```

## Comparing `meshemy-1.1.5.tar` & `meshemy-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1658 2023-03-02 12:06:03.949633 meshemy-1.1.5/LICENSE.md
--rw-r--r--   0        0        0     1318 2023-03-21 18:29:58.083024 meshemy-1.1.5/README.md
--rw-r--r--   0        0        0        0 2023-01-31 11:28:29.915526 meshemy-1.1.5/meshemy/__init__.py
--rw-r--r--   0        0        0      169 2023-03-02 12:06:03.950633 meshemy-1.1.5/meshemy/blender/__init__.py
--rw-r--r--   0        0        0      667 2023-02-01 16:09:27.499584 meshemy-1.1.5/meshemy/blender/constant.py
--rw-r--r--   0        0        0        0 2023-02-01 12:56:17.229830 meshemy-1.1.5/meshemy/blender/shortcut/__init__.py
--rw-r--r--   0        0        0      552 2023-02-08 10:43:11.259003 meshemy-1.1.5/meshemy/blender/shortcut/io.py
--rw-r--r--   0        0        0      766 2023-03-28 15:12:37.356681 meshemy-1.1.5/meshemy/blender/shortcut/select.py
--rw-r--r--   0        0        0     1262 2023-03-28 15:15:20.593671 meshemy-1.1.5/meshemy/blender/utils.py
--rw-r--r--   0        0        0      819 2023-03-28 15:12:37.359681 meshemy-1.1.5/meshemy/blender/workflows.py
--rw-r--r--   0        0        0        0 2023-01-31 12:08:37.561267 meshemy-1.1.5/meshemy/cookbook/__init__.py
--rw-r--r--   0        0        0     3599 2023-03-27 14:49:58.734912 meshemy-1.1.5/meshemy/cookbook/base.py
--rw-r--r--   0        0        0     2884 2023-03-21 18:29:58.084024 meshemy-1.1.5/meshemy/cookbook/blender.py
--rw-r--r--   0        0        0     2186 2023-03-21 18:29:58.084024 meshemy-1.1.5/meshemy/cookbook/open3d.py
--rw-r--r--   0        0        0     1535 2023-03-21 18:29:58.084024 meshemy-1.1.5/meshemy/cookbook/trimesh.py
--rw-r--r--   0        0        0        0 2023-01-31 12:10:55.639252 meshemy-1.1.5/meshemy/utility/__init__.py
--rw-r--r--   0        0        0     1199 2023-03-21 18:29:58.084024 meshemy-1.1.5/meshemy/utility/exception.py
--rw-r--r--   0        0        0      315 2023-01-31 14:37:28.643307 meshemy-1.1.5/meshemy/utility/io.py
--rw-r--r--   0        0        0      202 2023-02-01 14:40:31.236157 meshemy-1.1.5/meshemy/utility/seal.py
--rw-r--r--   0        0        0      933 2023-03-28 15:12:52.577680 meshemy-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 meshemy-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1658 2023-02-23 18:11:12.531986 meshemy-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     1318 2023-03-19 09:10:13.702858 meshemy-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-23 16:53:18.843654 meshemy-2.0.0/meshemy/__init__.py
+-rw-r--r--   0        0        0      169 2023-02-23 17:51:35.073971 meshemy-2.0.0/meshemy/blender/__init__.py
+-rw-r--r--   0        0        0      667 2023-02-23 16:53:18.843654 meshemy-2.0.0/meshemy/blender/constant.py
+-rw-r--r--   0        0        0        0 2023-02-23 16:53:18.843654 meshemy-2.0.0/meshemy/blender/shortcut/__init__.py
+-rw-r--r--   0        0        0     1493 2023-07-26 18:08:04.363115 meshemy-2.0.0/meshemy/blender/shortcut/io.py
+-rw-r--r--   0        0        0      955 2023-07-26 18:08:04.363115 meshemy-2.0.0/meshemy/blender/shortcut/select.py
+-rw-r--r--   0        0        0     1269 2023-07-26 18:08:04.363115 meshemy-2.0.0/meshemy/blender/utils.py
+-rw-r--r--   0        0        0     2236 2023-07-26 18:08:04.363115 meshemy-2.0.0/meshemy/blender/workflows.py
+-rw-r--r--   0        0        0        0 2023-02-23 16:53:18.844654 meshemy-2.0.0/meshemy/cookbook/__init__.py
+-rw-r--r--   0        0        0     3527 2023-07-26 18:08:04.363115 meshemy-2.0.0/meshemy/cookbook/base.py
+-rw-r--r--   0        0        0     4772 2023-07-26 18:08:04.364115 meshemy-2.0.0/meshemy/cookbook/blender.py
+-rw-r--r--   0        0        0     2669 2023-07-26 18:08:04.364115 meshemy-2.0.0/meshemy/cookbook/open3d.py
+-rw-r--r--   0        0        0     2050 2023-07-26 18:08:04.364115 meshemy-2.0.0/meshemy/cookbook/trimesh.py
+-rw-r--r--   0        0        0        0 2023-02-23 16:53:18.845654 meshemy-2.0.0/meshemy/utility/__init__.py
+-rw-r--r--   0        0        0     1202 2023-07-26 18:08:04.364115 meshemy-2.0.0/meshemy/utility/exception.py
+-rw-r--r--   0        0        0      356 2023-07-26 18:08:04.364115 meshemy-2.0.0/meshemy/utility/io.py
+-rw-r--r--   0        0        0      966 2023-07-26 18:08:04.365116 meshemy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 meshemy-2.0.0/PKG-INFO
```

### Comparing `meshemy-1.1.5/LICENSE.md` & `meshemy-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `meshemy-1.1.5/README.md` & `meshemy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `meshemy-1.1.5/meshemy/blender/constant.py` & `meshemy-2.0.0/meshemy/blender/constant.py`

 * *Files identical despite different names*

### Comparing `meshemy-1.1.5/meshemy/cookbook/base.py` & `meshemy-2.0.0/meshemy/cookbook/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,85 @@
 import logging
 from abc import ABC, abstractmethod
-from functools import cached_property
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, Generic, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Generic, TypeVar, Union
 
+import pymeshfix
 from pydantic import BaseModel, FilePath
-from pydantic.generics import GenericModel
-from pydantic_numpy import NDArray, NDArrayFp64
-
-from meshemy.utility.seal import seal_mesh
+from pydantic_numpy import NpNDArray
+from pydantic_numpy.typing import NpNDArrayFp64
 
 if TYPE_CHECKING:
     from meshemy.cookbook.blender import BlenderCookbook
     from meshemy.cookbook.open3d import Open3dCookbook
     from meshemy.cookbook.trimesh import TrimeshCookbook
 
 logger = logging.getLogger(__file__)
 
 
-class BaseCookbook(BaseModel, ABC):
+class BaseCookbook(BaseModel, ABC, arbitrary_types_allowed=True):   # type: ignore[call-arg]
     """
     The .from_data() and .from_file() class method also needs to be implemented, I did not make it an abstractmethod
-    because each Cookbook has its own function signature.
+    because each BaseCookbook has its own function signature.
     """
 
-    class Config:
-        arbitrary_types_allowed = True
-        keep_untouched = (cached_property,)
-
     @property
     @abstractmethod
-    def vertices_numpy_array(self) -> NDArrayFp64 | None:
+    def vertices_numpy_array(self) -> NpNDArrayFp64 | None:
         ...
 
     @property
     @abstractmethod
-    def edges_numpy_array(self) -> NDArray | None:
+    def edges_numpy_array(self) -> NpNDArray | None:
         ...
 
     @property
     @abstractmethod
-    def faces_numpy_array(self) -> NDArray | None:
+    def faces_numpy_array(self) -> NpNDArray | None:
         ...
 
     @property
     @abstractmethod
     def watertight(self) -> bool:
         """Check if a mesh is watertight, also known as manifold"""
         ...
 
     @abstractmethod
     def save(self, save_path: Path | str) -> None:
         ...
 
-    def attempt_seal_insurance(self) -> bool:
-        # TODO: Fix crash
+    def attempt_seal(self):
         # Perform seal only if mesh is leaky, ie not watertight
         if not self.watertight:
             logger.debug("Mesh is leaky, attempting to seal mesh")
-            self.mesh = self.from_data(*seal_mesh(self.vertices_numpy_array.copy(), self.faces_numpy_array.copy()))
-            if self.mesh.is_watertight():
+            fixed_vertices, fixed_faces = pymeshfix.clean_from_arrays(
+                self.vertices_numpy_array.copy(), self.faces_numpy_array.copy(), verbose=False
+            )
+            new = self.__class__.from_data(vertices=fixed_vertices, faces=fixed_faces)
+
+            if new.is_watertight():
                 logger.debug("The seal was success!")
+                return new
             else:
                 logger.debug("Failed to seal!")
-                return False
         else:
             logger.debug("Mesh is watertight, no action performed")
-        return True
 
-    def to_blender(self, name: str) -> "BlenderCookbook":
+    def to_blender(self, name: str, **kwargs) -> "BlenderCookbook":
         from meshemy.cookbook.blender import BlenderCookbook
 
         if isinstance(self, BlenderCookbook):
             return self
 
         return BlenderCookbook.from_data(
-            self.vertices_numpy_array, self.edges_numpy_array, self.faces_numpy_array, name
+            vertices=self.vertices_numpy_array,
+            edges=self.edges_numpy_array,
+            faces=self.faces_numpy_array,
+            name=name,
+            **kwargs,
         )
 
     def to_o3d(self) -> "Open3dCookbook":
         from meshemy.cookbook.open3d import Open3dCookbook
 
         if isinstance(self, Open3dCookbook):
             return self
@@ -91,29 +91,25 @@
 
         if isinstance(self, TrimeshCookbook):
             return self
 
         return TrimeshCookbook.from_data(self.vertices_numpy_array, self.faces_numpy_array)
 
 
-Cookbook = TypeVar("Cookbook", bound=BaseCookbook)
 T = TypeVar("T")
 
 
-class MeshIsObjectMixin(GenericModel, Generic[T]):
+class MeshIsObjectMixin(BaseModel, Generic[T]):
     mesh: T
 
-    mesh_from_file_loader: ClassVar[Callable[[str], Any]] = ...
+    mesh_from_file_loader: ClassVar[Callable[[str], Any]]
 
     class Config:
         arbitrary_types_allowed = True
 
     @classmethod
-    def from_native(cls, mesh: T) -> "MeshIsObjectCookbook":
+    def from_native(cls, mesh: T) -> "MeshIsObjectMixin":
         return cls(mesh=mesh)
 
     @classmethod
-    def from_file(cls, file_path: FilePath | str) -> "MeshIsObjectCookbook":
+    def from_file(cls, file_path: FilePath | str) -> "MeshIsObjectMixin":
         return cls.from_native(mesh=cls.mesh_from_file_loader(str(file_path)))
-
-
-MeshIsObjectCookbook = TypeVar("MeshIsObjectCookbook", bound=MeshIsObjectMixin)
```

### Comparing `meshemy-1.1.5/meshemy/cookbook/blender.py` & `meshemy-2.0.0/meshemy/cookbook/open3d.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,86 @@
+from functools import cached_property
+
+from pydantic import computed_field
+from pydantic_numpy.typing import NpNDArrayFp64
+
+try:
+    import open3d as o3d
+except ModuleNotFoundError as e:
+    from meshemy.utility.exception import open3d_module_not_installed_error
+
+    open3d_module_not_installed_error(e)
+
 import logging
-from typing import Optional
+from pathlib import Path
 
-import bpy
 import numpy as np
-from bmesh.types import BMesh
-from pydantic import FilePath
-from pydantic_numpy import NDArray, NDArrayFp64
-
-from meshemy.blender.constant import SUFFIX_TO_READER, SUFFIX_TO_WRITER
-from meshemy.blender.shortcut.select import latest_mesh, select_object
-from meshemy.blender.utils import load_mesh_from_numpy_arrays, triangular_bmesh
-from meshemy.blender.workflows import merge_close, planar_decimate_mesh
-from meshemy.cookbook.base import BaseCookbook
+from pydantic_numpy import NpNDArray
 
-logger = logging.getLogger(__file__)
+from meshemy.cookbook.base import BaseCookbook, MeshIsObjectMixin
+from meshemy.utility.io import o3d_from_vertices_faces
 
+logger = logging.getLogger(__file__)
 
-class BlenderCookbook(BaseCookbook):
-    mesh_name: str
 
-    cached_bm: BMesh | None
+class Open3dCookbook(BaseCookbook, MeshIsObjectMixin[o3d.geometry.TriangleMesh]):
+    mesh_from_file_loader = o3d.io.read_triangle_mesh
 
-    def reset_bm(self) -> None:
-        self.cached_bm = None
+    @computed_field(return_type=NpNDArrayFp64 | None)  # type: ignore[misc]
+    @property
+    def vertices_numpy_array(self) -> NpNDArrayFp64 | None:
+        return np.asarray(self.mesh.vertices)
 
+    @computed_field(return_type=NpNDArray | None)  # type: ignore[misc]
     @property
-    def triangular_bmesh(self) -> BMesh:
-        if not self.cached_bm:
-            self.cached_bm = triangular_bmesh(mesh_object_name=self.mesh_name)
-        return self.cached_bm
+    def edges_numpy_array(self) -> None:
+        return None
 
+    @computed_field(return_type=NpNDArray | None)  # type: ignore[misc]
     @property
-    def vertices_numpy_array(self) -> NDArrayFp64 | None:
-        return np.array([v.co.copy() for v in self.triangular_bmesh.verts], dtype=np.float64)
+    def faces_numpy_array(self) -> NpNDArray | None:
+        return np.asarray(self.triangles)
+
+    def smoothen(self, iterations: int, copy: bool = False) -> None:
+        result = self.mesh.filter_smooth_taubin(number_of_iterations=iterations)
+        if copy:
+            self.__class__(mesh=result)
+        self.mesh = result
+
+    def repair(self) -> None:
+        self.mesh = (
+            self.mesh.remove_duplicated_triangles()
+            .remove_duplicated_vertices()
+            .remove_degenerate_triangles()
+            .remove_unreferenced_vertices()
+        )
 
+    @computed_field(return_type=NpNDArray)  # type: ignore[misc]
     @property
-    def edges_numpy_array(self) -> NDArray | None:
-        return np.array([[v.index for v in e.verts] for e in self.triangular_bmesh.edges])
+    def vertices(self) -> NpNDArray:
+        return np.asarray(self.mesh.vertices)
 
+    @computed_field(return_type=NpNDArray)  # type: ignore[misc]
     @property
-    def faces_numpy_array(self) -> NDArray | None:
-        return np.array([[v.index for v in f.verts] for f in self.triangular_bmesh.faces])
+    def faces(self) -> NpNDArray:
+        return np.asarray(self.mesh.triangles)
 
+    @computed_field(return_type=NpNDArray)  # type: ignore[misc]
     @property
+    def triangles(self) -> NpNDArray:
+        return self.faces
+
+    @cached_property
     def watertight(self) -> bool:
-        for edge in self.triangular_bmesh.edges:
-            if len(edge.link_faces) != 2:
-                return False
-        return True
-
-    def planar_decimate(self, degree_tol: float) -> None:
-        planar_decimate_mesh(degree_tol, mesh_object_name=self.mesh_name)
-        logger.debug(f"Planar decimation on {self.mesh_name}, degree tolerance {degree_tol}")
-        self.reset_bm()
-
-    def merge_close(self, distance_tol: float) -> None:
-        merge_close(distance_tol, mesh_object_name=self.mesh_name)
-        logger.debug(f"Merging proximal vertices on {self.mesh_name}, distance tolerance {distance_tol}")
-        self.reset_bm()
-
-    def save(self, path: FilePath) -> None:
-        _ob = select_object(self.mesh_name)
-        SUFFIX_TO_WRITER[path.suffix](filepath=str(path))
+        return self.mesh.is_watertight()
 
-    @classmethod
-    def from_data(
-        cls, vertices: NDArrayFp64, edges: NDArray | None, faces: NDArray | None, name: str = "new_object"
-    ) -> "BlenderCookbook":
-        load_mesh_from_numpy_arrays(vertices, edges, faces, name)
-        return cls(mesh_name=name)
+    def save(self, save_path: Path | str) -> None:
+        o3d.io.write_triangle_mesh(
+            str(save_path),
+            self.mesh,
+            write_vertex_colors=False,
+            write_triangle_uvs=False,
+        )
 
     @classmethod
-    def from_file(cls, path: FilePath, name: Optional[str] = None, **kwargs) -> "BlenderCookbook":
-        SUFFIX_TO_READER[path.suffix](filepath=str(path), **kwargs)
-        if name:
-            ob = latest_mesh()
-            ob.name = name
-            ob.data.name = name
-        else:
-            name = latest_mesh().name
-
-        return cls(mesh_name=name)
+    def from_data(cls, vertices: NpNDArrayFp64, faces: NpNDArray) -> "Open3dCookbook":
+        return cls(mesh=o3d_from_vertices_faces(vertices, faces))
```

### Comparing `meshemy-1.1.5/meshemy/utility/exception.py` & `meshemy-2.0.0/meshemy/utility/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Callable, Type
+from typing import Callable
 
 
 def _raise_not_installed_error_callable(
-    exception_class: Type[Exception], name: str, extras_name: str
-) -> Callable[[], None]:
+    exception_class: type[Exception], name: str, extras_name: str
+) -> Callable[[Exception], None]:
     def raise_not_installed_error(e: Exception) -> None:
         raise exception_class(
             f"""
             {name} module, {extras_name}, must be installed.
 
             Please run `pip install meshemy[{extras_name}]`
             """
```

### Comparing `meshemy-1.1.5/pyproject.toml` & `meshemy-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "meshemy"
-version = "1.1.5"
+version = "2.0.0"
 description = "Developer friendly suite for manipulating mesh"
 authors = ["caniko <canhtart@gmail.com>"]
 readme = "README.md"
 license = "BSD-4"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11.0"
-pydantic = "^1.10.4"
+pydantic = "^2.0"
+
+# Owned by author
 pydantic-numpy = "*"
+# ---
 
 bpy = { version = "^3.4.0", optional = true }
 open3d-cpu = { version = "^0.17.0", optional = true }
 trimesh = { version = "^3.20.2", optional = true }
 
-numpy = "<1.24.0"
+numpy = "<1.25.0"
 
 pymeshfix = "^0.16.2"
 ordered-set = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 
-bpy = "*"
-open3d-cpu = "*"
-trimesh = "*"
+[tool.poetry.group.ci.dependencies]
+mypy = "^1.4.1"
 
 [tool.poetry.extras]
 full = ["bpy", "open3d-cpu", "trimesh"]
 blender = ["bpy"]
 open3d = ["open3d-cpu"]
 trimesh = ["trimesh"]
```

### Comparing `meshemy-1.1.5/PKG-INFO` & `meshemy-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: meshemy
-Version: 1.1.5
+Version: 2.0.0
 Summary: Developer friendly suite for manipulating mesh
 License: BSD-4
 Author: caniko
 Author-email: canhtart@gmail.com
 Requires-Python: >=3.10,<3.11.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: blender
 Provides-Extra: full
 Provides-Extra: open3d
 Provides-Extra: trimesh
 Requires-Dist: bpy (>=3.4.0,<4.0.0) ; extra == "full" or extra == "blender"
-Requires-Dist: numpy (<1.24.0)
+Requires-Dist: numpy (<1.25.0)
 Requires-Dist: open3d-cpu (>=0.17.0,<0.18.0) ; extra == "full" or extra == "open3d"
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pydantic-numpy
 Requires-Dist: pymeshfix (>=0.16.2,<0.17.0)
 Requires-Dist: trimesh (>=3.20.2,<4.0.0) ; extra == "full" or extra == "trimesh"
 Description-Content-Type: text/markdown
 
 # Meshemy: Python toolbelt for manipulating mesh
 Consolidation package for manipulating mesh. Comes with cookbook models from each package
```

