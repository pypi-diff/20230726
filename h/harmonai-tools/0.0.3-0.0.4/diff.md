# Comparing `tmp/harmonai-tools-0.0.3.tar.gz` & `tmp/harmonai-tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonai-tools-0.0.3.tar", last modified: Thu Jul 20 08:28:29 2023, max compression
+gzip compressed data, was "harmonai-tools-0.0.4.tar", last modified: Wed Jul 26 16:18:13 2023, max compression
```

## Comparing `harmonai-tools-0.0.3.tar` & `harmonai-tools-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.3/README.md
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/__init__.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/data/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/data/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.3/harmonai_tools/data/dataset.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/data/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/inference/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/inference/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2961 2023-07-20 08:07:05.000000 harmonai-tools-0.0.3/harmonai_tools/inference/generation.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5195 2023-07-10 05:18:12.000000 harmonai-tools-0.0.3/harmonai_tools/inference/sampling.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/interface/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.3/harmonai_tools/interface/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4641 2023-07-20 08:25:46.000000 harmonai-tools-0.0.3/harmonai_tools/interface/gradio.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/models/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/models/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15254 2023-07-12 02:44:15.000000 harmonai-tools-0.0.3/harmonai_tools/models/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.3/harmonai_tools/models/blocks.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.3/harmonai_tools/models/bottleneck.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12143 2023-07-18 19:21:16.000000 harmonai-tools-0.0.3/harmonai_tools/models/conditioners.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17998 2023-07-15 04:57:40.000000 harmonai-tools-0.0.3/harmonai_tools/models/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.3/harmonai_tools/models/discriminators.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4114 2023-07-12 03:20:54.000000 harmonai-tools-0.0.3/harmonai_tools/models/factory.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.3/harmonai_tools/models/pretransforms.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/models/wavelets.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/training/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.3/harmonai_tools/training/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11803 2023-07-19 19:11:44.000000 harmonai-tools-0.0.3/harmonai_tools/training/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18736 2023-07-11 18:15:31.000000 harmonai-tools-0.0.3/harmonai_tools/training/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4457 2023-07-12 02:51:29.000000 harmonai-tools-0.0.3/harmonai_tools/training/factory.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1041 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      417 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/top_level.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.3/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1096 2023-07-20 08:28:12.000000 harmonai-tools-0.0.3/setup.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/LICENSE
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.4/README.md
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/__init__.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools/data/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/data/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.4/harmonai_tools/data/dataset.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/data/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/inference/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/inference/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3162 2023-07-22 08:03:32.000000 harmonai-tools-0.0.4/harmonai_tools/inference/generation.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5146 2023-07-22 08:03:42.000000 harmonai-tools-0.0.4/harmonai_tools/inference/sampling.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      798 2023-07-25 21:08:25.000000 harmonai-tools-0.0.4/harmonai_tools/inference/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/interface/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.4/harmonai_tools/interface/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     7186 2023-07-26 16:13:56.000000 harmonai-tools-0.0.4/harmonai_tools/interface/gradio.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/models/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/models/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15321 2023-07-24 20:06:26.000000 harmonai-tools-0.0.4/harmonai_tools/models/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.4/harmonai_tools/models/blocks.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.4/harmonai_tools/models/bottleneck.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12143 2023-07-18 19:21:16.000000 harmonai-tools-0.0.4/harmonai_tools/models/conditioners.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18798 2023-07-23 21:05:39.000000 harmonai-tools-0.0.4/harmonai_tools/models/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.4/harmonai_tools/models/discriminators.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4148 2023-07-21 07:18:52.000000 harmonai-tools-0.0.4/harmonai_tools/models/factory.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.4/harmonai_tools/models/pretransforms.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/models/wavelets.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/training/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.4/harmonai_tools/training/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11972 2023-07-24 20:17:16.000000 harmonai-tools-0.0.4/harmonai_tools/training/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    27359 2023-07-21 05:02:50.000000 harmonai-tools-0.0.4/harmonai_tools/training/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5184 2023-07-21 03:28:12.000000 harmonai-tools-0.0.4/harmonai_tools/training/factory.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1075 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      424 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/requires.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/top_level.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.4/pyproject.toml
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/setup.cfg
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1103 2023-07-26 16:16:21.000000 harmonai-tools-0.0.4/setup.py
```

### Comparing `harmonai-tools-0.0.3/LICENSE` & `harmonai-tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/data/dataset.py` & `harmonai-tools-0.0.4/harmonai_tools/data/dataset.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/data/utils.py` & `harmonai-tools-0.0.4/harmonai_tools/data/utils.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/inference/generation.py` & `harmonai-tools-0.0.4/harmonai_tools/inference/generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,34 +44,38 @@
     #sampled = sample(model.model, noise, steps, 0, **conditioning_tensors, embedding_scale=cfg_scale)
     
     if init_audio is not None:
         in_sr, init_audio = init_audio
 
         init_audio = init_audio.to(device)
 
-        print(f"Init audio: {init_audio}")
-
         if in_sr != sample_rate:
             resample_tf = T.Resample(in_sr, sample_rate).to(device)
             init_audio = resample_tf(init_audio)
 
         init_audio = PadCrop(sample_size, randomize=False)(init_audio)
 
         # Add batch dimension if needed
         if len(init_audio.shape) == 2:
-            init_audio = init_audio.unsqueeze(0)       
+            init_audio = init_audio.unsqueeze(0)
 
         io_channels = model.io_channels
 
         if model.pretransform is not None:
             io_channels = model.pretransform.io_channels
 
         if io_channels == 1:
             # Convert to mono
             init_audio = init_audio.mean(1, keepdim=True)
+        elif io_channels == 2:
+            # Convert to stereo
+            if init_audio.shape[1] == 1:
+                init_audio = init_audio.repeat(1, 2, 1)
+            elif init_audio.shape[1] > 2:
+                init_audio = init_audio[:, :2, :]
 
         if model.pretransform is not None:
             init_audio = model.pretransform.encode(init_audio)
 
         sampled = variation_k(model.model, init_audio, init_noise_level, steps, **sampler_kwargs, **conditioning_tensors, cfg_scale=cfg_scale, batch_cfg=True, scale_cfg=True, device=device)
     else:
         if model.pretransform is not None:
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/inference/sampling.py` & `harmonai-tools-0.0.4/harmonai_tools/inference/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         
 
 def variation_k(model_fn, init_audio, init_noise_level=0.1, steps=100, sampler_type="dpmpp-2m-sde", sigma_max=80, sigma_min=0.5, rho=1.0, device="cuda", **extra_args):
 
     denoiser = K.external.VDenoiser(model_fn)
     sigmas = K.sampling.get_sigmas_polyexponential(steps, sigma_min, init_noise_level, rho, device=device)
 
-    init_audio = init_audio + torch.randn_like(init_audio) * init_noise_level #sigmas[0]
-
-    print(f"sigmas[0]: {sigmas[0]}")
+    init_audio = init_audio + torch.randn_like(init_audio) * init_noise_level
 
     with torch.cuda.amp.autocast():
         if sampler_type == "k-heun":
             return K.sampling.sample_heun(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
         elif sampler_type == "k-lms":
             return K.sampling.sample_lms(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
         elif sampler_type == "k-dpmpp-2s-ancestral":
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/autoencoders.py` & `harmonai-tools-0.0.4/harmonai_tools/models/autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,16 @@
 class OobleckDecoder(nn.Module):
     def __init__(self, 
                  out_channels=2, 
                  channels=128, 
                  latent_dim=32, 
                  c_mults = [1, 2, 4, 8], 
                  strides = [2, 4, 8, 8],
-                 use_snake=False):
+                 use_snake=False,
+                 final_tanh=True):
         super().__init__()
 
         c_mults = [1] + c_mults
         
         self.depth = len(c_mults)
 
         layers = [
@@ -177,15 +178,15 @@
         
         for i in range(self.depth-1, 0, -1):
             layers += [DecoderBlock(in_channels=c_mults[i]*channels, out_channels=c_mults[i-1]*channels, stride=strides[i-1], use_snake=use_snake)]
 
         layers += [
             Activation1d(SnakeBeta(c_mults[0] * channels)) if use_snake else nn.ELU(),
             WNConv1d(in_channels=c_mults[0] * channels, out_channels=out_channels, kernel_size=7, padding=3),
-            nn.Tanh()
+            nn.Tanh() if final_tanh else nn.Identity()
         ]
 
         self.layers = nn.Sequential(*layers)
 
     def forward(self, x):
         return self.layers(x)
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/blocks.py` & `harmonai-tools-0.0.4/harmonai_tools/models/blocks.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/bottleneck.py` & `harmonai-tools-0.0.4/harmonai_tools/models/bottleneck.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/conditioners.py` & `harmonai-tools-0.0.4/harmonai_tools/models/conditioners.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/diffusion.py` & `harmonai-tools-0.0.4/harmonai_tools/models/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,47 +87,55 @@
             self, 
             model: ConditionedDiffusionModel,
             conditioner: MultiConditioner,
             io_channels = 2,
             pretransform: Pretransform = None,
             cross_attn_cond_ids: tp.List[str] = [],
             global_cond_ids: tp.List[str] = [],
+            input_concat_ids: tp.List[str] = []
             ):
         super().__init__()
 
         self.model = model
         self.conditioner = conditioner
         self.io_channels = io_channels
         self.pretransform = pretransform
         self.cross_attn_cond_ids = cross_attn_cond_ids
         self.global_cond_ids = global_cond_ids
+        self.input_concat_ids = input_concat_ids
 
     def get_conditioning_inputs(self, cond: tp.Dict[str, tp.Any]):
         cross_attention_input = None
         cross_attention_masks = None
         global_cond = None
+        input_concat_cond = None
 
         if len(self.cross_attn_cond_ids) > 0:
             # Concatenate all cross-attention inputs over the sequence dimension
             # Assumes that the cross-attention inputs are of shape (batch, seq, channels)
             cross_attention_input = torch.cat([cond[key][0] for key in self.cross_attn_cond_ids], dim=1)
             cross_attention_masks = torch.cat([cond[key][1] for key in self.cross_attn_cond_ids], dim=1)
 
         if len(self.global_cond_ids) > 0:
             # Concatenate all global conditioning inputs over the channel dimension
             # Assumes that the global conditioning inputs are of shape (batch, channels)
             global_cond = torch.cat([cond[key][0] for key in self.global_cond_ids], dim=-1)
             if len(global_cond.shape) == 3:
                 global_cond = global_cond.squeeze(1)
         
+        if len(self.input_concat_ids) > 0:
+            # Concatenate all input concat conditioning inputs over the channel dimension
+            # Assumes that the input concat conditioning inputs are of shape (batch, channels, seq)
+            input_concat_cond = torch.cat([cond[key][0] for key in self.input_concat_ids], dim=1)
 
         return {
             "cross_attn_cond": cross_attention_input,
             "cross_attn_masks": cross_attention_masks,
-            "global_cond": global_cond
+            "global_cond": global_cond,
+            "input_concat_cond": input_concat_cond
         }
 
     def forward(self, x: torch.Tensor, t: torch.Tensor, cond: tp.Dict[str, tp.Any], **kwargs):
         outputs = self.model(x, t, **self.get_conditioning_inputs(cond), **kwargs)
         return outputs
     
     def generate(self, *args, **kwargs):
@@ -135,15 +143,15 @@
 
 class UNetCFG1DWrapper(ConditionedDiffusionModel):
     def __init__(
         self, 
         *args,
         **kwargs
     ):
-        super().__init__(supports_cross_attention=True, supports_global_cond=True, supports_input_concat=False)
+        super().__init__(supports_cross_attention=True, supports_global_cond=True, supports_input_concat=True)
 
         self.model = UNetCFG1d(*args, **kwargs)
 
         with torch.no_grad():
             for param in self.model.parameters():
                 param *= 0.5
 
@@ -159,20 +167,25 @@
                 batch_cfg: bool = False,
                 scale_cfg: bool = False,
                 **kwargs):
         p = Profiler()
 
         p.tick("start")
 
+        channels_list = None
+        if input_concat_cond is not None:
+            channels_list = [input_concat_cond]
+
         outputs = self.model(
             x, 
             t, 
             embedding=cross_attn_cond, 
             embedding_mask=cross_attn_masks, 
             features=global_cond, 
+            channels_list=channels_list,
             embedding_scale=cfg_scale, 
             embedding_mask_proba=cfg_dropout_prob, 
             batch_cfg=batch_cfg,
             scale_cfg=scale_cfg,
             **kwargs)
         
         p.tick("UNetCFG1D forward")
@@ -213,22 +226,22 @@
         block = nn.Identity()
 
         conv_block = partial(ResConvBlock, kernel_size=kernel_size, conv_bias = conv_bias, use_snake=use_snake)
 
         for i in range(depth, 0, -1):
             c = channels[i - 1]
             stride = strides[i-1]
-            if stride != 2 and not learned_resample:
+            if stride > 2 and not learned_resample:
                 raise ValueError("Must have stride 2 without learned resampling")
             
             if i > 1:
                 c_prev = channels[i - 2]
                 add_attn = i >= attn_layer and n_attn_layers > 0
                 block = SkipBlock(
-                    Downsample1d_2(c_prev, c_prev, stride) if learned_resample else Downsample1d("cubic"),
+                    Downsample1d_2(c_prev, c_prev, stride) if (learned_resample or stride == 1) else Downsample1d("cubic"),
                     conv_block(c_prev, c, c),
                     SelfAttention1d(
                         c, c // 32) if add_attn else nn.Identity(),
                     conv_block(c, c, c),
                     SelfAttention1d(
                         c, c // 32) if add_attn else nn.Identity(),
                     conv_block(c, c, c),
@@ -488,20 +501,22 @@
     conditioning_config = model_config.get('conditioning', None)
     assert conditioning_config is not None, "Must specify conditioning config"
 
     conditioner = create_multi_conditioner_from_conditioning_config(conditioning_config)
 
     cross_attention_ids = diffusion_config.get('cross_attention_cond_ids', [])
     global_cond_ids = diffusion_config.get('global_cond_ids', [])
+    input_concat_ids = diffusion_config.get('input_concat_ids', [])
 
     pretransform = model_config.get("pretransform", None)
     if pretransform is not None:
         pretransform = create_pretransform_from_config(pretransform)
 
     return ConditionedDiffusionModelWrapper(
         diffusion_model, 
         conditioner, 
         cross_attn_cond_ids=cross_attention_ids,
         global_cond_ids=global_cond_ids,
+        input_concat_ids=input_concat_ids,
         pretransform=pretransform, 
         io_channels=io_channels
     )
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/discriminators.py` & `harmonai-tools-0.0.4/harmonai_tools/models/discriminators.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/factory.py` & `harmonai-tools-0.0.4/harmonai_tools/models/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     if model_type == 'autoencoder':
         from .autoencoders import create_autoencoder_from_config
         return create_autoencoder_from_config(model_config["model"])
     elif model_type == 'diffusion_uncond':
         from .diffusion import create_diffusion_uncond_from_config
         return create_diffusion_uncond_from_config(model_config["model"])
-    elif model_type == 'diffusion_cond':
+    elif model_type == 'diffusion_cond' or model_type == 'diffusion_cond_inpaint':
         from .diffusion import create_diffusion_cond_from_config
         return create_diffusion_cond_from_config(model_config["model"])
     elif model_type == 'diffusion_autoencoder':
         from .autoencoders import create_diffAE_from_config
         return create_diffAE_from_config(model_config["model"])
     else:
         raise NotImplementedError(f'Unknown model type: {model_type}')
@@ -39,16 +39,16 @@
         levels = wavelet_config["levels"]
         wavelet = wavelet_config["wavelet"]
 
         pretransform = WaveletPretransform(channels, levels, wavelet)
     else:
         raise NotImplementedError(f'Unknown pretransform type: {pretransform_type}')
     
-    requires_grad = pretransform_config.get('requires_grad', False)
-    pretransform.requires_grad = requires_grad
+    enable_grad = pretransform_config.get('enable_grad', False)
+    pretransform.enable_grad = enable_grad
 
     return pretransform
 
 def create_bottleneck_from_config(bottleneck_config):
     bottleneck_type = bottleneck_config.get('type', None)
 
     assert bottleneck_type is not None, 'type must be specified in bottleneck config'
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/pretransforms.py` & `harmonai-tools-0.0.4/harmonai_tools/models/pretransforms.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/models/wavelets.py` & `harmonai-tools-0.0.4/harmonai_tools/models/wavelets.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.3/harmonai_tools/training/autoencoders.py` & `harmonai-tools-0.0.4/harmonai_tools/training/autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,21 @@
             l1_time_loss = l1_time_loss * self.loss_config['time']['weights']['l1']
 
             # Combine spectral loss, KL loss, time-domain loss, and adversarial loss
             loss = mrstft_loss + loss_adv + feature_matching_distance #+ l1_time_loss
 
             if isinstance(self.autoencoder.bottleneck, VAEBottleneck) or isinstance(self.autoencoder.bottleneck, DACRVQVAEBottleneck) or isinstance(self.autoencoder.bottleneck, RVQVAEBottleneck):
                 kl = encoder_info['kl']
-                kl_loss = 1e-6 * kl 
+
+                try:
+                    kl_weight = self.loss_config['bottleneck']['weights']['kl']
+                except:
+                    kl_weight = 1e-6
+
+                kl_loss = kl_weight * kl 
                 loss = loss + kl_loss
 
             if isinstance(self.autoencoder.bottleneck, RVQBottleneck) or isinstance(self.autoencoder.bottleneck, RVQVAEBottleneck):
                 quantizer_loss = encoder_info['quantizer_loss']
                 loss = loss + quantizer_loss
                 
             if isinstance(self.autoencoder.bottleneck, DACRVQBottleneck) or isinstance(self.autoencoder.bottleneck, DACRVQVAEBottleneck):
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/training/diffusion.py` & `harmonai-tools-0.0.4/harmonai_tools/training/diffusion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytorch_lightning as pl
 import sys, gc
+import random
 import torch
 import torchaudio
 import typing as tp
 import wandb
 
 from aeiou.viz import pca_point_cloud, audio_spectrogram_image, tokens_spectrogram_image
 from ema_pytorch import EMA
@@ -351,14 +352,247 @@
         except Exception as e:
             raise e
         finally:
             gc.collect()
             torch.cuda.empty_cache()
             module.train()
 
+class DiffusionCondInpaintTrainingWrapper(pl.LightningModule):
+    '''
+    Wrapper for training a conditional audio diffusion model.
+    '''
+    def __init__(
+            self,
+            model: ConditionedDiffusionModelWrapper,
+            lr: float = 1e-4,
+    ):
+        super().__init__()
+
+        self.diffusion = model
+        
+        self.diffusion_ema = EMA(
+            self.diffusion.model,
+            beta=0.9999,
+            power=3/4,
+            update_every=1,
+            update_after_step=1
+        )
+
+        self.lr = lr
+
+        self.rng = torch.quasirandom.SobolEngine(1, scramble=True)
+
+    def configure_optimizers(self):
+        return optim.Adam([*self.diffusion.parameters()], lr=self.lr)
+
+    def random_mask(self, sequence, max_mask_length):
+
+        b, _, sequence_length = sequence.size()
+
+        # Create a mask tensor for each batch element
+        masks = []
+        for i in range(b):
+            # Randomly choose the length and starting index of the mask
+            mask_length = random.randint(1, max_mask_length)
+            mask_start = random.randint(0, sequence_length-mask_length)
+
+            # Create the mask tensor
+            mask = torch.ones((1, 1, sequence_length))
+            mask[:, :, mask_start:mask_start+mask_length] = 0
+            mask = mask.to(sequence.device)
+
+            masks.append(mask)
+
+        # Concatenate the mask tensors into a single tensor
+        mask = torch.cat(masks, dim=0).to(sequence.device)
+
+        # Apply the mask to the sequence tensor for each batch element
+        masked_sequence = sequence * mask
+
+        return masked_sequence, mask
+
+    def training_step(self, batch, batch_idx):
+        reals, metadata = batch
+
+        p = Profiler()
+
+        if reals.ndim == 4 and reals.shape[0] == 1:
+            reals = reals[0]
+
+        # Draw uniformly distributed continuous timesteps
+        t = self.rng.draw(reals.shape[0])[:, 0].to(self.device)
+
+        # Calculate the noise schedule parameters for those timesteps
+        alphas, sigmas = get_alphas_sigmas(t)
+
+        diffusion_input = reals
+
+        p.tick("setup")
+        
+        with torch.cuda.amp.autocast():
+            conditioning = self.diffusion.conditioner(metadata, self.device)
+
+        p.tick("conditioning")
+
+        if self.diffusion.pretransform is not None:
+            self.diffusion.pretransform.to(self.device)
+            with torch.set_grad_enabled(self.diffusion.pretransform.enable_grad):
+                diffusion_input = self.diffusion.pretransform.encode(diffusion_input)
+                p.tick("pretransform")
+
+        max_mask_length = diffusion_input.shape[2] // 2
+
+        # Create a mask of random length for a random slice of the input
+        masked_input, mask = self.random_mask(diffusion_input, max_mask_length)
+
+        conditioning['inpaint_mask'] = [mask]
+        conditioning['inpaint_masked_input'] = [masked_input]
+
+        # Combine the ground truth images and the noise
+        alphas = alphas[:, None, None]
+        sigmas = sigmas[:, None, None]
+        noise = torch.randn_like(diffusion_input)
+        noised_inputs = diffusion_input * alphas + noise * sigmas
+        targets = noise * alphas - diffusion_input * sigmas
+
+        p.tick("noise")
+
+        with torch.cuda.amp.autocast():
+            p.tick("amp")
+            v = self.diffusion(noised_inputs, t, cond=conditioning, cfg_dropout_prob = 0.1)
+            p.tick("diffusion")
+            mse_loss = F.mse_loss(v, targets)
+            
+            # Check if mse_loss is NaN
+            if torch.isnan(mse_loss).any():
+                torch.set_printoptions(threshold=10000)
+                print("NaN")
+                md_string = [f"{md['prompt'], md['seconds_start'], md['seconds_total']}" for md in metadata]
+                print(f"Conditioning: {conditioning}")
+                print('\n\n'.join(md_string))
+                #print(f"t: {t}")
+                #print(f"v: {v}")
+
+            loss = mse_loss
+
+        log_dict = {
+            'train/loss': loss.detach(),
+            'train/mse_loss': mse_loss.detach(),
+            'train/std_data': diffusion_input.std(),
+        }
+
+        self.log_dict(log_dict, prog_bar=True, on_step=True)
+        p.tick("log")
+        #print(f"Profiler: {p}")
+        return loss
+    
+    def on_before_zero_grad(self, *args, **kwargs):
+        self.diffusion_ema.update()
+
+    def export_model(self, path):
+        self.diffusion.model = self.diffusion_ema.ema_model
+        export_state_dict = {"state_dict": self.diffusion.state_dict()}
+        
+        torch.save(export_state_dict, path)
+
+class DiffusionCondInpaintDemoCallback(pl.Callback):
+    def __init__(
+        self, 
+        demo_dl, 
+        demo_every=2000,
+        demo_steps=250,
+        sample_size=65536,
+        sample_rate=48000,
+        demo_cfg_scales: tp.Optional[tp.List[int]] = [3, 5, 7]
+    ):
+        super().__init__()
+        self.demo_every = demo_every
+        self.demo_steps = demo_steps
+        self.demo_samples = sample_size
+        self.demo_dl = iter(demo_dl)
+        self.sample_rate = sample_rate
+        self.demo_cfg_scales = demo_cfg_scales
+        self.last_demo_step = -1
+
+    @rank_zero_only
+    @torch.no_grad()
+    def on_train_batch_end(self, trainer, module: DiffusionCondTrainingWrapper, outputs, batch, batch_idx): 
+        if (trainer.global_step - 1) % self.demo_every != 0 or self.last_demo_step == trainer.global_step:
+            return
+        
+        self.last_demo_step = trainer.global_step
+
+        try:
+            log_dict = {}
+
+            demo_reals, metadata = next(self.demo_dl)
+
+            # Remove extra dimension added by WebDataset
+            if demo_reals.ndim == 4 and demo_reals.shape[0] == 1:
+                demo_reals = demo_reals[0]
+
+            demo_reals = demo_reals.to(module.device)
+
+
+            # Log the real audio
+            log_dict[f'demo_reals_melspec_left'] = wandb.Image(audio_spectrogram_image(rearrange(demo_reals, "b d n -> d (b n)").mul(32767).to(torch.int16).cpu()))
+            # log_dict[f'demo_reals'] = wandb.Audio(rearrange(demo_reals, "b d n -> d (b n)").mul(32767).to(torch.int16).cpu(), sample_rate=self.sample_rate, caption="demo reals")
+
+            if module.diffusion.pretransform is not None:
+                    demo_reals = module.diffusion.pretransform.encode(demo_reals)
+
+            demo_samples = demo_reals.shape[2]
+
+            # Get conditioning
+            conditioning = module.diffusion.conditioner(metadata, module.device)
+
+            masked_input, mask = module.random_mask(demo_reals, demo_reals.shape[2] // 2)
+
+            conditioning['inpaint_mask'] = [mask]
+            conditioning['inpaint_masked_input'] = [masked_input]
+
+            if module.diffusion.pretransform is not None:
+                log_dict[f'demo_masked_input'] = wandb.Image(tokens_spectrogram_image(masked_input.cpu()))
+            else:
+                log_dict[f'demo_masked_input'] = wandb.Image(audio_spectrogram_image(rearrange(masked_input, "b c t -> c (b t)").mul(32767).to(torch.int16).cpu()))
+
+            cond_inputs = module.diffusion.get_conditioning_inputs(conditioning)
+
+            noise = torch.randn([demo_reals.shape[0], module.diffusion.io_channels, demo_samples]).to(module.device)
+
+            trainer.logger.experiment.log(log_dict)
+
+            for cfg_scale in self.demo_cfg_scales:
+                
+                print(f"Generating demo for cfg scale {cfg_scale}")
+                fakes = sample(module.diffusion_ema.model, noise, self.demo_steps, 0, **cond_inputs, cfg_scale=cfg_scale, batch_cfg=True)
+
+                if module.diffusion.pretransform is not None:
+                    fakes = module.diffusion.pretransform.decode(fakes)
+
+                # Put the demos together
+                fakes = rearrange(fakes, 'b d n -> d (b n)')
+
+                log_dict = {}
+                
+                filename = f'demo_cfg_{cfg_scale}_{trainer.global_step:08}.wav'
+                fakes = fakes.clamp(-1, 1).mul(32767).to(torch.int16).cpu()
+                torchaudio.save(filename, fakes, self.sample_rate)
+
+                log_dict[f'demo_cfg_{cfg_scale}'] = wandb.Audio(filename,
+                                                    sample_rate=self.sample_rate,
+                                                    caption=f'Reconstructed')
+            
+                log_dict[f'demo_melspec_left_cfg_{cfg_scale}'] = wandb.Image(audio_spectrogram_image(fakes))
+
+                trainer.logger.experiment.log(log_dict)
+        except Exception as e:
+            print(f'{type(e).__name__}: {e}')
+            raise e
+
 class DiffusionAutoencoderTrainingWrapper(pl.LightningModule):
     '''
     Wrapper for training an unconditional audio diffusion model (like Dance Diffusion).
     '''
     def __init__(
             self,
             model: DiffusionAutoencoder,
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools/training/factory.py` & `harmonai-tools-0.0.4/harmonai_tools/training/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,20 @@
         )
     elif model_type == 'diffusion_cond':
         from .diffusion import DiffusionCondTrainingWrapper
         return DiffusionCondTrainingWrapper(
             model, 
             lr=training_config["learning_rate"]
         )
+    elif model_type == 'diffusion_cond_inpaint':
+        from .diffusion import DiffusionCondInpaintTrainingWrapper
+        return DiffusionCondInpaintTrainingWrapper(
+            model, 
+            lr=training_config["learning_rate"]
+        )
     elif model_type == 'diffusion_autoencoder':
         from .diffusion import DiffusionAutoencoderTrainingWrapper
         return DiffusionAutoencoderTrainingWrapper(
             model,
             lr=training_config["learning_rate"]
         )
     else:
@@ -96,9 +102,21 @@
             sample_size=model_config["sample_size"],
             sample_rate=model_config["sample_rate"],
             demo_steps=demo_config.get("demo_steps", 250), 
             num_demos=demo_config["num_demos"],
             demo_cfg_scales=demo_config["demo_cfg_scales"],
             demo_conditioning=demo_config["demo_cond"],
         )
+    elif model_type == "diffusion_cond_inpaint":
+        from .diffusion import DiffusionCondInpaintDemoCallback
+
+        return DiffusionCondInpaintDemoCallback(
+            demo_every=demo_config.get("demo_every", 2000), 
+            sample_size=model_config["sample_size"],
+            sample_rate=model_config["sample_rate"],
+            demo_steps=demo_config.get("demo_steps", 250),
+            demo_cfg_scales=demo_config["demo_cfg_scales"],
+            **kwargs
+        )
+
     else:
         raise NotImplementedError(f'Unknown model type: {model_type}')
```

### Comparing `harmonai-tools-0.0.3/harmonai_tools.egg-info/SOURCES.txt` & `harmonai-tools-0.0.4/harmonai_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 harmonai_tools.egg-info/top_level.txt
 harmonai_tools/data/__init__.py
 harmonai_tools/data/dataset.py
 harmonai_tools/data/utils.py
 harmonai_tools/inference/__init__.py
 harmonai_tools/inference/generation.py
 harmonai_tools/inference/sampling.py
+harmonai_tools/inference/utils.py
 harmonai_tools/interface/__init__.py
 harmonai_tools/interface/gradio.py
 harmonai_tools/models/__init__.py
 harmonai_tools/models/autoencoders.py
 harmonai_tools/models/blocks.py
 harmonai_tools/models/bottleneck.py
 harmonai_tools/models/conditioners.py
```

### Comparing `harmonai-tools-0.0.3/setup.py` & `harmonai-tools-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='harmonai-tools',
-    version='0.0.3',
+    version='0.0.4',
     url='https://github.com/Harmonai-org/harmonai-tools.git',
     author='Harmonai',
     description='Training and inference tools for generative audio models from Harmonai',
     packages=find_packages(),  
     install_requires=[
         'aeiou',
         'alias-free-torch',
         'audio-diffusion-pytorch-fork',
         'audio-metadata',
         'auraloss',
-        'descript-audio-codec',
+        'descript-audio-codec==0.0.3',
         'einops',
         'ema-pytorch',
         'encodec',
         'gradio',
         'importlib-resources==5.12.0',
         'k-diffusion',
         'laion_clap',
```

