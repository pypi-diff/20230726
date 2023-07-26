# Comparing `tmp/dataclass_array-1.4.2.tar.gz` & `tmp/dataclass_array-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_array-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dataclass_array-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dataclass_array-1.4.2.tar` & `dataclass_array-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/LICENSE
--rw-r--r--   0        0        0     6030 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/README.md
--rw-r--r--   0        0        0     1696 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/__init__.py
--rw-r--r--   0        0        0    38577 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/array_dataclass.py
--rw-r--r--   0        0        0      856 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/conftest.py
--rw-r--r--   0        0        0     2205 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/field_utils.py
--rw-r--r--   0        0        0     3720 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/ops.py
--rw-r--r--   0        0        0      336 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/shape_grammar.lark
--rw-r--r--   0        0        0     2906 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/shape_parsing.py
--rw-r--r--   0        0        0     2937 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/testing.py
--rw-r--r--   0        0        0     4467 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/type_parsing.py
--rw-r--r--   0        0        0     2157 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/typing.py
--rw-r--r--   0        0        0      804 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/file_utils.py
--rw-r--r--   0        0        0     7295 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/inspect_utils.py
--rw-r--r--   0        0        0     5792 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/np_utils.py
--rw-r--r--   0        0        0      845 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/py_utils.py
--rw-r--r--   0        0        0     2387 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/tree_utils.py
--rw-r--r--   0        0        0    13852 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/vectorization.py
--rw-r--r--   0        0        0     1789 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 dataclass_array-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6030 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/README.md
+-rw-r--r--   0        0        0     1696 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/__init__.py
+-rw-r--r--   0        0        0    40178 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/array_dataclass.py
+-rw-r--r--   0        0        0      856 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/conftest.py
+-rw-r--r--   0        0        0     2205 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/field_utils.py
+-rw-r--r--   0        0        0     3720 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/ops.py
+-rw-r--r--   0        0        0      336 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/shape_grammar.lark
+-rw-r--r--   0        0        0     2906 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/shape_parsing.py
+-rw-r--r--   0        0        0     2937 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/testing.py
+-rw-r--r--   0        0        0     4467 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/type_parsing.py
+-rw-r--r--   0        0        0     2157 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/typing.py
+-rw-r--r--   0        0        0      804 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/utils/file_utils.py
+-rw-r--r--   0        0        0     7444 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/utils/inspect_utils.py
+-rw-r--r--   0        0        0     5792 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/utils/np_utils.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:03:33.212824 dataclass_array-1.5.0/dataclass_array/utils/py_utils.py
+-rw-r--r--   0        0        0     2387 2023-07-26 16:03:33.216825 dataclass_array-1.5.0/dataclass_array/utils/tree_utils.py
+-rw-r--r--   0        0        0    15294 2023-07-26 16:03:33.216825 dataclass_array-1.5.0/dataclass_array/vectorization.py
+-rw-r--r--   0        0        0     1896 2023-07-26 16:03:33.216825 dataclass_array-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7591 1970-01-01 00:00:00.000000 dataclass_array-1.5.0/PKG-INFO
```

### Comparing `dataclass_array-1.4.2/LICENSE` & `dataclass_array-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/README.md` & `dataclass_array-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/__init__.py` & `dataclass_array-1.5.0/dataclass_array/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 
 # `dca.testing` do not depend on pytest or other heavy deps, so is safe to
 # import
 from dataclass_array import testing
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '1.4.2'
+__version__ = '1.5.0'
 
 del sys, pytest
```

### Comparing `dataclass_array-1.4.2/dataclass_array/array_dataclass.py` & `dataclass_array-1.5.0/dataclass_array/array_dataclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,15 +344,15 @@
       **axes_length: Any additional specifications for dimensions for einops
         support.
 
     Returns:
       The dataclass array with the new shape
     """
     if isinstance(shape, str):  # Einops support
-      return self._map_field(
+      return self._map_field(  # pylint: disable=protected-access
           array_fn=lambda f: einops.rearrange(  # pylint: disable=g-long-lambda
               f.value,
               np_utils.to_absolute_einops(shape, nlastdim=len(f.inner_shape)),
               **axes_length,
           ),
           dc_fn=lambda f: f.value.reshape(  # pylint: disable=g-long-lambda
               np_utils.to_absolute_einops(shape, nlastdim=len(f.inner_shape)),
@@ -361,23 +361,23 @@
       )
     else:  # Numpy support
       assert isinstance(shape, tuple)  # For pytest
 
       def _reshape(f: _ArrayField):
         return f.value.reshape(shape + f.inner_shape)
 
-      return self._map_field(array_fn=_reshape, dc_fn=_reshape)
+      return self._map_field(array_fn=_reshape, dc_fn=_reshape)  # pylint: disable=protected-access
 
   def flatten(self: _DcT) -> _DcT:
     """Flatten the batch shape."""
     return self.reshape((-1,))
 
   def broadcast_to(self: _DcT, shape: Shape) -> _DcT:
     """Broadcast the batch shape."""
-    return self._map_field(
+    return self._map_field(  # pylint: disable=protected-access
         array_fn=lambda f: f.broadcast_to(shape),
         dc_fn=lambda f: f.broadcast_to(shape),
     )
 
   def __getitem__(self: _DcT, indices: _IndicesArg) -> _DcT:
     """Slice indexing."""
     indices = np.index_exp[indices]  # Normalize indices
@@ -452,15 +452,15 @@
     return True
 
   def map_field(
       self: _DcT,
       fn: Callable[[Array['*din']], Array['*dout']],
   ) -> _DcT:
     """Apply a transformation on all arrays from the fields."""
-    return self._map_field(
+    return self._map_field(  # pylint: disable=protected-access
         array_fn=lambda f: fn(f.value),
         dc_fn=lambda f: f.value.map_field(fn),
     )
 
   # ====== Dataclass/Conversion utils ======
 
   def replace(self: _DcT, **kwargs: Any) -> _DcT:
@@ -526,15 +526,15 @@
         return xnp.asarray(arr)
 
       array_fn = _as_torch
     else:
       array_fn = lambda f: xnp.asarray(f.value)
 
     # Update all childs
-    new_self = self._map_field(
+    new_self = self._map_field(  # pylint: disable=protected-access
         array_fn=array_fn,
         dc_fn=lambda f: f.value.as_xnp(xnp),
     )
     return new_self
 
   # TODO(pytype): Remove hack. Currently, Python does not support typing
   # annotations for modules, by pytype auto-infer the correct type.
@@ -578,14 +578,34 @@
     if not lazy.is_torch_xnp(self.xnp):
       raise ValueError('`.cuda` can only be called when `xnp == torch`')
     return self.map_field(lambda f: f.cuda(*args, **kwargs))
 
   # ====== Internal ======
 
   @epy.cached_property
+  def _all_fields_empty(self) -> bool:
+    """Returns True if the `dataclass_array` is invalid."""
+    if not self._array_fields:  # All fields are `None` / `object`
+      # No fields have been defined.
+      # This can be the case internally by jax which apply some
+      # `tree_map(lambda x: sentinel)`.
+      return True
+
+    # `tf.nest` sometimes replace values by dummy `.` inside
+    # `assert_same_structure`
+    if enp.lazy.has_tf:
+      # pylint: disable=g-direct-tensorflow-import,g-import-not-at-top
+      from tensorflow.python.util import nest_util  # pytype: disable=import-error
+      # pylint: enable=g-direct-tensorflow-import,g-import-not-at-top
+
+      if any(f.value is nest_util._DOT for f in self._array_fields):  # pylint: disable=protected-access,not-an-iterable
+        return True
+    return False
+
+  @epy.cached_property
   def _all_array_fields(self) -> dict[str, _ArrayField]:
     """All array fields, including `None` values."""
     return {  # pylint: disable=g-complex-comprehension
         name: _ArrayField(
             name=name,
             host=self,
             **field_metadata.to_dict(),  # pylint: disable=not-a-mapping
@@ -599,15 +619,15 @@
     # Filter `None` values
     return [
         f for f in self._all_array_fields.values() if not f.is_value_missing
     ]
 
   def _cast_xnp_dtype_inplace(self) -> Optional[enp.NpModule]:
     """Validate `xnp` are consistent and cast `np` -> `xnp` in-place."""
-    if not self._array_fields:  # All fields are `None` / `object`
+    if self._all_fields_empty:  # pylint: disable=using-constant-test
       return None
 
     # Validate the dtype
     def _get_xnp(f: _ArrayField) -> enp.NpModule:
       try:
         return np_utils.get_xnp(
             f.value,
@@ -623,20 +643,27 @@
     )
     if not xnps:
       return None
     xnp = _infer_xnp(xnps)
 
     def _cast_field(f: _ArrayField) -> None:
       try:
-        new_value = np_utils.asarray(
-            f.value,
-            xnp=xnp,
-            dtype=f.dtype,
-            cast_dtype=self.__dca_params__.cast_dtype,
-        )
+        # Supports for TensorSpec (e.g. in `tf.function` signature)
+        if enp.lazy.is_tf_xnp(xnp) and isinstance(
+            f.value, enp.lazy.tf.TensorSpec
+        ):
+          # TODO(epot): Actually check the dtype
+          new_value = f.value
+        else:
+          new_value = np_utils.asarray(
+              f.value,
+              xnp=xnp,
+              dtype=f.dtype,
+              cast_dtype=self.__dca_params__.cast_dtype,
+          )
         self._setattr(f.name, new_value)
         # After the field has been set, we validate the shape
         f.assert_shape()
       except Exception as e:  # pylint: disable=broad-except
         epy.reraise(e, prefix=f'Invalid {f.qualname}: ')
 
     self._map_field(
@@ -644,17 +671,15 @@
         dc_fn=_cast_field,  # pytype: disable=wrong-arg-types
         _inplace=True,
     )
     return xnp
 
   def _broadcast_shape_inplace(self) -> Optional[Shape]:
     """Validate the shapes are consistent and broadcast values in-place."""
-    if not self._array_fields:  # No fields have been defined.
-      # This can be the case internally by jax which apply some
-      # `tree_map(lambda x: sentinel)`.
+    if self._all_fields_empty:  # pylint: disable=using-constant-test
       return None
 
     # First collect all shapes and compute the final shape.
     shape_to_names = epy.groupby(
         self._array_fields,
         key=lambda f: f.host_shape,
         value=lambda f: f.name,
@@ -731,25 +756,25 @@
 
     def _apply_field_dn(f: _ArrayField):
       if f.is_dataclass:  # Recurse on dataclasses
         return dc_fn(f)  # pylint: disable=protected-access
       else:
         return array_fn(f)
 
-    new_values = {f.name: _apply_field_dn(f) for f in self._array_fields}  # pylint: disable=not-an-iterable
+    new_values = {f.name: _apply_field_dn(f) for f in self._array_fields}  # pylint: disable=not-an-iterable,protected-access
     # For performance, do not call replace to save the constructor call
     if not _inplace:
       return self.replace(**new_values)
     else:
       return self
 
-  def tree_flatten(self) -> tuple[list[DcOrArray], _TreeMetadata]:
+  def tree_flatten(self) -> tuple[tuple[DcOrArray, ...], _TreeMetadata]:
     """`jax.tree_utils` support."""
     # We flatten all values (and not just the non-None ones)
-    array_field_values = [f.value for f in self._all_array_fields.values()]
+    array_field_values = tuple(f.value for f in self._all_array_fields.values())
     metadata = _TreeMetadata(
         array_field_names=list(self._all_array_fields.keys()),
         non_array_field_kwargs={
             f.name: getattr(self, f.name)
             for f in dataclasses.fields(self)  # pytype: disable=wrong-arg-types  # re-none
             if f.name not in self._all_array_fields  # pylint: disable=unsupported-membership-test
         },
@@ -788,14 +813,26 @@
             'propagated by `tree_map`.'
         )
       # TODO(py310): Delete once dataclass supports `kw_only=True`
       for k, v in non_init_fields.items():
         self._setattr(k, v)  # pylint: disable=protected-access
     return self
 
+  def __tf_flatten__(self) -> tuple[_TreeMetadata, tuple[DcOrArray, ...]]:
+    components, metadata = self.tree_flatten()
+    return metadata, components
+
+  @classmethod
+  def __tf_unflatten__(
+      cls: Type[_DcT],
+      metadata: _TreeMetadata,
+      components: list[DcOrArray],
+  ) -> _DcT:
+    return cls.tree_unflatten(metadata, components)
+
   def _setattr(self, name: str, value: Any) -> None:
     """Like setattr, but support `frozen` dataclasses."""
     object.__setattr__(self, name, value)
 
   def assert_same_xnp(self, x: Union[Array[...], DataclassArray]) -> None:
     """Assert the given array is of the same type as the current object."""
     xnp = np_utils.get_xnp(x)
@@ -851,15 +888,15 @@
   dca_fields_metadata = {  # Filter `None` values (static fields)
       k: v for k, v in dca_fields_metadata.items() if v is not None
   }
   if not dca_fields_metadata:
     # DataclassArray without any array fields
     # Hack: To support `.xnp`, `.shape`, we add a dummy empty field which
     # is propagated by the various ops.
-    dca_fields_metadata[_DUMMY_ARRAY_FIELD] = _ArrayFieldMetadata(
+    dca_fields_metadata[_DUMMY_ARRAY_FIELD] = _ArrayFieldMetadata(  # pytype: disable=wrong-arg-types
         inner_shape_non_static=(),
         dtype=np.float32,
     )
     default_dummy_array = np.zeros((), dtype=np.float32)
     _add_field_to_dataclass(
         cls, _DUMMY_ARRAY_FIELD, default=default_dummy_array
     )
@@ -967,29 +1004,29 @@
 @dataclasses.dataclass
 class _ArrayFieldMetadata:
   """Metadata of the array field (shared across all instances).
 
   Attributes:
     inner_shape_non_static: Inner shape. Can contain non-static dims (e.g.
       `(None, 3)`)
-    dtype: Type of the array. Can be `array_types.dtypes.DType` or
+    dtype: Type of the array. Can be `enp.dtypes.DType` or
       `dca.DataclassArray` for nested arrays.
   """
 
   inner_shape_non_static: DynamicShape
-  dtype: Union[array_types.dtypes.DType, Type[DataclassArray]]
+  dtype: Union[enp.dtypes.DType, Type[DataclassArray]]
 
   def __post_init__(self):
     """Normalizing/validating the shape/dtype."""
     # Validate shape
     self.inner_shape_non_static = tuple(self.inner_shape_non_static)
 
     # Validate/normalize the dtype
     if not self.is_dataclass:
-      self.dtype = array_types.dtypes.DType.from_value(self.dtype)
+      self.dtype = enp.dtypes.DType.from_value(self.dtype)
       # TODO(epot): Filter invalid dtypes, like `str` ?
 
   def to_dict(self) -> dict[str, Any]:
     """Returns the dict[field_name, field_value]."""
     return {f.name: getattr(self, f.name) for f in dataclasses.fields(self)}
 
   @property
```

### Comparing `dataclass_array-1.4.2/dataclass_array/conftest.py` & `dataclass_array-1.5.0/dataclass_array/conftest.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/field_utils.py` & `dataclass_array-1.5.0/dataclass_array/field_utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/ops.py` & `dataclass_array-1.5.0/dataclass_array/ops.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/shape_parsing.py` & `dataclass_array-1.5.0/dataclass_array/shape_parsing.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/testing.py` & `dataclass_array-1.5.0/dataclass_array/testing.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/type_parsing.py` & `dataclass_array-1.5.0/dataclass_array/type_parsing.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/typing.py` & `dataclass_array-1.5.0/dataclass_array/typing.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/utils/file_utils.py` & `dataclass_array-1.5.0/dataclass_array/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/utils/inspect_utils.py` & `dataclass_array-1.5.0/dataclass_array/utils/inspect_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
   for arg in bound_args:  # Iterate over args/kwargs
     print(f'{arg.fn_name} called with {arg.name}={arg.value!r}')
 
   bound_args = bound_args.map(_validate_or_transform_args)
 
   y = bound_args.call()  # Call the function
   ```
-
   """
 
   fn: _Fn[_OutT]
   signature: inspect.Signature = dataclasses.field(init=False)
 
   def __post_init__(self):
     self.signature = inspect.Signature.from_callable(self.fn)
@@ -198,28 +197,33 @@
 
     return self.map_bound_arg(_fn)
 
   def map_bound_arg(
       self,
       fn: Callable[[BoundArg[_ArgT]], _NewArgT],
   ) -> BoundArgs[_NewArgT, _OutT]:
-    """Apply validation/modification to the arguments value."""
+    """Apply validation/modification to all `BoundArg`."""
 
     def _fn(arg: BoundArg[_ArgT]) -> _NewArgT:  # pytype: disable=invalid-annotation
       try:
         return fn(arg)
       except Exception as e:  # pylint: disable=broad-except
         epy.reraise(
             e,
             prefix=f'For arg {arg.pos} ({arg.name!r}):\n',
         )
 
+    return self.replace_args_values({arg.name: _fn(arg) for arg in self})
+
+  def replace_args_values(
+      self, new_values: dict[str, _NewArgT]
+  ) -> BoundArgs[_NewArgT, _OutT]:
     bound_args = inspect.BoundArguments(
         signature=self.bound_args.signature,
-        arguments={arg.name: _fn(arg) for arg in self},  # pytype: disable=wrong-arg-types
+        arguments=new_values,  # pytype: disable=wrong-arg-types
     )
     return self.replace(bound_args=bound_args)  # pytype: disable=attribute-error
 
 
 @edc.dataclass
 @dataclasses.dataclass
 class BoundArg(Generic[_ArgT]):
```

### Comparing `dataclass_array-1.4.2/dataclass_array/utils/np_utils.py` & `dataclass_array-1.5.0/dataclass_array/utils/np_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 """Numpy utils.
 
 And utils intended to work on both `xnp.ndarray` and `dca.DataclassArray`.
 """
 
 from __future__ import annotations
 
-from typing import Any, Union, Optional
+from typing import Any, Optional, Union
 
 from dataclass_array import array_dataclass
-from dataclass_array.typing import Axes, DcOrArrayT, DTypeArg, Shape  # pylint: disable=g-multiple-import
-from etils import array_types
+from dataclass_array.typing import Axes, DTypeArg, DcOrArrayT, Shape  # pylint: disable=g-multiple-import,g-importing-member
 from etils import enp
-from etils.array_types import Array, ArrayLike  # pylint: disable=g-multiple-import
+from etils.array_types import Array, ArrayLike  # pylint: disable=g-multiple-import,g-importing-member
 
 # Maybe some of those could live in `enp` ?
 
 
 def size_of(shape: Shape) -> int:
   """Returns the size associated with the shape."""
   # TODO(b/198633198): Warning: In TF `bool(shape) == True` for `shape==()`
@@ -120,15 +119,15 @@
     if dtype is not None and (
         not isinstance(dtype, type) or not isinstance(x, dtype)
     ):
       raise TypeError(f'Expected {dtype}. Got: {type(x)}')
     return x.as_xnp(xnp)
 
   # Handle ndarray
-  dtype = array_types.dtypes.DType.from_value(dtype)
+  dtype = enp.dtypes.DType.from_value(dtype)
   return dtype.asarray(x, xnp=xnp, casting='all' if cast_dtype else 'none')
 
 
 def _assert_valid_xnp_cast(from_: enp.NpModule, to: enp.NpModule) -> None:
   """Only `np` -> `xnp` conversion is accepted."""
   if from_ is not enp.lazy.np and from_ is not to:
     raise TypeError(f'Expected {to.__name__} got {from_.__name__}')
```

### Comparing `dataclass_array-1.4.2/dataclass_array/utils/py_utils.py` & `dataclass_array-1.5.0/dataclass_array/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/utils/tree_utils.py` & `dataclass_array-1.5.0/dataclass_array/utils/tree_utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.2/dataclass_array/vectorization.py` & `dataclass_array-1.5.0/dataclass_array/vectorization.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import functools
 import typing
 from typing import Any, Callable, Optional, Set, TypeVar
 
 from dataclass_array import array_dataclass
 from dataclass_array import ops
-from dataclass_array.typing import DcOrArray, Shape  # pylint: disable=g-multiple-import
+from dataclass_array.typing import DcOrArray, Shape  # pylint: disable=g-multiple-import,g-importing-member
 from dataclass_array.utils import inspect_utils
 from dataclass_array.utils import np_utils
 from dataclass_array.utils import py_utils
 from dataclass_array.utils import tree_utils
 from etils import enp
 from etils import epy
 
@@ -303,29 +303,38 @@
 def _vmap_method(
     args: inspect_utils.BoundArgs,
     *,
     map_non_static: _MapNonStatic,
     xnp: enp.NpModule,
 ) -> _Out:
   """Vectorize self using the `xnp` backend. Assume `self` was flatten."""
-  if xnp is enp.lazy.np:
+  is_jax = enp.lazy.is_jax_xnp(xnp)
+  is_torch = enp.lazy.is_torch_xnp(xnp)
+
+  if enp.lazy.is_np_xnp(xnp):
     return _vmap_method_np(args, map_non_static=map_non_static)
-  elif xnp is enp.lazy.jnp:
+  elif is_jax or is_torch:
+    if is_jax:
+      make_vmap_fn = _jax_vmap_cached
+    elif is_torch:
+      make_vmap_fn = _torch_vmap_cached
+    else:
+      raise ValueError('Unexpected')
     return _vmap_method_jax_torch(
         args,
         map_non_static=map_non_static,
-        make_vmap_fn=_jax_vmap_cached,
+        make_vmap_fn=make_vmap_fn,
     )
-  elif xnp is enp.lazy.tnp:
-    return _vmap_method_tf(args, map_non_static=map_non_static)
-  elif xnp is enp.lazy.torch:
-    return _vmap_method_jax_torch(
-        args,
-        map_non_static=map_non_static,
-        make_vmap_fn=_torch_vmap_cached,
+  elif enp.lazy.is_tf_xnp(xnp):
+    # return _vmap_method_tf(args, map_non_static=map_non_static)
+
+    # TODO(epot): Use `tf.vectorized_map()` once TF support custom nesting
+    raise NotImplementedError(
+        'vectorization not supported in TF yet due to lack of `tf.nest` '
+        'support. Please upvote or comment b/152678472.'
     )
   raise TypeError(f'Invalid numpy module: {xnp}')
 
 
 def _vmap_method_np(
     args: inspect_utils.BoundArgs[Any, _OutT],
     *,
@@ -396,21 +405,60 @@
 
 def _vmap_method_tf(
     args: inspect_utils.BoundArgs[Any, _OutT],
     *,
     map_non_static: _MapNonStatic,
 ) -> _OutT:
   """vectorization using `tf` backend."""
-  # TODO(epot): Use `tf.vectorized_map()` once TF support custom nesting
-  raise NotImplementedError(
-      'vectorization not supported in TF yet due to lack of `tf.nest` '
-      'support. Please upvote or comment b/152678472.'
+
+  # Flatten args
+
+  args_info = args.map(lambda _: None)
+  # ... except the non-static ones
+  args_info = map_non_static(lambda _: 0, args_info)
+
+  # Split args in static/non-static
+  static_args = {}
+  nonstatic_args = {}
+  for a, ai in zip(args, args_info):
+    assert a.name == ai.name
+    if ai.value is None:
+      static_args[a.name] = a.value
+    else:
+      nonstatic_args[a.name] = a.value
+
+  def new_fn(non_statics, statics):
+    # Merge args and call the function
+    new_args = args.replace_args_values(dict(**non_statics, **statics))
+    return new_args.call()
+
+  # `vectorized_map(` uses autograph, which fails, so use tf.map_fn instead
+  return _better_map_fn(  #
+      functools.partial(new_fn, statics=static_args),
+      nonstatic_args,
   )
 
 
+# tf.map_fn do not support different output signature:
+def _better_map_fn(fn, elems, **kwargs):
+  """Like `tf.map_fn`."""
+  tf = enp.lazy.tf
+  if 'fn_output_signature' not in kwargs:
+    elem_spec = tf.nest.map_structure(
+        lambda t: tf.type_spec_from_value(t)._unbatch(), elems  # pylint: disable=protected-access
+    )
+    output_spec = tf.nest.map_structure(
+        tf.type_spec_from_value,
+        tf.function(fn).get_concrete_function(elem_spec).structured_outputs,
+    )
+    kwargs['fn_output_signature'] = output_spec
+
+  return tf.map_fn(fn, elems, **kwargs)
+
+
 def _stack(*vals: _OutT) -> _OutT:
   """Stack the given tree."""
   assert vals
   val = vals[0]
   if isinstance(val, array_dataclass.DataclassArray):
     return ops.stack(vals, axis=0)
   elif enp.lazy.is_array(val):
```

### Comparing `dataclass_array-1.4.2/pyproject.toml` & `dataclass_array-1.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 # This is set automatically by flit using `dataclass_array.__version__`
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/google-research/dataclass_array"
 repository = "https://github.com/google-research/dataclass_array"
-# Other: `documentation`, `changelog`
+documentation = "https://dataclass-array.readthedocs.io"
+changelog = "https://github.com/google-research/dataclass_array/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 # Development deps (unittest, linting, formating,...)
 # Installed through `pip install .[dev]`
 dev = [
     "pytest",
     "pytest-xdist",
```

### Comparing `dataclass_array-1.4.2/PKG-INFO` & `dataclass_array-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass_array
-Version: 1.4.2
+Version: 1.5.0
 Summary: Dataclasses that behave like numpy arrays (with indexing, slicing, vectorization).
 Keywords: dataclass,dataclasses,numpy,jax,tensorflow,array
 Author-email: dataclass_array team <dataclass_array@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -22,14 +22,16 @@
 Requires-Dist: pyink ; extra == "dev"
 Requires-Dist: chex ; extra == "dev"
 Requires-Dist: jax[cpu] ; extra == "dev"
 Requires-Dist: tf-nightly ; extra == "dev"
 Requires-Dist: torch ; extra == "dev"
 Requires-Dist: sphinx-apitree[ext] ; extra == "docs"
 Requires-Dist: dataclass_array[dev] ; extra == "docs"
+Project-URL: changelog, https://github.com/google-research/dataclass_array/blob/main/CHANGELOG.md
+Project-URL: documentation, https://dataclass-array.readthedocs.io
 Project-URL: homepage, https://github.com/google-research/dataclass_array
 Project-URL: repository, https://github.com/google-research/dataclass_array
 Provides-Extra: dev
 Provides-Extra: docs
 
 # Dataclass Array
```

