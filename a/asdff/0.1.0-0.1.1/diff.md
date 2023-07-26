# Comparing `tmp/asdff-0.1.0.tar.gz` & `tmp/asdff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asdff-0.1.0.tar", last modified: Fri Jul 21 13:29:13 2023, max compression
+gzip compressed data, was "asdff-0.1.1.tar", last modified: Sat Jul 22 00:55:32 2023, max compression
```

## Comparing `asdff-0.1.0.tar` & `asdff-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35184 2023-07-21 04:16:34.042881 asdff-0.1.0/LICENSE
--rw-r--r--   0        0        0     3426 2023-07-21 12:55:26.798856 asdff-0.1.0/README.md
--rw-r--r--   0        0        0      178 2023-07-21 10:43:29.239300 asdff-0.1.0/asdff/__init__.py
--rw-r--r--   0        0        0       23 2023-07-21 13:28:15.933316 asdff-0.1.0/asdff/__version__.py
--rw-r--r--   0        0        0     4282 2023-07-21 12:50:03.383098 asdff-0.1.0/asdff/sd.py
--rw-r--r--   0        0        0     1810 2023-07-21 12:51:58.465683 asdff-0.1.0/asdff/utils.py
--rw-r--r--   0        0        0     1993 2023-07-21 10:42:31.234547 asdff-0.1.0/asdff/yolo.py
--rw-r--r--   0        0        0      917 2023-07-21 13:29:13.746468 asdff-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 asdff-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2023-07-21 04:16:34.042881 asdff-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3436 2023-07-22 00:53:39.927745 asdff-0.1.1/README.md
+-rw-r--r--   0        0        0      178 2023-07-21 10:43:29.239300 asdff-0.1.1/asdff/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-22 00:55:05.426030 asdff-0.1.1/asdff/__version__.py
+-rw-r--r--   0        0        0     4356 2023-07-22 00:53:39.930172 asdff-0.1.1/asdff/sd.py
+-rw-r--r--   0        0        0     1810 2023-07-21 12:51:58.465683 asdff-0.1.1/asdff/utils.py
+-rw-r--r--   0        0        0     1993 2023-07-21 10:42:31.234547 asdff-0.1.1/asdff/yolo.py
+-rw-r--r--   0        0        0      949 2023-07-22 00:55:32.795355 asdff-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1299 2023-07-22 00:53:39.929618 asdff-0.1.1/tests/test_pipeline.py
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 asdff-0.1.1/PKG-INFO
```

### Comparing `asdff-0.1.0/LICENSE` & `asdff-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asdff-0.1.0/README.md` & `asdff-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,45 +28,49 @@
 
 pip 설치 필요없음
 
 ```py
 import torch
 from diffusers import DiffusionPipeline
 
-pipe = DiffusionPipeline.from_pretrained("stablediffusionapi/counterfeit-v30", torch_dtype=torch.float16, custom_pipeline="Bingsu/adetailer_pipeline")
+pipe = DiffusionPipeline.from_pretrained(
+    "stablediffusionapi/counterfeit-v30",
+    torch_dtype=torch.float16,
+    custom_pipeline="Bingsu/adsd_pipeline"
+)
 pipe.safety_checker = None
 pipe.to("cuda")
 
 common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 28}
 result = pipe(common=common)
 
 images = result[0]
 ```
 
 ## arguments
 
-- `common`: `Dict[str, Any] | None`
+- `common: Mapping[str, Any] | None`
 
 txt2img와 inpaint에서 공통적으로 사용할 인자들
 
-- `txt2img_only`: `Dict[str, Any] | None`
+- `txt2img_only: Mapping[str, Any] | None`
 
 txt2img에서만 사용할 인자. common과 겹치는 인자는 덮어씁니다.
 
-[`StableDiffusionPipeline.__call__`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__)
+[StableDiffusionPipeline.__call__](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__)
 
-- `inpaint_only`: `Dict[str, Any] | None`
+- `inpaint_only: Mapping[str, Any] | None`
 
 inpaint에서만 사용할 인자. common과 겹치는 인자는 덮어씁니다.
 
 `strength: 0.4`가 기본값으로 적용됩니다.
 
-[`StableDiffusionInpaintPipeline.__call__`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/inpaint#diffusers.StableDiffusionInpaintPipeline.__call__)
+[StableDiffusionInpaintPipeline.__call__](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/inpaint#diffusers.StableDiffusionInpaintPipeline.__call__)
 
-- `detectors`: `DetectorType | Iterable[DetectorType] | None`
+- `detectors: DetectorType | Iterable[DetectorType] | None`
 
 `DetectorType: Callable[[Image.Image], Optional[List[Image.Image]]]`
 
 pil Image를 입력으로 받아 마스크 이미지의 리스트(마스크), 또는 None을 반환하는 Callable.
 
 그런 Callable 하나, Callable의 리스트 또는 None
 
@@ -96,18 +100,18 @@
 person_model_path = hf_hub_download("Bingsu/adetailer", "person_yolov8s-seg.pt")
 person_detector = partial(yolo_detector, model_path=person_model_path)
 common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 28}
 result = pipe(common=common, detectors=[person_detector, pipe.default_detector])
 result
 ```
 
-- `mask_dilation`: int, default = 4
+- `mask_dilation: int, default = 4`
 
 마스크 감지 후, cv2.dilate 함수를 적용해 마스크 영역을 키우는 데, 이 때 적용할 커널의 크기.
 
-- `mask_blur`: int, default = 4
+- `mask_blur: int, default = 4`
 
 dilation 후 적용할 가우시안 블러의 커널 크기.
 
-- `mask_padding`: int, default = 32
+- `mask_padding: int, default = 32`
 
 dilation 적용 후 이 값만큼 bbox의 가로세로 영역을 더해서 이미지를 자른 뒤, inpaint를 시도하게 됩니다.
```

### Comparing `asdff-0.1.0/asdff/sd.py` & `asdff-0.1.1/asdff/sd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import cached_property
-from typing import Any, Callable, Iterable, List, Optional
+from typing import Any, Callable, Iterable, List, Mapping, Optional
 
 from diffusers import StableDiffusionInpaintPipeline, StableDiffusionPipeline
 from diffusers.utils import logging
 from PIL import Image
 
 from asdff.utils import (
     ADOutput,
@@ -25,43 +25,44 @@
 def ordinal(n: int) -> str:
     d = {1: "st", 2: "nd", 3: "rd"}
     return str(n) + ("th" if 11 <= n % 100 <= 13 else d.get(n % 10, "th"))
 
 
 class AdPipeline(StableDiffusionPipeline):
     @cached_property
-    def inpaine_pipeline(self):
+    def inpaint_pipeline(self):
         return StableDiffusionInpaintPipeline(
             vae=self.vae,
             text_encoder=self.text_encoder,
             tokenizer=self.tokenizer,
             unet=self.unet,
             scheduler=self.scheduler,
             safety_checker=self.safety_checker,
             feature_extractor=self.feature_extractor,
             requires_safety_checker=self.config.requires_safety_checker,
         )
 
     def __call__(  # noqa: C901
         self,
-        common: dict[str, Any] | None = None,
-        txt2img_only: dict[str, Any] | None = None,
-        inpaint_only: dict[str, Any] | None = None,
+        common: Mapping[str, Any] | None = None,
+        txt2img_only: Mapping[str, Any] | None = None,
+        inpaint_only: Mapping[str, Any] | None = None,
         detectors: DetectorType | Iterable[DetectorType] | None = None,
         mask_dilation: int = 4,
         mask_blur: int = 4,
         mask_padding: int = 32,
     ):
         if common is None:
             common = {}
         if txt2img_only is None:
             txt2img_only = {}
         if inpaint_only is None:
             inpaint_only = {}
-        inpaint_only.setdefault("strength", 0.4)
+        if "strength" not in inpaint_only:
+            inpaint_only = {**inpaint_only, "strength": 0.4}
 
         if detectors is None:
             detectors = [self.default_detector]
         elif callable(detectors):
             detectors = [detectors]
 
         txt2img_output = super().__call__(**common, **txt2img_only, output_type="pil")
@@ -91,15 +92,15 @@
                         continue
                     mask = mask_gaussian_blur(mask, mask_blur)
                     bbox_padded = bbox_padding(bbox, init_image.size, mask_padding)
 
                     crop_image = init_image.crop(bbox_padded)
                     crop_mask = mask.crop(bbox_padded)
 
-                    inpaint_output = self.inpaine_pipeline(
+                    inpaint_output = self.inpaint_pipeline(
                         **common,
                         **inpaint_only,
                         image=crop_image,
                         mask_image=crop_mask,
                         num_images_per_prompt=1,
                         output_type="pil",
                     )
```

### Comparing `asdff-0.1.0/asdff/utils.py` & `asdff-0.1.1/asdff/utils.py`

 * *Files identical despite different names*

### Comparing `asdff-0.1.0/asdff/yolo.py` & `asdff-0.1.1/asdff/yolo.py`

 * *Files identical despite different names*

### Comparing `asdff-0.1.0/pyproject.toml` & `asdff-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "diffusers[torch]>=0.18.2",
     "transformers>=4.25.1",
     "ultralytics",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.0"
+version = "0.1.1"
 
 [project.license]
 text = "AGPL-3.0"
 
 [project.urls]
 repository = "https://github.com/Bing-su/asdff"
 
@@ -29,14 +29,17 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black",
     "ruff",
     "pre-commit",
     "ipywidgets",
 ]
+test = [
+    "pytest>=7.4.0",
+]
 
 [tool.pdm.version]
 source = "file"
 path = "asdff/__version__.py"
 
 [tool.ruff]
 select = [
```

### Comparing `asdff-0.1.0/PKG-INFO` & `asdff-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdff
-Version: 0.1.0
+Version: 0.1.1
 Author-Email: Bingsu <ks2515@naver.com>
 License: AGPL-3.0
 Project-URL: Repository, https://github.com/Bing-su/asdff
 Requires-Python: >=3.8
 Requires-Dist: diffusers[torch]>=0.18.2
 Requires-Dist: transformers>=4.25.1
 Requires-Dist: ultralytics
@@ -40,45 +40,49 @@
 
 pip 설치 필요없음
 
 ```py
 import torch
 from diffusers import DiffusionPipeline
 
-pipe = DiffusionPipeline.from_pretrained("stablediffusionapi/counterfeit-v30", torch_dtype=torch.float16, custom_pipeline="Bingsu/adetailer_pipeline")
+pipe = DiffusionPipeline.from_pretrained(
+    "stablediffusionapi/counterfeit-v30",
+    torch_dtype=torch.float16,
+    custom_pipeline="Bingsu/adsd_pipeline"
+)
 pipe.safety_checker = None
 pipe.to("cuda")
 
 common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 28}
 result = pipe(common=common)
 
 images = result[0]
 ```
 
 ## arguments
 
-- `common`: `Dict[str, Any] | None`
+- `common: Mapping[str, Any] | None`
 
 txt2img와 inpaint에서 공통적으로 사용할 인자들
 
-- `txt2img_only`: `Dict[str, Any] | None`
+- `txt2img_only: Mapping[str, Any] | None`
 
 txt2img에서만 사용할 인자. common과 겹치는 인자는 덮어씁니다.
 
-[`StableDiffusionPipeline.__call__`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__)
+[StableDiffusionPipeline.__call__](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__)
 
-- `inpaint_only`: `Dict[str, Any] | None`
+- `inpaint_only: Mapping[str, Any] | None`
 
 inpaint에서만 사용할 인자. common과 겹치는 인자는 덮어씁니다.
 
 `strength: 0.4`가 기본값으로 적용됩니다.
 
-[`StableDiffusionInpaintPipeline.__call__`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/inpaint#diffusers.StableDiffusionInpaintPipeline.__call__)
+[StableDiffusionInpaintPipeline.__call__](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/inpaint#diffusers.StableDiffusionInpaintPipeline.__call__)
 
-- `detectors`: `DetectorType | Iterable[DetectorType] | None`
+- `detectors: DetectorType | Iterable[DetectorType] | None`
 
 `DetectorType: Callable[[Image.Image], Optional[List[Image.Image]]]`
 
 pil Image를 입력으로 받아 마스크 이미지의 리스트(마스크), 또는 None을 반환하는 Callable.
 
 그런 Callable 하나, Callable의 리스트 또는 None
 
@@ -108,18 +112,18 @@
 person_model_path = hf_hub_download("Bingsu/adetailer", "person_yolov8s-seg.pt")
 person_detector = partial(yolo_detector, model_path=person_model_path)
 common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 28}
 result = pipe(common=common, detectors=[person_detector, pipe.default_detector])
 result
 ```
 
-- `mask_dilation`: int, default = 4
+- `mask_dilation: int, default = 4`
 
 마스크 감지 후, cv2.dilate 함수를 적용해 마스크 영역을 키우는 데, 이 때 적용할 커널의 크기.
 
-- `mask_blur`: int, default = 4
+- `mask_blur: int, default = 4`
 
 dilation 후 적용할 가우시안 블러의 커널 크기.
 
-- `mask_padding`: int, default = 32
+- `mask_padding: int, default = 32`
 
 dilation 적용 후 이 값만큼 bbox의 가로세로 영역을 더해서 이미지를 자른 뒤, inpaint를 시도하게 됩니다.
```

