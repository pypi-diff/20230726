# Comparing `tmp/image2layout_computer_vision-0.0.5.tar.gz` & `tmp/image2layout_computer_vision-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.0.5.tar", last modified: Thu Jul 20 06:07:08 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.0.6.tar", last modified: Wed Jul 26 09:05:31 2023, max compression
```

## Comparing `image2layout_computer_vision-0.0.5.tar` & `image2layout_computer_vision-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/
--rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.0.5/LICENSE
--rw-rw-r--   0 test      (1001) test      (1001)     2319 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     1843 2023-07-20 05:34:07.000000 image2layout_computer_vision-0.0.5/README.md
--rw-rw-r--   0 test      (1001) test      (1001)      543 2023-07-20 06:06:32.000000 image2layout_computer_vision-0.0.5/pyproject.toml
--rw-rw-r--   0 test      (1001) test      (1001)       38 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/setup.cfg
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.134436 image2layout_computer_vision-0.0.5/src/
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/
--rw-rw-r--   0 test      (1001) test      (1001)      340 2023-07-20 05:34:25.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/__init__.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/color_extract/
--rw-rw-r--   0 test      (1001) test      (1001)       95 2023-07-19 10:08:46.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/color_extract/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     5044 2023-07-20 04:34:26.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/color_extract/main.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/
--rw-rw-r--   0 test      (1001) test      (1001)      143 2023-07-19 10:42:13.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    13036 2023-07-20 05:02:01.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/imagebox.py
--rw-rw-r--   0 test      (1001) test      (1001)     2332 2023-07-20 06:03:33.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/main.py
--rw-rw-r--   0 test      (1001) test      (1001)     3584 2023-07-20 05:04:21.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/utils/
--rw-rw-r--   0 test      (1001) test      (1001)      125 2023-07-19 10:08:52.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/utils/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     3972 2023-07-19 03:48:10.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/utils/color_system.py
--rw-rw-r--   0 test      (1001) test      (1001)     1398 2023-07-19 10:04:00.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/utils/imaging.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-07-20 06:07:08.138435 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision.egg-info/
--rw-rw-r--   0 test      (1001) test      (1001)     2319 2023-07-20 06:07:08.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)      771 2023-07-20 06:07:08.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1001) test      (1001)        1 2023-07-20 06:07:08.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1001) test      (1001)       29 2023-07-20 06:07:08.000000 image2layout_computer_vision-0.0.5/src/image2layout_computer_vision.egg-info/top_level.txt
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.110434 image2layout_computer_vision-0.0.6/
+-rw-r--r--   0 felixdo    (501) staff       (20)     1073 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/LICENSE
+-rw-r--r--   0 felixdo    (501) staff       (20)     2331 2023-07-26 09:05:31.110218 image2layout_computer_vision-0.0.6/PKG-INFO
+-rw-r--r--   0 felixdo    (501) staff       (20)     1761 2023-07-26 09:02:55.000000 image2layout_computer_vision-0.0.6/README.md
+-rw-r--r--   0 felixdo    (501) staff       (20)      637 2023-07-26 09:04:05.000000 image2layout_computer_vision-0.0.6/pyproject.toml
+-rw-r--r--   0 felixdo    (501) staff       (20)       38 2023-07-26 09:05:31.110492 image2layout_computer_vision-0.0.6/setup.cfg
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.105716 image2layout_computer_vision-0.0.6/src/
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.106193 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/
+-rw-r--r--   0 felixdo    (501) staff       (20)      364 2023-07-26 08:56:55.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/__init__.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.107503 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/
+-rw-r--r--   0 felixdo    (501) staff       (20)       95 2023-07-26 08:56:49.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     8717 2023-07-26 08:59:02.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/main.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.108847 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/
+-rw-r--r--   0 felixdo    (501) staff       (20)      143 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)    13036 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     2310 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/main.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     6286 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.109890 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/
+-rw-r--r--   0 felixdo    (501) staff       (20)      172 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     4896 2023-07-26 08:33:29.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/color_system.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     1398 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/imaging.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     1900 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/pixel_mask.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.107025 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/
+-rw-r--r--   0 felixdo    (501) staff       (20)     2331 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-r--r--   0 felixdo    (501) staff       (20)      851 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)        1 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)       42 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)    13593 2023-07-26 08:41:36.000000 image2layout_computer_vision-0.0.6/src/sandbox.py
+-rw-r--r--   0 felixdo    (501) staff       (20)      747 2023-07-26 09:01:24.000000 image2layout_computer_vision-0.0.6/src/test.py
```

### Comparing `image2layout_computer_vision-0.0.5/LICENSE` & `image2layout_computer_vision-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.5/PKG-INFO` & `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,95 @@
 Metadata-Version: 2.1
-Name: image2layout_computer_vision
-Version: 0.0.5
+Name: image2layout-computer-vision
+Version: 0.0.6
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
-Project-URL: Homepage, https://github.com
-Project-URL: Bug Tracker, https://github.com
+Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
+Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# image2layout-computer-vision
-Computer Vision related modules for image2layout
+# image2layout_computer_vision
 
-## Installation
+An image processing module for some computer vision tasks (public module for image2layout)
 
-1. Build and run Docker container, will contain the necessary requirements for all modules
+Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
-```bash
-sudo docker build --tag cv -f Dockerfile .
+Features:
 
-sudo docker run -it -v $(pwd):/app cv bash
-```
+1. Text Detection
+2. Color extraction (background and main foreground)
+
+## Installations
 
-2. OR, Install Conda
+### Install with `python`/`conda` [Linux]
+
+1. (Optional) Conda
 
 ```bash
 curl https://repo.anaconda.com/archive/Anaconda3-2023.03-1-Linux-x86_64.sh -o ~/conda.sh
 bash ~/conda.sh -b -f -p /opt/conda
 rm ~/conda.sh
 conda init --all --dry-run --verbose
-```
-
 
-## OCR - Text Detection
-
-### Installation [CPU]
-
-Follow instructions in [README](ocr/README.md) to build and run docker container for all modules
-
-Or install using conda locally:
+conda create -n cv python=3.10 -y
+conda activate cv
+```
 
-> Python [conda] + tesseract
+2. Tesseract
 
 ```bash
 sudo apt install tesseract-ocr libtesseract-dev -y
-
-conda create -n ocr python=3.8 -y
-conda activate ocr
-
-conda install -n ocr pytorch=1.10 torchvision -c pytorch -y
-
-python -m pip install Pillow pandas numpy
-python -m pip install detectron2 -f https://dl.fbaipublicfiles.com/detectron2/wheels/cpu/torch1.10/index.html
-python -m pip install pyyaml==5.1 chardet pytesseract
-python -m pip install --upgrade datasets transformers
 ```
 
-### Usage
-
-```python
-from main import detect_text
 
-# returns an ImageBoxes object
-imageboxes = detect_text('path/to/image.png')
+3. Python libraries (python>=3.8)
 
-# draw boxes
-imageboxes.draw_anno()
+```bash
+python -m pip install 'torch>=2.0' torchvision torchaudio
 
-# dataframe
-imageboxes.df
+python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
+python -m pip install --upgrade datasets transformers
 
-# boxes (x0, y0, x1, y1)
-boxes = np.array(list(imageboxes.df['box'])).astype(int)
+python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
 
+python -m pip install --upgrade image2layout-computer-vision
 ```
 
+### Install with `docker`
 
+Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU
+API Implementation is in-progress
+```bash
+sudo docker build --tag cv -f Dockerfile_cpu .
 
-## Color Extractor
+sudo docker run -it -v $(pwd):/app cv bash
+```
 
-### Installation
+## Usage
 
 > Python
+```python
+import image2layout_computer_vision as icv
 
-```bash
-python -m pip install Pillow pandas numpy scikit-learn
+imageboxes = icv.detect_text('path/to/image.png')
+boxes = icv.detect_text_boxes('path/to/image.png')
+
+color_bg, color_fg = icv.extract_colors('path/to/image.png')
 ```
 
-### Usage
 
-```python
-from PIL import Image
-from main import ColorExtractor
 
-image = Image.open('path/to/image.png').convert('RGB')
-color_extractor = ColorExtractor(image)
-color_extractor.colors
-color_extractor.color_bg    # background color
-color_extractor.color_fg    # foreground color
+## Build
+(for building and uploading this package)
+```bash
+python -m pip install --upgrade pip
+python -m pip install --upgrade build twine
+
+rm -rf dist
+python -m build
+python -m twine upload dist/* --verbose
 ```
```

### Comparing `image2layout_computer_vision-0.0.5/README.md` & `image2layout_computer_vision-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-# image2layout-computer-vision
-Computer Vision related modules for image2layout
+Metadata-Version: 2.1
+Name: image2layout_computer_vision
+Version: 0.0.6
+Summary: image processing and stuff
+Author-email: Felix Do <felix.do.1030@gmail.com>
+Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
+Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-## Installation
+# image2layout_computer_vision
 
-1. Build and run Docker container, will contain the necessary requirements for all modules
+An image processing module for some computer vision tasks (public module for image2layout)
 
-```bash
-sudo docker build --tag cv -f Dockerfile .
+Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
-sudo docker run -it -v $(pwd):/app cv bash
-```
+Features:
+
+1. Text Detection
+2. Color extraction (background and main foreground)
 
-2. OR, Install Conda
+## Installations
+
+### Install with `python`/`conda` [Linux]
+
+1. (Optional) Conda
 
 ```bash
 curl https://repo.anaconda.com/archive/Anaconda3-2023.03-1-Linux-x86_64.sh -o ~/conda.sh
 bash ~/conda.sh -b -f -p /opt/conda
 rm ~/conda.sh
 conda init --all --dry-run --verbose
-```
-
 
-## OCR - Text Detection
-
-### Installation [CPU]
-
-Follow instructions in [README](ocr/README.md) to build and run docker container for all modules
-
-Or install using conda locally:
+conda create -n cv python=3.10 -y
+conda activate cv
+```
 
-> Python [conda] + tesseract
+2. Tesseract
 
 ```bash
 sudo apt install tesseract-ocr libtesseract-dev -y
-
-conda create -n ocr python=3.8 -y
-conda activate ocr
-
-conda install -n ocr pytorch=1.10 torchvision -c pytorch -y
-
-python -m pip install Pillow pandas numpy
-python -m pip install detectron2 -f https://dl.fbaipublicfiles.com/detectron2/wheels/cpu/torch1.10/index.html
-python -m pip install pyyaml==5.1 chardet pytesseract
-python -m pip install --upgrade datasets transformers
 ```
 
-### Usage
-
-```python
-from main import detect_text
 
-# returns an ImageBoxes object
-imageboxes = detect_text('path/to/image.png')
+3. Python libraries (python>=3.8)
 
-# draw boxes
-imageboxes.draw_anno()
+```bash
+python -m pip install 'torch>=2.0' torchvision torchaudio
 
-# dataframe
-imageboxes.df
+python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
+python -m pip install --upgrade datasets transformers
 
-# boxes (x0, y0, x1, y1)
-boxes = np.array(list(imageboxes.df['box'])).astype(int)
+python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
 
+python -m pip install --upgrade image2layout-computer-vision
 ```
 
+### Install with `docker`
 
+Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU
+API Implementation is in-progress
+```bash
+sudo docker build --tag cv -f Dockerfile_cpu .
 
-## Color Extractor
+sudo docker run -it -v $(pwd):/app cv bash
+```
 
-### Installation
+## Usage
 
 > Python
+```python
+import image2layout_computer_vision as icv
 
-```bash
-python -m pip install Pillow pandas numpy scikit-learn
+imageboxes = icv.detect_text('path/to/image.png')
+boxes = icv.detect_text_boxes('path/to/image.png')
+
+color_bg, color_fg = icv.extract_colors('path/to/image.png')
 ```
 
-### Usage
 
-```python
-from PIL import Image
-from main import ColorExtractor
 
-image = Image.open('path/to/image.png').convert('RGB')
-color_extractor = ColorExtractor(image)
-color_extractor.colors
-color_extractor.color_bg    # background color
-color_extractor.color_fg    # foreground color
+## Build
+(for building and uploading this package)
+```bash
+python -m pip install --upgrade pip
+python -m pip install --upgrade build twine
+
+rm -rf dist
+python -m build
+python -m twine upload dist/* --verbose
 ```
```

### Comparing `image2layout_computer_vision-0.0.5/pyproject.toml` & `image2layout_computer_vision-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,23 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com"
-"Bug Tracker" = "https://github.com"
+"Homepage" = "https://github.com/felix-do-wizardry/image2layout-computer-vision"
+"Bug Tracker" = "https://github.com/felix-do-wizardry/image2layout-computer-vision"
```

### Comparing `image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from ..utils import get_image, ImageConvert
 from .imagebox import ImageBoxes, BoxMerge
 
 # %%
 model_dispatch_layout = ModelDispatch_LayoutMLv2(
     device='cpu',
 )
-model_dispatch_layout
 
 # %%
 def detect_text(image, **kwargs) -> ImageBoxes:
     '''predict boxes for text in the image
     Parameters:
         image: (PIL.Image.Image, bytes, np.ndarray) RGB image
         **kwargs:
```

### Comparing `image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/color_system.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # %%
 import numpy as np
 from PIL import Image
+import colorsys
 
 # %%
 class COLOR:
     m_rgb2yiq = np.array([
         [0.299, 0.587,  0.114],
         [0.5959, -0.2746, -0.3213],
         [0.2115, -0.5227,  0.3112],
@@ -31,23 +32,47 @@
         '''
         colors = cls.get_colors(colors)
         colors_yiq = np.matmul(colors.astype(float) / 255, cls.m_rgb2yiq)
         return colors_yiq
     
     @classmethod
     def yiq2rgb(cls, colors: np.ndarray, conform_rgb=True) -> np.ndarray:
-        '''convert colors from rgb[0~255] to yiq[0~1]
+        '''convert colors from yiq[0~1] to rgb[0~255]
         '''
         colors_yiq = cls.get_colors(colors)
         colors_rgb = np.matmul(colors_yiq, cls.m_yiq2rgb) * 255
         if conform_rgb:
             colors_rgb = np.clip(colors_rgb, 0, 255).astype(np.uint8)
         return colors_rgb
     
     @classmethod
+    def rgb2hsv(cls, colors: np.ndarray) -> np.ndarray:
+        '''convert colors from rgb[0~255] to hsv[0~1]
+        '''
+        colors_rgb = cls.get_colors(colors)
+        colors_hsv = np.array([
+            list(colorsys.rgb_to_hsv(*(color/255)))
+            for color in colors_rgb.reshape(-1, 3)
+        ])
+        return colors_hsv.reshape(*colors_rgb.shape)
+    
+    @classmethod
+    def hsv2rgb(cls, colors: np.ndarray, conform_rgb=True) -> np.ndarray:
+        '''convert colors from hsv[0~1] to rgb[0~255]
+        '''
+        colors_hsv = cls.get_colors(colors)
+        colors_rgb = np.array([
+            list(colorsys.hsv_to_rgb(*color))
+            for color in colors_hsv
+        ]) * 255
+        if conform_rgb:
+            colors_rgb = np.clip(colors_rgb, 0, 255).astype(np.uint8)
+        return colors_rgb
+    
+    @classmethod
     def rgb2hex(cls, colors: np.ndarray) -> np.ndarray:
         '''convert colors from rgb[0~255] to hex-code[#000000~#FFFFFF]
         '''
         colors = cls.get_colors(colors)
         assert colors.ndim <= 2
         _scale = 2 ** (np.arange(3)[::-1] * 8)
         for i in range(colors.ndim - 1):
@@ -58,44 +83,46 @@
         else:
             return [
                 f'#{hex(int(v))[2:].rjust(6,"0")}'
                 for v in colors_hex_int
             ]
     
     @classmethod
-    def hex2rgb(cls, colors: np.ndarray) -> np.ndarray:
+    def hex2rgb(cls, colors) -> np.ndarray:
         '''convert colors from hex-code[#000000~#FFFFFF] to rgb[0~255]
         '''
         return np.array([
             [
-                _code_formated[i * 2 : (i + 1) * 2]
+                int(_code_formated[i * 2 : (i + 1) * 2], 16)
                 for i in range(3)
             ]
             for _code in colors
             if isinstance(_code, str)
             for _code_formated in [_code.strip('#')[:6].rjust(6, '0')]
         ], np.uint8)
     
     @classmethod
-    def count_uniques(cls, a: np.ndarray, keep_axis=None, axis=None):
+    def count_uniques(cls, a: np.ndarray, keep_axis=None, axis=None, sort=True):
         '''count the return the sorted unique values with counts
         '''
         assert keep_axis is None or axis is None, 'either `keep_axis` or `axis` must be left as None'
         if keep_axis is not None:
             if isinstance(keep_axis, int):
                 _keep_axis = [keep_axis, a.ndim + keep_axis]
             elif isinstance(keep_axis, (list, tuple)):
                 _keep_axis = [v1 for v in keep_axis for v1 in [v, a.ndim + v]]
             else:
                 raise ValueError(f'`keep_axis` must be of types[int, list, tuple]')
             axis = [i for i in range(a.ndim) if i not in _keep_axis]
         
         uniques, counts = np.unique(a, axis=axis, return_counts=True)
-        sort_order = np.argsort(counts)[::-1]
-        return uniques[sort_order], counts[sort_order]
+        if sort:
+            sort_order = np.argsort(counts)[::-1]
+            return uniques[sort_order], counts[sort_order]
+        return uniques, counts
     
     @classmethod
     def count_unique_colors(cls, colors: np.ndarray):
         '''count the return the sorted unique colors (3-channel) with counts
         '''
         uniques, counts = cls.count_uniques(
             cls.get_colors(colors).reshape(-1, colors.shape[-1]),
```

### Comparing `image2layout_computer_vision-0.0.5/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.5/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
+src/sandbox.py
+src/test.py
 src/image2layout_computer_vision/__init__.py
 src/image2layout_computer_vision.egg-info/PKG-INFO
 src/image2layout_computer_vision.egg-info/SOURCES.txt
 src/image2layout_computer_vision.egg-info/dependency_links.txt
 src/image2layout_computer_vision.egg-info/top_level.txt
 src/image2layout_computer_vision/color_extract/__init__.py
 src/image2layout_computer_vision/color_extract/main.py
 src/image2layout_computer_vision/ocr/__init__.py
 src/image2layout_computer_vision/ocr/imagebox.py
 src/image2layout_computer_vision/ocr/main.py
 src/image2layout_computer_vision/ocr/model_layoutmlv2.py
 src/image2layout_computer_vision/utils/__init__.py
 src/image2layout_computer_vision/utils/color_system.py
-src/image2layout_computer_vision/utils/imaging.py
+src/image2layout_computer_vision/utils/imaging.py
+src/image2layout_computer_vision/utils/pixel_mask.py
```

