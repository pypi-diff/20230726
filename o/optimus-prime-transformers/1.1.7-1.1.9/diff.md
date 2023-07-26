# Comparing `tmp/optimus-prime-transformers-1.1.7.tar.gz` & `tmp/optimus-prime-transformers-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.1.7.tar", last modified: Mon Jul 24 13:55:44 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.1.9.tar", last modified: Wed Jul 26 17:12:35 2023, max compression
```

## Comparing `optimus-prime-transformers-1.1.7.tar` & `optimus-prime-transformers-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55309 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55945 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/setup.py
```

### Comparing `optimus-prime-transformers-1.1.7/LICENSE` & `optimus-prime-transformers-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/PKG-INFO` & `optimus-prime-transformers-1.1.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.7
+Version: 1.1.9
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.7/README.md` & `optimus-prime-transformers-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1871,7 +1871,14 @@
     title   = {Scaling Vision Transformers to 22 Billion Parameters},
     author  = {Mostafa Dehghani and Josip Djolonga and Basil Mustafa and Piotr Padlewski and Jonathan Heek and Justin Gilmer and Andreas Steiner and Mathilde Caron and Robert Geirhos and Ibrahim M. Alabdulmohsin and Rodolphe Jenatton and Lucas Beyer and Michael Tschannen and Anurag Arnab and Xiao Wang and Carlos Riquelme and Matthias Minderer and Joan Puigcerver and Utku Evci and Manoj Kumar and Sjoerd van Steenkiste and Gamaleldin F. Elsayed and Aravindh Mahendran and Fisher Yu and Avital Oliver and Fantine Huot and Jasmijn Bastings and Mark Collier and Alexey A. Gritsenko and Vighnesh Birodkar and Cristina Nader Vasconcelos and Yi Tay and Thomas Mensink and Alexander Kolesnikov and Filip Paveti'c and Dustin Tran and Thomas Kipf and Mario Luvci'c and Xiaohua Zhai and Daniel Keysers and Jeremiah Harmsen and Neil Houlsby},
     year    = {2023}
 }
 ```
 
 *solve intelligence... then use that to solve everything else.* - Demis Hassabis
+
+
+
+## Todo
+* Integrate flash attention 2.0 cuda and make it optional so if set to true it'll download then compile
+* Integrate dynamic sparse attention in triton
+* Integrate Parallelization and distributed setup of The Attention
```

#### html2text {}

```diff
@@ -721,8 +721,11 @@
 Matthias Minderer and Joan Puigcerver and Utku Evci and Manoj Kumar and Sjoerd
 van Steenkiste and Gamaleldin F. Elsayed and Aravindh Mahendran and Fisher Yu
 and Avital Oliver and Fantine Huot and Jasmijn Bastings and Mark Collier and
 Alexey A. Gritsenko and Vighnesh Birodkar and Cristina Nader Vasconcelos and Yi
 Tay and Thomas Mensink and Alexander Kolesnikov and Filip Paveti'c and Dustin
 Tran and Thomas Kipf and Mario Luvci'c and Xiaohua Zhai and Daniel Keysers and
 Jeremiah Harmsen and Neil Houlsby}, year = {2023} } ``` *solve intelligence...
-then use that to solve everything else.* - Demis Hassabis
+then use that to solve everything else.* - Demis Hassabis ## Todo * Integrate
+flash attention 2.0 cuda and make it optional so if set to true it'll download
+then compile * Integrate dynamic sparse attention in triton * Integrate
+Parallelization and distributed setup of The Attention
```

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/__init__.py` & `optimus-prime-transformers-1.1.9/optimus_prime/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from packaging import version
 
 if version.parse(torch.__version__) >= version.parse('2.0.0'):
     from einops._torch_specific import allow_ops_in_compiled_graph
     allow_ops_in_compiled_graph()
 
-from optimus_prime.x_transformers import XTransformer, Encoder, Decoder, CrossAttender, Attention, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
+from optimus_prime.x_transformers import XTransformer, Encoder, Decoder, CrossAttender, Attention, AttentionLayers, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
 from optimus_prime.x_transformers import AndromedaEmbedding #, AndromedaBnBEmbedding
 
 # d
 from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
 from optimus_prime.nonautoregressive_wrapper import NonAutoregressiveWrapper
 from optimus_prime.continuous_autoregressive_wrapper import ContinuousAutoregressiveWrapper
 from optimus_prime.xl_autoregressive_wrapper import XLAutoregressiveWrapper
```

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/attend.py` & `optimus-prime-transformers-1.1.9/optimus_prime/attend.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,28 @@
         *,
         dropout = 0.,
         causal = False,
         heads = None,
         talking_heads = False,
         scale = None,
         qk_norm = False,
+        add_zero_kv=False,
         flash = False,
     ):
         super().__init__()
         self.scale = scale
         self.qk_norm = qk_norm
         self.causal = causal
         self.attn_fn = partial(F.softmax, dtype = torch.float32) if not qk_norm else F.softmax
 
         self.dropout = dropout
         self.attn_dropout = nn.Dropout(dropout)
 
+        self.add_zero_kv = add_zero_kv
+
         # talking heads
 
         assert not (flash and talking_heads), 'talking heads not compatible with flash attention'
 
         self.talking_heads = talking_heads
         if talking_heads:
             self.pre_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
@@ -191,14 +194,23 @@
         d - feature dimension
         """
 
         n, device = q.shape[-2], q.device
 
         scale = default(self.scale, q.shape[-1] ** -0.5)
 
+        if self.add_zero_kv:
+            k, v = map(lambda t: F.pad(t, (0, 0, 1, 0), value=0.), (k, v))
+
+            if exists(mask):
+                mask = F.pad(mask, (1, 0), value=True)
+
+            if exists(attn_bias):
+                attn_bias = F.pad(attn_bias, (1, 0), value=0.)
+
         if self.flash:
             assert not exists(prev_attn), 'residual attention not compatible with flash attention'
             return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
             # return FlashAttention(q, k, v, mask=mask, attn_bias=attn_bias )
 
         kv_einsum_eq = 'b j d' if k.ndim == 3 else 'b h j d'
```

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.9/optimus_prime/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.9/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/flash.py` & `optimus-prime-transformers-1.1.9/optimus_prime/flash.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.1.9/optimus_prime/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/x_transformers.py` & `optimus-prime-transformers-1.1.9/optimus_prime/x_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,18 @@
         return bias
 
 class RotaryEmbedding(nn.Module):
     def __init__(
         self,
         dim,
         use_xpos = False,
-        scale_base = 512
+        scale_base = 512,
+        interpolated = False,
+        max_postion_embeddings=None, #2048
+        base=None, #10000
     ):
         super().__init__()
         inv_freq = 1. / (10000 ** (torch.arange(0, dim, 2).float() / dim))
         self.register_buffer('inv_freq', inv_freq)
 
         if not use_xpos:
             self.register_buffer('scale', None)
@@ -450,26 +453,40 @@
 
         scale = (torch.arange(0, dim, 2) + 0.4 * dim) / (1.4 * dim)
 
         self.scale_base = scale_base
         self.register_buffer('scale', scale)
 
     def forward(self, seq_len, device):
-        t = torch.arange(seq_len, device = device).type_as(self.inv_freq)
-        freqs = torch.einsum('i , j -> i j', t, self.inv_freq)
-        freqs = torch.cat((freqs, freqs), dim = -1)
-
-        if not exists(self.scale):
-            return freqs, 1.
-
-        power = (torch.arange(seq_len, device = device) - (seq_len // 2)) / self.scale_base
-        scale = self.scale ** rearrange(power, 'n -> n 1')
-        scale = torch.cat((scale, scale), dim = -1)
 
-        return freqs, scale
+        if self.interpolated:
+            max_position_embeddings = self.max_position_embeddings
+            self.max_seq_len_cached = max_position_embeddings
+            t = torch.arange(
+                self.max_seq_len_cached,
+                device=self.inv_freq.device,
+                dtype=self.inv_freq.dtype,
+            )
+            #interpolation
+            self.scale = 1 / 4
+            t *= self.scale
+        else:
+                
+            t = torch.arange(seq_len, device = device).type_as(self.inv_freq)
+            freqs = torch.einsum('i , j -> i j', t, self.inv_freq)
+            freqs = torch.cat((freqs, freqs), dim = -1)
+
+            if not exists(self.scale):
+                return freqs, 1.
+
+            power = (torch.arange(seq_len, device = device) - (seq_len // 2)) / self.scale_base
+            scale = self.scale ** rearrange(power, 'n -> n 1')
+            scale = torch.cat((scale, scale), dim = -1)
+
+            return freqs, scale
 
 
 def rotate_half(x):
     x = rearrange(x, '... (j d) -> ... j d', j = 2)
     x1, x2 = x.unbind(dim = -2)
     return torch.cat((-x2, x1), dim = -1)
 
@@ -658,15 +675,16 @@
         qk_norm = False,
         qk_norm_groups = 1,
         qk_norm_scale = 10,
         qk_norm_dim_scale = False,
         one_kv_head = False,
         shared_kv = False,
         value_dim_head = None,
-        tensor_product = False   # https://arxiv.org/abs/2208.06061
+        tensor_product = False,  # https://arxiv.org/abs/2208.06061
+        add_zero_kv = False
     ):
         super().__init__()
         self.scale = dim_head ** -0.5
 
         self.heads = heads
         self.causal = causal
         self.max_attend_past = max_attend_past
@@ -719,14 +737,15 @@
         self.attend = Attend(
             heads = heads,
             causal = causal,
             talking_heads = talking_heads,
             dropout = dropout,
             qk_norm = qk_norm,
             scale = qk_norm_scale if qk_norm else self.scale,
+            add_zero_kv=add_zero_kv,
             flash = flash
         )
 
         # head scaling
         self.head_scale = head_scale
         if head_scale:
             self.head_scale_params = nn.Parameter(torch.ones(1, heads, 1, 1))
@@ -1270,15 +1289,15 @@
     def __init__(
         self,
         *,
         num_tokens,
         max_seq_len,
         attn_layers,
         # tokenizer: BaseTokenizer,
-        embedding_provider: BaseEmbedding,
+        embedding_provider,
         emb_dim = None,
         max_mem_len = 0.,
         shift_mem_down = 0,
         emb_dropout = 0.,
         post_emb_norm = False,
         num_memory_tokens = None,
         tie_embedding = False,
```

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.9/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.7
+Version: 1.1.9
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/SOURCES.txt` & `optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.7/setup.py` & `optimus-prime-transformers-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.7',
+  version = '1.1.9',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
```

