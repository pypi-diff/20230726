# Comparing `tmp/gigagan-pytorch-0.2.6.tar.gz` & `tmp/gigagan-pytorch-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.2.6.tar", last modified: Tue Jul 25 00:13:11 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.2.8.tar", last modified: Wed Jul 26 14:38:37 2023, max compression
```

## Comparing `gigagan-pytorch-0.2.6.tar` & `gigagan-pytorch-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:13:11.573897 gigagan-pytorch-0.2.6/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    83976 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83779 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/setup.py
```

### Comparing `gigagan-pytorch-0.2.6/LICENSE` & `gigagan-pytorch-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.6/PKG-INFO` & `gigagan-pytorch-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.6
+Version: 0.2.8
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.6/README.md` & `gigagan-pytorch-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,22 +104,23 @@
     generator = dict(
         style_network = dict(
             dim = 64,
             depth = 4
         ),
         dim = 32,
         image_size = 256,
-        input_image_size = 128,
+        input_image_size = 64,
         unconditional = True
     ),
     discriminator = dict(
         dim_capacity = 16,
         dim_max = 512,
         image_size = 256,
         num_skip_layers_excite = 4,
+        multiscale_input_resolutions = (128,),
         unconditional = True
     ),
     amp = True
 ).cuda()
 
 dataset = ImageDataset(
     folder = '/path/to/your/data',
@@ -136,15 +137,15 @@
 gan(
     steps = 100,
     grad_accum_every = 8
 )
 
 # after much training
 
-lowres = torch.randn(1, 3, 128, 128).cuda()
+lowres = torch.randn(1, 3, 64, 64).cuda()
 
 images = gan.generate(lowres) # (1, 3, 256, 256)
 ```
 
 ## Losses
 
 * `G` - Generator
```

#### html2text {}

```diff
@@ -24,31 +24,32 @@
 dataloader for the GAN before training gan.set_dataloader(dataloader) #
 training the discriminator and generator alternating # for 100 steps in this
 example, batch size 1, gradient accumulated 8 times gan( steps = 100,
 grad_accum_every = 8 ) # after much training images = gan.generate(batch_size =
 4) # (4, 3, 256, 256) ``` For unconditional Unet Upsampler ```python import
 torch from gigagan_pytorch import ( GigaGAN, ImageDataset ) gan = GigaGAN
 ( train_upsampler = True, # set this to True generator = dict( style_network =
-dict( dim = 64, depth = 4 ), dim = 32, image_size = 256, input_image_size =
-128, unconditional = True ), discriminator = dict( dim_capacity = 16, dim_max =
-512, image_size = 256, num_skip_layers_excite = 4, unconditional = True ), amp
-= True ).cuda() dataset = ImageDataset( folder = '/path/to/your/data',
-image_size = 256 ) dataloader = dataset.get_dataloader(batch_size = 1)
-gan.set_dataloader(dataloader) # training the discriminator and generator
-alternating # for 100 steps in this example, batch size 1, gradient accumulated
-8 times gan( steps = 100, grad_accum_every = 8 ) # after much training lowres =
-torch.randn(1, 3, 128, 128).cuda() images = gan.generate(lowres) # (1, 3, 256,
-256) ``` ## Losses * `G` - Generator * `MSG` - Multiscale Generator * `D` -
-Discriminator * `MSD` - Multiscale Discriminator * `GP` - Gradient Penalty *
-`SSL` - Auxiliary Reconstruction in Discriminator (from Lightweight GAN) * `VD`
-- Vision-aided Discriminator * `VG` - Vision-aided Generator * `CL` - Generator
-Constrastive Loss * `MAL` - Matching Aware Loss A healthy run would have `G`,
-`MSG`, `D`, `MSD` with values hovering between `0` to `10`, and usually staying
-pretty constant. If at any time after 1k training steps these values persist at
-triple digits, that would mean something is wrong. It is ok for generator and
+dict( dim = 64, depth = 4 ), dim = 32, image_size = 256, input_image_size = 64,
+unconditional = True ), discriminator = dict( dim_capacity = 16, dim_max = 512,
+image_size = 256, num_skip_layers_excite = 4, multiscale_input_resolutions =
+(128,), unconditional = True ), amp = True ).cuda() dataset = ImageDataset
+( folder = '/path/to/your/data', image_size = 256 ) dataloader =
+dataset.get_dataloader(batch_size = 1) gan.set_dataloader(dataloader) #
+training the discriminator and generator alternating # for 100 steps in this
+example, batch size 1, gradient accumulated 8 times gan( steps = 100,
+grad_accum_every = 8 ) # after much training lowres = torch.randn(1, 3, 64,
+64).cuda() images = gan.generate(lowres) # (1, 3, 256, 256) ``` ## Losses * `G`
+- Generator * `MSG` - Multiscale Generator * `D` - Discriminator * `MSD` -
+Multiscale Discriminator * `GP` - Gradient Penalty * `SSL` - Auxiliary
+Reconstruction in Discriminator (from Lightweight GAN) * `VD` - Vision-aided
+Discriminator * `VG` - Vision-aided Generator * `CL` - Generator Constrastive
+Loss * `MAL` - Matching Aware Loss A healthy run would have `G`, `MSG`, `D`,
+`MSD` with values hovering between `0` to `10`, and usually staying pretty
+constant. If at any time after 1k training steps these values persist at triple
+digits, that would mean something is wrong. It is ok for generator and
 discriminator values to occasionally dip negative, but it should swing back up
 to the range above. `GP` and `SSL` should be pushed towards `0`. `GP` can
 occasionally spike; I like to imagine it as the networks undergoing some
 epiphany ## Multi-GPU Training The `GigaGAN` class is now equipped with ð¤
 Accelerator. You can easily do multi-gpu training in two steps using their
 `accelerate` CLI At the project root directory, where the training script is,
 run ```python $ accelerate config ``` Then, in the same directory ```python $
```

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/data.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1758,15 +1758,14 @@
         vision_aided_divergence_loss_weight = 0.5,
         generator_contrastive_loss_weight = 0.1,
         matching_awareness_loss_weight = 0.1,
         calc_multiscale_loss_every = 1,
         apply_gradient_penalty_every = 4,
         resize_image_mode = 'bilinear',
         train_upsampler = False,
-        upsampler_replace_rgb_with_input_lowres_image = False,
         log_steps_every = 20,
         create_ema_generator_at_init = True,
         save_and_sample_every = 1000,
         early_save_thres_steps = 2500,
         early_save_and_sample_every = 100,
         num_samples = 25,
         model_folder = './gigagan-models',
@@ -1800,16 +1799,14 @@
 
         if train_upsampler:
             from gigagan_pytorch.unet_upsampler import UnetUpsampler
             generator_klass = UnetUpsampler
         else:
             generator_klass = Generator
 
-        self.upsampler_replace_rgb_with_input_lowres_image = upsampler_replace_rgb_with_input_lowres_image
-
         # gradient penalty and auxiliary recon loss
 
         self.apply_gradient_penalty_every = apply_gradient_penalty_every
         self.calc_multiscale_loss_every = calc_multiscale_loss_every
 
         if isinstance(generator, dict):
             generator = generator_klass(**generator)
@@ -1834,15 +1831,15 @@
         self.G = generator
         self.D = discriminator
         self.VD = vision_aided_discriminator
 
         # validate multiscale input resolutions
 
         if train_upsampler:
-            assert is_empty(set(discriminator.multiscale_input_resolutions) - set(generator.allowable_rgb_resolutions)), f'only multiscale input resolutions of {generator.allowable_rgb_resolutions} is allowed based on the unet input and output image size'
+            assert is_empty(set(discriminator.multiscale_input_resolutions) - set(generator.allowable_rgb_resolutions)), f'only multiscale input resolutions of {generator.allowable_rgb_resolutions} is allowed based on the unet input and output image size. simply do Discriminator(multiscale_input_resolutions = unet.allowable_rgb_resolutions) to resolve this error'
 
         # ema
 
         self.has_ema_generator = False
 
         if self.is_main and create_ema_generator_at_init:
             self.create_ema_generator()
@@ -2094,18 +2091,15 @@
 
         # if training upsample generator, need to downsample real images
 
         if self.train_upsampler:
             size = self.G.input_image_size
             lowres_real_images = F.interpolate(real_images, (size, size))
 
-            G_kwargs = dict(
-                lowres_image = lowres_real_images,
-                replace_rgb_with_input_lowres_image = self.upsampler_replace_rgb_with_input_lowres_image
-            )
+            G_kwargs = dict(lowres_image = lowres_real_images)
         else:
             assert exists(batch_size)
 
             G_kwargs = dict(batch_size = batch_size)
 
         # create noise
```

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.2.8/gigagan_pytorch/unet_upsampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         self.style_to_conv_modulations = nn.Linear(style_network.dim, sum(style_embed_split_dims))
         self.style_embed_split_dims = style_embed_split_dims
 
     @property
     def allowable_rgb_resolutions(self):
         input_res_base = int(log2(self.input_image_size))
         output_res_base = int(log2(self.image_size))
-        allowed_rgb_res_base = list(range(input_res_base + 1, output_res_base))
+        allowed_rgb_res_base = list(range(input_res_base, output_res_base))
         return [*map(lambda p: 2 ** p, allowed_rgb_res_base)]
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @property
@@ -589,21 +589,12 @@
         if not return_all_rgbs:
             return rgb
 
         # only keep those rgbs whose feature map is greater than the input image to be upsampled
 
         rgbs = list(filter(lambda t: t.shape[-1] > shape[-1], rgbs))
 
-        if not replace_rgb_with_input_lowres_image:
-            return rgb, rgbs
+        # and return the original input image as the smallest rgb
 
-        # replace the rgb of the corresponding same dimension as the input low res image
+        rgbs = [lowres_image, *rgbs]
 
-        output_rgbs = []
-
-        for rgb in rgbs:
-            if rgb.shape[-1] == lowres_image.shape[-1]:
-                output_rgbs.append(lowres_image)
-            else:
-                output_rgbs.append(rgb)
-
-        return rgb, output_rgbs
+        return rgb, rgbs
```

### Comparing `gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.6
+Version: 0.2.8
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.6/setup.py` & `gigagan-pytorch-0.2.8/setup.py`

 * *Files identical despite different names*

