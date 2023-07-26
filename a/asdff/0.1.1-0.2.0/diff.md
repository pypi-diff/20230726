# Comparing `tmp/asdff-0.1.1.tar.gz` & `tmp/asdff-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asdff-0.1.1.tar", last modified: Sat Jul 22 00:55:32 2023, max compression
+gzip compressed data, was "asdff-0.2.0.tar", last modified: Wed Jul 26 06:09:54 2023, max compression
```

## Comparing `asdff-0.1.1.tar` & `asdff-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35184 2023-07-21 04:16:34.042881 asdff-0.1.1/LICENSE
--rw-r--r--   0        0        0     3436 2023-07-22 00:53:39.927745 asdff-0.1.1/README.md
--rw-r--r--   0        0        0      178 2023-07-21 10:43:29.239300 asdff-0.1.1/asdff/__init__.py
--rw-r--r--   0        0        0       23 2023-07-22 00:55:05.426030 asdff-0.1.1/asdff/__version__.py
--rw-r--r--   0        0        0     4356 2023-07-22 00:53:39.930172 asdff-0.1.1/asdff/sd.py
--rw-r--r--   0        0        0     1810 2023-07-21 12:51:58.465683 asdff-0.1.1/asdff/utils.py
--rw-r--r--   0        0        0     1993 2023-07-21 10:42:31.234547 asdff-0.1.1/asdff/yolo.py
--rw-r--r--   0        0        0      949 2023-07-22 00:55:32.795355 asdff-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1299 2023-07-22 00:53:39.929618 asdff-0.1.1/tests/test_pipeline.py
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 asdff-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2023-07-21 04:16:34.042881 asdff-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4314 2023-07-26 06:08:13.431503 asdff-0.2.0/README.md
+-rw-r--r--   0        0        0      213 2023-07-26 06:08:13.431503 asdff-0.2.0/asdff/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-26 06:09:33.880274 asdff-0.2.0/asdff/__version__.py
+-rw-r--r--   0        0        0     5259 2023-07-26 06:08:13.431503 asdff-0.2.0/asdff/base.py
+-rw-r--r--   0        0        0     1619 2023-07-26 06:08:13.430503 asdff-0.2.0/asdff/sd.py
+-rw-r--r--   0        0        0     1810 2023-07-21 12:51:58.465683 asdff-0.2.0/asdff/utils.py
+-rw-r--r--   0        0        0     2153 2023-07-26 06:08:13.430503 asdff-0.2.0/asdff/yolo.py
+-rw-r--r--   0        0        0      949 2023-07-26 06:09:54.111666 asdff-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2608 2023-07-26 06:08:13.431503 asdff-0.2.0/tests/test_pipeline.py
+-rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 asdff-0.2.0/PKG-INFO
```

### Comparing `asdff-0.1.1/LICENSE` & `asdff-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asdff-0.1.1/README.md` & `asdff-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 result = pipe(common=common)
 
 images = result[0]
 ```
 
 ### from custom pipeline
 
-pip 설치 필요없음
+ultralytics 설치 필요
+
+```
+pip install ultralytics
+```
 
 ```py
 import torch
 from diffusers import DiffusionPipeline
 
 pipe = DiffusionPipeline.from_pretrained(
     "stablediffusionapi/counterfeit-v30",
@@ -42,14 +46,35 @@
 
 common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 28}
 result = pipe(common=common)
 
 images = result[0]
 ```
 
+### 그 외
+
+스케줄러를 변경하고, 입력 이미지를 제공하는 예시
+
+```py
+import torch
+from asdff import AdPipeline
+from diffusers import DPMSolverMultistepScheduler
+from diffusers.utils import load_image
+
+pipe = AdPipeline.from_pretrained("stablediffusionapi/counterfeit-v30", torch_dtype=torch.float16)
+pipe.safety_checker = None
+pipe.scheduler = DPMSolverMultistepScheduler.from_config(pipe.scheduler.config)
+pipe = pipe.to("cuda")
+
+common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 20}
+images = load_image("https://i.imgur.com/8TX2AX6.png")
+result = pipe(common=common, images=[images])
+```
+
+
 ## arguments
 
 - `common: Mapping[str, Any] | None`
 
 txt2img와 inpaint에서 공통적으로 사용할 인자들
 
 - `txt2img_only: Mapping[str, Any] | None`
@@ -62,14 +87,18 @@
 
 inpaint에서만 사용할 인자. common과 겹치는 인자는 덮어씁니다.
 
 `strength: 0.4`가 기본값으로 적용됩니다.
 
 [StableDiffusionInpaintPipeline.__call__](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/inpaint#diffusers.StableDiffusionInpaintPipeline.__call__)
 
+- `images: Image | Iterable[Image] | None`
+
+inpaint를 수행할 이미지들. 주어지면 txt2img의 결과를 대체하기 때문에 `txt2img_only`는 무시됩니다.
+
 - `detectors: DetectorType | Iterable[DetectorType] | None`
 
 `DetectorType: Callable[[Image.Image], Optional[List[Image.Image]]]`
 
 pil Image를 입력으로 받아 마스크 이미지의 리스트(마스크), 또는 None을 반환하는 Callable.
 
 그런 Callable 하나, Callable의 리스트 또는 None
```

### Comparing `asdff-0.1.1/asdff/utils.py` & `asdff-0.2.0/asdff/utils.py`

 * *Files identical despite different names*

### Comparing `asdff-0.1.1/asdff/yolo.py` & `asdff-0.2.0/asdff/yolo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from __future__ import annotations
 
+from pathlib import Path
+
 import numpy as np
 import torch
 from huggingface_hub import hf_hub_download
 from PIL import Image, ImageDraw
 from torchvision.transforms.functional import to_pil_image
-from ultralytics import YOLO
+
+try:
+    from ultralytics import YOLO
+except ModuleNotFoundError:
+    print("Please install ultralytics using `pip install ultralytics`")
+    raise
 
 
 def create_mask_from_bbox(
     bboxes: np.ndarray, shape: tuple[int, int]
 ) -> list[Image.Image]:
     """
     Parameters
@@ -50,15 +57,15 @@
     images: list[Image.Image]
     """
     n = masks.shape[0]
     return [to_pil_image(masks[i], mode="L").resize(shape) for i in range(n)]
 
 
 def yolo_detector(
-    image: Image.Image, model_path: str | None = None, confidence: float = 0.3
+    image: Image.Image, model_path: str | Path | None = None, confidence: float = 0.3
 ) -> list[Image.Image] | None:
     if not model_path:
         model_path = hf_hub_download("Bingsu/adetailer", "face_yolov8n.pt")
     model = YOLO(model_path)
     pred = model(image, conf=confidence)
 
     bboxes = pred[0].boxes.xyxy.cpu().numpy()
```

### Comparing `asdff-0.1.1/pyproject.toml` & `asdff-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "diffusers[torch]>=0.18.2",
     "transformers>=4.25.1",
     "ultralytics",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.1"
+version = "0.2.0"
 
 [project.license]
 text = "AGPL-3.0"
 
 [project.urls]
 repository = "https://github.com/Bing-su/asdff"
```

### Comparing `asdff-0.1.1/PKG-INFO` & `asdff-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdff
-Version: 0.1.1
+Version: 0.2.0
 Author-Email: Bingsu <ks2515@naver.com>
 License: AGPL-3.0
 Project-URL: Repository, https://github.com/Bing-su/asdff
 Requires-Python: >=3.8
 Requires-Dist: diffusers[torch]>=0.18.2
 Requires-Dist: transformers>=4.25.1
 Requires-Dist: ultralytics
@@ -34,15 +34,19 @@
 result = pipe(common=common)
 
 images = result[0]
 ```
 
 ### from custom pipeline
 
-pip 설치 필요없음
+ultralytics 설치 필요
+
+```
+pip install ultralytics
+```
 
 ```py
 import torch
 from diffusers import DiffusionPipeline
 
 pipe = DiffusionPipeline.from_pretrained(
     "stablediffusionapi/counterfeit-v30",
@@ -54,14 +58,35 @@
 
 common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 28}
 result = pipe(common=common)
 
 images = result[0]
 ```
 
+### 그 외
+
+스케줄러를 변경하고, 입력 이미지를 제공하는 예시
+
+```py
+import torch
+from asdff import AdPipeline
+from diffusers import DPMSolverMultistepScheduler
+from diffusers.utils import load_image
+
+pipe = AdPipeline.from_pretrained("stablediffusionapi/counterfeit-v30", torch_dtype=torch.float16)
+pipe.safety_checker = None
+pipe.scheduler = DPMSolverMultistepScheduler.from_config(pipe.scheduler.config)
+pipe = pipe.to("cuda")
+
+common = {"prompt": "masterpiece, best quality, 1girl", "num_inference_steps": 20}
+images = load_image("https://i.imgur.com/8TX2AX6.png")
+result = pipe(common=common, images=[images])
+```
+
+
 ## arguments
 
 - `common: Mapping[str, Any] | None`
 
 txt2img와 inpaint에서 공통적으로 사용할 인자들
 
 - `txt2img_only: Mapping[str, Any] | None`
@@ -74,14 +99,18 @@
 
 inpaint에서만 사용할 인자. common과 겹치는 인자는 덮어씁니다.
 
 `strength: 0.4`가 기본값으로 적용됩니다.
 
 [StableDiffusionInpaintPipeline.__call__](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/inpaint#diffusers.StableDiffusionInpaintPipeline.__call__)
 
+- `images: Image | Iterable[Image] | None`
+
+inpaint를 수행할 이미지들. 주어지면 txt2img의 결과를 대체하기 때문에 `txt2img_only`는 무시됩니다.
+
 - `detectors: DetectorType | Iterable[DetectorType] | None`
 
 `DetectorType: Callable[[Image.Image], Optional[List[Image.Image]]]`
 
 pil Image를 입력으로 받아 마스크 이미지의 리스트(마스크), 또는 None을 반환하는 Callable.
 
 그런 Callable 하나, Callable의 리스트 또는 None
```

