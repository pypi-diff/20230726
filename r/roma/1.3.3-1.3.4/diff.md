# Comparing `tmp/roma-1.3.3.tar.gz` & `tmp/roma-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roma-1.3.3.tar", last modified: Wed Jun 28 08:51:02 2023, max compression
+gzip compressed data, was "roma-1.3.4.tar", last modified: Wed Jul 26 14:55:43 2023, max compression
```

## Comparing `roma-1.3.3.tar` & `roma-1.3.4.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-06-28 08:51:02.338345 roma-1.3.3/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21068 2023-02-08 15:17:32.000000 roma-1.3.3/LICENSE
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2023-02-08 15:17:32.000000 roma-1.3.3/NOTICE
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3987 2023-06-28 08:51:02.338345 roma-1.3.3/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3509 2023-02-08 15:17:32.000000 roma-1.3.3/README.md
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.3.3/pyproject.toml
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-06-28 08:51:02.334345 roma-1.3.3/roma/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      145 2023-02-08 15:17:32.000000 roma-1.3.3/roma/__init__.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2793 2023-06-23 14:54:33.000000 roma-1.3.3/roma/internal.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    18038 2023-04-26 08:34:41.000000 roma-1.3.3/roma/mappings copy.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    18727 2023-06-23 14:28:54.000000 roma-1.3.3/roma/mappings.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    19966 2023-06-23 15:01:06.000000 roma-1.3.3/roma/utils.py
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-06-28 08:51:02.338345 roma-1.3.3/roma.egg-info/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3987 2023-06-28 08:51:02.000000 roma-1.3.3/roma.egg-info/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      349 2023-06-28 08:51:02.000000 roma-1.3.3/roma.egg-info/SOURCES.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2023-06-28 08:51:02.000000 roma-1.3.3/roma.egg-info/dependency_links.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2023-06-28 08:51:02.000000 roma-1.3.3/roma.egg-info/top_level.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2023-06-28 08:51:02.338345 roma-1.3.3/setup.cfg
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2023-06-21 22:54:26.000000 roma-1.3.3/setup.py
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-06-28 08:51:02.338345 roma-1.3.3/test/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1018 2023-02-08 15:17:32.000000 roma-1.3.3/test/test_derivatives.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8457 2023-02-08 15:17:32.000000 roma-1.3.3/test/test_mappings.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3808 2023-06-21 22:50:53.000000 roma-1.3.3/test/test_procrustes_derivatives.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    14887 2023-06-17 20:02:02.000000 roma-1.3.3/test/test_utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-07-26 14:55:43.203286 roma-1.3.4/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21068 2023-02-08 15:17:32.000000 roma-1.3.4/LICENSE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2023-02-08 15:17:32.000000 roma-1.3.4/NOTICE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4226 2023-07-26 14:55:43.203286 roma-1.3.4/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3748 2023-07-26 12:33:00.000000 roma-1.3.4/README.md
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.3.4/pyproject.toml
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-07-26 14:55:43.203286 roma-1.3.4/roma/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      145 2023-02-08 15:17:32.000000 roma-1.3.4/roma/__init__.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3700 2023-07-26 13:01:51.000000 roma-1.3.4/roma/internal.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    18727 2023-06-23 14:28:54.000000 roma-1.3.4/roma/mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    19966 2023-06-23 15:01:06.000000 roma-1.3.4/roma/utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-07-26 14:55:43.203286 roma-1.3.4/roma.egg-info/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4226 2023-07-26 14:55:43.000000 roma-1.3.4/roma.egg-info/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      327 2023-07-26 14:55:43.000000 roma-1.3.4/roma.egg-info/SOURCES.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2023-07-26 14:55:43.000000 roma-1.3.4/roma.egg-info/dependency_links.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2023-07-26 14:55:43.000000 roma-1.3.4/roma.egg-info/top_level.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2023-07-26 14:55:43.203286 roma-1.3.4/setup.cfg
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2023-07-26 09:32:58.000000 roma-1.3.4/setup.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-07-26 14:55:43.203286 roma-1.3.4/test/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1018 2023-02-08 15:17:32.000000 roma-1.3.4/test/test_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8457 2023-02-08 15:17:32.000000 roma-1.3.4/test/test_mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3808 2023-06-21 22:50:53.000000 roma-1.3.4/test/test_procrustes_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    14887 2023-06-17 20:02:02.000000 roma-1.3.4/test/test_utils.py
```

### Comparing `roma-1.3.3/LICENSE` & `roma-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `roma-1.3.3/NOTICE` & `roma-1.3.4/NOTICE`

 * *Files identical despite different names*

### Comparing `roma-1.3.3/PKG-INFO` & `roma-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.3.3
+Version: 1.3.4
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -62,22 +62,26 @@
 
 
 ## Installation
 The easiest way to install *RoMa* is to use pip:
 ```
 pip install roma
 ```
-We also recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
-to achieve significant speed-up with the _special_procrustes_ function on a CUDA GPU.
 
 Alternatively one can install the latest version of *RoMa* directly from the source repository:
 ```
 pip install git+https://github.com/naver/roma
 ```
 
+**For pytorch versions older than 1.8**, we recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
+to achieve a significant speed-up with `special_procrustes` on CUDA GPUs.
+You can check that this module is properly loaded using the function `roma.utils.is_torch_batch_svd_available()`.
+**With recent pytorch installations (torch>=1.8), `torch-batch-svd` is no longer needed or used.**
+
+
 ## License
 *RoMa*, Copyright (c) 2021 NAVER Corp., is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
 
 Bits of code were adapted from SciPy. Documentation is generated, distributed and displayed with the support of Sphinx and other materials (see [notice](https://github.com/naver/roma/blob/master/NOTICE)).
 
 ## References
 For a more in-depth discussion regarding differentiable mappings on the rotation space, please refer to:
```

### Comparing `roma-1.3.3/README.md` & `roma-1.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -47,22 +47,26 @@
 
 
 ## Installation
 The easiest way to install *RoMa* is to use pip:
 ```
 pip install roma
 ```
-We also recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
-to achieve significant speed-up with the _special_procrustes_ function on a CUDA GPU.
 
 Alternatively one can install the latest version of *RoMa* directly from the source repository:
 ```
 pip install git+https://github.com/naver/roma
 ```
 
+**For pytorch versions older than 1.8**, we recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
+to achieve a significant speed-up with `special_procrustes` on CUDA GPUs.
+You can check that this module is properly loaded using the function `roma.utils.is_torch_batch_svd_available()`.
+**With recent pytorch installations (torch>=1.8), `torch-batch-svd` is no longer needed or used.**
+
+
 ## License
 *RoMa*, Copyright (c) 2021 NAVER Corp., is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
 
 Bits of code were adapted from SciPy. Documentation is generated, distributed and displayed with the support of Sphinx and other materials (see [notice](https://github.com/naver/roma/blob/master/NOTICE)).
 
 ## References
 For a more in-depth discussion regarding differentiable mappings on the rotation space, please refer to:
```

### Comparing `roma-1.3.3/roma/internal.py` & `roma-1.3.4/roma/internal.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,59 @@
 # Available only for non-commercial use.
 """
 Set of functions for internal module use.
 """
 
 import torch
 
+# SVD decomposition
+# Default behavior: vanilla svd
+_IS_TORCH_BATCH_SVD_AVAILABLE = False
 try:
-    import torch_batch_svd
-    _fast_gpu_svd = torch_batch_svd.svd
-    _IS_TORCH_BATCH_SVD_AVAILABLE = True
-except ModuleNotFoundError:
-    # torch_batch_svd (https://github.com/KinglittleQ/torch-batch-svd) is not installed
-    # and is required for maximum efficiency of special_procrustes using GPUs.
-    # Using torch.svd as a fallback.
-    _IS_TORCH_BATCH_SVD_AVAILABLE = False
-    _fast_gpu_svd = torch.svd
+    # Should raise an AttributeError exception if undefined.
+    torch.linalg.svd
+    def svd(M):
+        """
+        Singular Value Decomposition wrapper.
+        
+        Args:
+            M (BxMxN tensor): batch of real matrices.
+        Returns:
+            (U,D,V) decomposition, such as :math:`M = U @ diag(D) @ V^T`.
+        """
+        U, D, Vt = torch.linalg.svd(M)
+        return (U, D, Vt.transpose(-2,-1))
+except (NameError, AttributeError):
+    # deprecated in torch 2.0
+    svd = torch.svd
+
+# With PyTorch < 1.8,
+# we observed some significant speed-ups using torch_batch_svd (https://github.com/KinglittleQ/torch-batch-svd) instead of torch.svd on NVidia GPUs.
+# In more recent versions, this is no longer required (https://github.com/pytorch/pytorch/pull/48436).
+_torch_version_major, _torch_version_minor = [int(s) for s in torch.__version__.split(".")[:2]]
+if  _torch_version_major == 0 or (_torch_version_major == 1 and _torch_version_minor < 8):
+    try:
+        import torch_batch_svd
+        _IS_TORCH_BATCH_SVD_AVAILABLE = True
+        def svd(M):
+            """
+            Singular Value Decomposition wrapper, using efficient batch decomposition on GPU.
+
+            Args:
+                M (BxMxN tensor): batch of real matrices.
+            Returns:
+                (U,D,V) decomposition, such as :math:`M = U @ diag(D) @ V^T`.
+            """
+            if M.is_cuda and M.shape[1] < 32 and M.shape[2] < 32:
+                return torch_batch_svd.svd(M)
+            else:
+                return torch.svd(M)
+    except ModuleNotFoundError:
+        pass
+del _torch_version_major, _torch_version_minor
 
 def flatten_batch_dims(tensor, end_dim):
     """
     :meta private:
     Utility function: flatten multiple batch dimensions into a single one, or add a batch dimension if there is none.
     """
     batch_shape = tensor.shape[:end_dim+1]
@@ -41,28 +76,14 @@
     :meta private:
     Element-wise pseudo inverse.
     """
     inv = 1.0/x
     inv[torch.abs(x) < eps] = 0.0
     return inv    
 
-def svd(M):
-    """
-    Singular Value Decomposition wrapper, using efficient batch decomposition on GPU when available.
-
-    Args:
-        M (BxMxN tensor): batch of real matrices.
-    Returns:
-        (U,D,V) decomposition, such as :math:`M = U @ diag(D) @ V^T`.
-    """
-    if M.is_cuda and M.shape[1] < 32 and M.shape[2] < 32:
-        return _fast_gpu_svd(M)
-    else:
-        return torch.svd(M)
-
 # Batched eigenvalue decomposition.
 # Recent version of PyTorch deprecated the use of torch.symeig.
 try:
     torch.linalg.eigh
     def symeig_lower(A):
         """
         Batched eigenvalue decomposition. Only the lower part of the matrix is considered.
```

### Comparing `roma-1.3.3/roma/mappings copy.py` & `roma-1.3.4/roma/mappings.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,95 +18,91 @@
         U, D, V = roma.internal.svd(M)
         if force_rotation:
             # We flip the smallest singular value to ensure getting a rotation matrix
             with torch.no_grad():
                 flip = (torch.det(U) * torch.det(V) < 0)            
             # in-place modifications of variables not used afterwards.
             DS = D
-            DS[flip, -1] *= -1
+            DS[flip,-1] *= -1
             del D
             US = U
             US[flip,:,-1] *= -1
             del U
         else:
             flip = None
             DS = D
             US = U
         R = US @ V.transpose(-1, -2)
         # Store data for backprop:
         ctx.save_for_backward(US, DS, V, M, R)
         ctx.gradient_eps = gradient_eps
         ctx.regularization = regularization
-        return R
+        return R, DS
 
     @staticmethod
-    def backward(ctx, grad_R):
+    def backward(ctx, grad_R, grad_DS):
         US, DS, V, M, R = ctx.saved_tensors
         gradient_eps = ctx.gradient_eps
 
-
+        USik_Vjl = torch.einsum('bik,bjl -> bklij', US, V)
+        USil_Vjk = USik_Vjl.transpose(1,2)
+        DSl = DS[:,None,:,None,None]
+        DSk = DS[:,:,None,None,None]
+        Omega_klij = (USik_Vjl - USil_Vjk) * roma.internal._pseudo_inverse(DSk + DSl, gradient_eps)
+        # Note: this intermediary matrix may require lots of memory for large dimensional cases.
+        # Diagonal k==l should always be 0 thanks to the clamping of the pseudo-inverse.
         
-        
-        if False:
-            USik_Vjl = torch.einsum('bik,bjl -> bklij', US, V)
-            USil_Vjk = USik_Vjl.transpose(1,2)
-            DSl = DS[:,None,:,None,None]
-            DSk = DS[:,:,None,None,None]
-            Omega_klij = (USik_Vjl - USil_Vjk) * roma.internal._pseudo_inverse(DSk + DSl, gradient_eps)
-            # Note: this intermediary matrix may require lots of memory for large dimensional cases.
-            # Diagonal k==l should always be 0 thanks to the clamping of the pseudo-inverse.
-            grad_M = torch.einsum('bnm, bnk, bklij, bml -> bij', grad_R, US, Omega_klij, V)
-        else:
-            from pykeops.torch import LazyTensor
-            foo_kl = torch.einsum('bnm, bnk, bml -> bkl', grad_R, US, V)
-            foo_kl = foo_kl * roma.internal._pseudo_inverse(DS[:,:,None] + DS[:,None,:], gradient_eps)
-            # Reduction over l
-            TODO
-            USikl =
-            Vjlk ....
-            # Reduction over l
-
-
+        grad_M = torch.einsum('bnm, bnk, bklij, bml -> bij', grad_R, US, Omega_klij, V)
+        # Gradient contribution from singular values
+        grad_M += (US * grad_DS[:,None,:]) @ V.transpose(-1, -2)
         if ctx.regularization != 0.0:
             # Add a regularization term in the direction of the orthonormalized output.
             grad_M += ctx.regularization * (M - R)
         return grad_M, None, None, None
 
-def procrustes(M, force_rotation=False, regularization=0.0, gradient_eps=1e-5):
+def procrustes(M, force_rotation=False, regularization=0.0, gradient_eps=1e-5, return_singular_values : bool = False):
     """ 
     Returns the orthonormal matrix :math:`R` minimizing Frobenius norm :math:`\| M - R \|_F`.
 
     Args:
         M (...xNxN tensor): batch of square matrices.
         force_rotation (bool): if True, forces the output to be a rotation matrix.
         regularization (float >= 0): weight of a regularization term added to the gradient.
             Using this regularization is equivalent to adding a term :math:`regularization * \| M - R \|_F^2` to the training loss function.
         gradient_eps (float > 0): small value used to enforce numerical stability during backpropagation.
     Returns:
-        batch of orthonormal matrices (...xNxN tensor).
+        batch of orthonormal matrices (...xNxN tensor) and optional singular values.
+        For advanced users, singular values of the SVD decomposition with sign flipping (... tensor) can optionally be returned by setting the argument :code:`return_singular_values` to :code:`True`.
     """
     M, batch_shape = roma.internal.flatten_batch_dims(M, -3)
-    R = _ProcrustesManualDerivatives.apply(M, force_rotation, regularization, gradient_eps)
-    return roma.internal.unflatten_batch_dims(R, batch_shape)
+    R, DS = _ProcrustesManualDerivatives.apply(M, force_rotation, regularization, gradient_eps)
+    R = roma.internal.unflatten_batch_dims(R, batch_shape)
+    if not return_singular_values:
+        return R
+    else:
+        DS = roma.internal.unflatten_batch_dims(DS, batch_shape)
+        return R, DS
 
-def special_procrustes(M, regularization=0.0, gradient_eps=1e-5):
+def special_procrustes(M, regularization=0.0, gradient_eps=1e-5, return_singular_values : bool = False):
     """
     Returns the rotation matrix :math:`R` minimizing Frobenius norm :math:`\| M - R \|_F`.
 
     Args:
         M (...xNxN tensor): batch of square matrices.
         regularization (float >= 0): weight of a regularization term added to the gradient.
             Using this regularization is equivalent to adding a term :math:`regularization * \| M - R \|_F^2` to the training loss function.
         gradient_eps (float > 0): small value used to enforce numerical stability during backpropagation.
     Returns:
         batch of rotation matrices (...xNxN tensor).
+        For advanced users, singular values of the SVD decomposition with sign flipping (... tensor) can optionally be returned by setting the argument :code:`return_singular_values` to :code:`True`.
+
     """
-    return procrustes(M, True, regularization, gradient_eps)
+    return procrustes(M, True, regularization, gradient_eps, return_singular_values)
 
-def procrustes_naive(M, force_rotation : bool = False):
+def procrustes_naive(M, force_rotation : bool = False, return_singular_values : bool = False):
     """
     Implementation of :func:`~roma.mappings.procrustes` relying on default backward pass of autograd and SVD decomposition.
     Could be slightly less stable than :func:`~roma.mappings.procrustes`.
     """
     M, batch_shape = roma.internal.flatten_batch_dims(M, -3)
     assert (M.dim() == 3 and M.shape[1] == M.shape[2]), "Input should be a BxDxD batch of matrices."
     U, D, V = roma.internal.svd(M)
@@ -117,23 +113,31 @@
         with torch.no_grad():
             flip = (torch.det(U) * torch.det(V) < 0)
         if torch.is_grad_enabled():
             # This is needed to avoid a runtime error "one of the variables needed for gradient computation has been modified by an inplace operation"
             SVt = SVt.clone()
         SVt[flip,-1,:] *= -1
     R = U @ SVt
-    return roma.internal.unflatten_batch_dims(R, batch_shape)
+    R = roma.internal.unflatten_batch_dims(R, batch_shape)
+    if not return_singular_values:
+        return R
+    else:
+        DS = D.clone()
+        if force_rotation:
+            DS[flip, -1] *= -1
+        del D
+        return R, DS
 
 
-def special_procrustes_naive(M):
+def special_procrustes_naive(M, return_singular_values : bool = False):
     """
     Implementation of :func:`~roma.mappings.special_procrustes` relying on default backward pass of autograd and SVD decomposition.
     Could be slightly less stable than :func:`~roma.mappings.special_procrustes`.
     """
-    return procrustes_naive(M, force_rotation=True)
+    return procrustes_naive(M, force_rotation=True, return_singular_values=return_singular_values)
 
 def special_gramschmidt(M, epsilon=0):
     """
     Returns the 3x3 rotation matrix obtained by Gram-Schmidt orthonormalization of two 3D input vectors (first two columns of input matrix M).
 
     Args:
         M (...x3xN tensor): batch of 3xN matrices, with N >= 2.
```

### Comparing `roma-1.3.3/roma/utils.py` & `roma-1.3.4/roma/utils.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.3/roma.egg-info/PKG-INFO` & `roma-1.3.4/roma.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.3.3
+Version: 1.3.4
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -62,22 +62,26 @@
 
 
 ## Installation
 The easiest way to install *RoMa* is to use pip:
 ```
 pip install roma
 ```
-We also recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
-to achieve significant speed-up with the _special_procrustes_ function on a CUDA GPU.
 
 Alternatively one can install the latest version of *RoMa* directly from the source repository:
 ```
 pip install git+https://github.com/naver/roma
 ```
 
+**For pytorch versions older than 1.8**, we recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
+to achieve a significant speed-up with `special_procrustes` on CUDA GPUs.
+You can check that this module is properly loaded using the function `roma.utils.is_torch_batch_svd_available()`.
+**With recent pytorch installations (torch>=1.8), `torch-batch-svd` is no longer needed or used.**
+
+
 ## License
 *RoMa*, Copyright (c) 2021 NAVER Corp., is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
 
 Bits of code were adapted from SciPy. Documentation is generated, distributed and displayed with the support of Sphinx and other materials (see [notice](https://github.com/naver/roma/blob/master/NOTICE)).
 
 ## References
 For a more in-depth discussion regarding differentiable mappings on the rotation space, please refer to:
```

### Comparing `roma-1.3.3/setup.py` & `roma-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="roma",
-    version="1.3.3",
+    version="1.3.4",
     author="Romain Brégier",
     author_email="romain.bregier@naverlabs.com",
     description="A lightweight library to deal with 3D rotations in PyTorch.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/naver/roma",
     packages=["roma"],
```

### Comparing `roma-1.3.3/test/test_derivatives.py` & `roma-1.3.4/test/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.3/test/test_mappings.py` & `roma-1.3.4/test/test_mappings.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.3/test/test_procrustes_derivatives.py` & `roma-1.3.4/test/test_procrustes_derivatives.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.3/test/test_utils.py` & `roma-1.3.4/test/test_utils.py`

 * *Files identical despite different names*

